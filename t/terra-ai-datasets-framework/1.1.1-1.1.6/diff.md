# Comparing `tmp/terra-ai-datasets-framework-1.1.1.tar.gz` & `tmp/terra_ai_datasets_framework-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Serega\Downloads\terra_ai_datasets-1.1.1\terra_ai_datasets-1.1.1\dist\.tmp-upvdkw1k\terra-ai-datasets-framework-1.1.1.", last modified: Wed Apr 12 05:57:09 2023, max compression
+gzip compressed data, was "terra_ai_datasets_framework-1.1.6.tar", last modified: Fri Apr 14 16:13:33 2023, max compression
```

## Comparing `terra-ai-datasets-framework-1.1.1.tar` & `terra_ai_datasets_framework-1.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/
--rw-rw-rw-   0        0        0      288 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-04-12 05:55:15.000000 terra-ai-datasets-framework-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/__init__.py
--rw-rw-rw-   0        0        0    19074 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/create.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/__init__.py
--rw-rw-rw-   0        0        0    14466 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/arrays.py
--rw-rw-rw-   0        0        0    24383 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/dataset.py
--rw-rw-rw-   0        0        0     4619 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/preprocessings.py
--rw-rw-rw-   0        0        0     8401 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/creation_data.py
--rw-rw-rw-   0        0        0     3800 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/dataset.py
--rw-rw-rw-   0        0        0     4490 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/inputs.py
--rw-rw-rw-   0        0        0     1336 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/outputs.py
--rw-rw-rw-   0        0        0      328 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/structure.py
--rw-rw-rw-   0        0        0      945 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/tasks.py
--rw-rw-rw-   0        0        0     5187 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/visualize.py
--rw-rw-rw-   0        0        0     3036 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/load.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra_ai_datasets_framework.egg-info/
--rw-rw-rw-   0        0        0      288 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra_ai_datasets_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1234 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra_ai_datasets_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra_ai_datasets_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      177 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra_ai_datasets_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/terra_ai_datasets_framework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 05:57:09.000000 terra-ai-datasets-framework-1.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     7049 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/tests/test_classification.py
--rw-rw-rw-   0        0        0     1371 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/tests/test_regression.py
--rw-rw-rw-   0        0        0     1574 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/tests/test_segmentation.py
--rw-rw-rw-   0        0        0     1473 2023-04-11 10:42:34.000000 terra-ai-datasets-framework-1.1.1/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24447 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/preprocessings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/creation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 16:13:33.000000 terra_ai_datasets_framework-1.1.6/terra_ai_datasets_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:33.177627 terra_ai_datasets_framework-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-14 16:13:21.000000 terra_ai_datasets_framework-1.1.6/tests/test_timeseries.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/create.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/create.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/arrays.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,16 @@
 
 class ImageArray(Array):
 
     def create(self, source: str, parameters: ImageValidator):
 
         image = Image.open(source)
         array = np.asarray(image)
+        if array.ndim == 2:
+            array = np.stack([array, array, array], axis=-1)
         array = resize_frame(image_array=array,
                              target_shape=(parameters.height, parameters.width),
                              frame_mode=parameters.process)
         if parameters.network == ImageNetworkTypes.linear:
             array = array.reshape(np.prod(np.array(array.shape)))
 
         return array
@@ -237,15 +239,15 @@
         return array
 
 
 class RawArray(Array):
 
     def create(self, source: str, parameters: RawValidator):
 
-        array = np.array([source])
+        array = np.array([[source]])
 
         return array
 
     def preprocess(self, array: np.ndarray, preprocess: Any, parameters: RawValidator):
 
         return array
 
@@ -292,14 +294,16 @@
 
 class SegmentationArray(Array):
 
     def create(self, source: str, parameters: SegmentationValidator):
 
         image = Image.open(source)
         array = np.asarray(image)
+        if array.ndim == 2:
+            array = np.stack([array, array, array], axis=-1)
         array = resize_frame(image_array=array,
                              target_shape=(parameters.height, parameters.width),
                              frame_mode=parameters.process)
         array = self.image_to_ohe(array, parameters)
 
         return array
