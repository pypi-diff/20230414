# Comparing `tmp/mo-parsing-8.4.21326.tar.gz` & `tmp/mo-parsing-8.6.21337.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-parsing-8.4.21326.tar", last modified: Mon Nov 22 23:33:30 2021, max compression
+gzip compressed data, was "mo-parsing-8.6.21337.tar", last modified: Fri Dec  3 13:44:41 2021, max compression
```

## Comparing `mo-parsing-8.4.21326.tar` & `mo-parsing-8.6.21337.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-11-22 23:33:30.797754 mo-parsing-8.4.21326/
--rw-rw-rw-   0        0        0     1023 2019-10-01 00:43:04.000000 mo-parsing-8.4.21326/LICENSE
--rw-rw-rw-   0        0        0     8516 2021-11-22 23:33:30.793785 mo-parsing-8.4.21326/PKG-INFO
--rw-rw-rw-   0        0        0     6701 2021-11-20 14:07:33.000000 mo-parsing-8.4.21326/README.md
-drwxrwxrwx   0        0        0        0 2021-11-22 23:33:30.773743 mo-parsing-8.4.21326/mo_parsing/
--rw-rw-rw-   0        0        0     2732 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/mo_parsing/__init__.py
--rw-rw-rw-   0        0        0    25527 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/mo_parsing/core.py
--rw-rw-rw-   0        0        0     2834 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/mo_parsing/debug.py
--rw-rw-rw-   0        0        0    29279 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/mo_parsing/enhancement.py
--rw-rw-rw-   0        0        0     5385 2021-11-20 14:07:33.000000 mo-parsing-8.4.21326/mo_parsing/exceptions.py
--rw-rw-rw-   0        0        0    25413 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/mo_parsing/expressions.py
--rw-rw-rw-   0        0        0    31835 2021-10-30 18:24:02.000000 mo-parsing-8.4.21326/mo_parsing/helpers.py
--rw-rw-rw-   0        0        0    12894 2021-11-16 18:07:06.000000 mo-parsing-8.4.21326/mo_parsing/infix.py
--rw-rw-rw-   0        0        0     3125 2021-10-30 18:24:02.000000 mo-parsing-8.4.21326/mo_parsing/profile.py
--rw-rw-rw-   0        0        0    10120 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/mo_parsing/regex.py
--rw-rw-rw-   0        0        0    13553 2021-11-20 14:07:33.000000 mo-parsing-8.4.21326/mo_parsing/results.py
--rw-rw-rw-   0        0        0    23879 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/mo_parsing/tokens.py
--rw-rw-rw-   0        0        0    17684 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/mo_parsing/utils.py
--rw-rw-rw-   0        0        0     6116 2021-10-30 18:24:02.000000 mo-parsing-8.4.21326/mo_parsing/whitespaces.py
-drwxrwxrwx   0        0        0        0 2021-11-22 23:33:30.785794 mo-parsing-8.4.21326/mo_parsing.egg-info/
--rw-rw-rw-   0        0        0     8516 2021-11-22 23:33:30.000000 mo-parsing-8.4.21326/mo_parsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2021-11-22 23:33:30.000000 mo-parsing-8.4.21326/mo_parsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-22 23:33:30.000000 mo-parsing-8.4.21326/mo_parsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2021-11-22 23:33:30.000000 mo-parsing-8.4.21326/mo_parsing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-11-22 23:33:30.000000 mo-parsing-8.4.21326/mo_parsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-22 23:33:30.797754 mo-parsing-8.4.21326/setup.cfg
--rw-rw-rw-   0        0        0     7564 2021-11-22 23:33:23.000000 mo-parsing-8.4.21326/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-03 13:44:41.600689 mo-parsing-8.6.21337/
+-rw-rw-rw-   0        0        0     1023 2019-10-01 00:43:04.000000 mo-parsing-8.6.21337/LICENSE
+-rw-rw-rw-   0        0        0     8516 2021-12-03 13:44:41.600689 mo-parsing-8.6.21337/PKG-INFO
+-rw-rw-rw-   0        0        0     6701 2021-11-20 14:07:33.000000 mo-parsing-8.6.21337/README.md
+drwxrwxrwx   0        0        0        0 2021-12-03 13:44:41.579491 mo-parsing-8.6.21337/mo_parsing/
+-rw-rw-rw-   0        0        0     2732 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/__init__.py
+-rw-rw-rw-   0        0        0    25527 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/core.py
+-rw-rw-rw-   0        0        0     2989 2021-11-23 00:49:40.000000 mo-parsing-8.6.21337/mo_parsing/debug.py
+-rw-rw-rw-   0        0        0    29279 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/enhancement.py
+-rw-rw-rw-   0        0        0     5385 2021-11-20 14:07:33.000000 mo-parsing-8.6.21337/mo_parsing/exceptions.py
+-rw-rw-rw-   0        0        0    25413 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/expressions.py
+-rw-rw-rw-   0        0        0    31835 2021-10-30 18:24:02.000000 mo-parsing-8.6.21337/mo_parsing/helpers.py
+-rw-rw-rw-   0        0        0    12894 2021-11-16 18:07:06.000000 mo-parsing-8.6.21337/mo_parsing/infix.py
+-rw-rw-rw-   0        0        0     3125 2021-10-30 18:24:02.000000 mo-parsing-8.6.21337/mo_parsing/profile.py
+-rw-rw-rw-   0        0        0    10120 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/regex.py
+-rw-rw-rw-   0        0        0    13735 2021-12-03 13:44:36.000000 mo-parsing-8.6.21337/mo_parsing/results.py
+-rw-rw-rw-   0        0        0    23879 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/tokens.py
+-rw-rw-rw-   0        0        0    17765 2021-12-03 13:44:36.000000 mo-parsing-8.6.21337/mo_parsing/utils.py
+-rw-rw-rw-   0        0        0     6116 2021-10-30 18:24:02.000000 mo-parsing-8.6.21337/mo_parsing/whitespaces.py
+drwxrwxrwx   0        0        0        0 2021-12-03 13:44:41.590093 mo-parsing-8.6.21337/mo_parsing.egg-info/
+-rw-rw-rw-   0        0        0     8516 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-12-03 13:44:41.600689 mo-parsing-8.6.21337/setup.cfg
+-rw-rw-rw-   0        0        0     7564 2021-12-03 13:44:36.000000 mo-parsing-8.6.21337/setup.py
```

### Comparing `mo-parsing-8.4.21326/LICENSE` & `mo-parsing-8.6.21337/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/PKG-INFO` & `mo-parsing-8.6.21337/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-parsing
-Version: 8.4.21326
+Version: 8.6.21337
 Summary: Another PEG Parsing Tool
 Home-page: https://github.com/klahnakoski/mo-parsing
 Author: Various
 Author-email: kyle@lahnakoski.com
 License: MIT
 Description: # More Parsing!
