# Comparing `tmp/secapi-tl-1.1.0.tar.gz` & `tmp/secapi-tl-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secapi-tl-1.1.0.tar", last modified: Sat Apr  8 12:53:37 2023, max compression
+gzip compressed data, was "secapi-tl-1.1.1.tar", last modified: Fri Apr 14 12:13:09 2023, max compression
```

## Comparing `secapi-tl-1.1.0.tar` & `secapi-tl-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-08 12:53:37.181365 secapi-tl-1.1.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)     5134 2023-04-08 12:53:37.181365 secapi-tl-1.1.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     3695 2022-10-14 12:06:38.000000 secapi-tl-1.1.0/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-08 12:32:44.000000 secapi-tl-1.1.0/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-08 12:53:37.181365 secapi-tl-1.1.0/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-08 12:53:37.177365 secapi-tl-1.1.0/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-08 12:53:37.181365 secapi-tl-1.1.0/src/secapi_tl/
--rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.0/src/secapi_tl/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6025 2023-04-08 12:35:48.000000 secapi-tl-1.1.0/src/secapi_tl/filing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-08 12:35:48.000000 secapi-tl-1.1.0/src/secapi_tl/filing_query.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.0/src/secapi_tl/key_mapper.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1205 2022-10-14 12:06:38.000000 secapi-tl-1.1.0/src/secapi_tl/request.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-08 12:53:37.181365 secapi-tl-1.1.0/src/secapi_tl.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     5134 2023-04-08 12:53:37.000000 secapi-tl-1.1.0/src/secapi_tl.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-08 12:53:37.000000 secapi-tl-1.1.0/src/secapi_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-08 12:53:37.000000 secapi-tl-1.1.0/src/secapi_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-08 12:53:37.000000 secapi-tl-1.1.0/src/secapi_tl.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-08 12:53:37.000000 secapi-tl-1.1.0/src/secapi_tl.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.1/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.1/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-14 12:08:01.000000 secapi-tl-1.1.1/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/src/secapi_tl/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.1/src/secapi_tl/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6025 2023-04-08 12:35:48.000000 secapi-tl-1.1.1/src/secapi_tl/filing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-08 12:35:48.000000 secapi-tl-1.1.1/src/secapi_tl/filing_query.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.1/src/secapi_tl/key_mapper.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1206 2023-04-14 12:05:11.000000 secapi-tl-1.1.1/src/secapi_tl/request.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/src/secapi_tl.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/top_level.txt
```

### Comparing `secapi-tl-1.1.0/LICENSE` & `secapi-tl-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.0/PKG-INFO` & `secapi-tl-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.0
+Version: 1.1.1
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -55,19 +55,20 @@
 * form_types : filters all filings based on a list of form types, so only filings
 with a form type from the list will be returned
 * filings_information: returns only the metadata points for each filing that
 are included in the given list. This can be used to reduce the amount of data
 and to get rid of irrelevant data.
 A list of all possible data points can be found below
 
-The return value will be a list of dictionaries. Each dictionary represents
-one filing and holds multiple metadata points. Two of these metadata points
-are the ticker symbol and the cik which are always part of the metadata.
-By default, all other metadata points are contained in the dictionary, but
-they can also be specifically selected via the filing_information parameter.
+The return value will be a list of Filing Objects. Each Filing holds multiple 
+metadata points. Two of these metadata points are the ticker symbol 
+and the cik which are always part of the metadata.
+By default, all other metadata points are contained in the Filing, but
+they can also be specifically selected via the filing_information parameter
+of the get_filings function.
 Below is a list of all possible metadata points:
 * accessionNumber
 * filingDate
 * reportDate
 * acceptanceDateTime
 * act
 * form
@@ -76,15 +77,15 @@
 * items
 * size
 * isXBRL
 * isInlineXBRL
 * primaryDocument
 * primaryDocDescription
 
-These metadata can be used to create the links to the actual filings.
+These metadata can then be used to create the links to the actual filings.
 The process of finding a way to build the links from the metadata can be quite difficult, 
 and requires a lot of experimentation.
 
 ### How to make requests to the sec server
 The sec has restricted the access to their servers .Thereby it is not allowed
 to do more than 10 requests per second. To ensure that the amount of requests stays
 within the boundaries set by the sec this package provides the `Request.sec_request`
