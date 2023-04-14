# Comparing `tmp/griptape_tools-0.5.1.tar.gz` & `tmp/griptape_tools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.5.1.tar", max compression
+gzip compressed data, was "griptape_tools-0.5.2.tar", max compression
```

## Comparing `griptape_tools-0.5.1.tar` & `griptape_tools-0.5.2.tar`

### file list

```diff
@@ -1,47 +1,30 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.5.1/LICENSE
--rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.5.1/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.5.1/griptape/__init__.py
--rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.5.1/griptape/tools/__init__.py
--rw-r--r--   0        0        0      499 2023-04-13 16:44:18.759766 griptape_tools-0.5.1/griptape/tools/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.1/griptape/tools/aws_cli/__init__.py
--rw-r--r--   0        0        0      161 2023-04-13 16:44:18.862164 griptape_tools-0.5.1/griptape/tools/aws_cli/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1729 2023-04-13 17:32:12.692546 griptape_tools-0.5.1/griptape/tools/aws_cli/__pycache__/tool.cpython-310.pyc
--rw-r--r--   0        0        0     1790 2023-04-13 17:00:19.874640 griptape_tools-0.5.1/griptape/tools/aws_cli/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.5.1/griptape/tools/aws_cli/manifest.yml
--rw-r--r--   0        0        0       78 2023-04-13 21:55:09.487715 griptape_tools-0.5.1/griptape/tools/aws_cli/requirements.txt
--rw-r--r--   0        0        0     1516 2023-04-13 16:56:09.699727 griptape_tools-0.5.1/griptape/tools/aws_cli/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.1/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      164 2023-04-07 15:56:04.337980 griptape_tools-0.5.1/griptape/tools/calculator/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1782 2023-04-11 19:13:20.365906 griptape_tools-0.5.1/griptape/tools/calculator/__pycache__/tool.cpython-310.pyc
--rw-r--r--   0        0        0     1052 2023-04-13 16:51:04.094631 griptape_tools-0.5.1/griptape/tools/calculator/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.5.1/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-13 21:55:09.483314 griptape_tools-0.5.1/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0      725 2023-04-13 16:45:31.204704 griptape_tools-0.5.1/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.1/griptape/tools/email_client/__init__.py
--rw-r--r--   0        0        0      166 2023-04-12 21:41:15.550396 griptape_tools-0.5.1/griptape/tools/email_client/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2195 2023-04-13 16:44:18.859633 griptape_tools-0.5.1/griptape/tools/email_client/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.5.1/griptape/tools/email_client/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-13 21:55:09.481296 griptape_tools-0.5.1/griptape/tools/email_client/requirements.txt
--rw-r--r--   0        0        0     2354 2023-04-13 16:12:25.314046 griptape_tools-0.5.1/griptape/tools/email_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.1/griptape/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      164 2023-04-12 20:32:26.158552 griptape_tools-0.5.1/griptape/tools/sql_client/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1895 2023-04-13 16:51:04.196419 griptape_tools-0.5.1/griptape/tools/sql_client/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.5.1/griptape/tools/sql_client/manifest.yml
--rw-r--r--   0        0        0       33 2023-04-13 21:55:09.486224 griptape_tools-0.5.1/griptape/tools/sql_client/requirements.txt
--rw-r--r--   0        0        0     1328 2023-04-13 16:45:31.207393 griptape_tools-0.5.1/griptape/tools/sql_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.1/griptape/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      165 2023-04-12 16:01:57.738417 griptape_tools-0.5.1/griptape/tools/web_scraper/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3931 2023-04-13 20:35:47.051663 griptape_tools-0.5.1/griptape/tools/web_scraper/__pycache__/tool.cpython-310.pyc
--rw-r--r--   0        0        0     3994 2023-04-13 15:56:54.679897 griptape_tools-0.5.1/griptape/tools/web_scraper/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.5.1/griptape/tools/web_scraper/manifest.yml
--rw-r--r--   0        0        0       53 2023-04-13 21:55:09.484886 griptape_tools-0.5.1/griptape/tools/web_scraper/requirements.txt
--rw-r--r--   0        0        0     4506 2023-04-13 15:55:25.582021 griptape_tools-0.5.1/griptape/tools/web_scraper/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.1/griptape/tools/web_search/__init__.py
--rw-r--r--   0        0        0      167 2023-04-07 15:56:04.338570 griptape_tools-0.5.1/griptape/tools/web_search/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2374 2023-04-10 14:23:53.062035 griptape_tools-0.5.1/griptape/tools/web_search/__pycache__/tool.cpython-310.pyc
--rw-r--r--   0        0        0     2423 2023-04-12 19:48:43.940734 griptape_tools-0.5.1/griptape/tools/web_search/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.5.1/griptape/tools/web_search/manifest.yml
--rw-r--r--   0        0        0       29 2023-04-13 21:55:09.489187 griptape_tools-0.5.1/griptape/tools/web_search/requirements.txt
--rw-r--r--   0        0        0     2332 2023-04-12 19:48:33.963528 griptape_tools-0.5.1/griptape/tools/web_search/tool.py
--rw-r--r--   0        0        0      526 2023-04-13 21:56:28.623300 griptape_tools-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.5.2/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.5.2/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.5.2/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.2/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.5.2/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       78 2023-04-13 21:55:09.487715 griptape_tools-0.5.2/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1516 2023-04-13 16:56:09.699727 griptape_tools-0.5.2/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.2/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.5.2/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-13 21:55:09.483314 griptape_tools-0.5.2/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      725 2023-04-13 16:45:31.204704 griptape_tools-0.5.2/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.2/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.5.2/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-13 21:55:09.481296 griptape_tools-0.5.2/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     2409 2023-04-14 19:59:52.372885 griptape_tools-0.5.2/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.2/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.5.2/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       33 2023-04-13 21:55:09.486224 griptape_tools-0.5.2/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1328 2023-04-13 16:45:31.207393 griptape_tools-0.5.2/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.2/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.5.2/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       53 2023-04-13 21:55:09.484886 griptape_tools-0.5.2/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     4506 2023-04-13 15:55:25.582021 griptape_tools-0.5.2/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.2/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.5.2/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       29 2023-04-13 21:55:09.489187 griptape_tools-0.5.2/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2332 2023-04-12 19:48:33.963528 griptape_tools-0.5.2/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      526 2023-04-14 20:00:46.071902 griptape_tools-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.5.2/PKG-INFO
```

### Comparing `griptape_tools-0.5.1/LICENSE` & `griptape_tools-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.1/README.md` & `griptape_tools-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.1/griptape/tools/aws_cli/tool.py` & `griptape_tools-0.5.2/griptape/tools/aws_cli/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.1/griptape/tools/calculator/tool.py` & `griptape_tools-0.5.2/griptape/tools/calculator/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.1/griptape/tools/email_client/tool.py` & `griptape_tools-0.5.2/griptape/tools/email_client/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import json
+import ast
+import logging
 import smtplib
