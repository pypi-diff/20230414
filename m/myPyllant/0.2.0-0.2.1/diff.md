# Comparing `tmp/mypyllant-0.2.0.tar.gz` & `tmp/mypyllant-0.2.1.tar.gz`

## Comparing `mypyllant-0.2.0.tar` & `mypyllant-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.2.0/logo.png
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mypyllant-0.2.0/requirements-dev.txt
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.2.0/setup.cfg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.2.0/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    15218 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/api.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/export.py
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/models.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/conftest.py
--rwxr-xr-x   0        0        0      784 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/find_countries.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/generate_test_data.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/test_api.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/test_countries.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/test_generate_test_data.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.2.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.2.0/LICENSE
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 mypyllant-0.2.0/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 mypyllant-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.2.1/logo.png
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mypyllant-0.2.1/requirements-dev.txt
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.2.1/setup.cfg
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.2.1/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    15560 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/api.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/export.py
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/models.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/conftest.py
+-rwxr-xr-x   0        0        0      784 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/find_countries.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/generate_test_data.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/test_api.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/test_countries.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 mypyllant-0.2.1/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 mypyllant-0.2.1/PKG-INFO
```

### Comparing `mypyllant-0.2.0/.pre-commit-config.yaml` & `mypyllant-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/logo.png` & `mypyllant-0.2.1/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/setup.cfg` & `mypyllant-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/.github/workflows/build-test.yaml` & `mypyllant-0.2.1/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/src/myPyllant/api.py` & `mypyllant-0.2.1/src/myPyllant/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import datetime
 from html import unescape
 import logging
 import re
 from urllib.parse import parse_qs, urlencode, urlparse
 
 import aiohttp
+from aiohttp import ClientResponseError
 
 from myPyllant.const import (
     API_URL_BASE,
     AUTHENTICATE_URL,
     BRANDS,
     CLIENT_ID,
     COUNTRIES,
@@ -35,14 +36,18 @@
 logger = logging.getLogger(__name__)
 
 
 class AuthenticationFailed(ConnectionError):
     pass
 
 
+class LoginEndpointInvalid(ConnectionError):
+    pass
+
+
 async def on_request_start(session, context, params: aiohttp.TraceRequestStartParams):
     """
     See https://docs.aiohttp.org/en/stable/tracing_reference.html#aiohttp.TraceConfig.on_request_start
     """
     logger.debug(f"Starting request {params}")
 
 
@@ -105,37 +110,42 @@
             "code": "code_challenge",
             "redirect_uri": "enduservaillant.page.link://login",
             "code_challenge_method": "S256",
             "code_challenge": code_challenge,
         }
 
         # Grabbing the login URL from the HTML form of the login page
-        async with self.aiohttp_session.get(
-            AUTHENTICATE_URL.format(country=self.country, brand=self.brand)
-            + "?"
-            + urlencode(auth_querystring)
-        ) as resp:
-            login_html = await resp.text()
+        try:
+            async with self.aiohttp_session.get(
+                AUTHENTICATE_URL.format(country=self.country, brand=self.brand)
+                + "?"
+                + urlencode(auth_querystring)
+            ) as resp:
+                login_html = await resp.text()
+        except ClientResponseError as e:
+            raise LoginEndpointInvalid from e
 
         result = re.search(
             LOGIN_URL.format(country=self.country, brand=self.brand) + r"\?([^\"]*)",
             login_html,
         )
         login_url = unescape(result.group())
 
+        logger.debug(f"Got login url {login_url}")
+
         login_payload = {
             "username": self.username,
             "password": self.password,
             "credentialId": "",
         }
-
         # Obtaining the code
         async with self.aiohttp_session.post(
             login_url, data=login_payload, allow_redirects=False
         ) as resp:
+            logger.debug(f"Got login response headers {resp.headers}")
             if "Location" not in resp.headers:
                 raise AuthenticationFailed("Login failed")
             logger.debug(
                 f'Got location from authorize endpoint: {resp.headers["Location"]}'
             )
             parsed_url = urlparse(resp.headers["Location"])
             code = parse_qs(parsed_url.query)["code"]
```

### Comparing `mypyllant-0.2.0/src/myPyllant/const.py` & `mypyllant-0.2.1/src/myPyllant/const.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/src/myPyllant/export.py` & `mypyllant-0.2.1/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/src/myPyllant/models.py` & `mypyllant-0.2.1/src/myPyllant/models.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/src/myPyllant/sample.py` & `mypyllant-0.2.1/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/src/myPyllant/utils.py` & `mypyllant-0.2.1/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/conftest.py` & `mypyllant-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/find_countries.py` & `mypyllant-0.2.1/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/generate_test_data.py` & `mypyllant-0.2.1/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/test_api.py` & `mypyllant-0.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/test_generate_test_data.py` & `mypyllant-0.2.1/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json` & `mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json` & `mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json` & `mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json` & `mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json` & `mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json` & `mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/.gitignore` & `mypyllant-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/LICENSE` & `mypyllant-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/README.md` & `mypyllant-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/pyproject.toml` & `mypyllant-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.0/PKG-INFO` & `mypyllant-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