```

### Comparing `mo-parsing-8.4.21326/README.md` & `mo-parsing-8.6.21337/README.md`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/__init__.py` & `mo-parsing-8.6.21337/mo_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/core.py` & `mo-parsing-8.6.21337/mo_parsing/core.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/debug.py` & `mo-parsing-8.6.21337/mo_parsing/debug.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,20 @@
     quote as plain_quote, ParseException,
 )
 
 DEBUGGING = False
 
 
 class Debugger(object):
-    def __init__(self):
+    def __init__(self, silent=False):
         self.previous_parse = None
         self.was_debugging = False
         self.parse_count = 0
         self.max_stack_depth = 0
+        self.silent = silent
 
     def __enter__(self):
         global DEBUGGING
         self.was_debugging = DEBUGGING
         DEBUGGING = True
         self.previous_parse = ParserElement._parse
         ParserElement._parse = _debug_parse(self)
@@ -34,35 +35,38 @@
         global DEBUGGING
         ParserElement._parse = self.previous_parse
         DEBUGGING = self.was_debugging
 
 
 def _debug_parse(debugger):
     def debug_parse(self, string, start, do_actions=True):
-        _try(self, start, string)
+        if not debugger.silent:
+            _try(self, start, string)
         loc = start
         try:
             debugger.parse_count += 1
             debugger.max_stack_depth = stackdepth()
             tokens = self.parse_impl(string, loc, do_actions)
         except ParseException as cause:
             self.parser_config.fail_action and self.parser_config.fail_action(
                 self, start, string, cause
             )
-            fail(self, start, string, cause)
+            if not debugger.silent:
+                fail(self, start, string, cause)
             raise ParseException(self, start, string, cause=cause) from None
 
         if self.parse_action and (do_actions or self.parser_config.callDuringTry):
             try:
                 for fn in self.parse_action:
                     tokens = fn(tokens, start, string)
             except Exception as cause:
                 fail(self, start, string, cause)
                 raise
-        match(self, loc, tokens.end, string, tokens)
+        if not debugger.silent:
+            match(self, loc, tokens.end, string, tokens)
 
         return tokens
 
     return debug_parse
 
 
 def _try(expr, start, string):
```