```

### Comparing `secapi-tl-1.1.0/README.md` & `secapi-tl-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 * form_types : filters all filings based on a list of form types, so only filings
 with a form type from the list will be returned
 * filings_information: returns only the metadata points for each filing that
 are included in the given list. This can be used to reduce the amount of data
 and to get rid of irrelevant data.
 A list of all possible data points can be found below
 
-The return value will be a list of dictionaries. Each dictionary represents
-one filing and holds multiple metadata points. Two of these metadata points
-are the ticker symbol and the cik which are always part of the metadata.
-By default, all other metadata points are contained in the dictionary, but
-they can also be specifically selected via the filing_information parameter.
+The return value will be a list of Filing Objects. Each Filing holds multiple 
+metadata points. Two of these metadata points are the ticker symbol 
+and the cik which are always part of the metadata.
+By default, all other metadata points are contained in the Filing, but
+they can also be specifically selected via the filing_information parameter
+of the get_filings function.
 Below is a list of all possible metadata points:
 * accessionNumber
 * filingDate
 * reportDate
 * acceptanceDateTime
 * act
 * form
@@ -46,15 +47,15 @@
 * items
 * size
 * isXBRL
 * isInlineXBRL
 * primaryDocument
 * primaryDocDescription
 
-These metadata can be used to create the links to the actual filings.
+These metadata can then be used to create the links to the actual filings.
 The process of finding a way to build the links from the metadata can be quite difficult, 
 and requires a lot of experimentation.
 
 ### How to make requests to the sec server
 The sec has restricted the access to their servers .Thereby it is not allowed
 to do more than 10 requests per second. To ensure that the amount of requests stays
 within the boundaries set by the sec this package provides the `Request.sec_request`
```

### Comparing `secapi-tl-1.1.0/src/secapi_tl/filing.py` & `secapi-tl-1.1.1/src/secapi_tl/filing.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.0/src/secapi_tl/filing_query.py` & `secapi-tl-1.1.1/src/secapi_tl/filing_query.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.0/src/secapi_tl/key_mapper.py` & `secapi-tl-1.1.1/src/secapi_tl/key_mapper.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.0/src/secapi_tl/request.py` & `secapi-tl-1.1.1/src/secapi_tl/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 by exceeding the request limits when used with threading.
 These issues disappeared with the implementation as a static method.
 """
 
 import requests
 from ratelimit import limits, sleep_and_retry
 
-SEC_REQUEST_COUNT = 10
-SEC_PERIOD = 1
+SEC_REQUEST_COUNT = 1
+SEC_PERIOD = 0.1
 SEC_HEADER = {'User-Agent': "myUserAgent"}
 
 
 class Request:
 
     @staticmethod
     @sleep_and_retry
```

### Comparing `secapi-tl-1.1.0/src/secapi_tl.egg-info/PKG-INFO` & `secapi-tl-1.1.1/src/secapi_tl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.0
+Version: 1.1.1
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -55,19 +55,20 @@
 * form_types : filters all filings based on a list of form types, so only filings
 with a form type from the list will be returned
 * filings_information: returns only the metadata points for each filing that
 are included in the given list. This can be used to reduce the amount of data
 and to get rid of irrelevant data.
 A list of all possible data points can be found below
 
-The return value will be a list of dictionaries. Each dictionary represents
-one filing and holds multiple metadata points. Two of these metadata points
-are the ticker symbol and the cik which are always part of the metadata.
-By default, all other metadata points are contained in the dictionary, but
-they can also be specifically selected via the filing_information parameter.
+The return value will be a list of Filing Objects. Each Filing holds multiple 
+metadata points. Two of these metadata points are the ticker symbol 
+and the cik which are always part of the metadata.
+By default, all other metadata points are contained in the Filing, but
+they can also be specifically selected via the filing_information parameter
+of the get_filings function.
 Below is a list of all possible metadata points:
 * accessionNumber
 * filingDate
 * reportDate
 * acceptanceDateTime
 * act
 * form
@@ -76,15 +77,15 @@
 * items
 * size
 * isXBRL
 * isInlineXBRL
 * primaryDocument
 * primaryDocDescription
 
-These metadata can be used to create the links to the actual filings.
+These metadata can then be used to create the links to the actual filings.
 The process of finding a way to build the links from the metadata can be quite difficult, 
 and requires a lot of experimentation.
 
 ### How to make requests to the sec server
 The sec has restricted the access to their servers .Thereby it is not allowed
 to do more than 10 requests per second. To ensure that the amount of requests stays
 within the boundaries set by the sec this package provides the `Request.sec_request`
```

