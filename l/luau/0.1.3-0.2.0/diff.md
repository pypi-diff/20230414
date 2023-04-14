# Comparing `tmp/luau-0.1.3.tar.gz` & `tmp/luau-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.1.3.tar", last modified: Fri Apr  7 08:55:04 2023, max compression
+gzip compressed data, was "luau-0.2.0.tar", last modified: Fri Apr 14 03:20:29 2023, max compression
```

## Comparing `luau-0.1.3.tar` & `luau-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 08:55:04.598539 luau-0.1.3/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-07 08:55:04.597535 luau-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.1.3/README.md
--rw-rw-rw-   0        0        0      430 2023-04-07 08:54:08.000000 luau-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 08:55:04.598539 luau-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-07 08:55:04.568352 luau-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 08:55:04.576235 luau-0.1.3/src/luau/
--rw-rw-rw-   0        0        0     4309 2023-04-07 07:25:51.000000 luau-0.1.3/src/luau/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:55:04.596538 luau-0.1.3/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-07 08:55:04.000000 luau-0.1.3/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-04-07 08:55:04.000000 luau-0.1.3/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 08:55:04.000000 luau-0.1.3/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-07 08:55:04.000000 luau-0.1.3/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.765372 luau-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-14 03:20:29.765372 luau-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.0/README.md
+-rw-rw-rw-   0        0        0      494 2023-04-14 03:20:09.000000 luau-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 03:20:29.766369 luau-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.728628 luau-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.739314 luau-0.2.0/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.0/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.0/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.0/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.763381 luau-0.2.0/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-14 03:05:42.000000 luau-0.2.0/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-14 03:08:13.000000 luau-0.2.0/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1420 2023-04-14 03:05:42.000000 luau-0.2.0/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      839 2023-04-14 02:57:33.000000 luau-0.2.0/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2464 2023-04-14 03:14:17.000000 luau-0.2.0/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:20:29.756397 luau-0.2.0/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-14 03:20:29.000000 luau-0.2.0/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.1.3/LICENSE` & `luau-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.1.3/src/luau/__init__.py` & `luau-0.2.0/src/luau/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,144 +1,135 @@
-import re
-from typing import Any
 
-# creates a recursive luau table
-def insert_comma(enabled: bool) -> str:
+READ_STR_AS_LITERAL_PREFIX = "<LITERAL_STRING_START>_!_"
+READ_STR_AS_LITERAL_SUFFIX = "_!_<LITERAL_STRING_END>"
+
+def _insert_comma(enabled: bool) -> str:
 	if enabled:
 		return ","
 	else:
 		return ""
 
-def get_indent(indent_count: int) -> str:
+def _get_indent(indent_count: int) -> str:
 	return "\t"*indent_count
 
-def dump_bool(value: bool, indent_count=0, add_comma_at_end=False) -> str:
-	return get_indent(indent_count) + str(value).lower() + insert_comma(add_comma_at_end)
+def from_bool(value: bool, indent_count=0, add_comma_at_end=False) -> str:
+	return _get_indent(indent_count) + str(value).lower() + _insert_comma(add_comma_at_end)
 
-def dump_str(value: str, indent_count=0, add_comma_at_end=False) -> str:
-	return get_indent(indent_count) + f"\"{value}\"" + insert_comma(add_comma_at_end)
+def from_str(value: str, indent_count=0, add_comma_at_end=False) -> str:
+	suffix_index = value.find(READ_STR_AS_LITERAL_SUFFIX)
+	
+	starts_with_prefix = READ_STR_AS_LITERAL_PREFIX == value[0:len(READ_STR_AS_LITERAL_PREFIX)]
+	if starts_with_prefix and suffix_index != -1:
+		raw_val = value.replace(READ_STR_AS_LITERAL_PREFIX, "").replace(READ_STR_AS_LITERAL_SUFFIX, "")
+		return _get_indent(indent_count) + raw_val + _insert_comma(add_comma_at_end)
+	else:
+		return _get_indent(indent_count) + f"\"{value}\"" + _insert_comma(add_comma_at_end)
 
-def dump_number(value: int | float, indent_count=0, add_comma_at_end=False) -> str:
-	return get_indent(indent_count) + str(value) + insert_comma(add_comma_at_end)
+def from_number(value: int | float, indent_count=0, add_comma_at_end=False) -> str:
+	return _get_indent(indent_count) + str(value) + _insert_comma(add_comma_at_end)
 
-def dump_nil(indent_count=0, add_comma_at_end=False) -> str:
-	return f"{get_indent(indent_count)} nil" + insert_comma(add_comma_at_end)
+def from_nil(indent_count=0, add_comma_at_end=False) -> str:
+	return f"{_get_indent(indent_count)} nil" + _insert_comma(add_comma_at_end)
 
 
-def dump_list(value: list, indent_count=0, add_comma_at_end=False, multi_line=True, skip_initial_indent=False):
+def from_list(value: list, indent_count=0, add_comma_at_end=False, multi_line=True, skip_initial_indent=False):
 	
 	# start list
 	list_val = ""
 	if skip_initial_indent:
 		list_val += "{"
 	else:
-		list_val += get_indent(indent_count) + "{"
+		list_val += _get_indent(indent_count) + "{"
 
 	# iterate through values
 	for v in value:
 		
 		# write entry
 		if type(v) == dict or type(v) == list:
-			entry = dump(v, indent_count+1, False, multi_line, True) + insert_comma(True)
+			entry = from_any(v, indent_count+1, False, multi_line, True) + _insert_comma(True)
 		else:
-			entry = dump(v, indent_count, False, multi_line, True) + insert_comma(True)
+			entry = from_any(v, indent_count, False, multi_line, True) + _insert_comma(True)
 
 		# add it to existing string
 		if multi_line:
-			list_val += "\n" + get_indent(indent_count+1) + entry
+			list_val += "\n" + _get_indent(indent_count+1) + entry
 		else:
 			list_val += entry
 
 	# end the table on a new line if multi-line
 	if multi_line:
-		list_val += "\n" + get_indent(indent_count)
+		list_val += "\n" + _get_indent(indent_count)
 
 	# close the table
 	list_val += "}"
 
 	# indent as needed and return value
-	return get_indent(indent_count) + list_val + insert_comma(add_comma_at_end)
+	return _get_indent(indent_count) + list_val + _insert_comma(add_comma_at_end)
 
-def dump_dict(value: dict, indent_count=0, add_comma_at_end=False, multi_line=True, skip_initial_indent=False):
+def from_dict(value: dict, indent_count=0, add_comma_at_end=False, multi_line=True, skip_initial_indent=False):
 	
 	# start dictionary
 	list_val = ""
 	if skip_initial_indent:
 		list_val += "{"
 	else:
-		list_val += get_indent(indent_count) + "{"
+		list_val += _get_indent(indent_count) + "{"
 
 	# iterate through key-val pairs
 	for k, v in value.items():
 
 		# write entry
 		if type(v) == dict or type(v) == list:
-			entry = f"[{dump(k, 0, False)}] = {dump(v, indent_count+1, False, multi_line, True)}" + insert_comma(True)
+			entry = f"[{from_any(k, 0, False)}] = {from_any(v, indent_count+1, False, multi_line, True)}" + _insert_comma(True)
 		else:
-			entry = f"[{dump(k, 0, False)}] = {dump(v, 0, False, multi_line, True)}" + insert_comma(True)
+			entry = f"[{from_any(k, 0, False)}] = {from_any(v, 0, False, multi_line, True)}" + _insert_comma(True)
 
 		# add it to existing string
 		if multi_line:
-			list_val += "\n" + get_indent(indent_count+1) + entry
+			list_val += "\n" + _get_indent(indent_count+1) + entry
 		else:
 			list_val += entry
 
 	# end the table on a new line if multi-line
 	if multi_line:
-		list_val += "\n" + get_indent(indent_count)
+		list_val += "\n" + _get_indent(indent_count)
 
 	# close the table
 	list_val += "}"
 
 	# indent as needed and return value
 	if skip_initial_indent:
-		return get_indent(0) + list_val + insert_comma(add_comma_at_end)
-	else:
-		return get_indent(indent_count) + list_val + insert_comma(add_comma_at_end)
-
-def dump_type(type_table: dict, indent_count=0, skip_initial_indent=False, add_comma_at_end = False) -> str:
-	out = ""
-	if skip_initial_indent:
-		out += "{"
+		return _get_indent(0) + list_val + _insert_comma(add_comma_at_end)
 	else:
-		out += get_indent(indent_count) + "{"
+		return _get_indent(indent_count) + list_val + _insert_comma(add_comma_at_end)
 
-	for k in type_table:
-		v = type_table[k]
-
-		# write entry
-		if type(v) == dict or type(v) == list:
-			entry = f"{k}: {dump_type(type_table, indent_count+1, True, False)}" + insert_comma(True)
-		else:
-			entry = f"{k}: {v}" + insert_comma(True)
-	
-		out += "\n" + get_indent(indent_count+1) + entry
-
-	out += "\n" + get_indent(indent_count) + "}" + insert_comma(add_comma_at_end)
-	return out
-
-def dump(
+def from_any(
 	value: int | str | None | float | dict | list = None, 
 	indent_count = 0, 
 	add_comma_at_end = False, 
 	multi_line=True,
 	skip_initial_indent=False
 ) -> str:
 
 	if type(value) == list:
 
-		return dump_list(value, indent_count, add_comma_at_end, multi_line, skip_initial_indent)
+		return from_list(value, indent_count, add_comma_at_end, multi_line, skip_initial_indent)
 
 	elif type(value) == dict:
 		
-		return dump_dict(value, indent_count, add_comma_at_end, multi_line, skip_initial_indent)
+		return from_dict(value, indent_count, add_comma_at_end, multi_line, skip_initial_indent)
 
 	elif type(value) == float or type(value) == int:
-		return dump_number(value, indent_count, add_comma_at_end)
+		return from_number(value, indent_count, add_comma_at_end)
 		
 	elif type(value) == bool:
-		return dump_bool(value, indent_count, add_comma_at_end)
+		return from_bool(value, indent_count, add_comma_at_end)
 		
 	elif type(value) == str:
-		return dump_str(value, indent_count, add_comma_at_end)
+		return from_str(value, indent_count, add_comma_at_end)
 		
-	return dump_nil(indent_count, add_comma_at_end)
+	return from_nil(indent_count, add_comma_at_end)
+
+
+# allows for processing of text in the other methods as is without being wrapped in quotes as a string
+def mark_as_literal(text: str) -> str:
+	return READ_STR_AS_LITERAL_PREFIX+text+READ_STR_AS_LITERAL_SUFFIX
```