-import ssl
-from email.message import EmailMessage
+from email.mime.text import MIMEText
 from typing import Optional
 from attr import define, field
 from griptape.core import BaseTool, action
 from schema import Schema, Literal
 
 
 @define
@@ -34,37 +34,39 @@
                     description="Email body"
                 ): str
             }
         })
     })
     def send(self, value: bytes) -> str:
         server: Optional[smtplib.SMTP] = None
-        params = json.loads(value.decode())
+        params = ast.literal_eval(value.decode())
+        host = self.env_value("SMTP_HOST")
+        port = int(self.env_value("SMTP_PORT"))
         to_email = params["to"]
+        from_email = self.env_value("FROM_EMAIL")
         subject = params["subject"]
-        body = params["body"]
-        msg = EmailMessage()
-
-        msg['Subject'] = subject
-        msg['From'] = self.env_value("FROM_EMAIL")
-        msg['To'] = to_email
+        password = self.env_value("SMTP_PASSWORD")
+        msg = MIMEText(params["body"])
 
         try:
-            server = smtplib.SMTP(self.env_value("SMTP_HOST"), int(self.env_value("SMTP_PORT")))
-
             if self.env_value("SMTP_USE_SSL") == "True":
-                server.starttls(context=ssl.create_default_context())
+                server = smtplib.SMTP_SSL(host, port)
+            else:
+                server = smtplib.SMTP(host, port)
+
+            msg["Subject"] = subject
+            msg["From"] = from_email
+            msg["To"] = to_email
 
-            if self.env_value("SMTP_PASSWORD") != "":
-                server.login(self.env_value("FROM_EMAIL"), self.env_value("SMTP_PASSWORD"))
-
-            msg.set_content(body)
-            server.send_message(msg)
+            server.login(from_email, password)
+            server.sendmail(from_email, [to_email], msg.as_string())
 
             return "email was successfully sent"
         except Exception as e:
+            logging.error(e)
+
             return f"error sending email: {e}"
         finally:
             try:
                 server.quit()
             except:
                 pass
```

### Comparing `griptape_tools-0.5.1/griptape/tools/sql_client/tool.py` & `griptape_tools-0.5.2/griptape/tools/sql_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.1/griptape/tools/web_scraper/tool.py` & `griptape_tools-0.5.2/griptape/tools/web_scraper/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.1/griptape/tools/web_search/tool.py` & `griptape_tools-0.5.2/griptape/tools/web_search/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.1/pyproject.toml` & `griptape_tools-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.5.1"
+version = "0.5.2"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
```

### Comparing `griptape_tools-0.5.1/PKG-INFO` & `griptape_tools-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

