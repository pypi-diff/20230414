# Comparing `tmp/sectxt-0.8.1.tar.gz` & `tmp/sectxt-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sectxt-0.8.1.tar", last modified: Wed Feb 22 08:19:36 2023, max compression
+gzip compressed data, was "sectxt-0.8.2.tar", last modified: Fri Apr 14 08:14:18 2023, max compression
```

## Comparing `sectxt-0.8.1.tar` & `sectxt-0.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 08:19:36.610770 sectxt-0.8.1/
--rw-rw-rw-   0        0        0    13827 2023-02-22 08:18:47.000000 sectxt-0.8.1/LICENCE
--rw-rw-rw-   0        0        0    10136 2023-02-22 08:19:36.610770 sectxt-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     9090 2023-02-22 08:18:47.000000 sectxt-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-22 08:19:36.555769 sectxt-0.8.1/sectxt/
--rw-rw-rw-   0        0        0    15885 2023-02-22 08:18:47.000000 sectxt-0.8.1/sectxt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:19:36.595772 sectxt-0.8.1/sectxt.egg-info/
--rw-rw-rw-   0        0        0    10136 2023-02-22 08:19:36.000000 sectxt-0.8.1/sectxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-02-22 08:19:36.000000 sectxt-0.8.1/sectxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 08:19:36.000000 sectxt-0.8.1/sectxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-02-22 08:19:36.000000 sectxt-0.8.1/sectxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-22 08:19:36.000000 sectxt-0.8.1/sectxt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-22 08:19:35.000000 sectxt-0.8.1/sectxt.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1021 2023-02-22 08:19:36.612770 sectxt-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0       60 2023-02-22 08:18:47.000000 sectxt-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:19:36.609768 sectxt-0.8.1/test/
--rw-rw-rw-   0        0        0     7170 2023-02-22 08:18:47.000000 sectxt-0.8.1/test/test_sectxt.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:14:18.023958 sectxt-0.8.2/
+-rw-rw-rw-   0        0        0    13827 2023-04-14 07:57:53.000000 sectxt-0.8.2/LICENCE
+-rw-rw-rw-   0        0        0    10927 2023-04-14 08:14:18.024885 sectxt-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9876 2023-04-14 07:57:53.000000 sectxt-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 08:14:17.985293 sectxt-0.8.2/sectxt/
+-rw-rw-rw-   0        0        0    17312 2023-04-14 07:57:53.000000 sectxt-0.8.2/sectxt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:14:18.020958 sectxt-0.8.2/sectxt.egg-info/
+-rw-rw-rw-   0        0        0    10927 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1021 2023-04-14 08:14:18.027878 sectxt-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0       60 2023-04-14 07:57:53.000000 sectxt-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:14:18.021956 sectxt-0.8.2/test/
+-rw-rw-rw-   0        0        0     9029 2023-04-14 07:57:53.000000 sectxt-0.8.2/test/test_sectxt.py
```

### Comparing `sectxt-0.8.1/LICENCE` & `sectxt-0.8.2/LICENCE`

 * *Files identical despite different names*

### Comparing `sectxt-0.8.1/PKG-INFO` & `sectxt-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectxt
-Version: 0.8.1
+Version: 0.8.2
 Summary: security.txt parser and validator
 Author: DigitalTrustCenter
 Author-email: algemeen@digitaltrustcenter.nl
 License: EUPL-1.2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -66,60 +66,65 @@
 |---------|------------------------------------------------------------------------------------------------------------|
 | code    | A fixed error code string                                                                                  |
 | message | A human readable error message in English                                                                  |
 | line    | The 1 based integer line number where the error occurred or None when the error applies to the entire file |
 
 ### Possible errors
 
-| code                 | message                                                                                                                                                                |
-|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| "no_security_txt"    | "security.txt could not be located."                                                                                                                                   |
-| "location"           | "security.txt was located on the top-level path (legacy place), but must be placed under the '/.well-known/' path."                                                    |
-| "invalid_uri_scheme" | "Insecure URI scheme HTTP is not allowed. The security.txt file access must use the HTTPS scheme"                                                                      |
-| "invalid_cert"       | "security.txt must be served with a valid TLS certificate."                                                                                                            |
-| "no_content_type"    | "HTTP Content-Type header must be sent."                                                                                                                               |
-| "invalid_media"      | "Media type in Content-Type header must be 'text/plain'."                                                                                                              |
-| "invalid_charset"    | "Charset parameter in Content-Type header must be 'utf-8' if present."                                                                                                 |
-| "utf8"               | "Content must be utf-8 encoded."                                                                                                                                       |
-| "no_expire"          | "'Expires' field must be present."                                                                                                                                     |
-| "multi_expire"       | "'Expires' field must not appear more than once."                                                                                                                      |
-| "invalid_expiry"     | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
-| "expired"            | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
-| "no_contact"         | "'Contact' field must appear at least once."                                                                                                                           |
-| "no_canonical_match" | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
-| "multi_lang"         | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
-| "invalid_lang"       | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
-| "no_uri"             | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
-| "no_https"           | "Web URI must begin with 'https://'."                                                                                                                                  |
-| "prec_ws"            | "There must be no whitespace before the field separator (colon)."                                                                                                      |
-| "no_space"           | "Field separator (colon) must be followed by a space."                                                                                                                 | 
-| "empty_key"          | "Field name must not be empty."                                                                                                                                        |
-| "empty_value"        | "Field value must not be empty."                                                                                                                                       |
-| "invalid_line"       | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
-| "no_line_separators" | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
-| "signed_format_issue"| "Signed security.txt files must start with the begin pgp signed message as the document header"                                                                        |
+| code                  | message                                                                                                                                                                |
+|-----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| "no_security_txt"     | "security.txt could not be located."                                                                                                                                   |
+| "location"            | "security.txt was located on the top-level path (legacy place), but must be placed under the '/.well-known/' path."                                                    |
+| "invalid_uri_scheme"  | "Insecure URI scheme HTTP is not allowed. The security.txt file access must use the HTTPS scheme"                                                                      |
+| "invalid_cert"        | "security.txt must be served with a valid TLS certificate."                                                                                                            |
+| "no_content_type"     | "HTTP Content-Type header must be sent."                                                                                                                               |
+| "invalid_media"       | "Media type in Content-Type header must be 'text/plain'."                                                                                                              |
+| "invalid_charset"     | "Charset parameter in Content-Type header must be 'utf-8' if present."                                                                                                 |
+| "utf8"                | "Content must be utf-8 encoded."                                                                                                                                       |
+| "no_expire"           | "'Expires' field must be present."                                                                                                                                     |
+| "multi_expire"        | "'Expires' field must not appear more than once."                                                                                                                      |
+| "invalid_expiry"      | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
+| "expired"             | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
+| "no_contact"          | "'Contact' field must appear at least once."                                                                                                                           |
+| "no_canonical_match"  | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
+| "multi_lang"          | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
+| "invalid_lang"        | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
+| "no_uri"              | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
+| "no_https"            | "Web URI must begin with 'https://'."                                                                                                                                  |
+| "prec_ws"             | "There must be no whitespace before the field separator (colon)."                                                                                                      |
+| "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
+| "empty_key"           | "Field name must not be empty."                                                                                                                                        |
+| "empty_value"         | "Field value must not be empty."                                                                                                                                       |
+| "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
+| "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
+| "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
+| "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
+| "no_csaf_file"        | "All CSAF field in the security.txt must point to a provider-metadata.json file"                                                                                       |
+
 
 ### Possible recommendations
 
