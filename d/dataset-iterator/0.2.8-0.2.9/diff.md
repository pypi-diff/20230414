# Comparing `tmp/dataset_iterator-0.2.8.tar.gz` & `tmp/dataset_iterator-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_iterator-0.2.8.tar", last modified: Wed Jan 25 15:09:54 2023, max compression
+gzip compressed data, was "dataset_iterator-0.2.9.tar", last modified: Fri Apr 14 08:41:18 2023, max compression
```

## Comparing `dataset_iterator-0.2.8.tar` & `dataset_iterator-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-01-25 15:09:54.701871 dataset_iterator-0.2.8/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    10141 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/LICENSE.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3541 2023-01-25 15:09:54.701871 dataset_iterator-0.2.8/PKG-INFO
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     2412 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/README.md
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-01-25 15:09:54.701871 dataset_iterator-0.2.8/dataset_iterator/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      589 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/__init__.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3335 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/concat_iterator.py
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-01-25 15:09:54.701871 dataset_iterator-0.2.8/dataset_iterator/datasetIO/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      320 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/datasetIO/__init__.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     2468 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/datasetIO/concatenate_datasetIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1540 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/datasetIO/datasetIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3011 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/datasetIO/group_datasetIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     2923 2022-05-30 11:41:58.000000 dataset_iterator-0.2.8/dataset_iterator/datasetIO/h5pyIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1306 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/datasetIO/memoryIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3632 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/datasetIO/multiple_datasetIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    11943 2022-05-31 14:54:54.000000 dataset_iterator-0.2.8/dataset_iterator/datasetIO/multiple_fileIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     7471 2022-06-08 12:38:03.000000 dataset_iterator-0.2.8/dataset_iterator/helpers.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1732 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/index_array_iterator.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    53261 2022-06-20 14:57:17.000000 dataset_iterator-0.2.8/dataset_iterator/multichannel_iterator.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      808 2022-05-17 16:13:43.000000 dataset_iterator-0.2.8/dataset_iterator/preprocessing_image_generator.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    17450 2023-01-25 15:07:22.000000 dataset_iterator-0.2.8/dataset_iterator/tile_utils.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    16622 2023-01-17 12:17:24.000000 dataset_iterator-0.2.8/dataset_iterator/tracking_iterator.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3984 2022-06-20 14:21:49.000000 dataset_iterator-0.2.8/dataset_iterator/utils.py
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-01-25 15:09:54.701871 dataset_iterator-0.2.8/dataset_iterator.egg-info/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3541 2023-01-25 15:09:54.000000 dataset_iterator-0.2.8/dataset_iterator.egg-info/PKG-INFO
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      898 2023-01-25 15:09:54.000000 dataset_iterator-0.2.8/dataset_iterator.egg-info/SOURCES.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)        1 2023-01-25 15:09:54.000000 dataset_iterator-0.2.8/dataset_iterator.egg-info/dependency_links.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       59 2023-01-25 15:09:54.000000 dataset_iterator-0.2.8/dataset_iterator.egg-info/requires.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       17 2023-01-25 15:09:54.000000 dataset_iterator-0.2.8/dataset_iterator.egg-info/top_level.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       38 2023-01-25 15:09:54.701871 dataset_iterator-0.2.8/setup.cfg
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1457 2023-01-25 15:08:36.000000 dataset_iterator-0.2.8/setup.py
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-04-14 08:41:18.465908 dataset_iterator-0.2.9/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)    10141 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/LICENSE.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     3541 2023-04-14 08:41:18.465908 dataset_iterator-0.2.9/PKG-INFO
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     2412 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/README.md
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-04-14 08:41:18.461907 dataset_iterator-0.2.9/dataset_iterator/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      589 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/__init__.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     3335 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/concat_iterator.py
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-04-14 08:41:18.465908 dataset_iterator-0.2.9/dataset_iterator/datasetIO/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      320 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/datasetIO/__init__.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     2468 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/datasetIO/concatenate_datasetIO.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     1540 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/datasetIO/datasetIO.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     3011 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/datasetIO/group_datasetIO.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     2923 2022-05-30 11:41:58.000000 dataset_iterator-0.2.9/dataset_iterator/datasetIO/h5pyIO.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     1306 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/datasetIO/memoryIO.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     3632 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/datasetIO/multiple_datasetIO.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)    11943 2022-05-31 14:54:54.000000 dataset_iterator-0.2.9/dataset_iterator/datasetIO/multiple_fileIO.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     7471 2022-06-08 12:38:03.000000 dataset_iterator-0.2.9/dataset_iterator/helpers.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     1732 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/index_array_iterator.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)    53301 2023-04-14 08:32:43.000000 dataset_iterator-0.2.9/dataset_iterator/multichannel_iterator.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      808 2022-05-17 16:13:43.000000 dataset_iterator-0.2.9/dataset_iterator/preprocessing_image_generator.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)    17450 2023-01-25 15:07:22.000000 dataset_iterator-0.2.9/dataset_iterator/tile_utils.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)    16622 2023-01-17 12:17:24.000000 dataset_iterator-0.2.9/dataset_iterator/tracking_iterator.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     3984 2022-06-20 14:21:49.000000 dataset_iterator-0.2.9/dataset_iterator/utils.py
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-04-14 08:41:18.461907 dataset_iterator-0.2.9/dataset_iterator.egg-info/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     3541 2023-04-14 08:41:18.000000 dataset_iterator-0.2.9/dataset_iterator.egg-info/PKG-INFO
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      898 2023-04-14 08:41:18.000000 dataset_iterator-0.2.9/dataset_iterator.egg-info/SOURCES.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)        1 2023-04-14 08:41:18.000000 dataset_iterator-0.2.9/dataset_iterator.egg-info/dependency_links.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       59 2023-04-14 08:41:18.000000 dataset_iterator-0.2.9/dataset_iterator.egg-info/requires.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       17 2023-04-14 08:41:18.000000 dataset_iterator-0.2.9/dataset_iterator.egg-info/top_level.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       38 2023-04-14 08:41:18.465908 dataset_iterator-0.2.9/setup.cfg
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     1457 2023-04-14 08:32:55.000000 dataset_iterator-0.2.9/setup.py
```

### Comparing `dataset_iterator-0.2.8/LICENSE.txt` & `dataset_iterator-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/PKG-INFO` & `dataset_iterator-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.2.8
+Version: 0.2.9
 Summary: data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files. Based on tensorflow.keras.preprocessing.image.Iterator
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.2.8.tar.gz
+Download-URL: https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.2.9.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 License: UNKNOWN
 Keywords: Iterator,Dataset,Image,Numpy
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset_iterator-0.2.8/README.md` & `dataset_iterator-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/__init__.py` & `dataset_iterator-0.2.9/dataset_iterator/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/concat_iterator.py` & `dataset_iterator-0.2.9/dataset_iterator/concat_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/datasetIO/concatenate_datasetIO.py` & `dataset_iterator-0.2.9/dataset_iterator/datasetIO/concatenate_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/datasetIO/datasetIO.py` & `dataset_iterator-0.2.9/dataset_iterator/datasetIO/datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/datasetIO/group_datasetIO.py` & `dataset_iterator-0.2.9/dataset_iterator/datasetIO/group_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/datasetIO/h5pyIO.py` & `dataset_iterator-0.2.9/dataset_iterator/datasetIO/h5pyIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/datasetIO/memoryIO.py` & `dataset_iterator-0.2.9/dataset_iterator/datasetIO/memoryIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/datasetIO/multiple_datasetIO.py` & `dataset_iterator-0.2.9/dataset_iterator/datasetIO/multiple_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/datasetIO/multiple_fileIO.py` & `dataset_iterator-0.2.9/dataset_iterator/datasetIO/multiple_fileIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/helpers.py` & `dataset_iterator-0.2.9/dataset_iterator/helpers.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/index_array_iterator.py` & `dataset_iterator-0.2.9/dataset_iterator/index_array_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/multichannel_iterator.py` & `dataset_iterator-0.2.9/dataset_iterator/multichannel_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         size of the batch (first axis of returned tensors)
     shuffle : boolean
         if true, image indices are shuffled
     perform_data_augmentation : boolean
         if false, image_data_generators are ignored
     elasticdeform_parameters : dict
         parameters passed to elasticdeform function. see: https://github.com/gvtulder/elasticdeform/blob/master/elasticdeform/deform_grid.py
