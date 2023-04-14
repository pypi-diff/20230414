# Comparing `tmp/gradio_tools-0.0.1-py3-none-any.whl.zip` & `tmp/gradio_tools-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,10 @@
-Zip file size: 193032 bytes, number of entries: 9
+Zip file size: 192965 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      101 b- defN 20-Feb-02 00:00 gradio_tools/__init__.py
 -rw-r--r--  2.0 unx    93174 b- defN 20-Feb-02 00:00 gradio_tools/test_image.jpg
 -rw-r--r--  2.0 unx    93174 b- defN 20-Feb-02 00:00 gradio_tools/test_image.webp
--rw-r--r--  2.0 unx      740 b- defN 20-Feb-02 00:00 gradio_tools/test_script.py
--rw-r--r--  2.0 unx     4510 b- defN 20-Feb-02 00:00 gradio_tools/tools.py
-?rw-r--r--  2.0 unx     6182 b- defN 20-Feb-02 00:00 gradio_tools-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 gradio_tools-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 gradio_tools-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      735 b- defN 20-Feb-02 00:00 gradio_tools-0.0.1.dist-info/RECORD
-9 files, 199774 bytes uncompressed, 191770 bytes compressed:  4.0%
+-rw-r--r--  2.0 unx     5732 b- defN 20-Feb-02 00:00 gradio_tools/tools.py
+?rw-r--r--  2.0 unx     6625 b- defN 20-Feb-02 00:00 gradio_tools-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 gradio_tools-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 gradio_tools-0.0.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      652 b- defN 20-Feb-02 00:00 gradio_tools-0.0.2.dist-info/RECORD
+8 files, 200616 bytes uncompressed, 191833 bytes compressed:  4.4%
```

## zipnote {}

```diff
@@ -3,26 +3,23 @@
 
 Filename: gradio_tools/test_image.jpg
 Comment: 
 
 Filename: gradio_tools/test_image.webp
 Comment: 
 
-Filename: gradio_tools/test_script.py
-Comment: 
-
 Filename: gradio_tools/tools.py
 Comment: 
 
-Filename: gradio_tools-0.0.1.dist-info/METADATA
+Filename: gradio_tools-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: gradio_tools-0.0.1.dist-info/WHEEL
+Filename: gradio_tools-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gradio_tools-0.0.1.dist-info/licenses/LICENSE
+Filename: gradio_tools-0.0.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: gradio_tools-0.0.1.dist-info/RECORD
+Filename: gradio_tools-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gradio_tools/tools.py

