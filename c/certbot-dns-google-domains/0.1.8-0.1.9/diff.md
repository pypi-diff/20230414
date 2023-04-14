# Comparing `tmp/certbot_dns_google_domains-0.1.8.tar.gz` & `tmp/certbot_dns_google_domains-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot_dns_google_domains-0.1.8.tar", max compression
+gzip compressed data, was "certbot_dns_google_domains-0.1.9.tar", max compression
```

## Comparing `certbot_dns_google_domains-0.1.8.tar` & `certbot_dns_google_domains-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11340 2023-03-21 02:13:40.890438 certbot_dns_google_domains-0.1.8/LICENSE
--rw-r--r--   0        0        0     3514 2023-03-21 02:13:40.890438 certbot_dns_google_domains-0.1.8/README.md
--rw-r--r--   0        0        0      656 2023-03-21 02:13:40.890438 certbot_dns_google_domains-0.1.8/certbot_dns_google_domains/__init__.py
--rw-r--r--   0        0        0     6286 2023-03-21 02:13:40.890438 certbot_dns_google_domains-0.1.8/certbot_dns_google_domains/dns_google_domains.py
--rw-r--r--   0        0        0     2032 2023-03-21 02:13:40.890438 certbot_dns_google_domains-0.1.8/certbot_dns_google_domains/test_dns_google_domains.py
--rw-r--r--   0        0        0      788 2023-03-21 02:13:40.890438 certbot_dns_google_domains-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 certbot_dns_google_domains-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-03-24 23:23:00.828058 certbot_dns_google_domains-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3514 2023-03-24 23:23:00.828058 certbot_dns_google_domains-0.1.9/README.md
+-rw-r--r--   0        0        0      656 2023-03-24 23:23:00.828058 certbot_dns_google_domains-0.1.9/certbot_dns_google_domains/__init__.py
+-rw-r--r--   0        0        0     6296 2023-03-24 23:23:00.828058 certbot_dns_google_domains-0.1.9/certbot_dns_google_domains/dns_google_domains.py
+-rw-r--r--   0        0        0     2032 2023-03-24 23:23:00.828058 certbot_dns_google_domains-0.1.9/certbot_dns_google_domains/test_dns_google_domains.py
+-rw-r--r--   0        0        0      788 2023-03-24 23:23:00.828058 certbot_dns_google_domains-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 certbot_dns_google_domains-0.1.9/PKG-INFO
```

### Comparing `certbot_dns_google_domains-0.1.8/LICENSE` & `certbot_dns_google_domains-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot_dns_google_domains-0.1.8/README.md` & `certbot_dns_google_domains-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `certbot_dns_google_domains-0.1.8/certbot_dns_google_domains/__init__.py` & `certbot_dns_google_domains-0.1.9/certbot_dns_google_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_google_domains-0.1.8/certbot_dns_google_domains/dns_google_domains.py` & `certbot_dns_google_domains-0.1.9/certbot_dns_google_domains/dns_google_domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     keep_expired_records: bool = False
 
 
 @dataclass
 class AcmeChallengeSet(DataClassJsonMixin):
     dataclass_json_config = config(letter_case=LetterCase.CAMEL)[
         "dataclasses_json"]
-    record: List[AcmeTxtRecord]
+    record: Optional[List[AcmeTxtRecord]]
 
 
 class GDSApi:
     ROTATE_CHALLENGES: str = "https://acmedns.googleapis.com/v1/acmeChallengeSets/{domain}:rotateChallenges"
     DEFAULT_TIMEOUT: int = 30  # 30 seconds timeout
     access_token: str
```

### Comparing `certbot_dns_google_domains-0.1.8/certbot_dns_google_domains/test_dns_google_domains.py` & `certbot_dns_google_domains-0.1.9/certbot_dns_google_domains/test_dns_google_domains.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_google_domains-0.1.8/pyproject.toml` & `certbot_dns_google_domains-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "certbot-dns-google-domains"
-version = "0.1.8"
+version = "0.1.9"
 description = "Certbot DNS authenticator for Google Domains"
 authors = ["Amir Omidi <amir@aaomidi.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 include = [
   "LICENSE",
 ]
```

### Comparing `certbot_dns_google_domains-0.1.8/PKG-INFO` & `certbot_dns_google_domains-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-google-domains
-Version: 0.1.8
+Version: 0.1.9
 Summary: Certbot DNS authenticator for Google Domains
 License: Apache 2.0
 Author: Amir Omidi
 Author-email: amir@aaomidi.com
 Requires-Python: >=3.7.2
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