### Comparing `mo-parsing-8.4.21326/mo_parsing/enhancement.py` & `mo-parsing-8.6.21337/mo_parsing/enhancement.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/exceptions.py` & `mo-parsing-8.6.21337/mo_parsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/expressions.py` & `mo-parsing-8.6.21337/mo_parsing/expressions.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/helpers.py` & `mo-parsing-8.6.21337/mo_parsing/helpers.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/infix.py` & `mo-parsing-8.6.21337/mo_parsing/infix.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/profile.py` & `mo-parsing-8.6.21337/mo_parsing/profile.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/regex.py` & `mo-parsing-8.6.21337/mo_parsing/regex.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/results.py` & `mo-parsing-8.6.21337/mo_parsing/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # encoding: utf-8
 import inspect
 
 from mo_dots import is_many, is_null
 from mo_future import is_text, text, NEXT, zip_longest, MutableMapping
 from mo_imports import expect, export
 
-from mo_parsing.utils import Log, listwrap
-from mo_parsing.utils import is_forward, forward_type
-
+from mo_parsing.utils import Log, listwrap, is_forward, forward_type
 
 Suppress, ParserElement, NO_PARSER, NO_RESULTS, Group, Dict, Token, Empty = expect(
     "Suppress",
     "ParserElement",
     "NO_PARSER",
     "NO_RESULTS",
     "Group",
@@ -161,32 +159,35 @@
     __nonzero__ = __bool__
 
     def __iter__(self):
         if is_forward(self.type):
             if len(self.tokens) != 1:
                 Log.error("not expected")
 
-            output = list(self.tokens[0])
-            for i in output:
-                yield i
+            yield from self.tokens[0]
             return
 
         for r in self.tokens:
             if isinstance(r, Annotation):
                 continue
             elif isinstance(r, ParseResults):
                 if isinstance(r, Annotation):
                     return
                 elif isinstance(r.type, Group):
                     yield r
                 elif is_forward(r.type) and isinstance(forward_type(r), Group):
                     yield r
+                # elif is_forward(r.type):
+                #     r = self.tokens[0]
+                #     if isinstance(r.type, Group):
+                #         yield r
+                #     else:
+                #         yield from r
                 elif not isinstance(r.type, Group):
-                    for mm in r:
-                        yield mm
+                    yield from r
             else:
                 yield r
 
     def __delitem__(self, key):
         if isinstance(key, (int, slice)):
             Log.error("not allowed")
         else:
@@ -448,8 +449,11 @@
 
     def __repr__(self):
         return "Annotation(" + repr(self.name) + ", " + repr(self.tokens) + ")"
 
 
 MutableMapping.register(ParseResults)
 
+from mo_parsing import utils
+utils.register_type(ParseResults)
+
 export("mo_parsing.utils", ParseResults)
```

### Comparing `mo-parsing-8.4.21326/mo_parsing/tokens.py` & `mo-parsing-8.6.21337/mo_parsing/tokens.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing/utils.py` & `mo-parsing-8.6.21337/mo_parsing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 
 MAX_INT = sys.maxsize
 empty_list = []
 empty_tuple = tuple()
 many_types = (list, tuple, set) + generator_types
 
 
+def register_type(t):
+    global many_types
+    many_types = many_types + (t,)
+
+
 def extend(cls):
     """
     DECORATOR TO ADD METHODS TO CLASSES
     :param cls: THE CLASS TO ADD THE METHOD TO
     :return:
     """
```

### Comparing `mo-parsing-8.4.21326/mo_parsing/whitespaces.py` & `mo-parsing-8.6.21337/mo_parsing/whitespaces.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.4.21326/mo_parsing.egg-info/PKG-INFO` & `mo-parsing-8.6.21337/mo_parsing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-parsing
-Version: 8.4.21326
+Version: 8.6.21337
 Summary: Another PEG Parsing Tool
 Home-page: https://github.com/klahnakoski/mo-parsing
 Author: Various
 Author-email: kyle@lahnakoski.com
 License: MIT
 Description: # More Parsing!
```

### Comparing `mo-parsing-8.4.21326/setup.py` & `mo-parsing-8.6.21337/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     install_requires=["mo-dots==8.4.21326","mo-future==6.2.21303"],
     license='MIT',
     long_description='# More Parsing!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)\n[![Build Status](https://app.travis-ci.com/klahnakoski/mo-parsing.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-parsing)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)\n\nA fork of [pyparsing](https://github.com/pyparsing/pyparsing) for faster parsing\n\n\n## Installation\n\nThis is a pypi package\n\n    pip install mo-parsing\n    \n## Usage\n\nThis module allows you to define a PEG parser using predefined patterns and Python operators.  Here is an example \n\n```\n>>> from mo_parsing import Word\n>>> from mo_parsing.utils import alphas\n>>>\n>>> greet = Word(alphas)("greeting") + "," + Word(alphas)("person") + "!"\n>>> result = greet.parse_string("Hello, World!")\n```\n\nThe `result` can be accessed as a nested list\n\n```\n>>> list(result)\n[\'Hello\', \',\', \'World\', \'!\']\n```\n\nThe `result` can also be accessed as a dictionary\n\n```\n>>> dict(result)\n{\'greeting\': \'Hello\', \'person\': \'World\'}\n```\n\nRead the [pyparsing documentation](https://github.com/pyparsing/pyparsing/#readme) for more\n\n### The `Whitespace` Skipper\n\nThe `mo_parsing.whitespaces.CURRENT` is used during parser creation: It is effectively defines what "whitespace" to skip during parsing, with additional features to simplify the language definition.  You declare "standard" `Whitespace` like so:\n\n    with Whitespace() as whitespace:\n        # PUT YOUR LANGUAGE DEFINITION HERE (space, tab and CR are "whitespace")\n\nIf you are declaring a large language, and you want to minimize indentation, and you are careful, you may also use this pattern:\n\n    whitespace = Whitespace().use()\n    # PUT YOUR LANGUAGE DEFINITION HERE\n    whitespace.release()\n\nThe whitespace can be used to set global parsing parameters, like\n\n* `set_whitespace()` - set the ignored characters (default: `"\\t\\n "`)\n* `add_ignore()` - include whole patterns that are ignored (like comments)\n* `set_literal()` - Set the definition for what `Literal()` means\n* `set_keyword_chars()` - For default `Keyword()` (important for defining word boundary)\n\n\n### Navigating ParseResults\n\nThe results of parsing are in `ParseResults` and are in the form of an n-ary tree; with the children found in `ParseResults.tokens`.  Each `ParseResult.type` points to the `ParserElement` that made it.  In general, if you want to get fancy with post processing (or in a `parse_action`), you will be required to navigate the raw `tokens` to generate a final result\n\nThere are some convenience methods;  \n* `__iter__()` - allows you to iterate through parse results in **depth first search**. Empty results are skipped, and `Group`ed results are treated as atoms (which can be further iterated if required) \n* `name` is a convenient property for `ParseResults.type.token_name`\n* `__getitem__()` - allows you to jump into the parse tree to the given `name`. This is blocked by any names found inside `Group`ed results (because groups are considered atoms).      \n\n### Parse Actions\n\nParse actions are methods that are run after a ParserElement found a match. \n\n* Parameters must be accepted in `(tokens, index, string)` order (the opposite of pyparsing)\n* Parse actions are wrapped to ensure the output is a legitimate ParseResult\n  * If your parse action returns `None` then the result is the original `tokens`\n  * If your parse action returns an object, or list, or tuple, then it will be packaged in a `ParseResult` with same type as `tokens`.\n  * If your parse action returns a `ParseResult` then it is accepted ***even if is belongs to some other pattern***\n  \n#### Simple example:\n\n```\ninteger = Word("0123456789").add_parse_action(lambda t, i, s: int(t[0]))\nresult = integer.parse_string("42")\nassert (result[0] == 42)\n```\n\nFor slightly shorter specification, you may use the `/` operator and only parameters you need:\n\n```\ninteger = Word("0123456789") / (lambda t: int(t[0]))\nresult = integer.parse_string("42")\nassert (result[0] == 42)\n```\n\n### Debugging\n\nThe PEG-style of mo-parsing (from pyparsing) makes a very expressible and readable specification, but debugging a parser is still hard.  To look deeper into what the parser is doing use the `Debugger`:\n\n```\nwith Debugger():\n    expr.parse_string("my new language")\n```\n\nThe debugger will print out details of what\'s happening\n\n* Each attempt, and if it matched or failed\n* A small number of bytes to show you the current position\n* location, line and column for more info about the current position\n* whitespace indicating stack depth\n* print out of the ParserElement performing the attempt\n\nThis should help to isolate the exact position your grammar is failing. \n\n### Regular Expressions\n\n`mo-parsing` can parse and generate regular expressions. `ParserElement` has a `__regex__()` function that returns the regular expression for the given grammar; which works up to a limit, and is used internally to accelerate parsing.  The `Regex` class parses regular expressions into a grammar; it is used to optimize parsing, and you may find it useful to decompose regular expressions that look like line noise.\n\n\n\n\n\n\n\n\n\n\n## Differences from PyParsing\n\nThis fork was originally created to support faster parsing for [mo-sql-parsing](https://github.com/klahnakoski/moz-sql-parser).  Since then it has deviated sufficiently to be it\'s own collection of parser specification functions.  Here are the differences:\n\n* Added `Whitespace`, which controls parsing context and whitespace.  It replaces the whitespace modifying methods of pyparsing\n* the wildcard ("`*`") could be used in pyparsing to indicate multi-values are expected; this is not allowed in `mo-parsing`: all values are multi-values\n* ParserElements are static: For example, `expr.add_parse_action(action)` creates a new ParserElement, so must be assigned to variable or it is lost. **This is the biggest source of bugs when converting from pyparsing**\n* removed all backward-compatibility settings\n* no support for binary serialization (no pickle)\n\nFaster Parsing\n\n* faster infix operator parsing (main reason for this fork)\n* ParseResults point to ParserElement for reduced size\n* regex used to reduce the number of failed parse attempts  \n* packrat parser is not need\n* less stack used \n\n\n\n## Contributing\n\nIf you plan to extend or enhance this code, please [see the README in the tests directory](https://github.com/klahnakoski/mo-parsing/blob/dev/tests/README.md)',
     long_description_content_type='text/markdown',
     name='mo-parsing',
     packages=["mo_parsing"],
     url='https://github.com/klahnakoski/mo-parsing',
-    version='8.4.21326'
+    version='8.6.21337'
 )
```

