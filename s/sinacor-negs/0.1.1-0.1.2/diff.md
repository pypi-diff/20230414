# Comparing `tmp/sinacor_negs-0.1.1.tar.gz` & `tmp/sinacor_negs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinacor_negs-0.1.1.tar", max compression
+gzip compressed data, was "sinacor_negs-0.1.2.tar", max compression
```

## Comparing `sinacor_negs-0.1.1.tar` & `sinacor_negs-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 sinacor_negs-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      495 2023-04-14 18:37:25.317262 sinacor_negs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      730 2023-04-14 18:46:01.625815 sinacor_negs-0.1.1/README.md
--rw-r--r--   0        0        0       57 2023-04-14 18:43:29.830332 sinacor_negs-0.1.1/sinacor_negs/__init__.py
--rw-r--r--   0        0        0      678 2023-04-14 18:38:11.492281 sinacor_negs-0.1.1/sinacor_negs/negs.py
--rw-r--r--   0        0        0     5450 2023-04-14 18:44:16.598652 sinacor_negs-0.1.1/sinacor_negs/reader.py
--rw-r--r--   0        0        0      224 2023-04-14 18:43:33.618980 sinacor_negs-0.1.1/sinacor_negs/utils.py
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 sinacor_negs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 sinacor_negs-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      556 2023-04-14 18:50:03.179858 sinacor_negs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      730 2023-04-14 18:46:01.625815 sinacor_negs-0.1.2/README.md
+-rw-r--r--   0        0        0       57 2023-04-14 18:43:29.830332 sinacor_negs-0.1.2/sinacor_negs/__init__.py
+-rw-r--r--   0        0        0      678 2023-04-14 18:38:11.492281 sinacor_negs-0.1.2/sinacor_negs/negs.py
+-rw-r--r--   0        0        0     5450 2023-04-14 18:44:16.598652 sinacor_negs-0.1.2/sinacor_negs/reader.py
+-rw-r--r--   0        0        0      224 2023-04-14 18:43:33.618980 sinacor_negs-0.1.2/sinacor_negs/utils.py
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 sinacor_negs-0.1.2/PKG-INFO
```

### Comparing `sinacor_negs-0.1.1/LICENSE.txt` & `sinacor_negs-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sinacor_negs-0.1.1/README.md` & `sinacor_negs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sinacor_negs-0.1.1/sinacor_negs/negs.py` & `sinacor_negs-0.1.2/sinacor_negs/negs.py`

 * *Files identical despite different names*

### Comparing `sinacor_negs-0.1.1/sinacor_negs/reader.py` & `sinacor_negs-0.1.2/sinacor_negs/reader.py`

 * *Files identical despite different names*

### Comparing `sinacor_negs-0.1.1/PKG-INFO` & `sinacor_negs-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: sinacor-negs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Leitor do arquivo NEGS.txt da B3 (Sinacor)
+Home-page: https://github.com/renanmoretto/sinacor_negs
 License: MIT
 Author: renanmoretto
 Author-email: himynameisrenan@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Project-URL: Repository, https://github.com/renanmoretto/sinacor_negs
 Description-Content-Type: text/markdown
 
 # sinacor_negs
 'sinacor_negs' é uma lib feita para facilitar a leitura de arquivos negs.txt da bolsa (B3/Sinacor). A lib foi feita utilizando pandas e retorna os dados em forma de DataFrames.
 
 Para mais informações sobre o formato do arquivo:
 https://clientes.b3.com.br/data/files/95/D2/6D/BC/0556F71034D833F7BFC9F9C2/Leiautes%20de%20Arquivos%20SINACOR%20-%20Ampliacao%20Codigo%20do%20Investidor_v2.pdf
```