-| code                       | message                                                                                                  |
-|----------------------------|----------------------------------------------------------------------------------------------------------|
-| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                           |
-| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address."                   |
-| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                                               |
-| "no_canonical"             | "'Canonical' field should be present in a signed file."                                                  |
+| code                       | message                                                                                |
+|----------------------------|----------------------------------------------------------------------------------------|
+| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."         |
+| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address." |
+| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                             |
+| "no_canonical"             | "'Canonical' field should be present in a signed file."                                |
+| "no_csaf"                  | "'CSAF' field should appear at least once"                                             |
 
 ### Possible notifications
 
-| code                          | message                                                                                                  |
-|-------------------------------|----------------------------------------------------------------------------------------------------------|
-| "unknown_field"<sup>[2]</sup> | "security.txt contains an unknown field. Either this is a custom field which may not be widely supported, or there is a typo in a standardised field name." |
+| code                          | message                                                                                                                                                                     |
+|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
+| "multiple_csaf_fields"        | "It is allowed to have more than one CSAF field, however this should be removed if possible."                                                                               |
 
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
-[2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported should be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
+[2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
 
 >>> from sectxt import SecurityTXT
 >>> s = SecurityTXT("www.example.com", recommend_unknown_fields=False)
 ```
```

### Comparing `sectxt-0.8.1/README.md` & `sectxt-0.8.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -42,60 +42,65 @@
 |---------|------------------------------------------------------------------------------------------------------------|
 | code    | A fixed error code string                                                                                  |
 | message | A human readable error message in English                                                                  |
 | line    | The 1 based integer line number where the error occurred or None when the error applies to the entire file |
 
 ### Possible errors
 
-| code                 | message                                                                                                                                                                |
-|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| "no_security_txt"    | "security.txt could not be located."                                                                                                                                   |
-| "location"           | "security.txt was located on the top-level path (legacy place), but must be placed under the '/.well-known/' path."                                                    |
-| "invalid_uri_scheme" | "Insecure URI scheme HTTP is not allowed. The security.txt file access must use the HTTPS scheme"                                                                      |
-| "invalid_cert"       | "security.txt must be served with a valid TLS certificate."                                                                                                            |
-| "no_content_type"    | "HTTP Content-Type header must be sent."                                                                                                                               |
-| "invalid_media"      | "Media type in Content-Type header must be 'text/plain'."                                                                                                              |
-| "invalid_charset"    | "Charset parameter in Content-Type header must be 'utf-8' if present."                                                                                                 |
-| "utf8"               | "Content must be utf-8 encoded."                                                                                                                                       |
-| "no_expire"          | "'Expires' field must be present."                                                                                                                                     |
-| "multi_expire"       | "'Expires' field must not appear more than once."                                                                                                                      |
-| "invalid_expiry"     | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
-| "expired"            | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
-| "no_contact"         | "'Contact' field must appear at least once."                                                                                                                           |
-| "no_canonical_match" | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
-| "multi_lang"         | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
-| "invalid_lang"       | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
-| "no_uri"             | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
-| "no_https"           | "Web URI must begin with 'https://'."                                                                                                                                  |
-| "prec_ws"            | "There must be no whitespace before the field separator (colon)."                                                                                                      |
-| "no_space"           | "Field separator (colon) must be followed by a space."                                                                                                                 | 
-| "empty_key"          | "Field name must not be empty."                                                                                                                                        |
-| "empty_value"        | "Field value must not be empty."                                                                                                                                       |
-| "invalid_line"       | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
-| "no_line_separators" | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
-| "signed_format_issue"| "Signed security.txt files must start with the begin pgp signed message as the document header"                                                                        |
+| code                  | message                                                                                                                                                                |
+|-----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| "no_security_txt"     | "security.txt could not be located."                                                                                                                                   |
+| "location"            | "security.txt was located on the top-level path (legacy place), but must be placed under the '/.well-known/' path."                                                    |
+| "invalid_uri_scheme"  | "Insecure URI scheme HTTP is not allowed. The security.txt file access must use the HTTPS scheme"                                                                      |
+| "invalid_cert"        | "security.txt must be served with a valid TLS certificate."                                                                                                            |
+| "no_content_type"     | "HTTP Content-Type header must be sent."                                                                                                                               |
+| "invalid_media"       | "Media type in Content-Type header must be 'text/plain'."                                                                                                              |
+| "invalid_charset"     | "Charset parameter in Content-Type header must be 'utf-8' if present."                                                                                                 |
+| "utf8"                | "Content must be utf-8 encoded."                                                                                                                                       |
+| "no_expire"           | "'Expires' field must be present."                                                                                                                                     |
+| "multi_expire"        | "'Expires' field must not appear more than once."                                                                                                                      |
+| "invalid_expiry"      | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
+| "expired"             | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
+| "no_contact"          | "'Contact' field must appear at least once."                                                                                                                           |
+| "no_canonical_match"  | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
+| "multi_lang"          | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
+| "invalid_lang"        | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
+| "no_uri"              | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
+| "no_https"            | "Web URI must begin with 'https://'."                                                                                                                                  |
+| "prec_ws"             | "There must be no whitespace before the field separator (colon)."                                                                                                      |
+| "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
+| "empty_key"           | "Field name must not be empty."                                                                                                                                        |
+| "empty_value"         | "Field value must not be empty."                                                                                                                                       |
+| "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
+| "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
+| "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
+| "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
+| "no_csaf_file"        | "All CSAF field in the security.txt must point to a provider-metadata.json file"                                                                                       |
+
 
 ### Possible recommendations
 
-| code                       | message                                                                                                  |
-|----------------------------|----------------------------------------------------------------------------------------------------------|
-| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                           |
-| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address."                   |
-| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                                               |
-| "no_canonical"             | "'Canonical' field should be present in a signed file."                                                  |
+| code                       | message                                                                                |
+|----------------------------|----------------------------------------------------------------------------------------|
+| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."         |
+| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address." |
+| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                             |
+| "no_canonical"             | "'Canonical' field should be present in a signed file."                                |
+| "no_csaf"                  | "'CSAF' field should appear at least once"                                             |
 
 ### Possible notifications
 
-| code                          | message                                                                                                  |
-|-------------------------------|----------------------------------------------------------------------------------------------------------|
-| "unknown_field"<sup>[2]</sup> | "security.txt contains an unknown field. Either this is a custom field which may not be widely supported, or there is a typo in a standardised field name." |
+| code                          | message                                                                                                                                                                     |
+|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
+| "multiple_csaf_fields"        | "It is allowed to have more than one CSAF field, however this should be removed if possible."                                                                               |
 
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
-[2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported should be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
+[2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
 
 >>> from sectxt import SecurityTXT
 >>> s = SecurityTXT("www.example.com", recommend_unknown_fields=False)
 ```
```

### Comparing `sectxt-0.8.1/sectxt/__init__.py` & `sectxt-0.8.2/sectxt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 import dateutil.parser
 import requests
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 s = requests.Session()
 
 
 class ErrorDict(TypedDict):
     code: str
     message: str
@@ -31,45 +31,52 @@
 
 class LineDict(TypedDict):
     type: str
     field_name: Optional[str]
     value: str
 
 
-def strlist_from_arg(
-        arg: Union[str, List[str], None]) -> Union[List[str], None]:
+def strlist_from_arg(arg: Union[str, List[str], None]) -> Union[List[str], None]:
     if isinstance(arg, str):
         return [arg]
     return arg
 
 
 PREFERRED_LANGUAGES = "preferred-languages"
 
 
 class Parser:
     iso8601_re = re.compile(
         r"\d{4}-\d{2}-\d{2}[T ]\d{2}:\d{2}:\d{2}(\.\d+)?(Z|[-+]\d{2}:\d{2})$",
-        re.IGNORECASE | re.ASCII)
+        re.IGNORECASE | re.ASCII,
+    )
 
     uri_fields = [
-        "acknowledgments", "canonical", "contact", "encryption", "hiring",
-        "policy"]
+        "acknowledgments",
+        "canonical",
+        "contact",
+        "encryption",
+        "hiring",
+        "policy",
+        "csaf",
+    ]
 
     known_fields = uri_fields + [PREFERRED_LANGUAGES, "expires"]
 
     def __init__(
-            self,
-            content: str,
-            urls: Optional[str] = None,
-            recommend_unknown_fields: bool = True,
+        self,
+        content: str,
+        urls: Optional[str] = None,
+        recommend_unknown_fields: bool = True,
     ):
         self._urls = strlist_from_arg(urls)
         self._line_info: List[LineDict] = []
         self._errors: List[ErrorDict] = []
         self._recommendations: List[ErrorDict] = []
+        self._notifications: List[ErrorDict] = []
         self._values: DefaultDict[str, List[str]] = defaultdict(list)
         self._langs: Optional[List[str]] = None
         self._signed = False
         self._reading_sig = False
         self._finished_sig = False
         self._content = content
         self.recommend_unknown_fields = recommend_unknown_fields
@@ -82,53 +89,64 @@
         for line in lines:
             self._line_info.append(self._parse_line(line))
             self._line_no += 1
         self._line_no = None
         self.validate_contents()
 
     def _add_error(
-            self,
-            code: str,
-            message: str,
+        self,
+        code: str,
+        message: str,
     ) -> None:
-        err_dict: ErrorDict = {
-            "code": code, "message": message, "line": self._line_no}
+        err_dict: ErrorDict = {"code": code, "message": message, "line": self._line_no}
         self._errors.append(err_dict)
 
     def _add_recommendation(
-            self,
-            code: str,
-            message: str,
+        self,
+        code: str,
+        message: str,
     ) -> None:
-        err_dict: ErrorDict = {
-            "code": code, "message": message, "line": self._line_no}
+        err_dict: ErrorDict = {"code": code, "message": message, "line": self._line_no}
         self._recommendations.append(err_dict)
 
+    def _add_notification(
+        self,
+        code: str,
+        message: str,
+    ) -> None:
+        err_dict: ErrorDict = {"code": code, "message": message, "line": self._line_no}
+        self._notifications.append(err_dict)
+
     def _parse_line(self, line: str) -> LineDict:
         line = line.rstrip()
 
         if self._reading_sig:
             if line == "-----END PGP SIGNATURE-----":
                 self._reading_sig = False
                 self._finished_sig = True
             return {"type": "pgp_envelope", "field_name": None, "value": line}
 
         if line and self._finished_sig:
-            self._add_error("data_after_sig", "Data exists after signature")
+            self._add_error(
+                "data_after_sig",
+                "Signed security.txt must not contain data after the signature.",
+            )
             return {"type": "error", "field_name": None, "value": line}
 
         # signed content might be dash escaped
         if self._signed and not self._reading_sig and line.startswith("- "):
             line = line[2:]
 
         if line == "-----BEGIN PGP SIGNED MESSAGE-----":
             if self._line_no != 1:
                 self._add_error(
                     "signed_format_issue",
-                    "Signed security.txt files must start with the begin pgp signed message as the document header")
+                    "Signed security.txt must start with the header "
+                    "'-----BEGIN PGP SIGNED MESSAGE-----'.",
+                )
             self._signed = True
             return {"type": "pgp_envelope", "field_name": None, "value": line}
 
         if line == "-----BEGIN PGP SIGNATURE-----" and self._signed:
             self._reading_sig = True
             return {"type": "pgp_envelope", "field_name": None, "value": line}
 
@@ -138,181 +156,214 @@
         if ":" in line:
             return self._parse_field(line)
 
         if line:
             self._add_error(
                 "invalid_line",
                 "Line must contain a field name and value, "
-                "unless the line is blank or contains a comment.")
+                "unless the line is blank or contains a comment.",
+            )
             return {"type": "error", "value": line, "field_name": None}
 
         return {"type": "empty", "value": "", "field_name": None}
 
     def _parse_field(self, line: str) -> LineDict:
         key, value = line.split(":", 1)
         key = key.lower()
         if key.rstrip() != key:
             self._add_error(
                 "prec_ws",
-                "There must be no whitespace before the field separator "
-                "(colon).")
+                "There must be no whitespace before the field separator (colon).",
+            )
             key = key.rstrip()
 
         if value:
             if value[0] != " ":
                 self._add_error(
-                    "no_space",
-                    "Field separator (colon) must be followed by a space.")
+                    "no_space", "Field separator (colon) must be followed by a space."
+                )
             value = value.lstrip()
 
         if key == "hash" and self._signed:
             return {"type": "pgp_envelope", "field_name": None, "value": line}
 
         if not key:
             self._add_error("empty_key", "Field name must not be empty.")
             return {"type": "error", "value": line, "field_name": None}
 
         if not value:
-            self._add_error(
-                "empty_value", "Field value must not be empty.")
+            self._add_error("empty_value", "Field value must not be empty.")
             return {"type": "error", "value": line, "field_name": None}
 
         if key in self.uri_fields:
             url_parts = urlsplit(value)
             if url_parts.scheme == "":
                 self._add_error(
-                    "no_uri", "Field value must be a URI "
-                              "(e.g. beginning with 'mailto:').")
+                    "no_uri",
+                    "Field value must be a URI (e.g. beginning with 'mailto:').",
+                )
             elif url_parts.scheme == "http":
-                self._add_error(
-                    "no_https",
-                    "Web URI must begin with 'https://'.")
+                self._add_error("no_https", "Web URI must begin with 'https://'.")
         elif key == "expires":
             self._parse_expires(value)
         elif key == PREFERRED_LANGUAGES:
             self._langs = [v.strip() for v in value.split(",")]
 
             # Check if all the languages are valid according to RFC5646.
             for lang in self._langs:
                 if not langcodes.tag_is_valid(lang):
                     self._add_error(
                         "invalid_lang",
                         "Value in 'Preferred-Languages' field must match one "
                         "or more language tags as defined in RFC5646, "
-                        "separated by commas.")
+                        "separated by commas.",
+                    )
 