```diff
@@ -1,130 +1,192 @@
+import os
+import time
 from abc import abstractmethod
+from functools import wraps
+from typing import Any, Tuple, Union
 
-from langchain.agents import Tool
-
-import gradio as gr
 import gradio_client as grc
 from gradio_client.client import Job
 from gradio_client.utils import QueueError
-import time
-import os
-from typing import Tuple, Any
 
+try:
+    import gradio as gr
 
-class GradioTool:
+    GRADIO_INSTALLED = True
+except (ModuleNotFoundError, ImportError):
+    GRADIO_INSTALLED = False
+
+try:
+    import langchain as lc
+
+    LANGCHAIN_INSTALLED = True
+except (ModuleNotFoundError, ImportError):
+    LANGCHAIN_INSTALLED = False
+
+
+def raises_without_gradio(f):
+    @wraps(f)
+    def _f(*args, **kwargs):
+        if not GRADIO_INSTALLED:
+            raise ModuleNotFoundError(f"gradio must be installed to call {f.__name__}")
 
+    return _f
+
+
+class GradioTool:
     def __init__(self, name: str, description: str, src: str) -> None:
         self.name = name
         self.description = description
         self.src = src
         self.client = grc.Client(self.src)
-        self.description += ("If the output is the string QUEUE_FULL you "
-                        "should try this action again and never stop until you "
-                        "don't see this message.")
-        self._langchain = Tool(name=self.name, func=self.run, description=self.description)
-    
-    def __repr__(self) -> str:
-        return f"GradioTool(name={self.name}, src={self.src})"
+        self.description += (
+            "If the output is the string QUEUE_FULL you "
+            "should try this action again and never stop until you "
+            "don't see this message."
+        )
+        self._block = None
 
     @abstractmethod
     def create_job(self, query: str) -> Job:
         pass
 
     @abstractmethod
-    def postprocess(self, output: Tuple[Any]) -> str:
+    def postprocess(self, output: Union[Tuple[Any], Any]) -> str:
         pass
 
-    def block_input(self) -> gr.components.Component:
-        return gr.Textbox()
-
-    def block_output(self) -> gr.components.Component:
-        return gr.Textbox()
-    
     def run(self, query: str):
         job = self.create_job(query)
         while not job.done():
             status = job.status()
             print(f"\nJob Status: {str(status.code)} eta: {status.eta}")
             time.sleep(30)
         try:
             output = self.postprocess(job.result())
         except QueueError:
             output = "QUEUE_FULL"
         return output
-    
+
+    # Optional gradio functionalities
+    def _block_input(self) -> "gr.components.Component":
+        return gr.Textbox()
+
+    def _block_output(self) -> "gr.components.Component":
+        return gr.Textbox()
+
+    @raises_without_gradio
+    def block_input(self) -> "gr.components.Component":
+        return self._block_input()
+
+    @raises_without_gradio
+    def block_output(self) -> "gr.components.Component":
+        return self._block_output()
+
+    @raises_without_gradio
     def block(self):
-        """Get the gradio Blocks corresponding to this tool - useful for visualization."""
-        return gr.load(name=self.src, src="spaces")
-    
+        """Get the gradio Blocks of this tool for visualization."""
+        if not self._block:
+            self._block = gr.load(name=self.src, src="spaces")
+        return self._block
+
+    # Optional langchain functionalities
     @property
-    def langchain(self):
-        return self._langchain
-    
+    def langchain(self) -> "langchain.agents.Tool":
+        if not LANGCHAIN_INSTALLED:
+            raise ModuleNotFoundError(
+                "langchain must be installed to access langchain tool"
+            )
+
+        return lc.agents.Tool(
+            name=self.name, func=self.run, description=self.description
+        )
+
+    def __repr__(self) -> str:
+        return f"GradioTool(name={self.name}, src={self.src})"
+
 
 class StableDiffusionTool(GradioTool):
     """Tool for calling stable diffusion from llm"""
 
-    def __init__(self, name="StableDiffusion",
-                 description=("An image generator. Use this to generate images based on "
-                   "text input. Input should be a description of what the image should "
-                   "look like. The output will be a path to an image file."),
-                   src= "gradio-client-demos/stable-diffusion") -> None:
+    def __init__(
+        self,
+        name="StableDiffusion",
+        description=(
+            "An image generator. Use this to generate images based on "
+            "text input. Input should be a description of what the image should "
+            "look like. The output will be a path to an image file."
+        ),
+        src="gradio-client-demos/stable-diffusion",
+    ) -> None:
         super().__init__(name, description, src)
 
-
     def create_job(self, query: str) -> Job:
         return self.client.submit(query, "", 9, fn_index=1)
-    
-    def postprocess(self, output: Tuple[Any]) -> str:
-        return [os.path.join(output, i) for i in os.listdir(output) if not i.endswith("json")][0]
-    
-    def block_input(self) -> gr.components.Component:
+
+    def postprocess(self, output: Union[Tuple[Any], Any]) -> str:
+        assert isinstance(output, str)
+        return [
+            os.path.join(output, i)
+            for i in os.listdir(output)
+            if not i.endswith("json")
+        ][0]
+
+    def _block_input(self) -> "gr.components.Component":
         return gr.Textbox()
-    
-    def block_output(self) -> gr.components.Component:
+
+    def _block_output(self) -> "gr.components.Component":
         return gr.Image()
 
 
 class ImageCaptioningTool(GradioTool):
     """Tool for captioning images."""
 
-    def __init__(self, name= "ImageCaptioner",
-                 description=("An image captioner. Use this to create a caption for an image. "
-                   "Input will be a path to an image file. "
-                   "The output will be a caption of that image."),
-                   src="gradio-client-demos/comparing-captioning-models") -> None:
+    def __init__(
+        self,
+        name="ImageCaptioner",
+        description=(
+            "An image captioner. Use this to create a caption for an image. "
+            "Input will be a path to an image file. "
+            "The output will be a caption of that image."
+        ),
+        src="gradio-client-demos/comparing-captioning-models",
+    ) -> None:
         super().__init__(name, description, src)
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(query.strip("'"), fn_index=0)
-    
-    def postprocess(self, output: Tuple[Any]) -> str:
-        return output[1]
-    
-    def block_input(self) -> gr.components.Component:
+
+    def postprocess(self, output: Union[Tuple[Any], Any]) -> str:
+        return output[1]  # type: ignore
+
+    def _block_input(self) -> "gr.components.Component":
         return gr.Image()
-    
-    def block_output(self) -> gr.components.Component:
+
+    def _block_output(self) -> "gr.components.Component":
         return gr.Textbox()
 
 
 class ImageToMusicTool(GradioTool):
-
-    def __init__(self, name="ImagetoMusic",
-                 description=("A tool for creating music from images. Use this tool to create a musical "
-                              "track from an image. Input will be a path to an image file. "
-                              "The output will be an audio file generated from that image."),
-                src="fffiloni/img-to-music") -> None:
+    def __init__(
+        self,
+        name="ImagetoMusic",
+        description=(
+            "A tool for creating music from images. Use this tool to create a musical "
+            "track from an image. Input will be a path to an image file. "
+            "The output will be an audio file generated from that image."
+        ),
+        src="fffiloni/img-to-music",
+    ) -> None:
         super().__init__(name, description, src)
 
     def create_job(self, query: str) -> Job:
-        return self.client.submit(query.strip("'"), 15, "medium", "loop", None, fn_index=0)
+        return self.client.submit(
+            query.strip("'"), 15, "medium", "loop", None, fn_index=0
+        )
 
-    def postprocess(self, output: Tuple[Any]) -> str:
-        return output[1]
-    
-    def block_input(self) -> gr.components.Component:
+    def postprocess(self, output: Union[Tuple[Any], Any]) -> str:
+        return output[1]  # type: ignore
+
+    def _block_input(self) -> "gr.components.Component":
         return gr.Image()
-    
-    def block_output(self) -> gr.components.Component:
+
+    def _block_output(self) -> "gr.components.Component":
         return gr.Audio()
```

