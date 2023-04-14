# Comparing `tmp/x-Metaformer-0.3.0.tar.gz` & `tmp/x-Metaformer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-Metaformer-0.3.0.tar", last modified: Fri Apr 14 10:29:19 2023, max compression
+gzip compressed data, was "x-Metaformer-0.3.1.tar", last modified: Fri Apr 14 10:38:44 2023, max compression
```

## Comparing `x-Metaformer-0.3.0.tar` & `x-Metaformer-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/x_Metaformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/x_metaformer/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/x_metaformer/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/act_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/attention_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/conv_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/mixing_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/mlp_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/norm_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/metaformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/x_metaformer/pretraining/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/pretraining/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/pretraining/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/pretraining/mocov3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/pretraining/vicreg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:38:44.380152 x-Metaformer-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-14 10:38:44.380152 x-Metaformer-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:38:44.380152 x-Metaformer-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:38:44.376152 x-Metaformer-0.3.1/x_Metaformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-14 10:38:44.000000 x-Metaformer-0.3.1/x_Metaformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 10:38:44.000000 x-Metaformer-0.3.1/x_Metaformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:38:44.000000 x-Metaformer-0.3.1/x_Metaformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 10:38:44.000000 x-Metaformer-0.3.1/x_Metaformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 10:38:44.000000 x-Metaformer-0.3.1/x_Metaformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:38:44.376152 x-Metaformer-0.3.1/x_metaformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:38:44.376152 x-Metaformer-0.3.1/x_metaformer/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/layers/act_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/layers/attention_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/layers/conv_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/layers/mixing_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/layers/mlp_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/layers/norm_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/metaformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:38:44.380152 x-Metaformer-0.3.1/x_metaformer/pretraining/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/pretraining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/pretraining/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/pretraining/mocov3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 10:38:34.000000 x-Metaformer-0.3.1/x_metaformer/pretraining/vicreg.py
```

### Comparing `x-Metaformer-0.3.0/LICENSE` & `x-Metaformer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/PKG-INFO` & `x-Metaformer-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-Metaformer
-Version: 0.3.0
+Version: 0.3.1
 Summary: A PyTorch implementation of "MetaFormer Baselines" with optional extensions.
 Home-page: https://github.com/romue404/x-metaformer
 Author: Robert Müller
 Author-email: robert.mueller1990@googlemail.com
 License: MIT
 Keywords: artificial intelligence,pytorch,metaformer,transformer,attention,convolutions
 Classifier: Development Status :: 4 - Beta