-        main parameters are: "sigma" and "points". alternatively "grid_spacing" can be passed and points will be infered (size//grid_spacing) as well as sigma (min(sigma_factor*size/points)) with sigma_factor defaults to 1./6 (increase this factor to increase deformation)
+        main parameters are: "sigma" and "points". alternatively "grid_spacing" can be passed and points will be infered (size//grid_spacing) as well as sigma (min(sigma_factor*size/points)) with sigma_factor defaults to 1/9 (increase this factor to increase deformation)
         "axis" should not be provided. default "order" is 1 and automatically set to 0 for mask channels.
         mode: out-of-bound strategy
         Applied before channels_postprocessing_function and extract_tile and after image_data_generators
     seed : int
         random seed
     dtype : numpy datatype
 
@@ -432,28 +432,29 @@
             self.channels_postprocessing_function(batch_by_channel)
 
         return batch_by_channel, aug_param_array, channels[0]
 
     def _apply_elasticdeform(self, batch_by_channel):
         if self.elasticdeform_parameters is not None:
             channels = [c for c in batch_by_channel.keys() if c>=0]
-            order = self.elasticdeform_parameters.pop("order", 1)
+            elasticdeform_parameters = self.elasticdeform_parameters.copy()
+            order = elasticdeform_parameters.pop("order", 1)
             order = ensure_multiplicity(len(channels), order)
             if len(self.mask_channels)>0:
                 for i, chan_idx in enumerate(channels):
                     if chan_idx in self.mask_channels:
                         order[i]=0
             axis = tuple([i+1 for i in range(self.n_spatial_dims)])
-            mode = self.elasticdeform_parameters.pop('mode', 'mirror')
+            mode = elasticdeform_parameters.pop('mode', 'mirror')
             image_shape = batch_by_channel[channels[0]].shape[1:-1]
-            grid_spacing = ensure_multiplicity(len(image_shape), self.elasticdeform_parameters.pop('grid_spacing', 15))
-            points = self.elasticdeform_parameters.pop('points', [max(5, 1+s//gs) for s, gs in zip(image_shape, grid_spacing)])
+            grid_spacing = ensure_multiplicity(len(image_shape), elasticdeform_parameters.pop('grid_spacing', 15))
+            points = elasticdeform_parameters.pop('points', [max(5, 1+s//gs) for s, gs in zip(image_shape, grid_spacing)])
             grid_spacing = [s/float(n-1) for s, n in zip(image_shape, points)] # actual grid spacing
-            sigma_factor = self.elasticdeform_parameters.pop('sigma_factor', 1./6)
-            sigma = self.elasticdeform_parameters.pop('sigma', np.min([sigma_factor*s/(p-1) for s, p in zip(image_shape, points)]))
+            sigma_factor = elasticdeform_parameters.pop('sigma_factor', 1./9)
+            sigma = elasticdeform_parameters.pop('sigma', np.min([sigma_factor*s/(p-1) for s, p in zip(image_shape, points)]))
             batches = [batch_by_channel[chan_idx] for chan_idx in channels]
 
             Xs = _normalize_inputs(batches)
             axis, deform_shape = _normalize_axis_list(axis, Xs)
 
             if not isinstance(points, (list, tuple)):
                 points = [points] * len(deform_shape)
@@ -461,15 +462,15 @@
             displacement = np.random.randn(len(deform_shape), *points) * sigma
             # set zero displacement at edges to avoid out-of-bounds artifacts
             displacement[:, [0,-1], :] = 0
             displacement[:, :, [0,-1]] = 0
             # limit displacement to half of grid spacing to avoid "spirals" (crossing points)
             displacement[0] = np.minimum(np.abs(displacement[0]), grid_spacing[0]/4) * np.sign(displacement[0])
             displacement[1] = np.minimum(np.abs(displacement[1]), grid_spacing[1]/4) * np.sign(displacement[1])
-            batches = ed.deform_grid(batches, displacement, order=order, mode=mode, axis=axis, **self.elasticdeform_parameters)
+            batches = ed.deform_grid(batches, displacement, order=order, mode=mode, axis=axis, **elasticdeform_parameters)
 
             for i, chan_idx in enumerate(channels):
                 batch_by_channel[chan_idx] = batches[i]
 
     def _apply_tiling(self, batch_by_channel):
         if self.extract_tile_function is not None:
             channels = [c for c in batch_by_channel.keys() if c>=0]
```

### Comparing `dataset_iterator-0.2.8/dataset_iterator/preprocessing_image_generator.py` & `dataset_iterator-0.2.9/dataset_iterator/preprocessing_image_generator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/tile_utils.py` & `dataset_iterator-0.2.9/dataset_iterator/tile_utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/tracking_iterator.py` & `dataset_iterator-0.2.9/dataset_iterator/tracking_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator/utils.py` & `dataset_iterator-0.2.9/dataset_iterator/utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/dataset_iterator.egg-info/PKG-INFO` & `dataset_iterator-0.2.9/dataset_iterator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset-iterator
-Version: 0.2.8
+Version: 0.2.9
 Summary: data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files. Based on tensorflow.keras.preprocessing.image.Iterator
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.2.8.tar.gz
+Download-URL: https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.2.9.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 License: UNKNOWN
 Keywords: Iterator,Dataset,Image,Numpy
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset_iterator-0.2.8/dataset_iterator.egg-info/SOURCES.txt` & `dataset_iterator-0.2.9/dataset_iterator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.2.8/setup.py` & `dataset_iterator-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dataset_iterator",
-    version="0.2.8",
+    version="0.2.9",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files. Based on tensorflow.keras.preprocessing.image.Iterator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/dataset_iterator.git",
-    download_url = 'https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.2.8.tar.gz',
+    download_url = 'https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.2.9.tar.gz',
     keywords = ['Iterator', 'Dataset', 'Image', 'Numpy'],
     packages=setuptools.find_packages(),
     classifiers=[ #https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

