# Comparing `tmp/dateparse-1.3.1.tar.gz` & `tmp/dateparse-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dateparse-1.3.1.tar", max compression
+gzip compressed data, was "dateparse-1.4.0.tar", max compression
```

## Comparing `dateparse-1.3.1.tar` & `dateparse-1.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1211 2023-04-13 22:30:21.466944 dateparse-1.3.1/LICENSE.rst
--rw-r--r--   0        0        0     4050 2023-04-13 22:30:21.466944 dateparse-1.3.1/README.rst
--rw-r--r--   0        0        0      728 2023-04-13 22:30:21.466944 dateparse-1.3.1/dateparse/__init__.py
--rw-r--r--   0        0        0     5760 2023-04-13 22:30:21.466944 dateparse-1.3.1/dateparse/dateparser.py
--rw-r--r--   0        0        0     7249 2023-04-13 22:30:21.466944 dateparse-1.3.1/dateparse/parsefunctions.py
--rw-r--r--   0        0        0     8958 2023-04-13 22:30:21.466944 dateparse-1.3.1/dateparse/parseutil.py
--rw-r--r--   0        0        0     3191 2023-04-13 22:43:52.150230 dateparse-1.3.1/dateparse/regex_utils.py
--rw-r--r--   0        0        0      852 2023-04-13 22:44:23.600228 dateparse-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4838 1970-01-01 00:00:00.000000 dateparse-1.3.1/setup.py
--rw-r--r--   0        0        0     4581 1970-01-01 00:00:00.000000 dateparse-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-13 22:30:21.466944 dateparse-1.4.0/LICENSE.rst
+-rw-r--r--   0        0        0     4050 2023-04-13 22:30:21.466944 dateparse-1.4.0/README.rst
+-rw-r--r--   0        0        0      728 2023-04-13 22:30:21.466944 dateparse-1.4.0/dateparse/__init__.py
+-rw-r--r--   0        0        0     5808 2023-04-13 23:14:18.196790 dateparse-1.4.0/dateparse/dateparser.py
+-rw-r--r--   0        0        0     7249 2023-04-13 22:30:21.466944 dateparse-1.4.0/dateparse/parsefunctions.py
+-rw-r--r--   0        0        0     8979 2023-04-13 23:05:46.653487 dateparse-1.4.0/dateparse/parseutil.py
+-rw-r--r--   0        0        0     3191 2023-04-13 22:43:52.150230 dateparse-1.4.0/dateparse/regex_utils.py
+-rw-r--r--   0        0        0      852 2023-04-13 23:14:49.040122 dateparse-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4838 1970-01-01 00:00:00.000000 dateparse-1.4.0/setup.py
+-rw-r--r--   0        0        0     4581 1970-01-01 00:00:00.000000 dateparse-1.4.0/PKG-INFO
```

### Comparing `dateparse-1.3.1/LICENSE.rst` & `dateparse-1.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dateparse-1.3.1/README.rst` & `dateparse-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `dateparse-1.3.1/dateparse/__init__.py` & `dateparse-1.4.0/dateparse/__init__.py`

 * *Files identical despite different names*

