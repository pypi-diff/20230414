# Comparing `tmp/vagas_cfs-0.1.tar.gz` & `tmp/vagas_cfs-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagas_cfs-0.1.tar", last modified: Fri Apr 14 13:05:18 2023, max compression
+gzip compressed data, was "vagas_cfs-0.2.tar", last modified: Fri Apr 14 14:02:48 2023, max compression
```

## Comparing `vagas_cfs-0.1.tar` & `vagas_cfs-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:05:18.629483 vagas_cfs-0.1/
--rw-rw-rw-   0        0        0     1094 2023-01-27 13:16:28.000000 vagas_cfs-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-04-14 13:05:18.630567 vagas_cfs-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-04-14 12:57:05.000000 vagas_cfs-0.1/README.md
--rw-rw-rw-   0        0        0      114 2023-04-14 13:05:18.637791 vagas_cfs-0.1/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-04-14 12:57:05.000000 vagas_cfs-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:05:18.590618 vagas_cfs-0.1/vagas_cfs/
--rw-rw-rw-   0        0        0       26 2023-04-14 12:57:05.000000 vagas_cfs-0.1/vagas_cfs/__init__.py
--rw-rw-rw-   0        0        0     8578 2023-04-14 13:03:16.000000 vagas_cfs-0.1/vagas_cfs/acompanhamento-vagas-cfs.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:05:18.626384 vagas_cfs-0.1/vagas_cfs.egg-info/
--rw-rw-rw-   0        0        0      768 2023-04-14 13:05:18.000000 vagas_cfs-0.1/vagas_cfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-04-14 13:05:18.000000 vagas_cfs-0.1/vagas_cfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:05:18.000000 vagas_cfs-0.1/vagas_cfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 13:05:18.000000 vagas_cfs-0.1/vagas_cfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 14:02:48.046367 vagas_cfs-0.2/
+-rw-rw-rw-   0        0        0     1094 2023-01-27 13:16:28.000000 vagas_cfs-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-04-14 14:02:48.047366 vagas_cfs-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-04-14 12:57:05.000000 vagas_cfs-0.2/README.md
+-rw-rw-rw-   0        0        0      114 2023-04-14 14:02:48.054114 vagas_cfs-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-04-14 14:01:48.000000 vagas_cfs-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:02:48.011225 vagas_cfs-0.2/vagas_cfs/
+-rw-rw-rw-   0        0        0       41 2023-04-14 14:01:30.000000 vagas_cfs-0.2/vagas_cfs/__init__.py
+-rw-rw-rw-   0        0        0     8578 2023-04-14 13:03:16.000000 vagas_cfs-0.2/vagas_cfs/acompanhamento_vagas_cfs.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:02:48.043364 vagas_cfs-0.2/vagas_cfs.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-04-14 14:02:47.000000 vagas_cfs-0.2/vagas_cfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-04-14 14:02:47.000000 vagas_cfs-0.2/vagas_cfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:02:47.000000 vagas_cfs-0.2/vagas_cfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 14:02:47.000000 vagas_cfs-0.2/vagas_cfs.egg-info/top_level.txt
```

### Comparing `vagas_cfs-0.1/LICENSE.txt` & `vagas_cfs-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vagas_cfs-0.1/PKG-INFO` & `vagas_cfs-0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagas_cfs
-Version: 0.1
+Version: 0.2
 Summary: Conversor utilizado para a geração do Relatório de Vagas dos CFS
 Author: Gabriel Ernesto Barboza Pereira
 Author-email: ernesto.gabriel@pucpr.br
 License: MIT
 Keywords: conversor vagas_cfs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `vagas_cfs-0.1/setup.py` & `vagas_cfs-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as arq:
     readme = arq.read()
 
 setup(
     name='vagas_cfs',
-    version='0.1',
+    version='0.2',
     author='Gabriel Ernesto Barboza Pereira',
     author_email='ernesto.gabriel@pucpr.br',
     packages=['vagas_cfs'],
     description='Conversor utilizado para a geração do Relatório de Vagas dos CFS',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='MIT',
```

### Comparing `vagas_cfs-0.1/vagas_cfs/acompanhamento-vagas-cfs.py` & `vagas_cfs-0.2/vagas_cfs/acompanhamento_vagas_cfs.py`

 * *Files identical despite different names*

### Comparing `vagas_cfs-0.1/vagas_cfs.egg-info/PKG-INFO` & `vagas_cfs-0.2/vagas_cfs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagas-cfs
-Version: 0.1
+Version: 0.2
 Summary: Conversor utilizado para a geração do Relatório de Vagas dos CFS
 Author: Gabriel Ernesto Barboza Pereira
 Author-email: ernesto.gabriel@pucpr.br
 License: MIT
 Keywords: conversor vagas_cfs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

