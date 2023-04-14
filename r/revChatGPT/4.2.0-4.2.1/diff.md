# Comparing `tmp/revChatGPT-4.2.0.tar.gz` & `tmp/revChatGPT-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.2.0.tar", last modified: Wed Apr 12 03:12:27 2023, max compression
+gzip compressed data, was "revChatGPT-4.2.1.tar", last modified: Fri Apr 14 00:34:15 2023, max compression
```

## Comparing `revChatGPT-4.2.0.tar` & `revChatGPT-4.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.720898 revChatGPT-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-12 03:12:27.720898 revChatGPT-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 03:12:27.720898 revChatGPT-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.712898 revChatGPT-4.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.716898 revChatGPT-4.2.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    47327 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23144 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.716898 revChatGPT-4.2.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.716898 revChatGPT-4.2.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    47003 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23144 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.2.0/LICENSE` & `revChatGPT-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.0/PKG-INFO` & `revChatGPT-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.0
+Version: 4.2.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-4.2.0/README.md` & `revChatGPT-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.0/setup.py` & `revChatGPT-4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.2.0",
+    version="4.2.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.2.0/src/revChatGPT/V1.py` & `revChatGPT-4.2.1/src/revChatGPT/V1.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
 from pathlib import Path
 from typing import NoReturn, Generator, AsyncGenerator
 
-import requests
+import requests, httpx
 from httpx import AsyncClient
 from OpenAIAuth import Authenticator
 from OpenAIAuth import Error as AuthError
 
 from . import typings as t
 from .utils import create_completer
 from .utils import create_session
@@ -152,15 +152,15 @@
         self.conversation_id = conversation_id
         self.parent_id = parent_id
         self.conversation_mapping = {}
         self.conversation_id_prev_queue = []
         self.parent_id_prev_queue = []
         self.lazy_loading = lazy_loading
 
-        if "_puid" in self.config:
+        if "_puid" in self.config and self.config["_puid"]:
             self.base_url = "https://chat.openai.com/backend-api/"
             self.__set_puid(self.config["_puid"])
         else:
             self.base_url = base_url or BASE_URL
 
         self.__check_credentials()
 
@@ -350,376 +350,317 @@
             log.debug("Using authenticator to get access token")
             auth.begin()
             auth.get_access_token()
 
         self.set_access_token(auth.access_token)
 
     @logger(is_timed=True)
