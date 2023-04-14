# Comparing `tmp/bingbong-0.1.6.1-py3-none-any.whl.zip` & `tmp/bingbong-0.1.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10960 bytes, number of entries: 15
--rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-14 05:35 pingpong/__init__.py
--rw-rw-rw-  2.0 unx     1234 b- defN 23-Apr-14 05:21 pingpong/alpaca.py
--rw-rw-rw-  2.0 unx     1216 b- defN 23-Apr-14 05:35 pingpong/dolly.py
+Zip file size: 10978 bytes, number of entries: 15
+-rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-14 12:55 pingpong/__init__.py
+-rw-rw-rw-  2.0 unx     1199 b- defN 23-Apr-14 12:44 pingpong/alpaca.py
+-rw-rw-rw-  2.0 unx     1215 b- defN 23-Apr-14 12:55 pingpong/dolly.py
 -rw-rw-rw-  2.0 unx      987 b- defN 23-Apr-14 05:26 pingpong/gradio.py
--rw-rw-rw-  2.0 unx     1046 b- defN 23-Apr-14 05:14 pingpong/pingpong.py
+-rw-rw-rw-  2.0 unx     1192 b- defN 23-Apr-14 12:50 pingpong/pingpong.py
 -rw-rw-rw-  2.0 unx      173 b- defN 23-Apr-12 04:36 pingpong/context/__init__.py
 -rw-rw-rw-  2.0 unx      589 b- defN 23-Apr-12 00:59 pingpong/context/auto_summary_strategy.py
 -rw-rw-rw-  2.0 unx      711 b- defN 23-Apr-13 23:18 pingpong/context/last_window_strategy.py
 -rw-rw-rw-  2.0 unx      840 b- defN 23-Apr-12 04:54 pingpong/context/search_window_strategy.py
 -rw-rw-rw-  2.0 unx      119 b- defN 23-Apr-11 14:54 pingpong/context/strategy.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-14 05:35 bingbong-0.1.6.1.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-14 05:35 bingbong-0.1.6.1.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-14 05:35 bingbong-0.1.6.1.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-14 05:35 bingbong-0.1.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-14 05:35 bingbong-0.1.6.1.dist-info/RECORD
-15 files, 23011 bytes uncompressed, 8906 bytes compressed:  61.3%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/RECORD
+15 files, 23121 bytes uncompressed, 8924 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.1.6.1.dist-info/LICENSE
+Filename: bingbong-0.1.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.1.6.1.dist-info/METADATA
+Filename: bingbong-0.1.6.2.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.1.6.1.dist-info/WHEEL
+Filename: bingbong-0.1.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.1.6.1.dist-info/top_level.txt
+Filename: bingbong-0.1.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.1.6.1.dist-info/RECORD
+Filename: bingbong-0.1.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.6.1'
+__version__ = '0.1.6.2'
 
 from .pingpong import PingPong
```

## pingpong/alpaca.py

```diff
@@ -3,15 +3,15 @@
 
 class AlpacaPromptFmt(PromptFmt):
   @classmethod
   def ctx(cls, context):
     if context is None or context == "":
       return ""
     else:
-      return f"""### Input: {context}
+      return f"""### Input:{context}
 
 """
 
   @classmethod
   def prompt(cls, pingpong):
     return f"""### Instruction: {pingpong.ping}
 
@@ -20,32 +20,29 @@
 class AlpacaChatPPManager(PPManager):
   def add_ping(self, ping, fmt: PromptFmt=AlpacaPromptFmt):
     allowed = super().add_ping(ping, fmt)
 
     if allowed:
       prompts = f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.
 
-### Instruction:
-{ping}
+### Instruction:{ping}
 {fmt.ctx(self.ctx)}
-### Response:
-"""
+### Response:"""
       return prompts
 
     return None
 
 
   def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=AlpacaPromptFmt):
     if to_idx == -1 or to_idx >= len(self.pingpongs):
       to_idx = len(self.pingpongs)
 
-    results = fmt.ctx(self.ctx)
+    results = ""
 
     for idx, pingpong in enumerate(self.pingpongs[from_idx:to_idx]):
-      print(idx)
       results += fmt.prompt(pingpong)
 
       if from_idx+idx != to_idx-1:
         results += """
 
 """
```

## pingpong/dolly.py

```diff
@@ -26,15 +26,14 @@
 
     if allowed:
       prompts = f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.
 
 ### Instruction:
 {ping}
 {fmt.ctx(self.ctx)}