## Comparing `gradio_tools-0.0.1.dist-info/METADATA` & `gradio_tools-0.0.2.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: gradio_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Use Gradio Apps as tools for LLM Agents
 Author-email: Freddy Boulton <alfonsoboulton@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: AsyncIO
-Classifier: Framework :: FastAPI
-Classifier: Framework :: Pydantic
-Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
-Requires-Dist: gradio
-Requires-Dist: gradio-client>=0.0.8
-Requires-Dist: langchain
-Requires-Dist: openai
+Requires-Dist: gradio-client>=0.1.2
+Provides-Extra: all
+Requires-Dist: gradio-tools[langchain]; extra == 'all'
+Requires-Dist: gradio-tools[minichain]; extra == 'all'
+Provides-Extra: langchain
+Requires-Dist: langchain; extra == 'langchain'
+Requires-Dist: openai; extra == 'langchain'
+Provides-Extra: minichain
+Requires-Dist: gradio; extra == 'minichain'
+Requires-Dist: minichain; extra == 'minichain'
+Provides-Extra: test
+Requires-Dist: black==22.6.0; extra == 'test'
+Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
+Requires-Dist: pyright==1.1.298; extra == 'test'
+Requires-Dist: ruff==0.0.260; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Gradio Tools: Gradio 🤝 LLM Agents
 
 Any [Gradio](https://github.com/gradio-app/gradio) application at the tips of your LLM's fingers 🦾
 
 [gradio_tool](https://github.com/freddyaboulton/gradio-tool) can turn any [Gradio](https://github.com/gradio-app/gradio) application into a [tool](https://python.langchain.com/en/latest/modules/agents/tools.html) that an
@@ -90,24 +91,26 @@
     def __init__(self, name: str, description: str, src: str) -> None:
 
     @abstractmethod
     def create_job(self, query: str) -> Job:
         pass
 
     @abstractmethod
-    def postprocess(self, output: Tuple[Any]) -> str:
+    def postprocess(self, output: Tuple[Any] | Any) -> str:
         pass
 ```
 
 The requirements are:
 1. The name for your tool
 2. The description for your tool. This is crucial! Agents decide which tool to use based on their description. Be precise and be sure to inclue example of what the input and the output of the tool should look like.
 3. The url or space id, e.g. `freddyaboulton/calculator`, of the Gradio application. Based on this value, `gradio_tool` will create a [gradio client](https://github.com/gradio-app/gradio/blob/main/client/python/README.md) instance to query the upstream application via API. Be sure to click the link and learn more about the gradio client library if you are not familiar with it.
 4. create_job - Given a string, this method should parse that string and return a job from the client. Most times, this is as simple as passing the string to the `submit` function of the client. More info on creating jobs [here](https://github.com/gradio-app/gradio/blob/main/client/python/README.md#making-a-prediction)
 5. postprocess - Given the result of the job, convert it to a string the LLM can display to the user.
+6. *Optional* - Some libraries, e.g. [MiniChain](https://github.com/srush/MiniChain/tree/main), may need some info about the underlying gradio input and output types used by the tool. By default, this will return gr.Textbox() but 
+if you'd like to provide more accurate info, implement the `_block_input(self)` and `_block_output(self)` methods of the tool.
 
 And that's it!
 
 ## Pre-built tools
 
 gradio_tool comes with a set of pre-built tools you can leverage immediately! These are
```

## Comparing `gradio_tools-0.0.1.dist-info/licenses/LICENSE` & `gradio_tools-0.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