-        if self.recommend_unknown_fields and not key in self.known_fields:
-            self._add_recommendation(
+        if self.recommend_unknown_fields and key not in self.known_fields:
+            self._add_notification(
                 "unknown_field",
-                "security.txt contains an unknown field. "
-                "Either this is a custom field which may not be widely "
-                "supported, or there is a typo in a standardised field name.")
+                "Security.txt contains an unknown field. "
+                'Field "%s" is either a custom field which may not be widely '
+                "supported, or there is a typo in a standardised field name." % key,
+            )
 
         self._values[key].append(value)
         return {"type": "field", "field_name": key, "value": value}
 
     def _parse_expires(self, value: str) -> None:
         try:
             date_value = dateutil.parser.parse(value)
         except dateutil.parser.ParserError:
             self._add_error(
                 "invalid_expiry",
                 "Date and time in 'Expires' field must be formatted "
-                "according to ISO 8601.")
+                "according to ISO 8601.",
+            )
         else:
             self._expires_date = date_value
             if not self.iso8601_re.match(value):
                 # dateutil parses more than just iso8601 format
                 self._add_error(
                     "invalid_expiry",
                     "Date and time in 'Expires' field must be formatted "
-                    "according to ISO 8601.")
-                # Stop to prevent errors when comparing the current datetime, 
+                    "according to ISO 8601.",
+                )
+                # Stop to prevent errors when comparing the current datetime,
                 # which is set with a timezone, and the parsed date, that
                 # could potentially not have a timezone.
                 return
 
             now = datetime.now(timezone.utc)
             max_value = now.replace(year=now.year + 1)
             if date_value > max_value:
                 self._add_recommendation(
                     "long_expiry",
                     "Date and time in 'Expires' field should be less than "
-                    "a year into the future.")
+                    "a year into the future.",
+                )
             elif date_value < now:
                 self._add_error(
                     "expired",
-                    "Date and time in 'Expires' field must not be in "
-                    "the past.")
+                    "Date and time in 'Expires' field must not be in the past.",
+                )
 
     def validate_contents(self) -> None:
         if "expires" not in self._values:
             self._add_error("no_expire", "'Expires' field must be present.")
         elif len(self._values["expires"]) > 1:
             self._add_error(
-                "multi_expire",
-                "'Expires' field must not appear more than once.")
+                "multi_expire", "'Expires' field must not appear more than once."
+            )
         if self._urls and "canonical" in self._values:
             if all(url not in self._values["canonical"] for url in self._urls):
                 self._add_error(
                     "no_canonical_match",
                     "Web URI where security.txt is located must match with a "
                     "'Canonical' field. In case of redirecting either the "
-                    "first or last web URI of the redirect chain must match.")
-        if self.lines[-1]["type"] != 'empty':
-            self._add_error("no_line_separators",
-                            "Every line must end with either a carriage "
-                            "return and line feed characters or just a line "
-                            "feed character")
-        if "contact" not in self._values:
+                    "first or last web URI of the redirect chain must match.",
+                )
+        if self.lines[-1]["type"] != "empty":
             self._add_error(
-                "no_contact", "'Contact' field must appear at least once.")
+                "no_line_separators",
+                "Every line must end with either a carriage "
+                "return and line feed characters or just a line "
+                "feed character",
+            )
+
+        if "csaf" not in self._values:
+            self._add_recommendation(
+                "no_csaf", "'CSAF' field should appear at least once"
+            )
         else:
-            if (any(v.startswith("mailto:") for v in self._values['contact'])
-                    and "encryption" not in self._values):
+            if not all(
+                v.endswith("provider-metadata.json") for v in self._values["csaf"]
+            ):
+                self._add_error(
+                    "no_csaf_file",
+                    "All CSAF field in the security.txt must point "
+                    "to a provider-metadata.json file",
+                )
+            if len(self._values["csaf"]) > 1:
+                self._add_notification(
+                    "multiple_csaf_fields",
+                    "It is allowed to have more than one csaf field, "
+                    "however this should be removed if possible.",
+                )
+
+        if "contact" not in self._values:
+            self._add_error("no_contact", "'Contact' field must appear at least once.")
+        else:
+            if (
+                any(v.startswith("mailto:") for v in self._values["contact"])
+                and "encryption" not in self._values
+            ):
                 self._add_recommendation(
                     "no_encryption",
                     "'Encryption' field should be present when 'Contact' "
-                    "field contains an email address.")
+                    "field contains an email address.",
+                )
         if PREFERRED_LANGUAGES in self._values:
             if len(self._values[PREFERRED_LANGUAGES]) > 1:
                 self._add_error(
                     "multi_lang",
-                    "'Preferred-Languages' field must not appear more "
-                    "than once.")
+                    "'Preferred-Languages' field must not appear more than once.",
+                )
 
         if not self._signed:
             self._add_recommendation(
-                "not_signed", "security.txt should be digitally signed.")
+                "not_signed", "security.txt should be digitally signed."
+            )
         if self._signed and not self._values.get("canonical"):
             self._add_recommendation(
-                "no_canonical",
-                "'Canonical' field should be present in a signed file.")
+                "no_canonical", "'Canonical' field should be present in a signed file."
+            )
 
     def is_valid(self) -> bool:
         return not self._errors
 
     @property
     def errors(self) -> List[ErrorDict]:
         return self._errors
 
     @property
     def recommendations(self) -> List[ErrorDict]:
         return self._recommendations
 
     @property
+    def notifications(self) -> List[ErrorDict]:
+        return self._notifications
+
+    @property
     def lines(self) -> List[LineDict]:
         return self._line_info
 
     @property
     def preferred_languages(self) -> Union[List[str], None]:
         if PREFERRED_LANGUAGES in self._values:
-            return [
-                v.strip() for v in
-                self._values[PREFERRED_LANGUAGES][0].split(",")]
+            return [v.strip() for v in self._values[PREFERRED_LANGUAGES][0].split(",")]
         return None
 
     @property
     def contact_email(self) -> Union[None, str]:
         if "contact" in self._values:
             for value in self._values["contact"]:
                 if value.startswith("mailto:"):
@@ -328,27 +379,26 @@
         return None
 
 
 CORRECT_PATH = ".well-known/security.txt"
 
 
 class SecurityTXT(Parser):
-
     def __init__(self, url: str, recommend_unknown_fields: bool = True):
         url_parts = urlsplit(url)
         if url_parts.scheme:
             if not url_parts.netloc:
                 raise ValueError("Invalid URL")
             netloc = url_parts.netloc
         else:
             netloc = url
         self._netloc = netloc
         self._path: Optional[str] = None
         self._url: Optional[str] = None
-        super().__init__('', recommend_unknown_fields=recommend_unknown_fields)
+        super().__init__("", recommend_unknown_fields=recommend_unknown_fields)
 
     def _get_str(self, content: bytes) -> str:
         try:
             return content.decode()
         except UnicodeError:
             self._add_error("utf8", "Content must be utf-8 encoded.")
         return content.decode(errors="replace")
