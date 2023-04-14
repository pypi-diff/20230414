# Comparing `tmp/StaticVar-0.0.2.tar.gz` & `tmp/StaticVar-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StaticVar-0.0.2.tar", last modified: Fri Apr 14 04:42:00 2023, max compression
+gzip compressed data, was "StaticVar-0.0.3.tar", last modified: Fri Apr 14 12:15:59 2023, max compression
```

## Comparing `StaticVar-0.0.2.tar` & `StaticVar-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 04:42:00.928134 StaticVar-0.0.2/
--rw-rw-rw-   0        0        0      508 2023-04-14 04:42:00.927097 StaticVar-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-04-04 12:32:56.000000 StaticVar-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 04:42:00.915128 StaticVar-0.0.2/StaticVar/
--rw-rw-rw-   0        0        0     2084 2023-04-14 04:01:44.000000 StaticVar-0.0.2/StaticVar/StaticVar.py
--rw-rw-rw-   0        0        0       28 2023-04-14 04:01:52.000000 StaticVar-0.0.2/StaticVar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 04:42:00.926046 StaticVar-0.0.2/StaticVar.egg-info/
--rw-rw-rw-   0        0        0      508 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 04:42:00.928134 StaticVar-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-04-14 04:41:45.000000 StaticVar-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:15:59.324553 StaticVar-0.0.3/
+-rw-rw-rw-   0        0        0     1080 2023-04-14 12:04:40.000000 StaticVar-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      670 2023-04-14 12:15:59.323115 StaticVar-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1980 2023-04-14 05:00:11.000000 StaticVar-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 12:15:59.321120 StaticVar-0.0.3/StaticVar.egg-info/
+-rw-rw-rw-   0        0        0      670 2023-04-14 12:15:58.000000 StaticVar-0.0.3/StaticVar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-04-14 12:15:58.000000 StaticVar-0.0.3/StaticVar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:15:58.000000 StaticVar-0.0.3/StaticVar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 12:15:58.000000 StaticVar-0.0.3/StaticVar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:15:58.000000 StaticVar-0.0.3/StaticVar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:15:59.324553 StaticVar-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2023-04-14 12:15:54.000000 StaticVar-0.0.3/setup.py
```

### Comparing `StaticVar-0.0.2/README.md` & `StaticVar-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
 
 `> 3`<br><br>
 
 To change the value of the variable, use the `set()` method:
 
 ```python
 foo.set(4)
-print(foo.value)
+print(foo.value())
 ```
 Output:
 
 `> 4`<br><br>
 
 Alternatively, you can just redefine the variable object with the new value:
 
 ```python
 foo = StaticInt(5)
-print(foo.value)
+print(foo.value())
 ```
 Ouput:
 
 `> 5`<br><br>
 
 Variables set using the StaticVar module are not dynamic. Trying to later assign data with different types from the originally set one will raise an error if it cannot be converted/casted:
```

### Comparing `StaticVar-0.0.2/setup.py` & `StaticVar-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Static variables for Python'
 LONG_DESCRIPTION = 'Static variables for Python like in C'
 
 setup(
         name="StaticVar", 
         version=VERSION,
         author="AbdelRahman Rahal",
         author_email="<abdelrahman.rahal.mail@gmail.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
+        url="https://github.com/AbdelRahmanRahal/StaticVar",
         packages=find_packages(),
         install_requires=['varname'],
+        python_requires=">=3.10",
+
         
         keywords=['Static', 'Static Variables', 'StaticVar'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Developers",
+            "License :: OSI Approved :: MIT License",
             "Programming Language :: Python :: 3 :: Only",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

