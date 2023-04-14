# Comparing `tmp/x-Metaformer-0.2.9.tar.gz` & `tmp/x-Metaformer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-Metaformer-0.2.9.tar", last modified: Wed Mar 29 13:17:28 2023, max compression
+gzip compressed data, was "x-Metaformer-0.3.0.tar", last modified: Fri Apr 14 10:29:19 2023, max compression
```

## Comparing `x-Metaformer-0.2.9.tar` & `x-Metaformer-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:17:28.777832 x-Metaformer-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-29 13:17:28.777832 x-Metaformer-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 13:17:28.777832 x-Metaformer-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:17:28.777832 x-Metaformer-0.2.9/x_Metaformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-29 13:17:28.000000 x-Metaformer-0.2.9/x_Metaformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-29 13:17:28.000000 x-Metaformer-0.2.9/x_Metaformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:17:28.000000 x-Metaformer-0.2.9/x_Metaformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-29 13:17:28.000000 x-Metaformer-0.2.9/x_Metaformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-29 13:17:28.000000 x-Metaformer-0.2.9/x_Metaformer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:17:28.777832 x-Metaformer-0.2.9/x_metaformer/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:17:28.777832 x-Metaformer-0.2.9/x_metaformer/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/layers/act_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/layers/attention_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/layers/conv_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/layers/mixing_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/layers/mlp_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/layers/norm_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/metaformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:17:28.777832 x-Metaformer-0.2.9/x_metaformer/pretraining/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/pretraining/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/pretraining/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/pretraining/mocov3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-29 13:17:17.000000 x-Metaformer-0.2.9/x_metaformer/pretraining/vicreg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/x_Metaformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 10:29:19.000000 x-Metaformer-0.3.0/x_Metaformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/x_metaformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/x_metaformer/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/act_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/attention_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/conv_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/mixing_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/mlp_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/layers/norm_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/metaformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:29:19.447666 x-Metaformer-0.3.0/x_metaformer/pretraining/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/pretraining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/pretraining/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/pretraining/mocov3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 10:29:05.000000 x-Metaformer-0.3.0/x_metaformer/pretraining/vicreg.py
```

### Comparing `x-Metaformer-0.2.9/LICENSE` & `x-Metaformer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/PKG-INFO` & `x-Metaformer-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-Metaformer
-Version: 0.2.9
+Version: 0.3.0
 Summary: A PyTorch implementation of "MetaFormer Baselines" with optional extensions.
 Home-page: https://github.com/romue404/x-metaformer
 Author: Robert Müller
 Author-email: robert.mueller1990@googlemail.com
 License: MIT
 Keywords: artificial intelligence,pytorch,metaformer,transformer,attention,convolutions
 Classifier: Development Status :: 4 - Beta
```

### Comparing `x-Metaformer-0.2.9/README.md` & `x-Metaformer-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/setup.py` & `x-Metaformer-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='x-Metaformer',
-      version='0.2.9',
+      version='0.3.0',
       description='A PyTorch implementation of "MetaFormer Baselines" with optional extensions.',
       author='Robert Müller',
       author_email='robert.mueller1990@googlemail.com',
       url='https://github.com/romue404/x-metaformer',
       license='MIT',
       keywords=[
             'artificial intelligence',
```

### Comparing `x-Metaformer-0.2.9/x_Metaformer.egg-info/PKG-INFO` & `x-Metaformer-0.3.0/x_Metaformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-Metaformer
-Version: 0.2.9
+Version: 0.3.0
 Summary: A PyTorch implementation of "MetaFormer Baselines" with optional extensions.
 Home-page: https://github.com/romue404/x-metaformer
 Author: Robert Müller
 Author-email: robert.mueller1990@googlemail.com
 License: MIT
 Keywords: artificial intelligence,pytorch,metaformer,transformer,attention,convolutions
 Classifier: Development Status :: 4 - Beta
```

### Comparing `x-Metaformer-0.2.9/x_Metaformer.egg-info/SOURCES.txt` & `x-Metaformer-0.3.0/x_Metaformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/layers/act_layers.py` & `x-Metaformer-0.3.0/x_metaformer/layers/act_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/layers/attention_layers.py` & `x-Metaformer-0.3.0/x_metaformer/layers/attention_layers.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,47 +15,61 @@
                  proj_dropout=0.0,
                  scale_value=1.0,
                  num_mem_vecs=0,
                  sparse_topk=0,
                  l2=False,
                  trainable_scale=False,
                  improve_locality=False,
+                 multi_query_attention=False,
                  **kwargs):
         super().__init__()
         assert channel_loc in [1, -1], 'Token dimension must be 1 or -1.'
         assert scale_value > 0, 'scale_value must be > 0'
         self.num_heads       = num_heads
         self.trainable_scale = trainable_scale
         self.head_dim        = head_dim
         self.dim             = dim
         self.channel_dim  = channel_loc
         self.sparse_topk  = sparse_topk
         self.num_mem_vecs = num_mem_vecs
         self.improve_locality = improve_locality
         self.l2 = l2