@@ -357,51 +407,55 @@
         security_txt_found = False
         for scheme in ["https", "http"]:
             for path in [".well-known/security.txt", "security.txt"]:
                 url = urlunsplit((scheme, self._netloc, path, None, None))
                 try:
                     resp = requests.get(url, timeout=5)
                 except requests.exceptions.SSLError:
-                    if not any(d['code'] == 'invalid_cert' for d in self._errors):
-                        self._add_error("invalid_cert", "security.txt must be served with a valid TLS certificate.")
+                    if not any(d["code"] == "invalid_cert" for d in self._errors):
+                        self._add_error(
+                            "invalid_cert",
+                            "security.txt must be served with a valid TLS certificate.",
+                        )
                     try:
                         resp = requests.get(url, timeout=5, verify=False)
                     except:
                         continue
                 except:
                     continue
                 if resp.status_code == 200:
                     self._path = path
                     self._url = url
                     if scheme != "https":
                         self._add_error(
                             "invalid_uri_scheme",
                             "Insecure URI scheme HTTP is not allowed. "
                             "The security.txt file access MUST use "
-                            "the \"https\" scheme")
+                            'the "https" scheme',
+                        )
                     if path != CORRECT_PATH:
                         self._add_error(
                             "location",
                             "security.txt was located on the top-level path "
                             "(legacy place), but must be placed under "
-                            "the '/.well-known/' path.")
-                    if 'content-type' not in resp.headers:
+                            "the '/.well-known/' path.",
+                        )
+                    if "content-type" not in resp.headers:
                         self._add_error(
-                            "no_content_type",
-                            "HTTP Content-Type header must be sent.")
+                            "no_content_type", "HTTP Content-Type header must be sent."
+                        )
                     else:
-                        media_type, params = parse_header(
-                            resp.headers["content-type"])
+                        media_type, params = parse_header(resp.headers["content-type"])
                         if media_type.lower() != "text/plain":
                             self._add_error(
                                 "invalid_media",
                                 "Media type in Content-Type header must be "
                                 "'text/plain'.",
                             )
-                        charset = params.get('charset', "utf-8").lower()
+                        charset = params.get("charset", "utf-8").lower()
                         if charset != "utf-8" and charset != "csutf8":
                             # According to RFC9116, charset default is utf-8
                             self._add_error(
                                 "invalid_charset",
                                 "Charset parameter in Content-Type header must be "
                                 "'utf-8' if present.",
                             )
```

### Comparing `sectxt-0.8.1/sectxt.egg-info/PKG-INFO` & `sectxt-0.8.2/sectxt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectxt
-Version: 0.8.1
+Version: 0.8.2
 Summary: security.txt parser and validator
 Author: DigitalTrustCenter
 Author-email: algemeen@digitaltrustcenter.nl
 License: EUPL-1.2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -66,60 +66,65 @@
 |---------|------------------------------------------------------------------------------------------------------------|
 | code    | A fixed error code string                                                                                  |
 | message | A human readable error message in English                                                                  |
 | line    | The 1 based integer line number where the error occurred or None when the error applies to the entire file |
 
 ### Possible errors
 
-| code                 | message                                                                                                                                                                |
-|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| "no_security_txt"    | "security.txt could not be located."                                                                                                                                   |
-| "location"           | "security.txt was located on the top-level path (legacy place), but must be placed under the '/.well-known/' path."                                                    |
-| "invalid_uri_scheme" | "Insecure URI scheme HTTP is not allowed. The security.txt file access must use the HTTPS scheme"                                                                      |
-| "invalid_cert"       | "security.txt must be served with a valid TLS certificate."                                                                                                            |
-| "no_content_type"    | "HTTP Content-Type header must be sent."                                                                                                                               |
-| "invalid_media"      | "Media type in Content-Type header must be 'text/plain'."                                                                                                              |
-| "invalid_charset"    | "Charset parameter in Content-Type header must be 'utf-8' if present."                                                                                                 |
-| "utf8"               | "Content must be utf-8 encoded."                                                                                                                                       |
-| "no_expire"          | "'Expires' field must be present."                                                                                                                                     |
-| "multi_expire"       | "'Expires' field must not appear more than once."                                                                                                                      |
-| "invalid_expiry"     | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
-| "expired"            | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
-| "no_contact"         | "'Contact' field must appear at least once."                                                                                                                           |
-| "no_canonical_match" | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
-| "multi_lang"         | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
-| "invalid_lang"       | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
-| "no_uri"             | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
-| "no_https"           | "Web URI must begin with 'https://'."                                                                                                                                  |
-| "prec_ws"            | "There must be no whitespace before the field separator (colon)."                                                                                                      |
-| "no_space"           | "Field separator (colon) must be followed by a space."                                                                                                                 | 
-| "empty_key"          | "Field name must not be empty."                                                                                                                                        |
-| "empty_value"        | "Field value must not be empty."                                                                                                                                       |
-| "invalid_line"       | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
-| "no_line_separators" | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
-| "signed_format_issue"| "Signed security.txt files must start with the begin pgp signed message as the document header"                                                                        |
+| code                  | message                                                                                                                                                                |
+|-----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| "no_security_txt"     | "security.txt could not be located."                                                                                                                                   |
+| "location"            | "security.txt was located on the top-level path (legacy place), but must be placed under the '/.well-known/' path."                                                    |
+| "invalid_uri_scheme"  | "Insecure URI scheme HTTP is not allowed. The security.txt file access must use the HTTPS scheme"                                                                      |
+| "invalid_cert"        | "security.txt must be served with a valid TLS certificate."                                                                                                            |
+| "no_content_type"     | "HTTP Content-Type header must be sent."                                                                                                                               |
+| "invalid_media"       | "Media type in Content-Type header must be 'text/plain'."                                                                                                              |
+| "invalid_charset"     | "Charset parameter in Content-Type header must be 'utf-8' if present."                                                                                                 |
+| "utf8"                | "Content must be utf-8 encoded."                                                                                                                                       |
+| "no_expire"           | "'Expires' field must be present."                                                                                                                                     |
+| "multi_expire"        | "'Expires' field must not appear more than once."                                                                                                                      |
+| "invalid_expiry"      | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
+| "expired"             | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
+| "no_contact"          | "'Contact' field must appear at least once."                                                                                                                           |
+| "no_canonical_match"  | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
+| "multi_lang"          | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
+| "invalid_lang"        | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
+| "no_uri"              | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
+| "no_https"            | "Web URI must begin with 'https://'."                                                                                                                                  |
+| "prec_ws"             | "There must be no whitespace before the field separator (colon)."                                                                                                      |
+| "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
+| "empty_key"           | "Field name must not be empty."                                                                                                                                        |
+| "empty_value"         | "Field value must not be empty."                                                                                                                                       |
+| "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
+| "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
+| "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
+| "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
+| "no_csaf_file"        | "All CSAF field in the security.txt must point to a provider-metadata.json file"                                                                                       |
+
 
 ### Possible recommendations
 