```

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/dataset.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                         if self.preprocessing.get(col_name) and split == "train":
                             if put_data.type == LayerInputTypeChoice.Text:
                                 pass
                             elif put_data.type == LayerInputTypeChoice.Image and put_data.parameters.preprocessing == ImageScalers.terra_image_scaler:
                                 self.preprocessing[col_name].fit(sample_array)
                             else:
                                 self.preprocessing[col_name].partial_fit(sample_array.reshape(-1, 1))
-                        if not use_generator:
+                        if not use_generator or use_generator and put_data.type == LayerInputTypeChoice.Text:
                             col_array.append(
                                 sample_array[0] if type(sample_array) == np.ndarray and len(sample_array) == 1 else sample_array
                             )
 
                     if self.preprocessing.get(col_name) and split == "train":
                         if put_data.type == LayerInputTypeChoice.Text:
                             if put_data.parameters.preprocessing != TextProcessTypes.word_to_vec:
```

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/preprocessings.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/preprocessings.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/utils.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,27 +143,27 @@
         data_to_return.append(' '.join(words_list))
 
     return data_to_return
 
 
 def extract_image_data(folder_path: Path, parameters: Union[ImageValidator, SegmentationValidator]):
     image_samples = []
-    for image_path in folder_path.iterdir():
+    for image_path in sorted(folder_path.iterdir()):
         image_samples.append(image_path)
 
     return image_samples
 
 
 def extract_segmentation_data(folder_path: Path, parameters: SegmentationValidator):
     return extract_image_data(folder_path, parameters)
 
 
 def extract_text_data(folder_path: Path, parameters: TextValidator):
     text_samples = []
-    for text_path in folder_path.iterdir():
+    for text_path in sorted(folder_path.iterdir()):
         with open(text_path, 'r', encoding="utf-8") as text_file:
             text = ' '.join(text_to_word_sequence(
                 text_file.read().strip(), **{'lower': False, 'filters': parameters.filters, 'split': ' '})
             ).split()
         if parameters.mode == TextModeTypes.full:
             text_samples.append(' '.join(text[:parameters.max_words]))
         else:
@@ -173,19 +173,19 @@
                 if len(text_sample) < parameters.length:
                     break
     return text_samples
 
 
 def extract_audio_data(folder_path: Path, parameters: AudioValidator):
     audio_samples = []
-    for audio_path in folder_path.iterdir():
+    for audio_path in sorted(folder_path.iterdir()):
         if parameters.mode == TextModeTypes.full:
             audio_samples.append(';'.join([str(audio_path), f"0:{parameters.max_seconds}"]))
         else:
-            duration = librosa.get_duration(str(audio_path))
+            duration = librosa.get_duration(path=str(audio_path))
             start_idx, stop_idx = 0, parameters.length
             audio_samples.append(';'.join([str(audio_path), f"{start_idx}:{stop_idx}"]))
             while stop_idx < duration:
                 start_idx += parameters.step
                 stop_idx += parameters.step
                 audio_samples.append(';'.join([str(audio_path), f"{start_idx}:{stop_idx}"]))
     return audio_samples
```

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/creation_data.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/creation_data.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/dataset.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/dataset.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/inputs.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/inputs.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/outputs.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/outputs.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/validators/tasks.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/validators/tasks.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/creation/visualize.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/creation/visualize.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/terra-ai-datasets-framework/load.py` & `terra_ai_datasets_framework-1.1.6/terra_ai_datasets/load.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/tests/test_classification.py` & `terra_ai_datasets_framework-1.1.6/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/tests/test_regression.py` & `terra_ai_datasets_framework-1.1.6/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/tests/test_segmentation.py` & `terra_ai_datasets_framework-1.1.6/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `terra-ai-datasets-framework-1.1.1/tests/test_timeseries.py` & `terra_ai_datasets_framework-1.1.6/tests/test_timeseries.py`

 * *Files identical despite different names*