@@ -32,14 +32,15 @@
 from x_metaformer import CAFormer, ConvFormer
 
 
 my_metaformer = CAFormer(
     in_channels=3,
     depths=(3, 3, 9, 3),
     dims=(64, 128, 320, 512),
+    multi_query_attention=False,  # share keys and values across query heads
     use_seqpool=True,  # use sequence pooling vom CCT
     init_kernel_size=3,
     init_stride=2,
     drop_path_rate=0.4,
     norm='ln',  # ln, bn, rms (layernorm, batchnorm, rmsnorm)
     use_grn_mlp=True,  # use global response norm in mlps
     use_dual_patchnorm=False,  # norm on both sides for the patch embedding
```

### Comparing `x-Metaformer-0.3.0/README.md` & `x-Metaformer-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from x_metaformer import CAFormer, ConvFormer
 
 
 my_metaformer = CAFormer(
     in_channels=3,
     depths=(3, 3, 9, 3),
     dims=(64, 128, 320, 512),
+    multi_query_attention=False,  # share keys and values across query heads
     use_seqpool=True,  # use sequence pooling vom CCT
     init_kernel_size=3,
     init_stride=2,
     drop_path_rate=0.4,
     norm='ln',  # ln, bn, rms (layernorm, batchnorm, rmsnorm)
     use_grn_mlp=True,  # use global response norm in mlps
     use_dual_patchnorm=False,  # norm on both sides for the patch embedding
```

### Comparing `x-Metaformer-0.3.0/setup.py` & `x-Metaformer-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='x-Metaformer',
-      version='0.3.0',
+      version='0.3.1',
       description='A PyTorch implementation of "MetaFormer Baselines" with optional extensions.',
       author='Robert Müller',
       author_email='robert.mueller1990@googlemail.com',
       url='https://github.com/romue404/x-metaformer',
       license='MIT',
       keywords=[
             'artificial intelligence',
```

### Comparing `x-Metaformer-0.3.0/x_Metaformer.egg-info/PKG-INFO` & `x-Metaformer-0.3.1/x_Metaformer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-Metaformer
-Version: 0.3.0
+Version: 0.3.1
 Summary: A PyTorch implementation of "MetaFormer Baselines" with optional extensions.
 Home-page: https://github.com/romue404/x-metaformer
 Author: Robert Müller
 Author-email: robert.mueller1990@googlemail.com
 License: MIT
 Keywords: artificial intelligence,pytorch,metaformer,transformer,attention,convolutions
 Classifier: Development Status :: 4 - Beta
@@ -32,14 +32,15 @@
 from x_metaformer import CAFormer, ConvFormer
 
 
 my_metaformer = CAFormer(
     in_channels=3,
     depths=(3, 3, 9, 3),
     dims=(64, 128, 320, 512),
+    multi_query_attention=False,  # share keys and values across query heads
     use_seqpool=True,  # use sequence pooling vom CCT
     init_kernel_size=3,
     init_stride=2,
     drop_path_rate=0.4,
     norm='ln',  # ln, bn, rms (layernorm, batchnorm, rmsnorm)
     use_grn_mlp=True,  # use global response norm in mlps
     use_dual_patchnorm=False,  # norm on both sides for the patch embedding
```

### Comparing `x-Metaformer-0.3.0/x_Metaformer.egg-info/SOURCES.txt` & `x-Metaformer-0.3.1/x_Metaformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/layers/act_layers.py` & `x-Metaformer-0.3.1/x_metaformer/layers/act_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/layers/attention_layers.py` & `x-Metaformer-0.3.1/x_metaformer/layers/attention_layers.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,16 +49,17 @@
                                           bias=False
                                           )
         self.proj_dropout = nn.Dropout(proj_dropout)
         self.attn_dropout = nn.Dropout(attn_dropout)
         self.scale = nn.Parameter(torch.ones(1, num_heads, 1, 1).mul_(scale_value).float(),
                                   requires_grad=trainable_scale)
         if num_mem_vecs > 0:
-            self.mem_k = nn.Parameter(torch.randn(num_heads, num_mem_vecs, head_dim))
-            self.mem_v = nn.Parameter(torch.randn(num_heads, num_mem_vecs, head_dim))
+            n_mv = num_heads if not multi_query_attention else 1
+            self.mem_k = nn.Parameter(torch.randn(n_mv, num_mem_vecs, head_dim))
+            self.mem_v = nn.Parameter(torch.randn(n_mv, num_mem_vecs, head_dim))
 
     def reshape_qkv(self, qkv):
         B = qkv.shape[0]
         if self.mqa:
             hd2 =  2*self.head_dim
             kv  = qkv[:, :hd2] if self.channel_dim == 1 else qkv[..., :hd2]
             q   = qkv[:, hd2:] if self.channel_dim == 1 else qkv[..., hd2:]
@@ -116,15 +117,15 @@
 
 
 
 if __name__ == '__main__':
     for c, f, t in [(64, 16, 8), (128, 22, 44)]:
         test_batch = torch.randn(12, c, f, t)
         out = AttentionConv(c, l2=True, scale_value=10,
-                            trainable_scale=False,
+                            trainable_scale=False, num_mem_vecs=2,
                             multi_query_attention=True)(test_batch)
         print(f'Attention:   {out.shape}')
     print('TinyTest1 successful')
 
     for c, f, t in [(64, 16, 8), (128, 22, 44)]:
         test_batch = torch.randn(12, f, t, c)
         out = Attention(-1, c, l2=True, scale_value=10,
```

### Comparing `x-Metaformer-0.3.0/x_metaformer/layers/conv_layers.py` & `x-Metaformer-0.3.1/x_metaformer/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/layers/mixing_layers.py` & `x-Metaformer-0.3.1/x_metaformer/layers/mixing_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/layers/mlp_layers.py` & `x-Metaformer-0.3.1/x_metaformer/layers/mlp_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/layers/norm_layers.py` & `x-Metaformer-0.3.1/x_metaformer/layers/norm_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/metaformer.py` & `x-Metaformer-0.3.1/x_metaformer/metaformer.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/misc.py` & `x-Metaformer-0.3.1/x_metaformer/misc.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/pretraining/barlowtwins.py` & `x-Metaformer-0.3.1/x_metaformer/pretraining/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/pretraining/mocov3.py` & `x-Metaformer-0.3.1/x_metaformer/pretraining/mocov3.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.3.0/x_metaformer/pretraining/vicreg.py` & `x-Metaformer-0.3.1/x_metaformer/pretraining/vicreg.py`

 * *Files identical despite different names*