-
 """
       return prompts
 
     return None
 
   def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=DollyPromptFmt):
     if to_idx == -1 or to_idx >= len(self.pingpongs):
```

## pingpong/pingpong.py

```diff
@@ -27,19 +27,24 @@
 
   def add_ping(self, ping, fmt: PromptFmt):
     if len(self.pingpongs) == 0 \
       or (len(self.pingpongs) >= 1 and self.pingpongs[-1].pong is not None):
       self.pingpongs.append(PingPong(ping, None))
       return True
     return False
-    
 
   def add_pong(self, pong):
+    self.replace_last_pong(pong)
+
+  def replace_last_pong(self, pong):
     self.pingpongs[-1].pong = pong
 
+  def append_pong(self, piece_pong):
+    self.pingpongs[-1].pong += piece_pong
+
   def add_pingpong(self, pingpong):
     self.pingpongs.append(pingpong)
 
   def pop_pingpong(self):
     return self.pingpongs.pop()
 
   def build_prompts(self, from_idx: int, to_idx: int, fmt: PromptFmt):
```

## Comparing `bingbong-0.1.6.1.dist-info/LICENSE` & `bingbong-0.1.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.1.6.1.dist-info/METADATA` & `bingbong-0.1.6.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.6.1
+Version: 0.1.6.2
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `bingbong-0.1.6.1.dist-info/RECORD` & `bingbong-0.1.6.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-pingpong/__init__.py,sha256=1jl0ZrLU3Ib7hi-QqLJ1lqCFClS9k6oGsnk5qtYeyks,55
-pingpong/alpaca.py,sha256=C70bD8DJh1pDt1tvuwbVUPEMaI7wEu-gBJGSrRP_Eq0,1234
-pingpong/dolly.py,sha256=2xUJfdskS-a9SYbjUH1TAW4-oLxdkntqCmO5xEzW7Hg,1216
+pingpong/__init__.py,sha256=urOQF36qoe_DAoPImWQlUpY1lrQG0QiKV1yALpkTFlY,55
+pingpong/alpaca.py,sha256=3z9EnziOat6P9DzuBlDXPh8wU47IaAUrLz8Z27zrb3s,1199
+pingpong/dolly.py,sha256=jAWnieNLTPFzGNBI5hBaSIhx7XW0c7xGyO1PVGaBy9g,1215
 pingpong/gradio.py,sha256=IchvS_gOuPk3TCATVKDWMaLEaIRqjPpi3MFnYwa0JwU,987
-pingpong/pingpong.py,sha256=W4miUWWb0wGnFFl3sIHJpnrciMf-pbFh4da5KSBNoyQ,1046
+pingpong/pingpong.py,sha256=yQcXkdWc9aWem0vdbqtwMMvJXsqmLnwlSuGBkM4ZHk8,1192
 pingpong/context/__init__.py,sha256=ksYP7nq8inYK7SHDwpd7Hs_h87gPKdP9Ac6E5w0X6zM,173
 pingpong/context/auto_summary_strategy.py,sha256=s2lrlGKzLFNBGdLMAkaC6d2VY8aJSdgtrwa_Rvmt3Fc,589
 pingpong/context/last_window_strategy.py,sha256=37Gu94VVIMlj-pK3r7NMrOPp_XufMYsSthf5-ZJNw00,711
 pingpong/context/search_window_strategy.py,sha256=OPd2xxiI9FrzU4w2R5luaDEKiNEj4KYr_EF53Qi6l_Q,840
 pingpong/context/strategy.py,sha256=xGoy7T92gYubrwekz0Kz2Vxv10njgXG44K48bC9BqAU,119
-bingbong-0.1.6.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-bingbong-0.1.6.1.dist-info/METADATA,sha256=htAOtlVOPu971iWOi88V7HoKHiITdBrrF7M2HYZM1ZI,3348
-bingbong-0.1.6.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bingbong-0.1.6.1.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
-bingbong-0.1.6.1.dist-info/RECORD,,
+bingbong-0.1.6.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+bingbong-0.1.6.2.dist-info/METADATA,sha256=8O1yonxpEFHXis5NUuXPYhy2aV7x6FpQrE4p7Iaddu0,3348
+bingbong-0.1.6.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bingbong-0.1.6.2.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
+bingbong-0.1.6.2.dist-info/RECORD,,
```

