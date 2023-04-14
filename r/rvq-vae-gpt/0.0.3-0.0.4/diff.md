# Comparing `tmp/rvq-vae-gpt-0.0.3.tar.gz` & `tmp/rvq-vae-gpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rvq-vae-gpt-0.0.3.tar", last modified: Mon Mar 13 20:13:50 2023, max compression
+gzip compressed data, was "rvq-vae-gpt-0.0.4.tar", last modified: Fri Apr 14 16:37:21 2023, max compression
```

## Comparing `rvq-vae-gpt-0.0.3.tar` & `rvq-vae-gpt-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:13:50.107782 rvq-vae-gpt-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-13 20:13:19.000000 rvq-vae-gpt-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-13 20:13:50.107782 rvq-vae-gpt-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-13 20:13:19.000000 rvq-vae-gpt-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:13:50.107782 rvq-vae-gpt-0.0.3/rvq_vae_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-13 20:13:19.000000 rvq-vae-gpt-0.0.3/rvq_vae_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-03-13 20:13:19.000000 rvq-vae-gpt-0.0.3/rvq_vae_gpt/rvq_vae_gpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:13:50.107782 rvq-vae-gpt-0.0.3/rvq_vae_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-13 20:13:50.000000 rvq-vae-gpt-0.0.3/rvq_vae_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-13 20:13:50.000000 rvq-vae-gpt-0.0.3/rvq_vae_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 20:13:50.000000 rvq-vae-gpt-0.0.3/rvq_vae_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-13 20:13:50.000000 rvq-vae-gpt-0.0.3/rvq_vae_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-13 20:13:50.000000 rvq-vae-gpt-0.0.3/rvq_vae_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 20:13:50.107782 rvq-vae-gpt-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-13 20:13:19.000000 rvq-vae-gpt-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:37:21.420644 rvq-vae-gpt-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 16:37:11.000000 rvq-vae-gpt-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 16:37:21.420644 rvq-vae-gpt-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-14 16:37:11.000000 rvq-vae-gpt-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:37:21.420644 rvq-vae-gpt-0.0.4/rvq_vae_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 16:37:11.000000 rvq-vae-gpt-0.0.4/rvq_vae_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-04-14 16:37:11.000000 rvq-vae-gpt-0.0.4/rvq_vae_gpt/rvq_vae_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:37:21.420644 rvq-vae-gpt-0.0.4/rvq_vae_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 16:37:21.000000 rvq-vae-gpt-0.0.4/rvq_vae_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 16:37:21.000000 rvq-vae-gpt-0.0.4/rvq_vae_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:37:21.000000 rvq-vae-gpt-0.0.4/rvq_vae_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 16:37:21.000000 rvq-vae-gpt-0.0.4/rvq_vae_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 16:37:21.000000 rvq-vae-gpt-0.0.4/rvq_vae_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:37:21.420644 rvq-vae-gpt-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-14 16:37:11.000000 rvq-vae-gpt-0.0.4/setup.py
```

### Comparing `rvq-vae-gpt-0.0.3/LICENSE` & `rvq-vae-gpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rvq-vae-gpt-0.0.3/PKG-INFO` & `rvq-vae-gpt-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvq-vae-gpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Yet another attempt at GPT in quantized latent space
 Home-page: https://github.com/lucidrains/rvq-vae-gpt
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rvq-vae-gpt-0.0.3/README.md` & `rvq-vae-gpt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rvq-vae-gpt-0.0.3/rvq_vae_gpt/rvq_vae_gpt.py` & `rvq-vae-gpt-0.0.4/rvq_vae_gpt/rvq_vae_gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
         dim = cast_tuple(dim, num_layers)
         depth = cast_tuple(depth, num_layers)
         local_attn_window_size = cast_tuple(local_attn_window_size, num_layers)
 
         assert num_layers == len(depth) == len(local_attn_window_size) == len(dim)
 
-        init_dim, *_, vq_dim = dim
+        init_dim, vq_dim = dim[0], dim[-1]
 
         dims = [first(dim), *dim]
         dim_pairs = tuple(zip(dims[:-1], dims[1:]))
 
         self.token_emb = nn.Embedding(num_tokens, init_dim)
 
         self.total_strides = torch.tensor(list(strides)).cumprod(dim = -1)[-1].item()
```

### Comparing `rvq-vae-gpt-0.0.3/rvq_vae_gpt.egg-info/PKG-INFO` & `rvq-vae-gpt-0.0.4/rvq_vae_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvq-vae-gpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Yet another attempt at GPT in quantized latent space
 Home-page: https://github.com/lucidrains/rvq-vae-gpt
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rvq-vae-gpt-0.0.3/setup.py` & `rvq-vae-gpt-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rvq-vae-gpt',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'Yet another attempt at GPT in quantized latent space',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/rvq-vae-gpt',
   keywords = [
```