### Comparing `dateparse-1.3.1/dateparse/dateparser.py` & `dateparse-1.4.0/dateparse/dateparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         Constructor for DateParser
 
         """
 
         self.named_days = self.default_named_days
         self.escape = escape
 
+        self.cache: dict[str, DateResult] = {}
+
         if named_days is not None:
             self.named_days.update(named_days)
 
         if base_date is None:
             base_date = datetime.date.today()
         self.base_date = base_date
```

### Comparing `dateparse-1.3.1/dateparse/parsefunctions.py` & `dateparse-1.4.0/dateparse/parsefunctions.py`

 * *Files identical despite different names*

### Comparing `dateparse-1.3.1/dateparse/parseutil.py` & `dateparse-1.4.0/dateparse/parseutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     expr_content = delta_content + " " + anchor_content
 
     new_date_result = DateResult(resulting_date, start, end, expr_content)
 
     return new_date_result
 
 
+@fn.cache
 def basic_parse(
     base_date: datetime.date,
     text: str,
     from_right: bool = False,
     allow_past: bool = False,
     escape: str = "\\",
 ):
@@ -270,14 +271,15 @@
 
     if parsed_tuple is None:
         return None
 
     return parsed_tuple.date
 
 
+@fn.cache
 def parse_all(
     base_date: datetime.date,
     text: str,
     from_right: bool = False,
     allow_past: bool = False,
     escape: str = "\\",
 ):
@@ -295,14 +297,15 @@
         _reduce_expression(base_date, expr, allow_past=allow_past)
         for expr in expressions
     ]
 
     return date_tuple_results
 
 
+
 def parse_all_dates(
     base_date: datetime.date,
     text: str,
     from_right: bool = False,
     allow_past: bool = False,
     escape: str = "\\",
 ):
```

### Comparing `dateparse-1.3.1/dateparse/regex_utils.py` & `dateparse-1.4.0/dateparse/regex_utils.py`

 * *Files identical despite different names*

### Comparing `dateparse-1.3.1/pyproject.toml` & `dateparse-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dateparse"
-version = "1.3.1"
+version = "1.4.0"
 description = "A pure Python library for parsing natural language time expressions, with minimal dependencies"
 authors = ["keagud <keagud@protonmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dateparse-1.3.1/setup.py` & `dateparse-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['datetime>=4.9,<5.0']
 
 setup_kwargs = {
     'name': 'dateparse',
-    'version': '1.3.1',
+    'version': '1.4.0',
     'description': 'A pure Python library for parsing natural language time expressions, with minimal dependencies',
     'long_description': 'Dateparse\n===========\n\nA python library for parsing natural language time descriptions. \n\nInstallation\n-------------\nDateparse is on PyPi; install with Pip: :code:`$ pip install dateparse`\n\nUsage\n------ \n>>> import dateparse\n>>> from datetime import date\n\n>>> # The main use case is extracting a single date from a string\n>>> dateparse.basic_parse(date.today(), "a week from friday")\nDateResult(date=datetime.date(2023, 2, 10), start=0, end=15, content=\'a week from fri\')\n\n>>> # by default the first (leftmost) encountered date is returned\n>>> dateparse.basic_parse(date.today(), "a week from thursday and a week from friday")\nDateResult(date=datetime.date(2023, 2, 9), start=0, end=15, content=\'a week from thu\') \n\n>>> # the from_right option changes this\n>>> dateparse.get_first(date.today(), "a week from thursday and a week from friday")\nDateResult(date=datetime.date(2023, 2, 10), start=0, end=15, content=\'a week from fri\')\n\n>>> # default behavior for all parse functions is to get the next future date matching the expression\n>>> # relative to the given base date\n>>> # this can be changed with the allow_past option\n>>> dateparse.basic_parse(date(1970, 9, 8), "january 1", allow_past=True)\nDateResult(date=datetime.date(1970, 1, 1), start=0, end=9, content=\' january 1\')\n\n>>> # parse_all gets all expressions in a list\n>>> dateparse.parse_all(date.today(), "a week from thursday and four days before march 11")\n[DateResult(date=datetime.date(2023, 2, 9), start=0, end=15, content=\'a week from thu\'), DateResult(date=datetime.date(2023, 3, 7), start=24, end=50, content=\'four days before march 11\')]\n\n>>> # the default return type for dates is a DateResult, a simple named tuple containing the date\'s info\n>>> # For convenience, there are also functions to just get the date\n>>> dateparse.basic_date_parse(date.today(), "february 9")\ndatetime.date(2023, 2, 9)\n\n>>> # parse_all_dates works in the same way\n>>> # a DateParser object holds a specified baseline date \n>>> # by default, assumes the baseline date is date.today()\n>>> parser = dateparse.DateParser() \n\n>>> # parses dates with a reference point of january 17, 2021 \n>>> parser_january = dateparse.DateParser(base_date = date(2021, 17, 1)) \n\n>>> # DateParser also supports named days by default\n>>> parser.get_first("four days after halloween 2024")\nDateResult(date=datetime.date(2024, 11, 4), start=0, end=31, content=\'four days after october 31 2024\')\n\n>>> # You can also define your own custom named days as a string dictionary and pass it into the parser\n>>> my_dates = {\'my birthday\' : \'june 11\'}\n>>> my_parser = dateparse.DateParser(named_days = my_dates)\n>>> my_parser.get_first("a month before my birthday")\nDateResult(date=datetime.date(2023, 5, 14), start=0, end=22, content=\'a month before june 11\')\n\n>>> # DateParser.get_first and DateParser.get_last are convenience wrappers around basic_parse\n>>> # to get the first or last expression, with the base date defined at initialization\n>>> my_parser.get_first("a week from thurs and two months after friday")\nDateResult(date=datetime.date(2023, 2, 9), start=0, end=15, content=\'a week from thu\')\n>>> my_parser.get_last("a week from thurs and two months after friday")\nDateResult(date=datetime.date(2023, 4, 3), start=21, end=42, content=\'two months after fri\')\n\n>>> # DateParser.get_all and DateParser.get_all_dates wrap parse_all and parse_all_dates\n>>> my_parser.get_all("a week from thurs and two months after friday")\n[DateResult(date=datetime.date(2023, 2, 9), start=0, end=15, content=\'a week from thu\'), DateResult(date=datetime.date(2023, 4, 3), start=21, end=42, content=\'two months after fri\')]\n>>> my_parser.get_all_dates("a week from thurs and two months after friday")\n[datetime.date(2023, 2, 9), datetime.date(2023, 4, 3)]\n\n\nOther Info\n----------\n**This project is under active development.** The core API is unlikely to change much at this point, but the under-the-hood details are still very much in flux. \n\nDateparse requires Python 3.10 or higher, thanks the author\'s neurotic devotion to type annotations. \n',
     'author': 'keagud',
     'author_email': 'keagud@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dateparse-1.3.1/PKG-INFO` & `dateparse-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateparse
-Version: 1.3.1
+Version: 1.4.0
 Summary: A pure Python library for parsing natural language time expressions, with minimal dependencies
 License: Unlicense
 Author: keagud
 Author-email: keagud@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