-| code                       | message                                                                                                  |
-|----------------------------|----------------------------------------------------------------------------------------------------------|
-| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                           |
-| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address."                   |
-| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                                               |
-| "no_canonical"             | "'Canonical' field should be present in a signed file."                                                  |
+| code                       | message                                                                                |
+|----------------------------|----------------------------------------------------------------------------------------|
+| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."         |
+| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address." |
+| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                             |
+| "no_canonical"             | "'Canonical' field should be present in a signed file."                                |
+| "no_csaf"                  | "'CSAF' field should appear at least once"                                             |
 
 ### Possible notifications
 
-| code                          | message                                                                                                  |
-|-------------------------------|----------------------------------------------------------------------------------------------------------|
-| "unknown_field"<sup>[2]</sup> | "security.txt contains an unknown field. Either this is a custom field which may not be widely supported, or there is a typo in a standardised field name." |
+| code                          | message                                                                                                                                                                     |
+|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
+| "multiple_csaf_fields"        | "It is allowed to have more than one CSAF field, however this should be removed if possible."                                                                               |
 
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
-[2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported should be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
+[2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
 
 >>> from sectxt import SecurityTXT
 >>> s = SecurityTXT("www.example.com", recommend_unknown_fields=False)
 ```
```

### Comparing `sectxt-0.8.1/setup.cfg` & `sectxt-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sectxt-0.8.1/test/test_sectxt.py` & `sectxt-0.8.2/test/test_sectxt.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 
 # Our security policy
 Policy: https://example.com/security-policy.html
 
 # Our security acknowledgments page
 Acknowledgments: https://example.com/hall-of-fame.html
 
+# CSAF link
+CSAF: https://example.com/.well-known/csaf/provider-metadata.json
+
 Expires: {(date.today() + timedelta(days=10)).isoformat()}T18:37:07z
 -----BEGIN PGP SIGNATURE-----
 Version: GnuPG v2.2
 
 [signature]
 -----END PGP SIGNATURE-----
 """
 
 
 class SecTxtTestCase(TestCase):
-
     def test_future_expires(self):
         content = f"Expires: {date.today().year + 3}-01-01T12:00:00Z\n"
         p = Parser(content)
         self.assertEqual(p._recommendations[0]["code"], "long_expiry")
 
     def test_invalid_expires(self):
         content = "Expires: Nonsense\n"
@@ -63,15 +65,16 @@
         self.assertEqual(line_info["value"], "# Wow")
 
     def test_preferred_languages(self):
         # Define content for a valid security.txt.
         static_content = (
             f"Expires: {(date.today() + timedelta(days=10)).isoformat()}"
             "T18:37:07z\n"
-            "Contact: mailto:security@example.com\n")
+            "Contact: mailto:security@example.com\n"
+        )
 
         # Single invalid value.
         content = static_content + "Preferred-Languages: English"
         p = Parser(content)
         self.assertEqual(p._errors[0]["code"], "invalid_lang")
 
         # Mix of valid and invalid value.
@@ -79,20 +82,15 @@
         p = Parser(content)
         self.assertEqual(p._errors[0]["code"], "invalid_lang")
 
         # Both ISO 639-1 (2 char) and ISO 639-2 (3 char) should be valid.
         # Case should be ignored.
         content = static_content + "Preferred-Languages: En, dUT"
         p = Parser(content)
-        self.assertFalse(
-            any(
-                error["code"] == "invalid_lang"
-                for error in p._errors
-            )
-        )
+        self.assertFalse(any(error["code"] == "invalid_lang" for error in p._errors))
 
     def test_prec_ws(self):
         content = "Contact : mailto:me@example.com\n# Wow"
         p = Parser(content)
         self.assertEqual(p._errors[0]["code"], "prec_ws")
 
     def test_empty_key(self):
@@ -127,67 +125,127 @@
 
     def test_signed(self):
         p = Parser(_signed_example)
         self.assertTrue(p.is_valid())
 
     def test_signed_no_canonical(self):
         content = _signed_example.replace(
-            "Canonical: https://example.com/.well-known/security.txt", "")
+            "Canonical: https://example.com/.well-known/security.txt", ""
+        )
         p = Parser(content)
-        self.assertEqual(p._recommendations[0]['code'], "no_canonical")
+        self.assertEqual(p._recommendations[0]["code"], "no_canonical")
 
     def test_signed_dash_escaped(self):
         content = _signed_example.replace("Expires", "- Expires")
         p = Parser(content)
         self.assertTrue(p.is_valid())
 
     def test_pgp_signed_formatting(self):
         content = "\r\n" + _signed_example
         p = Parser(content)
         self.assertFalse(p.is_valid())
-        self.assertTrue(any(d['code'] == 'signed_format_issue' for d in p.errors))
+        self.assertTrue(any(d["code"] == "signed_format_issue" for d in p.errors))
 
     def test_unknown_fields(self):
         # Define a security.txt that contains unknown fields (but is valid).
         # The fields Last-updated and Unknown, should be marked as unknown.
         content = (
             f"Expires: {(date.today() + timedelta(days=10)).isoformat()}"
             "T18:37:07z\n"
             "Contact: mailto:security@example.com\n"
             "Last-updated: {date.today().isoformat()}T12:00:00z\n"
             "Unknown: value\n"
-            "Encryption: https://example.com/pgp-key.txt\n")
+            "Encryption: https://example.com/pgp-key.txt\n"
+        )
 
         # By default, recommend that there are unknown fields.
         p = Parser(content)
         self.assertTrue(p.is_valid())
-        self.assertEqual(len([1 for r in p._recommendations if r["code"] == "unknown_field"]), 2)
+        self.assertEqual(
+            len([1 for r in p._notifications if r["code"] == "unknown_field"]), 2
+        )
 
         # When turned off, there should be no unknown_field recommendations.
         p = Parser(content, recommend_unknown_fields=False)
         self.assertTrue(p.is_valid())
-        self.assertEqual(len([1 for r in p._recommendations if r["code"] == "unknown_field"]), 0)
+        self.assertEqual(
+            len([1 for r in p._notifications if r["code"] == "unknown_field"]), 0
+        )
 
     def test_no_line_separators(self):
-        single_line_security_txt = f"Contact: mailto:security@example.com  Expires: {(date.today() + timedelta(days=10)).isoformat()}T18:37:07z  # All on a single line"
+        expire_date = (date.today() + timedelta(days=10)).isoformat()
+        single_line_security_txt = (
+            f"Contact: mailto:security@example.com  Expires: "
+            f"{expire_date}T18:37:07z  # All on a single line"
+        )
         p = Parser(single_line_security_txt)
         self.assertFalse(p.is_valid())
-        self.assertEqual(len([1 for r in p._errors if r["code"] == "no_line_separators"]), 1)
+        self.assertEqual(
+            len([1 for r in p._errors if r["code"] == "no_line_separators"]), 1
+        )
+
+    def test_csaf_optional(self):
+        content = _signed_example.replace(
+            "CSAF: https://example.com/.well-known/csaf/provider-metadata.json", ""
+        )
+        p = Parser(content)
+        self.assertTrue(p.is_valid())
+        self.assertEqual(
+            len([1 for r in p._recommendations if r["code"] == "no_csaf"]), 1
+        )
+
+    def test_csaf_https_uri(self):
+        content = _signed_example.replace(
+            "CSAF: https://example.com/.well-known/csaf/provider-metadata.json",
+            "CSAF: http://example.com/.well-known/csaf/provider-metadata.json",
+        )
+        p = Parser(content)
+        self.assertFalse(p.is_valid())
+        self.assertEqual(len([1 for r in p._errors if r["code"] == "no_https"]), 1)
+
+    def test_csaf_provider_file(self):
+        content = _signed_example.replace(
+            "CSAF: https://example.com/.well-known/csaf/provider-metadata.json",
+            "CSAF: https://example.com/.well-known/csaf/other_provider_name.json",
+        )
+        p = Parser(content)
+        self.assertFalse(p.is_valid())
+        self.assertEqual(len([1 for r in p._errors if r["code"] == "no_csaf_file"]), 1)
+
+    def test_multiple_csaf_notification(self):
+        content = _signed_example.replace(
+            "# CSAF link",
+            "# CSAF link\n"
+            "CSAF: https://example2.com/.well-known/csaf/provider-metadata.json",
+        )
+        p = Parser(content)
+        self.assertTrue(p.is_valid())
+        self.assertEqual(
+            len([1 for r in p._notifications if r["code"] == "multiple_csaf_fields"]), 1
+        )
 
 
 def test_not_correct_path(requests_mock: Mocker):
     with Mocker() as m:
-        m.get('https://example.com/.well-known/security.txt', exc=requests.exceptions.ConnectTimeout)
-        m.get('https://example.com/security.txt', text=_signed_example)
-        s = SecurityTXT('example.com')
-        if not any(d['code'] == 'location' for d in s.errors):
+        m.get(
+            "https://example.com/.well-known/security.txt",
+            exc=requests.exceptions.ConnectTimeout,
+        )
+        m.get("https://example.com/security.txt", text=_signed_example)
+        s = SecurityTXT("example.com")
+        if not any(d["code"] == "location" for d in s.errors):
             pytest.fail("location error code should be given")
 
 
 def test_invalid_uri_scheme(requests_mock: Mocker):
     with Mocker() as m:
-        m.get('https://example.com/.well-known/security.txt', exc=requests.exceptions.ConnectTimeout)
-        m.get('https://example.com/security.txt', exc=requests.exceptions.ConnectTimeout)
-        m.get('http://example.com/.well-known/security.txt', text=_signed_example)
-        s = SecurityTXT('example.com')
-        if not any(d['code'] == 'invalid_uri_scheme' for d in s.errors):
+        m.get(
+            "https://example.com/.well-known/security.txt",
+            exc=requests.exceptions.ConnectTimeout,
+        )
+        m.get(
+            "https://example.com/security.txt", exc=requests.exceptions.ConnectTimeout
+        )
+        m.get("http://example.com/.well-known/security.txt", text=_signed_example)
+        s = SecurityTXT("example.com")
+        if not any(d["code"] == "invalid_uri_scheme" for d in s.errors):
             pytest.fail("invalid_uri_scheme error code should be given")
```