+        self.mqa = multi_query_attention
+
+        n_qkv = 3*self.head_dim*self.num_heads if not self.mqa else self.head_dim*self.num_heads + 2*self.head_dim
+
         self.qkv = GeneralizedLinear(in_features=self.dim,
-                                     out_features=3*self.head_dim*self.num_heads,
+                                     out_features=n_qkv,
                                      feature_dim=channel_loc,
                                      bias=False
                                      )
+
         self.proj_out = GeneralizedLinear(in_features=self.head_dim*self.num_heads,
                                           out_features=self.dim,
                                           feature_dim=channel_loc,
                                           bias=False
                                           )
         self.proj_dropout = nn.Dropout(proj_dropout)
         self.attn_dropout = nn.Dropout(attn_dropout)
         self.scale = nn.Parameter(torch.ones(1, num_heads, 1, 1).mul_(scale_value).float(),
                                   requires_grad=trainable_scale)
         if num_mem_vecs > 0:
             self.mem_k = nn.Parameter(torch.randn(num_heads, num_mem_vecs, head_dim))
             self.mem_v = nn.Parameter(torch.randn(num_heads, num_mem_vecs, head_dim))
 
     def reshape_qkv(self, qkv):
-        return qkv.reshape(3, qkv.shape[0], self.num_heads, -1, self.head_dim)
+        B = qkv.shape[0]
+        if self.mqa:
+            hd2 =  2*self.head_dim
+            kv  = qkv[:, :hd2] if self.channel_dim == 1 else qkv[..., :hd2]
+            q   = qkv[:, hd2:] if self.channel_dim == 1 else qkv[..., hd2:]
+            q   = q.reshape(B, self.num_heads, -1, self.head_dim)
+            kv  = kv.reshape(2, B, 1, -1, self.head_dim)
+            return q, *(kv.unbind(0))
+        return qkv.reshape(3, B, self.num_heads, -1, self.head_dim).unbind(0)
 
     def reshape_attention(self, attention, x_shape):
         if len(x_shape) > 3:  # initial shape of  B C H W or B H W C
             shape = (-1, *tuple(x_shape[2:])) if self.channel_dim == 1 else (*tuple(x_shape[1:3]), -1)
             return attention.transpose(1, 2).flatten(-2).reshape(x_shape[0], *shape)
         return attention
 
@@ -86,30 +100,35 @@
         if self.improve_locality:
             mask = torch.eye(*scores.shape[-2:], device=scores.device).bool()
             mask_value = -torch.finfo(scores.dtype).max
             scores.masked_fill_(mask, mask_value)  # inplace
         return scores
 
     def forward(self, x):
-        qkv = self.reshape_qkv(self.qkv(x))
-        q, k, v = qkv.unbind(0)
+        q, k, v = self.reshape_qkv(self.qkv(x))
         k, v = self.cat_mem_vecs(k, v, x.shape[0])
         scores = self.sparsify(self.adjust_scores(self.scale_scores(self.compute_scores(q, k))))
         attention = self.attn_dropout(scores.softmax(-1)) @ v
         out = self.reshape_attention(attention, x.shape)
         return self.proj_dropout(self.proj_out(out))
 
 
 AttentionConv = partial(Attention, 1)
 
 
 
 if __name__ == '__main__':
     for c, f, t in [(64, 16, 8), (128, 22, 44)]:
         test_batch = torch.randn(12, c, f, t)
-        print(f'Attention:   {AttentionConv(c, l2=True, scale_value=10, trainable_scale=False)(test_batch).shape}')
+        out = AttentionConv(c, l2=True, scale_value=10,
+                            trainable_scale=False,
+                            multi_query_attention=True)(test_batch)
+        print(f'Attention:   {out.shape}')
     print('TinyTest1 successful')
 
     for c, f, t in [(64, 16, 8), (128, 22, 44)]:
         test_batch = torch.randn(12, f, t, c)
-        print(f'Attention:   {Attention(-1, c, l2=True, scale_value=10, trainable_scale=False)(test_batch).shape}')
+        out = Attention(-1, c, l2=True, scale_value=10,
+                        trainable_scale=False,
+                        multi_query_attention=True)(test_batch)
+        print(f'Attention:   {out.shape}')
     print('TinyTest2 successful')
```

### Comparing `x-Metaformer-0.2.9/x_metaformer/layers/conv_layers.py` & `x-Metaformer-0.3.0/x_metaformer/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/layers/mixing_layers.py` & `x-Metaformer-0.3.0/x_metaformer/layers/mixing_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/layers/mlp_layers.py` & `x-Metaformer-0.3.0/x_metaformer/layers/mlp_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/layers/norm_layers.py` & `x-Metaformer-0.3.0/x_metaformer/layers/norm_layers.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/metaformer.py` & `x-Metaformer-0.3.0/x_metaformer/metaformer.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/misc.py` & `x-Metaformer-0.3.0/x_metaformer/misc.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/pretraining/barlowtwins.py` & `x-Metaformer-0.3.0/x_metaformer/pretraining/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/pretraining/mocov3.py` & `x-Metaformer-0.3.0/x_metaformer/pretraining/mocov3.py`

 * *Files identical despite different names*

### Comparing `x-Metaformer-0.2.9/x_metaformer/pretraining/vicreg.py` & `x-Metaformer-0.3.0/x_metaformer/pretraining/vicreg.py`

 * *Files identical despite different names*