-    def ask(
+    def __send_request(
         self,
-        prompt: str,
+        data: dict,
+        auto_continue: bool = False,
+        timeout: float = 360,
+    ) -> Generator[dict, None, None]:
+        log.debug("Sending the payload")
+
+        cid, pid = data["conversation_id"], data["parent_message_id"]
+        model, message = None, ""
+
+        self.conversation_id_prev_queue.append(cid)
+        self.parent_id_prev_queue.append(pid)
+        response = self.session.post(
+            url=f"{self.base_url}conversation",
+            data=json.dumps(data),
+            timeout=timeout,
+            stream=True,
+        )
+        self.__check_response(response)
+
+        finish_details = None
+        for line in response.iter_lines():
+            # remove b' and ' at the beginning and end and ignore case
+            line = str(line)[2:-1]
+            if line.lower() == "internal server error":
+                log.error(f"Internal Server Error: {line}")
+                error = t.Error(
+                    source="ask",
+                    message="Internal Server Error",
+                    code=t.ErrorType.SERVER_ERROR,
+                )
+                raise error
+            if not line or line is None:
+                continue
+            if "data: " in line:
+                line = line[6:]
+            if line == "[DONE]":
+                break
+
+            line = line.replace('\\"', '"')
+            line = line.replace("\\'", "'")
+            line = line.replace("\\\\", "\\")
+
+            try:
+                line = json.loads(line)
+            except json.decoder.JSONDecodeError:
+                continue
+            if not self.__check_fields(line):
+                raise ValueError(f"Field missing. Details: {str(line)}")
+            if line.get("message").get("author").get("role") != "assistant":
+                continue
+            message: str = line["message"]["content"]["parts"][0]
+            cid = line["conversation_id"]
+            pid = line["message"]["id"]
+            metadata = line["message"].get("metadata", {})
+            model = metadata.get("model_slug", None)
+            finish_details = metadata.get("finish_details", {"type": None})["type"]
+            yield {
+                "message": message,
+                "conversation_id": cid,
+                "parent_id": pid,
+                "model": model,
+                "finish_details": finish_details,
+                "end_turn": line["message"].get("end_turn", True),
+                "recipient": line["message"].get("recipient", "all"),
+            }
+
+        self.conversation_mapping[cid] = pid
+        if pid is not None:
+            self.parent_id = pid
+        if cid is not None:
+            self.conversation_id = cid
+
+        if not (auto_continue and finish_details == "max_tokens"):
+            return
+        message = message.strip("\n")
+        for i in self.continue_write(
+            conversation_id=cid,
+            model=model,
+            timeout=timeout,
+        ):
+            i["message"] = message + i["message"]
+            yield i
+
+    @logger(is_timed=True)
+    def post_messages(
+        self,
+        messages: list[dict],
         conversation_id: str | None = None,
         parent_id: str | None = None,
         model: str | None = None,
         auto_continue: bool = False,
         timeout: float = 360,
     ) -> Generator[dict, None, None]:
         """Ask a question to the chatbot
         Args:
-            prompt (str): The question
+            messages (list[dict]): The messages to send
             conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): UUID for the message to continue on. Defaults to None.
+            model (str | None, optional): The model to use. Defaults to None.
+            auto_continue (bool, optional): Whether to continue the conversation automatically. Defaults to False.
             timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
 
-        Raises:
-            Error: _description_
-            Exception: _description_
-            Error: _description_
-            Error: _description_
-            Error: _description_
-
-        Yields:
-            _type_: _description_
+        Yields: Generator[dict, None, None] - The response from the chatbot
+            dict: {
+                "message": str,
+                "conversation_id": str,
+                "parent_id": str,
+                "model": str,
+                "finish_details": str, # "max_tokens" or "stop"
+                "end_turn": bool,
+                "recipient": str,
+            }
         """
-
-        if parent_id is not None and conversation_id is None:
-            log.error("conversation_id must be set once parent_id is set")
-            error = t.Error(
+        if parent_id and not conversation_id:
+            raise t.Error(
                 source="User",
                 message="conversation_id must be set once parent_id is set",
                 code=t.ErrorType.USER_ERROR,
             )
-            raise error
 
-        if conversation_id is not None and conversation_id != self.conversation_id:
-            log.debug("Updating to new conversation by setting parent_id to None")
+        if conversation_id and conversation_id != self.conversation_id:
             self.parent_id = None
-
         conversation_id = conversation_id or self.conversation_id
-        parent_id = parent_id or self.parent_id
-        if conversation_id is None and parent_id is None:
+        parent_id = parent_id or self.parent_id or ""
+        if not conversation_id and not parent_id:
             parent_id = str(uuid.uuid4())
-            log.debug(f"New conversation, setting parent_id to new UUID4: {parent_id}")
 
-        if conversation_id is not None and parent_id is None:
+        if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 if self.lazy_loading:
                     log.debug(
                         f"Conversation ID {conversation_id} not found in conversation mapping, try to get conversation history for the given ID",
                     )
                     with contextlib.suppress(Exception):
                         history = self.get_msg_history(conversation_id)
                         self.conversation_mapping[conversation_id] = history[
                             "current_node"
                         ]
                 else:
                     log.debug(
                         f"Conversation ID {conversation_id} not found in conversation mapping, mapping conversations",
                     )
-
                     self.__map_conversations()
-
             if conversation_id in self.conversation_mapping:
                 log.debug(
                     f"Conversation ID {conversation_id} found in conversation mapping, setting parent_id to {self.conversation_mapping[conversation_id]}",
                 )
                 parent_id = self.conversation_mapping[conversation_id]
             else:  # invalid conversation_id provided, treat as a new conversation
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
+
         data = {
             "action": "next",
-            "messages": [
-                {
-                    "id": str(uuid.uuid4()),
-                    "role": "user",
-                    "author": {"role": "user"},
-                    "content": {"content_type": "text", "parts": [prompt]},
-                },
-            ],
+            "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model
             or self.config.get("model")
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
         }
-        log.debug("Sending the payload")
-        log.debug(json.dumps(data, indent=2))
 
-        self.conversation_id_prev_queue.append(
-            data["conversation_id"],
-        )
-        self.parent_id_prev_queue.append(data["parent_message_id"])
-        response = self.session.post(
-            url=f"{self.base_url}conversation",
-            data=json.dumps(data),
-            timeout=timeout,
-            stream=True,
+        yield from self.__send_request(
+            data, timeout=timeout, auto_continue=auto_continue
         )
-        self.__check_response(response)
 
-        finish_reason = None
-        for line in response.iter_lines():
-            # remove b' and ' at the beginning and end and ignore case
-            line = str(line)[2:-1]
-            if line.lower() == "internal server error":
-                log.error(f"Internal Server Error: {line}")
-                error = t.Error(
-                    source="ask",
-                    message="Internal Server Error",
-                    code=t.ErrorType.SERVER_ERROR,
-                )
-                raise error
-            if not line or line is None:
-                continue
-            if "data: " in line:
-                line = line[6:]
-            if line == "[DONE]":
-                break
-
-            line = line.replace('\\"', '"')
-            line = line.replace("\\'", "'")
-            line = line.replace("\\\\", "\\")
-
-            try:
-                line = json.loads(line)
-            except json.decoder.JSONDecodeError:
-                continue
-            if not self.__check_fields(line) or response.status_code != 200:
-                log.error("Field missing", exc_info=True)
-                log.error(response.text)
-                if response.status_code == 401:
-                    error = t.Error(
-                        source="ask",
-                        message="Permission denied",
-                        code=t.ErrorType.AUTHENTICATION_ERROR,
-                    )
-                elif response.status_code == 403:
-                    error = t.Error(
-                        source="ask",
-                        message="Cloudflare triggered a 403 error",
-                        code=t.ErrorType.CLOUDFLARE_ERROR,
-                    )
-                elif response.status_code == 429:
-                    error = t.Error(
-                        source="ask",
-                        message="Rate limit exceeded",
-                        code=t.ErrorType.RATE_LIMIT_ERROR,
-                    )
-                else:
-                    error = t.Error(
-                        source="ask",
-                        message=line,
-                        code=t.ErrorType.SERVER_ERROR,
-                    )
-                raise error
+    @logger(is_timed=True)
+    def ask(
+        self,
+        prompt: str,
+        conversation_id: str | None = None,
+        parent_id: str | None = None,
+        model: str | None = None,
+        auto_continue: bool = False,
+        timeout: float = 360,
+    ) -> Generator[dict, None, None]:
+        """Ask a question to the chatbot
+        Args:
+            prompt (str): The question
+            conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
+            parent_id (str | None, optional): UUID for the message to continue on. Defaults to None.
+            model (str | None, optional): The model to use. Defaults to None.
+            auto_continue (bool, optional): Whether to continue the conversation automatically. Defaults to False.
+            timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
 
-            message: str = line["message"]["content"]["parts"][0]
-            if message == prompt:
-                continue
-            conversation_id = line["conversation_id"]
-            parent_id = line["message"]["id"]
-            metadata = line["message"].get("metadata", {})
-            model = metadata.get("model_slug", None)
-            finish_reason = metadata.get("finish_details", {"type": None})["type"]
-            yield {
-                "message": message.strip("\n"),
-                "conversation_id": conversation_id,
-                "parent_id": parent_id,
-                "model": model,
-                "finish_details": finish_reason,
+        Yields: Generator[dict, None, None] - The response from the chatbot
+            dict: {
+                "message": str,
+                "conversation_id": str,
+                "parent_id": str,
+                "model": str,
+                "finish_details": str, # "max_tokens" or "stop"
+                "end_turn": bool,
+                "recipient": str,
             }
+        """
+        messages = [
+            {
+                "id": str(uuid.uuid4()),
+                "role": "user",
+                "author": {"role": "user"},
+                "content": {"content_type": "text", "parts": [prompt]},
+            },
+        ]
 
-        self.conversation_mapping[conversation_id] = parent_id
-        if parent_id is not None:
-            self.parent_id = parent_id
-        if conversation_id is not None:
-            self.conversation_id = conversation_id
-
-        if not (auto_continue and finish_reason == "max_tokens"):
-            return
-        message = message.strip("\n")
-        for i in self.continue_write(
+        yield from self.post_messages(
+            messages,
             conversation_id=conversation_id,
+            parent_id=parent_id,
+            model=model,
+            auto_continue=auto_continue,
             timeout=timeout,
-        ):
-            i["message"] = message + i["message"]
-            yield i
+        )
 
     @logger(is_timed=True)
     def continue_write(
         self,
         conversation_id: str | None = None,
-        parent_id: str | None = None,
-        model: str | None = None,
+        parent_id: str = "",
+        model: str = "",
+        auto_continue: bool = False,
         timeout: float = 360,
     ) -> Generator[dict, None, None]:
         """let the chatbot continue to write
         Args:
             conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): UUID for the message to continue on. Defaults to None.
+            model (str | None, optional): The model to use. Defaults to None.
+            auto_continue (bool, optional): Whether to continue the conversation automatically. Defaults to False.
             timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
 
-        Raises:
-            Error: _description_
-            Exception: _description_
-            Error: _description_
-            Error: _description_
-            Error: _description_
-
         Yields:
-            _type_: _description_
+            dict: {
+                "message": str,
+                "conversation_id": str,
+                "parent_id": str,
+                "model": str,
+                "finish_details": str, # "max_tokens" or "stop"
+                "end_turn": bool,
+                "recipient": str,
+            }
         """
-        if parent_id is not None and conversation_id is None:
-            log.error("conversation_id must be set once parent_id is set")
-            error = t.Error(
+        if parent_id and not conversation_id:
+            raise t.Error(
                 source="User",
                 message="conversation_id must be set once parent_id is set",
                 code=t.ErrorType.USER_ERROR,
             )
-            raise error
 
-        if conversation_id is not None and conversation_id != self.conversation_id:
-            log.debug("Updating to new conversation by setting parent_id to None")
+        if conversation_id and conversation_id != self.conversation_id:
             self.parent_id = None
-
         conversation_id = conversation_id or self.conversation_id
-        parent_id = parent_id or self.parent_id
-        if conversation_id is None and parent_id is None:
+        parent_id = parent_id or self.parent_id or ""
+        if not conversation_id and not parent_id:
             parent_id = str(uuid.uuid4())
-            log.debug(f"New conversation, setting parent_id to new UUID4: {parent_id}")
 
-        if conversation_id is not None and parent_id is None:
+        if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 if self.lazy_loading:
                     log.debug(
                         f"Conversation ID {conversation_id} not found in conversation mapping, try to get conversation history for the given ID",
                     )
                     with contextlib.suppress(Exception):
                         history = self.get_msg_history(conversation_id)
                         self.conversation_mapping[conversation_id] = history[
                             "current_node"
                         ]
                 else:
                     log.debug(
                         f"Conversation ID {conversation_id} not found in conversation mapping, mapping conversations",
                     )
-
                     self.__map_conversations()
-
             if conversation_id in self.conversation_mapping:
                 log.debug(
                     f"Conversation ID {conversation_id} found in conversation mapping, setting parent_id to {self.conversation_mapping[conversation_id]}",
                 )
                 parent_id = self.conversation_mapping[conversation_id]
             else:  # invalid conversation_id provided, treat as a new conversation
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
+
         data = {
             "action": "continue",
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model
             or self.config.get("model")
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
         }
-        log.debug("Sending the payload")
-        log.debug(json.dumps(data, indent=2))
 
-        self.conversation_id_prev_queue.append(
-            data["conversation_id"],
+        yield from self.__send_request(
+            data, timeout=timeout, auto_continue=auto_continue
         )
-        self.parent_id_prev_queue.append(data["parent_message_id"])
-        response = self.session.post(
-            url=f"{self.base_url}conversation",
-            data=json.dumps(data),
-            timeout=timeout,
-            stream=True,
-        )
-        self.__check_response(response)
-        for line in response.iter_lines():
-            # remove b' and ' at the beginning and end and ignore case
-            line = str(line)[2:-1]
-            if line.lower() == "internal server error":
-                log.error(f"Internal Server Error: {line}")
-                error = t.Error(
-                    source="ask",
-                    message="Internal Server Error",
-                    code=t.ErrorType.SERVER_ERROR,
-                )
-                raise error
-            if not line or line is None:
-                continue
-            if "data: " in line:
-                line = line[6:]
-            if line == "[DONE]":
-                break
-
-            line = line.replace('\\"', '"')
-            line = line.replace("\\'", "'")
-            line = line.replace("\\\\", "\\")
-
-            try:
-                line = json.loads(line)
-            except json.decoder.JSONDecodeError:
-                continue
-            if not self.__check_fields(line) or response.status_code != 200:
-                log.error("Field missing", exc_info=True)
-                log.error(response.text)
-                if response.status_code == 401:
-                    error = t.Error(
-                        source="continue_write",
-                        message="Permission denied",
-                        code=t.ErrorType.AUTHENTICATION_ERROR,
-                    )
-                elif response.status_code == 403:
-                    error = t.Error(
-                        source="continue_write",
-                        message="Cloudflare triggered a 403 error",
-                        code=t.ErrorType.CLOUDFLARE_ERROR,
-                    )
-                elif response.status_code == 429:
-                    error = t.Error(
-                        source="continue_write",
-                        message="Rate limit exceeded",
-                        code=t.ErrorType.RATE_LIMIT_ERROR,
-                    )
-                else:
-                    error = t.Error(
-                        source="continue_write",
-                        message=line,
-                        code=t.ErrorType.SERVER_ERROR,
-                    )
-                raise error
-            message: str = line["message"]["content"]["parts"][0]
-            conversation_id = line["conversation_id"]
-            parent_id = line["message"]["id"]
-            metadata = line["message"].get("metadata", {})
-            model = metadata.get("model_slug", None)
-            finish_reason = metadata.get("finish_details", {"type": None})["type"]
-            yield {
-                "message": message.strip("\n"),
-                "conversation_id": conversation_id,
-                "parent_id": parent_id,
-                "model": model,
-                "finish_details": finish_reason,
-            }
-        self.conversation_mapping[conversation_id] = parent_id
-        if parent_id is not None:
-            self.parent_id = parent_id
-        if conversation_id is not None:
-            self.conversation_id = conversation_id
 
     @logger(is_timed=False)
     def __check_fields(self, data: dict) -> bool:
         try:
             data["message"]["content"]
         except (TypeError, KeyError):
             return False
@@ -731,16 +672,17 @@
 
         Args:
             response (_type_): _description_
 
         Raises:
             Error: _description_
         """
-        if response.status_code != 200:
-            print(response.text)
+        try:
+            response.raise_for_status()
+        except requests.exceptions.HTTPError:
             error = t.Error(
                 source="OpenAI",
                 message=response.text,
                 code=response.status_code,
             )
             raise error
 
@@ -856,247 +798,296 @@
     Async Chatbot class for ChatGPT
     """
 
     def __init__(
         self,
         config: dict,
         conversation_id: str | None = None,
-        parent_id: str | None = None,
-        base_url: str = None,
+        parent_id: str = "",
+        base_url: str = "",
     ) -> None:
+        """
+        Same as Chatbot class, but with async methods.
+
+        Note:
+            AsyncChatbot is not compatible with OpenAI Web API, I don't know why the stream method doesn't work.
+            (But the sync version works fine)
+            So, if you want to use AsyncChatbot, you don't need to set the "_puid" parameter in the config.
+        """
         super().__init__(
             config=config,
             conversation_id=conversation_id,
             parent_id=parent_id,
             session_client=AsyncClient,
             base_url=base_url,
         )
 
-    async def ask(
+    async def __send_request(
+        self, data: dict, auto_continue: bool = False, timeout: float = 360
+    ) -> AsyncGenerator[dict, None]:
+        cid, pid = data["conversation_id"], data["parent_message_id"]
+
+        self.conversation_id_prev_queue.append(cid)
+        self.parent_id_prev_queue.append(pid)
+        message = ""
+
+        finish_details = None
+        response = None
+        async with self.session.stream(
+            method="POST",
+            url=f"{self.base_url}conversation",
+            data=json.dumps(data),
+            timeout=timeout,
+        ) as response:
+            await self.__check_response(response)
+            async for line in response.aiter_lines():
+                if not line or line is None:
+                    continue
+                if "data: " in line:
+                    line = line[6:]
+                if "[DONE]" in line:
+                    break
+
+                try:
+                    line = json.loads(line)
+                except json.decoder.JSONDecodeError:
+                    continue
+                if not self.__check_fields(line):
+                    raise ValueError(f"Field missing. Details: {str(line)}")
+
+                message: str = line["message"]["content"]["parts"][0]
+                cid = line["conversation_id"]
+                pid = line["message"]["id"]
+                metadata = line["message"].get("metadata", {})
+                model = metadata.get("model_slug", None)
+                finish_details = metadata.get("finish_details", {"type": None})["type"]
+                yield {
+                    "message": message,
+                    "conversation_id": cid,
+                    "parent_id": pid,
+                    "model": model,
+                    "finish_details": finish_details,
+                    "end_turn": line["message"].get("end_turn", True),
+                    "recipient": line["message"].get("recipient", "all"),
+                }
+
+            self.conversation_mapping[cid] = pid
+            if pid:
+                self.parent_id = pid
+            if cid:
+                self.conversation_id = cid
+
+        if not (auto_continue and finish_details == "max_tokens"):
+            return
+        async for msg in self.continue_write(
+            conversation_id=cid,
+            auto_continue=auto_continue,
+            timeout=timeout,
+        ):
+            msg["message"] = message + msg["message"]
+            yield msg
+
+    async def post_messages(
         self,
-        prompt: str,
+        messages: list[dict],
         conversation_id: str | None = None,
-        parent_id: str | None = None,
+        parent_id: str = "",
+        model: str = "",
         auto_continue: bool = False,
         timeout: int = 360,
     ) -> AsyncGenerator[dict, None]:
+        """Post messages to the chatbot
+
+        Args:
+            messages (list[dict]): the messages to post
+            conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
+            parent_id (str, optional): UUID for the message to continue on. Defaults to "".
+            model (str, optional): The model to use. Defaults to "".
+            auto_continue (bool, optional): Whether to continue the conversation automatically. Defaults to False.
+            timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
+
+        Yields:
+            AsyncGenerator[dict, None]: The response from the chatbot
+            {
+                "message": str,
+                "conversation_id": str,
+                "parent_id": str,
+                "model": str,
+                "finish_details": str,
+                "end_turn": bool,
+                "recipient": str,
+            }
         """
-        Ask a question to the chatbot
-        """
-        if parent_id is not None and conversation_id is None:
+        if parent_id and not conversation_id:
             error = t.Error(
                 source="User",
                 message="conversation_id must be set once parent_id is set",
                 code=t.ErrorType.SERVER_ERROR,
             )
             raise error
-
-        if conversation_id is not None and conversation_id != self.conversation_id:
+        if conversation_id and conversation_id != self.conversation_id:
             self.parent_id = None
-
         conversation_id = conversation_id or self.conversation_id
-        parent_id = parent_id or self.parent_id
-        if conversation_id is None and parent_id is None:
-            parent_id = str(uuid.uuid4())
 
-        if conversation_id is not None and parent_id is None:
+        parent_id = parent_id or self.parent_id or ""
+        if not conversation_id and not parent_id:
+            parent_id = str(uuid.uuid4())
+        if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 await self.__map_conversations()
             parent_id = self.conversation_mapping[conversation_id]
+
         data = {
             "action": "next",
-            "messages": [
-                {
-                    "id": str(uuid.uuid4()),
-                    "role": "user",
-                    "content": {"content_type": "text", "parts": [prompt]},
-                },
-            ],
+            "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
-            "model": self.config.get("model")
+            "model": model
+            or self.config.get("model")
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
         }
 
-        self.conversation_id_prev_queue.append(
-            data["conversation_id"],
-        )
-        self.parent_id_prev_queue.append(data["parent_message_id"])
-
-        finish_reason = None
-        message = ""
-        async with self.session.stream(
-            method="POST",
-            url=f"{self.base_url}conversation",
-            data=json.dumps(data),
+        async for msg in self.__send_request(
+            data=data,
+            auto_continue=auto_continue,
             timeout=timeout,
-        ) as response:
-            self.__check_response(response)
-            async for line in response.aiter_lines():
-                if not line or line is None:
-                    continue
-                if "data: " in line:
-                    line = line[6:]
-                if "[DONE]" in line:
-                    break
+        ):
+            yield msg
 
-                try:
-                    line = json.loads(line)
-                except json.decoder.JSONDecodeError:
-                    continue
-                if not self.__check_fields(line):
-                    raise ValueError(f"Field missing. Details: {str(line)}")
+    async def ask(
+        self,
+        prompt: str,
+        conversation_id: str | None = None,
+        parent_id: str = "",
+        model: str = "",
+        auto_continue: bool = False,
+        timeout: int = 360,
+    ) -> AsyncGenerator[dict, None]:
+        """Ask a question to the chatbot
 
-                message = line["message"]["content"]["parts"][0]
-                finish_reason = line["message"]["metadata"].get(
-                    "finish_details", {"type": None}
-                )["type"]
-                conversation_id = line["conversation_id"]
-                parent_id = line["message"]["id"]
-                model = (
-                    line["message"]["metadata"]["model_slug"]
-                    if "model_slug" in line["message"]["metadata"]
-                    else None
-                )
+        Args:
+            prompt (str): The question to ask
+            conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
+            parent_id (str, optional): UUID for the message to continue on. Defaults to "".
+            model (str, optional): The model to use. Defaults to "".
+            auto_continue (bool, optional): Whether to continue the conversation automatically. Defaults to False.
+            timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
 
-                yield {
-                    "message": message,
-                    "conversation_id": conversation_id,
-                    "parent_id": parent_id,
-                    "model": model,
-                    "finish_details": finish_reason,
-                }
-            self.conversation_mapping[conversation_id] = parent_id
-            if parent_id is not None:
-                self.parent_id = parent_id
-            if conversation_id is not None:
-                self.conversation_id = conversation_id
-        if not (auto_continue or finish_reason == "max_tokens"):
-            return
-        async for msg in self.continue_write(
+        Yields:
+            AsyncGenerator[dict, None]: The response from the chatbot
+            {
+                "message": str,
+                "conversation_id": str,
+                "parent_id": str,
+                "model": str,
+                "finish_details": str,
+                "end_turn": bool,
+                "recipient": str,
+            }
+        """
+
+        messages = [
+            {
+                "id": str(uuid.uuid4()),
+                "author": {"role": "user"},
+                "content": {"content_type": "text", "parts": [prompt]},
+            },
+        ]
+
+        async for msg in self.post_messages(
+            messages=messages,
             conversation_id=conversation_id,
+            parent_id=parent_id,
+            model=model,
+            auto_continue=auto_continue,
             timeout=timeout,
         ):
-            msg["message"] = message + msg["message"]
             yield msg
 
     async def continue_write(
         self,
         conversation_id: str | None = None,
-        parent_id: str | None = None,
-        timeout: int = 360,
+        parent_id: str = "",
+        model: str = "",
+        auto_continue: bool = False,
+        timeout: float = 360,
     ) -> AsyncGenerator[dict, None]:
         """let the chatbot continue to write
         Args:
             conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
-            parent_id (str | None, optional): UUID for the message to continue on. Defaults to None.
+            parent_id (str, optional): UUID for the message to continue on. Defaults to None.
+            model (str, optional): Model to use. Defaults to None.
+            auto_continue (bool, optional): Whether to continue writing automatically. Defaults to False.
             timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
 
-        Raises:
-            Error: _description_
-            Exception: _description_
-            Error: _description_
-            Error: _description_
-            Error: _description_
 
         Yields:
-            _type_: _description_
+            AsyncGenerator[dict, None]: The response from the chatbot
+            {
+                "message": str,
+                "conversation_id": str,
+                "parent_id": str,
+                "model": str,
+                "finish_details": str,
+                "end_turn": bool,
+                "recipient": str,
+            }
         """
-        if parent_id is not None and conversation_id is None:
+        if parent_id and not conversation_id:
             error = t.Error(
                 source="User",
                 message="conversation_id must be set once parent_id is set",
                 code=t.ErrorType.SERVER_ERROR,
             )
             raise error
-
-        if conversation_id is not None and conversation_id != self.conversation_id:
+        if conversation_id and conversation_id != self.conversation_id:
             self.parent_id = None
-
         conversation_id = conversation_id or self.conversation_id
-        parent_id = parent_id or self.parent_id
-        if conversation_id is None and parent_id is None:
-            parent_id = str(uuid.uuid4())
 
-        if conversation_id is not None and parent_id is None:
+        parent_id = parent_id or self.parent_id or ""
+        if not conversation_id and not parent_id:
+            parent_id = str(uuid.uuid4())
+        if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 await self.__map_conversations()
             parent_id = self.conversation_mapping[conversation_id]
+
         data = {
             "action": "continue",
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
-            "model": self.config.get("model")
+            "model": model
+            or self.config.get("model")
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
         }
 
-        self.conversation_id_prev_queue.append(
-            data["conversation_id"],
-        )
-        self.parent_id_prev_queue.append(data["parent_message_id"])
-
-        async with self.session.stream(
-            method="POST",
-            url=f"{self.base_url}conversation",
-            data=json.dumps(data),
+        async for msg in self.__send_request(
+            data=data,
+            auto_continue=auto_continue,
             timeout=timeout,
-        ) as response:
-            self.__check_response(response)
-            async for line in response.aiter_lines():
-                if not line or line is None:
-                    continue
-                if "data: " in line:
-                    line = line[6:]
-                if "[DONE]" in line:
-                    break
-
-                try:
-                    line = json.loads(line)
-                except json.decoder.JSONDecodeError:
-                    continue
-                if not self.__check_fields(line):
-                    raise ValueError(f"Field missing. Details: {str(line)}")
-
-                message = line["message"]["content"]["parts"][0]
-                conversation_id = line["conversation_id"]
-                parent_id = line["message"]["id"]
-                model = (
-                    line["message"]["metadata"]["model_slug"]
-                    if "model_slug" in line["message"]["metadata"]
-                    else None
-                )
-                yield {
-                    "message": message,
-                    "conversation_id": conversation_id,
-                    "parent_id": parent_id,
-                    "model": model,
-                }
-            self.conversation_mapping[conversation_id] = parent_id
-            if parent_id is not None:
-                self.parent_id = parent_id
-            if conversation_id is not None:
-                self.conversation_id = conversation_id
+        ):
+            yield msg
 
     async def get_conversations(self, offset: int = 0, limit: int = 20) -> list:
         """
         Get conversations
         :param offset: Integer
         :param limit: Integer
         """
         url = f"{self.base_url}conversations?offset={offset}&limit={limit}"
         response = await self.session.get(url)
-        self.__check_response(response)
+        await self.__check_response(response)
         data = json.loads(response.text)
         return data["items"]
 
     async def get_msg_history(
         self,
         convo_id: str,
         encoding: str | None = "utf-8",
@@ -1105,15 +1096,15 @@
         Get message history
         :param id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
         response = await self.session.get(url)
         if encoding is not None:
             response.encoding = encoding
-            self.__check_response(response)
+            await self.__check_response(response)
             return json.loads(response.text)
         return None
 
     async def gen_title(self, convo_id: str, message_id: str) -> None:
         """
         Generate title for conversation
         """
@@ -1130,48 +1121,58 @@
         """
         Change title of conversation
         :param convo_id: UUID of conversation
         :param title: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
         response = await self.session.patch(url, data=f'{{"title": "{title}"}}')
-        self.__check_response(response)
+        await self.__check_response(response)
 
     async def delete_conversation(self, convo_id: str) -> None:
         """
         Delete conversation
         :param convo_id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
         response = await self.session.patch(url, data='{"is_visible": false}')
-        self.__check_response(response)
+        await self.__check_response(response)
 
     async def clear_conversations(self) -> None:
         """
         Delete all conversations
         """
         url = f"{self.base_url}conversations"
         response = await self.session.patch(url, data='{"is_visible": false}')
-        self.__check_response(response)
+        await self.__check_response(response)
 
     async def __map_conversations(self) -> None:
         conversations = await self.get_conversations()
         histories = [await self.get_msg_history(x["id"]) for x in conversations]
         for x, y in zip(conversations, histories):
             self.conversation_mapping[x["id"]] = y["current_node"]
 
     def __check_fields(self, data: dict) -> bool:
         try:
             data["message"]["content"]
         except (TypeError, KeyError):
             return False
         return True
 
-    def __check_response(self, response) -> None:
-        response.raise_for_status()
+    async def __check_response(self, response: httpx.Response) -> None:
+        # 改成自带的错误处理
+        try:
+            response.raise_for_status()
+        except httpx.HTTPStatusError:
+            await response.aread()
+            error = t.Error(
+                source="OpenAI",
+                message=response.text,
+                code=response.status_code,
+            )
+            raise error
 
 
 get_input = logger(is_timed=False)(get_input)
 
 
 @logger(is_timed=False)
 def configure() -> dict:
@@ -1300,15 +1301,15 @@
 
 
 if __name__ == "__main__":
     print(
         """
         ChatGPT - A command-line interface to OpenAI's ChatGPT (https://chat.openai.com/chat)
         Repo: github.com/acheong08/ChatGPT
-        Version: 4.1.6
+        Version: 4.2.0
         """,
     )
     print("Type '!help' to show a full list of commands")
     print(
         f"{bcolors.BOLD}{bcolors.WARNING}Press Esc followed by Enter or Alt+Enter to send a message.{bcolors.ENDC}",
     )
     main(configure())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `revChatGPT-4.2.0/src/revChatGPT/V3.py` & `revChatGPT-4.2.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.0/src/revChatGPT/__init__.py` & `revChatGPT-4.2.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.0/src/revChatGPT/__main__.py` & `revChatGPT-4.2.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.2.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.0/src/revChatGPT/typings.py` & `revChatGPT-4.2.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.0/src/revChatGPT/utils.py` & `revChatGPT-4.2.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.2.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.0
+Version: 4.2.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

