# Comparing `tmp/mltu-1.0.5.tar.gz` & `tmp/mltu-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltu-1.0.5.tar", last modified: Wed Mar 22 14:06:50 2023, max compression
+gzip compressed data, was "mltu-1.0.6.tar", last modified: Thu Apr 13 13:57:19 2023, max compression
```

## Comparing `mltu-1.0.5.tar` & `mltu-1.0.6.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 14:06:50.533687 mltu-1.0.5/
--rw-rw-rw-   0        0        0     1083 2022-11-19 15:23:48.000000 mltu-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       24 2023-01-05 13:30:48.000000 mltu-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2544 2023-03-22 14:06:50.533687 mltu-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-03-20 11:37:25.000000 mltu-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 14:06:50.500690 mltu-1.0.5/mltu/
--rw-rw-rw-   0        0        0       61 2023-03-22 14:06:25.000000 mltu-1.0.5/mltu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 14:06:50.513687 mltu-1.0.5/mltu/annotations/
--rw-rw-rw-   0        0        0        0 2023-03-21 12:48:19.000000 mltu-1.0.5/mltu/annotations/__init__.py
--rw-rw-rw-   0        0        0     3383 2023-03-22 13:35:36.000000 mltu-1.0.5/mltu/annotations/image.py
--rw-rw-rw-   0        0        0    10566 2023-03-21 12:48:19.000000 mltu-1.0.5/mltu/augmentors.py
--rw-rw-rw-   0        0        0      898 2023-03-14 13:28:45.000000 mltu-1.0.5/mltu/configs.py
--rw-rw-rw-   0        0        0    10673 2023-03-21 12:48:19.000000 mltu-1.0.5/mltu/dataProvider.py
--rw-rw-rw-   0        0        0     2058 2023-03-20 11:37:25.000000 mltu-1.0.5/mltu/inferenceModel.py
--rw-rw-rw-   0        0        0     6272 2023-03-22 13:35:36.000000 mltu-1.0.5/mltu/preprocessors.py
-drwxrwxrwx   0        0        0        0 2023-03-22 14:06:50.519690 mltu-1.0.5/mltu/tensorflow/
--rw-rw-rw-   0        0        0     2789 2023-03-22 14:06:23.000000 mltu-1.0.5/mltu/tensorflow/callbacks.py
--rw-rw-rw-   0        0        0      231 2023-03-06 09:04:00.000000 mltu-1.0.5/mltu/tensorflow/dataProvider.py
--rw-rw-rw-   0        0        0      916 2023-03-06 09:04:00.000000 mltu-1.0.5/mltu/tensorflow/losses.py
--rw-rw-rw-   0        0        0    12669 2023-03-14 13:28:45.000000 mltu-1.0.5/mltu/tensorflow/metrics.py
--rw-rw-rw-   0        0        0     3495 2023-03-14 13:28:45.000000 mltu-1.0.5/mltu/tensorflow/model_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-22 14:06:50.528688 mltu-1.0.5/mltu/torch/
--rw-rw-rw-   0        0        0        0 2023-03-06 13:22:39.000000 mltu-1.0.5/mltu/torch/__init__.py
--rw-rw-rw-   0        0        0    14935 2023-03-20 11:37:25.000000 mltu-1.0.5/mltu/torch/callbacks.py
--rw-rw-rw-   0        0        0     3889 2023-03-20 11:37:25.000000 mltu-1.0.5/mltu/torch/dataProvider.py
--rw-rw-rw-   0        0        0     3790 2023-03-14 13:28:45.000000 mltu-1.0.5/mltu/torch/handlers.py
--rw-rw-rw-   0        0        0     1188 2023-03-20 11:37:25.000000 mltu-1.0.5/mltu/torch/losses.py
--rw-rw-rw-   0        0        0     5350 2023-03-20 11:37:25.000000 mltu-1.0.5/mltu/torch/metrics.py
--rw-rw-rw-   0        0        0     8395 2023-03-20 11:37:25.000000 mltu-1.0.5/mltu/torch/model.py
--rw-rw-rw-   0        0        0     6411 2023-03-21 12:48:19.000000 mltu-1.0.5/mltu/transformers.py
-drwxrwxrwx   0        0        0        0 2023-03-22 14:06:50.530687 mltu-1.0.5/mltu/utils/
--rw-rw-rw-   0        0        0        0 2023-03-02 11:34:41.000000 mltu-1.0.5/mltu/utils/__init__.py
--rw-rw-rw-   0        0        0     4061 2023-01-10 15:14:11.000000 mltu-1.0.5/mltu/utils/text_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-22 14:06:50.510687 mltu-1.0.5/mltu.egg-info/
--rw-rw-rw-   0        0        0     2544 2023-03-22 14:06:50.000000 mltu-1.0.5/mltu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      766 2023-03-22 14:06:50.000000 mltu-1.0.5/mltu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 14:06:50.000000 mltu-1.0.5/mltu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-03-22 14:06:50.000000 mltu-1.0.5/mltu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-22 14:06:50.000000 mltu-1.0.5/mltu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-03-20 11:37:25.000000 mltu-1.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 14:06:50.534687 mltu-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1704 2023-03-21 12:48:19.000000 mltu-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 14:06:50.532688 mltu-1.0.5/tests/
--rw-rw-rw-   0        0        0     3501 2023-01-10 15:14:11.000000 mltu-1.0.5/tests/test_text_utils.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-13 13:57:19.021740 mltu-1.0.6/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1062 2022-12-01 14:15:30.000000 mltu-1.0.6/LICENSE
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       24 2023-03-21 13:22:41.000000 mltu-1.0.6/MANIFEST.in
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-04-13 13:57:19.021740 mltu-1.0.6/PKG-INFO
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2054 2023-03-21 13:22:41.000000 mltu-1.0.6/README.md
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-13 13:57:19.017740 mltu-1.0.6/mltu/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       59 2023-04-13 13:33:57.000000 mltu-1.0.6/mltu/__init__.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-13 13:57:19.021740 mltu-1.0.6/mltu/annotations/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-22 13:58:16.000000 mltu-1.0.6/mltu/annotations/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3276 2023-03-22 13:58:36.000000 mltu-1.0.6/mltu/annotations/image.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    11735 2023-04-13 13:39:09.000000 mltu-1.0.6/mltu/augmentors.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      867 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/configs.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    10449 2023-04-13 13:26:50.000000 mltu-1.0.6/mltu/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2006 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/inferenceModel.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6112 2023-03-22 13:58:36.000000 mltu-1.0.6/mltu/preprocessors.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-13 13:57:19.021740 mltu-1.0.6/mltu/tensorflow/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2718 2023-03-22 13:58:41.000000 mltu-1.0.6/mltu/tensorflow/callbacks.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      224 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/tensorflow/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      896 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/tensorflow/losses.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    12415 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/tensorflow/metrics.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3402 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/tensorflow/model_utils.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-13 13:57:19.021740 mltu-1.0.6/mltu/torch/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/torch/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    14543 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/torch/callbacks.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3810 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/torch/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3691 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/torch/handlers.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1154 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/torch/losses.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     5184 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/torch/metrics.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     8139 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/torch/model.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6224 2023-03-22 13:58:16.000000 mltu-1.0.6/mltu/transformers.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-13 13:57:19.021740 mltu-1.0.6/mltu/utils/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/utils/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3938 2023-03-21 13:22:41.000000 mltu-1.0.6/mltu/utils/text_utils.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-13 13:57:19.021740 mltu-1.0.6/mltu.egg-info/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-04-13 13:57:19.000000 mltu-1.0.6/mltu.egg-info/PKG-INFO
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      741 2023-04-13 13:57:19.000000 mltu-1.0.6/mltu.egg-info/SOURCES.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        1 2023-04-13 13:57:19.000000 mltu-1.0.6/mltu.egg-info/dependency_links.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      118 2023-04-13 13:57:19.000000 mltu-1.0.6/mltu.egg-info/requires.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        5 2023-04-13 13:57:19.000000 mltu-1.0.6/mltu.egg-info/top_level.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      128 2023-03-21 13:22:41.000000 mltu-1.0.6/requirements.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       38 2023-04-13 13:57:19.021740 mltu-1.0.6/setup.cfg
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1654 2023-03-22 13:58:16.000000 mltu-1.0.6/setup.py
```

### Comparing `mltu-1.0.5/PKG-INFO` & `mltu-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1
-Name: mltu
-Version: 1.0.5
-Summary: Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch
-Home-page: https://pylessons.com/
-Author: PyLessons
-Author-email: pythonlessons0@gmail.com
-Project-URL: Source, https://github.com/pythonlessons/mltu/
-Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-License-File: LICENSE
-
-# MLTU - Machine Learning Training Utilities
-Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
-<p align="center">
-  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
-</p>
-
-# Installation:
-To use MLTU in your own project, you can install it from PyPI:
-```bash
-pip install mltu
-```
-When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
-```bash
-pip install mltu==0.1.3
-```
-Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
-
-# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
-1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
-2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
-3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
-4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
-5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
-6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
-7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
-8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
+Metadata-Version: 2.1
+Name: mltu
+Version: 1.0.6
+Summary: Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch
+Home-page: https://pylessons.com/
+Author: PyLessons
+Author-email: pythonlessons0@gmail.com
+Project-URL: Source, https://github.com/pythonlessons/mltu/
+Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+Provides-Extra: gpu
+License-File: LICENSE
+
+# MLTU - Machine Learning Training Utilities
+Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
+<p align="center">
+  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
+</p>
+
+# Installation:
+To use MLTU in your own project, you can install it from PyPI:
+```bash
+pip install mltu
+```
+When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
+```bash
+pip install mltu==0.1.3
+```
+Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
+
+# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
+1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
+2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
+3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
+4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
+5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
+6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
+7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
+8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
```

### Comparing `mltu-1.0.5/README.md` & `mltu-1.0.6/mltu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,40 @@
-# MLTU - Machine Learning Training Utilities
-Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
-<p align="center">
-  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
-</p>
-
-# Installation:
-To use MLTU in your own project, you can install it from PyPI:
-```bash
-pip install mltu
-```
-When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
-```bash
-pip install mltu==0.1.3
-```
-Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
-
-# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
-1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
-2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
-3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
-4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
-5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
-6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
-7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
-8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
+Metadata-Version: 2.1
+Name: mltu
+Version: 1.0.6
+Summary: Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch
+Home-page: https://pylessons.com/
+Author: PyLessons
+Author-email: pythonlessons0@gmail.com
+Project-URL: Source, https://github.com/pythonlessons/mltu/
+Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+Provides-Extra: gpu
+License-File: LICENSE
+
+# MLTU - Machine Learning Training Utilities
+Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
+<p align="center">
+  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
+</p>
+
+# Installation:
+To use MLTU in your own project, you can install it from PyPI:
+```bash
+pip install mltu
+```
+When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
+```bash
+pip install mltu==0.1.3
+```
+Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
+
+# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
+1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
+2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
+3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
+4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
+5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
+6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
+7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
+8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
```

### Comparing `mltu-1.0.5/mltu/augmentors.py` & `mltu-1.0.6/mltu/augmentors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,281 +1,322 @@
-import cv2
-import typing
-import numpy as np
-import logging
-
-from . import Image
-
-""" Implemented augmentors:
-- RandomBrightness
-- RandomRotate
-- RandomErodeDilate
-- RandomSharpen
-"""
-
-def randomness_decorator(func):
-    """ Decorator for randomness """
-    def wrapper(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Decorator for randomness and type checking
-
-        Args:
-            image (Image): Image to be adjusted
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            image (Image): Adjusted image
-            annotation (typing.Any): Adjusted annotation
-        """
-        # check if image is Image object
-        if not isinstance(image, Image):
-            self.logger.error(f"image must be Image object, not {type(image)}, skipping augmentor")
-            return image, annotation
-
-        if np.random.rand() > self._random_chance:
-            return image, annotation
-
-        # return result of function
-        return func(self, image, annotation)
-
-    return wrapper
-
-
-class Augmentor:
-    """ Object that should be inherited by all augmentors
-
-    Args:
-        random_chance (float, optional): Chance of applying the augmentor. Where 0.0 is never and 1.0 is always. Defaults to 0.5.
-        log_level (int, optional): Log level for the augmentor. Defaults to logging.INFO.
-    """
-    def __init__(self, random_chance: float=0.5, log_level: int = logging.INFO) -> None:
-        self._random_chance = random_chance
-        self._log_level = log_level
-
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(logging.INFO)
-
-        assert 0 <= self._random_chance <= 1.0, "random chance must be between 0.0 and 1.0"
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        # do the augmentation here
-        return image, annotation
-
-
-class RandomBrightness(Augmentor):
-    """ Randomly adjust image brightness """
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        delta: int = 100,
-        log_level: int = logging.INFO,
-        ) -> None:
-        """ Randomly adjust image brightness
-
-        Args:
-            random_chance (float, optional): Chance of applying the augmentor. Where 0.0 is never and 1.0 is always. Defaults to 0.5.
-            delta (int, optional): Integer value for brightness adjustment. Defaults to 100.
-            log_level (int, optional): Log level for the augmentor. Defaults to logging.INFO.
-        """
-        super(RandomBrightness, self).__init__(random_chance, log_level)
-
-        assert 0 <= delta <= 255.0, "Delta must be between 0.0 and 255.0"
-
-        self._delta = delta
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly adjust image brightness
-
-        Args:
-            image (Image): Image to be adjusted
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            image (Image): Adjusted image
-            annotation (typing.Any): Adjusted annotation
-        """
-        value = 1 + np.random.uniform(-self._delta, self._delta) / 255
-
-        hsv = np.array(image.HSV(), dtype = np.float32)
-
-        hsv[:, :, 1] = hsv[:, :, 1] * value
-        hsv[:, :, 2] = hsv[:, :, 2] * value
-
-        hsv = np.uint8(np.clip(hsv, 0, 255))
-
-        img = cv2.cvtColor(hsv, cv2.COLOR_HSV2BGR)
-
-        image.update(img)
-
-        return image, annotation
-
-
-class RandomRotate(Augmentor):
-    """ Randomly rotate image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        angle: typing.Union[int, typing.List]=30, 
-        borderValue: typing.Tuple[int, int, int]=None,
-        log_level: int = logging.INFO,
-        ) -> None:
-        """ Randomly rotate image 
-
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            angle (int, list): Integer value or list of integer values for image rotation
-            borderValue (tuple): Tuple of 3 integers, setting border color for image rotation
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-        """
-        super(RandomRotate, self).__init__(random_chance, log_level)
-
-        self._angle = angle
-        self._borderValue = borderValue
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly rotate image
-
-        Args:
-            image (Image): Image to be adjusted
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            image (Image): Adjusted image
-            annotation (typing.Any): Adjusted annotation
-        """
-        # check if angle is list of angles or signle angle value
-        if isinstance(self._angle, list):
-            angle = float(np.random.choice(self._angle))
-        else:
-            angle = float(np.random.uniform(-self._angle, self._angle))
-
-        # generate random border color
-        borderValue = np.random.randint(0, 255, 3) if self._borderValue is None else self._borderValue
-        borderValue = [int(v) for v in borderValue]
-
-        # grab the dimensions of the image and then determine the centre
-        center_x, center_y = image.center
-
-        # grab the rotation matrix (applying the negative of the
-        # angle to rotate clockwise), then grab the sine and cosine
-        # (i.e., the rotation components of the matrix)
-        M = cv2.getRotationMatrix2D((center_x, center_y), angle, 1.0)
-        cos = np.abs(M[0, 0])
-        sin = np.abs(M[0, 1])
-
-        # compute the new bounding dimensions of the image
-        nW = int((image.height * sin) + (image.width * cos))
-        nH = int((image.height * cos) + (image.width * sin))
-
-        # adjust the rotation matrix to take into account translation
-        M[0, 2] += (nW / 2) - center_x
-        M[1, 2] += (nH / 2) - center_y
-
-        # perform the actual rotation and return the image
-        img = cv2.warpAffine(image.numpy(), M, (nW, nH), borderValue=borderValue)
-        image.update(img)
-
-        return image, annotation
-
-
-class RandomErodeDilate(Augmentor):
-    """ Randomly erode and dilate image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        kernel_size: typing.Tuple[int, int]=(1, 1), 
-        log_level: int = logging.INFO,
-        ) -> None:
-        """ Randomly erode and dilate image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            kernel_size (tuple): Tuple of 2 integers, setting kernel size for erosion and dilation
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-        """
-        super(RandomErodeDilate, self).__init__(random_chance, log_level)
-        self._kernel_size = kernel_size
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly erode and dilate image
-
-        Args:
-            image (np.ndarray): Image to be eroded and dilated
-
-        Returns:
-            image (np.ndarray): Eroded and dilated image
-        """
-        kernel = np.ones(self._kernel_size, np.uint8)
-
-        if np.random.rand() <= 0.5:
-            img = cv2.erode(image.numpy(), kernel, iterations=1)
-        else:
-            img = cv2.dilate(image.numpy(), kernel, iterations=1)
-
-        image.update(img)
-
-        return image, annotation
-
-class RandomSharpen(Augmentor):
-    """ Randomly sharpen image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        alpha: float = 0.25,
-        lightness_range: typing.Tuple = (0.75, 2.0),
-        kernel: np.ndarray = None,
-        kernel_anchor: np.ndarray = None,
-        log_level: int = logging.INFO,
-        ) -> None:
-        """ Randomly sharpen image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            alpha (float): Float between 0.0 and 1.0 setting bounds for random probability
-            lightness_range (tuple): Tuple of 2 floats, setting bounds for random lightness change
-            kernel (np.ndarray): Numpy array of kernel for image convolution
-            kernel_anchor (np.ndarray): Numpy array of kernel anchor for image convolution
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-        """
-        super(RandomSharpen, self).__init__(random_chance, log_level)
-
-        self._alpha_range = (alpha, 1.0)
-        self._ligtness_range = lightness_range
-        self._lightness_anchor = 8
-
-        self._kernel = np.array([[-1, -1, -1], [-1,  1, -1], [-1, -1, -1]], dtype=np.float32) if kernel is None else kernel
-        self._kernel_anchor = np.array([[0, 0, 0], [0, 1, 0], [0, 0, 0]], dtype=np.float32) if kernel_anchor is None else kernel_anchor
-
-        assert 0 <= alpha <= 1.0, "Alpha must be between 0.0 and 1.0"
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly sharpen image
-
-        Args:
-            image (np.ndarray): Image to be sharpened
-            annotation (typing.Any): Annotation to be sharpened
-
-        Returns:
-            image (np.ndarray): Sharpened image
-            annotation (typing.Any): Sharpened annotation
-        """
-        lightness = np.random.uniform(*self._ligtness_range)
-        alpha = np.random.uniform(*self._alpha_range)
-
-        kernel = self._kernel_anchor  * (self._lightness_anchor + lightness) + self._kernel
-        kernel -= self._kernel_anchor
-        kernel = (1 - alpha) * self._kernel_anchor + alpha * kernel
-
-        # Apply sharpening to each channel
-        r, g, b = cv2.split(image.numpy())
-        r_sharp = cv2.filter2D(r, -1, kernel)
-        g_sharp = cv2.filter2D(g, -1, kernel)
-        b_sharp = cv2.filter2D(b, -1, kernel)
-
-        # Merge the sharpened channels back into the original image
-        image.update(cv2.merge([r_sharp, g_sharp, b_sharp]))
-
+import cv2
+import typing
+import numpy as np
+import logging
+
+from . import Image
+
+""" Implemented augmentors:
+- RandomBrightness
+- RandomRotate
+- RandomErodeDilate
+- RandomSharpen
+- RandomGaussianBlur
+"""
+
+def randomness_decorator(func):
+    """ Decorator for randomness """
+    def wrapper(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Decorator for randomness and type checking
+
+        Args:
+            image (Image): Image to be adjusted
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Adjusted image
+            annotation (typing.Any): Adjusted annotation
+        """
+        # check if image is Image object
+        if not isinstance(image, Image):
+            self.logger.error(f"image must be Image object, not {type(image)}, skipping augmentor")
+            return image, annotation
+
+        if np.random.rand() > self._random_chance:
+            return image, annotation
+
+        # return result of function
+        return func(self, image, annotation)
+
+    return wrapper
+
+
+class Augmentor:
+    """ Object that should be inherited by all augmentors
+
+    Args:
+        random_chance (float, optional): Chance of applying the augmentor. Where 0.0 is never and 1.0 is always. Defaults to 0.5.
+        log_level (int, optional): Log level for the augmentor. Defaults to logging.INFO.
+    """
+    def __init__(self, random_chance: float=0.5, log_level: int = logging.INFO) -> None:
+        self._random_chance = random_chance
+        self._log_level = log_level
+
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(logging.INFO)
+
+        assert 0 <= self._random_chance <= 1.0, "random chance must be between 0.0 and 1.0"
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        # do the augmentation here
+        return image, annotation
+
+
+class RandomBrightness(Augmentor):
+    """ Randomly adjust image brightness """
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        delta: int = 100,
+        log_level: int = logging.INFO,
+        ) -> None:
+        """ Randomly adjust image brightness
+
+        Args:
+            random_chance (float, optional): Chance of applying the augmentor. Where 0.0 is never and 1.0 is always. Defaults to 0.5.
+            delta (int, optional): Integer value for brightness adjustment. Defaults to 100.
+            log_level (int, optional): Log level for the augmentor. Defaults to logging.INFO.
+        """
+        super(RandomBrightness, self).__init__(random_chance, log_level)
+
+        assert 0 <= delta <= 255.0, "Delta must be between 0.0 and 255.0"
+
+        self._delta = delta
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly adjust image brightness
+
+        Args:
+            image (Image): Image to be adjusted
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Adjusted image
+            annotation (typing.Any): Adjusted annotation if necessary
+        """
+        value = 1 + np.random.uniform(-self._delta, self._delta) / 255
+
+        hsv = np.array(image.HSV(), dtype = np.float32)
+
+        hsv[:, :, 1] = hsv[:, :, 1] * value
+        hsv[:, :, 2] = hsv[:, :, 2] * value
+
+        hsv = np.uint8(np.clip(hsv, 0, 255))
+
+        img = cv2.cvtColor(hsv, cv2.COLOR_HSV2BGR)
+
+        image.update(img)
+
+        return image, annotation
+
+
+class RandomRotate(Augmentor):
+    """ Randomly rotate image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        angle: typing.Union[int, typing.List]=30, 
+        borderValue: typing.Tuple[int, int, int]=None,
+        log_level: int = logging.INFO,
+        ) -> None:
+        """ Randomly rotate image 
+
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            angle (int, list): Integer value or list of integer values for image rotation
+            borderValue (tuple): Tuple of 3 integers, setting border color for image rotation
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+        """
+        super(RandomRotate, self).__init__(random_chance, log_level)
+
+        self._angle = angle
+        self._borderValue = borderValue
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly rotate image
+
+        Args:
+            image (Image): Image to be adjusted
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Adjusted image
+            annotation (typing.Any): Adjusted annotation
+        """
+        # check if angle is list of angles or signle angle value
+        if isinstance(self._angle, list):
+            angle = float(np.random.choice(self._angle))
+        else:
+            angle = float(np.random.uniform(-self._angle, self._angle))
+
+        # generate random border color
+        borderValue = np.random.randint(0, 255, 3) if self._borderValue is None else self._borderValue
+        borderValue = [int(v) for v in borderValue]
+
+        # grab the dimensions of the image and then determine the centre
+        center_x, center_y = image.center
+
+        # grab the rotation matrix (applying the negative of the
+        # angle to rotate clockwise), then grab the sine and cosine
+        # (i.e., the rotation components of the matrix)
+        M = cv2.getRotationMatrix2D((center_x, center_y), angle, 1.0)
+        cos = np.abs(M[0, 0])
+        sin = np.abs(M[0, 1])
+
+        # compute the new bounding dimensions of the image
+        nW = int((image.height * sin) + (image.width * cos))
+        nH = int((image.height * cos) + (image.width * sin))
+
+        # adjust the rotation matrix to take into account translation
+        M[0, 2] += (nW / 2) - center_x
+        M[1, 2] += (nH / 2) - center_y
+
+        # perform the actual rotation and return the image
+        img = cv2.warpAffine(image.numpy(), M, (nW, nH), borderValue=borderValue)
+        image.update(img)
+
+        return image, annotation
+
+
+class RandomErodeDilate(Augmentor):
+    """ Randomly erode and dilate image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        kernel_size: typing.Tuple[int, int]=(1, 1), 
+        log_level: int = logging.INFO,
+        ) -> None:
+        """ Randomly erode and dilate image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            kernel_size (tuple): Tuple of 2 integers, setting kernel size for erosion and dilation
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+        """
+        super(RandomErodeDilate, self).__init__(random_chance, log_level)
+        self._kernel_size = kernel_size
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly erode and dilate image
+
+        Args:
+            image (Image): Image to be eroded and dilated
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Eroded and dilated image
+            annotation (typing.Any): Adjusted annotation if necessary
+        """
+        kernel = np.ones(self._kernel_size, np.uint8)
+
+        if np.random.rand() <= 0.5:
+            img = cv2.erode(image.numpy(), kernel, iterations=1)
+        else:
+            img = cv2.dilate(image.numpy(), kernel, iterations=1)
+
+        image.update(img)
+
+        return image, annotation
+
+
+class RandomSharpen(Augmentor):
+    """ Randomly sharpen image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        alpha: float = 0.25,
+        lightness_range: typing.Tuple = (0.75, 2.0),
+        kernel: np.ndarray = None,
+        kernel_anchor: np.ndarray = None,
+        log_level: int = logging.INFO,
+        ) -> None:
+        """ Randomly sharpen image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            alpha (float): Float between 0.0 and 1.0 setting bounds for random probability
+            lightness_range (tuple): Tuple of 2 floats, setting bounds for random lightness change
+            kernel (np.ndarray): Numpy array of kernel for image convolution
+            kernel_anchor (np.ndarray): Numpy array of kernel anchor for image convolution
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+        """
+        super(RandomSharpen, self).__init__(random_chance, log_level)
+
+        self._alpha_range = (alpha, 1.0)
+        self._ligtness_range = lightness_range
+        self._lightness_anchor = 8
+
+        self._kernel = np.array([[-1, -1, -1], [-1,  1, -1], [-1, -1, -1]], dtype=np.float32) if kernel is None else kernel
+        self._kernel_anchor = np.array([[0, 0, 0], [0, 1, 0], [0, 0, 0]], dtype=np.float32) if kernel_anchor is None else kernel_anchor
+
+        assert 0 <= alpha <= 1.0, "Alpha must be between 0.0 and 1.0"
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly sharpen image
+
+        Args:
+            image (Image): Image to be sharpened
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Sharpened image
+            annotation (typing.Any): Adjusted annotation if necessary
+        """
+        lightness = np.random.uniform(*self._ligtness_range)
+        alpha = np.random.uniform(*self._alpha_range)
+
+        kernel = self._kernel_anchor  * (self._lightness_anchor + lightness) + self._kernel
+        kernel -= self._kernel_anchor
+        kernel = (1 - alpha) * self._kernel_anchor + alpha * kernel
+
+        # Apply sharpening to each channel
+        r, g, b = cv2.split(image.numpy())
+        r_sharp = cv2.filter2D(r, -1, kernel)
+        g_sharp = cv2.filter2D(g, -1, kernel)
+        b_sharp = cv2.filter2D(b, -1, kernel)
+
+        # Merge the sharpened channels back into the original image
+        image.update(cv2.merge([r_sharp, g_sharp, b_sharp]))
+
+        return image, annotation
+    
+
+class RandomGaussianBlur(Augmentor):
+    """ Randomly erode and dilate image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        sigma: typing.Union[int, float] = 0.5,
+        ) -> None:
+        """ Randomly erode and dilate image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            sigma (int, float): standard deviation of the Gaussian kernel
+        """
+        super(RandomGaussianBlur, self).__init__(random_chance, log_level)
+        self.sigma = sigma
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly blurs an image with a Gaussian filter
+
+        Args:
+            image (Image): Image to be blurred
+            annotation (typing.Any): Annotation to be blurred
+
+        Returns:
+            image (Image): Blurred image
+            annotation (typing.Any): Blurred annotation if necessary
+        """
+        img = cv2.GaussianBlur(image.numpy(), (0, 0), self.sigma)
+
+        image.update(img)
+
         return image, annotation
```

### Comparing `mltu-1.0.5/mltu/preprocessors.py` & `mltu-1.0.6/mltu/preprocessors.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-import os
-import cv2
-import typing
-import librosa
-import librosa.display
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib
-matplotlib.interactive(False)
-
-import logging
-logging.basicConfig(format='%(asctime)s %(levelname)s %(name)s: %(message)s')
-
-from . import Image
-
-class ImageReader:
-    """Read image with cv2 from path and return image and label"""
-    def __init__(self, method: int = cv2.IMREAD_COLOR, log_level: int = logging.INFO) -> None:
-        self._method = method
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(log_level)
-
-    def __call__(self, image_path: typing.Union[str, np.ndarray], label: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Read image with cv2 from path and return image and label
-        
-        Args:
-            image_path (typing.Union[str, np.ndarray]): Path to image or numpy array
-            label (Any): Label of image
-
-        Returns:
-            Image: Image object
-            Any: Label of image
-        """
-        if isinstance(image_path, str):
-            # check whether image_path exists
-            if not os.path.exists(image_path):
-                raise FileNotFoundError(f"Image {image_path} not found.")
-        elif isinstance(image_path, np.ndarray):
-            pass
-        else:
-            raise TypeError(f"Image {image_path} is not a string or numpy array.")
-
-        image = Image(image = image_path, method = self._method)
-        if image.image is None:
-            image = None
-            self.logger.warning(f"Image {image_path} could not be read, returning None.")
-
-        return image, label
-
-class WavReader:
-    """Read wav file with librosa and return audio and label
-    
-    Attributes:
-        frame_length (int): Length of the frames in samples.
-        frame_step (int): Step size between frames in samples.
-        fft_length (int): Number of FFT components.
-    """
-    def __init__(
-        self, 
-        frame_length: int=256, 
-        frame_step: int=160,
-        fft_length: int=384,
-        *args, **kwargs
-        ) -> None:
-        self.frame_length = frame_length
-        self.frame_step = frame_step
-        self.fft_length = fft_length
-
-    @staticmethod
-    def get_spectrogram(wav_path: str, frame_length: int, frame_step: int, fft_length: int) -> np.ndarray:
-        """Compute the spectrogram of a WAV file
-
-        Args:
-            wav_path (str): Path to the WAV file.
-            frame_length (int): Length of the frames in samples.
-            frame_step (int): Step size between frames in samples.
-            fft_length (int): Number of FFT components.
-
-        Returns:
-            np.ndarray: Spectrogram of the WAV file.
-        """
-        # Load the wav file and store the audio data in the variable 'audio' and the sample rate in 'orig_sr'
-        audio, orig_sr = librosa.load(wav_path) 
-
-        # Compute the Short Time Fourier Transform (STFT) of the audio data and store it in the variable 'spectrogram'
-        # The STFT is computed with a hop length of 'frame_step' samples, a window length of 'frame_length' samples, and 'fft_length' FFT components.
-        # The resulting spectrogram is also transposed for convenience
-        spectrogram = librosa.stft(audio, hop_length=frame_step, win_length=frame_length, n_fft=fft_length).T
-
-        # Take the absolute value of the spectrogram to obtain the magnitude spectrum
-        spectrogram = np.abs(spectrogram)
-
-        # Take the square root of the magnitude spectrum to obtain the log spectrogram
-        spectrogram = np.power(spectrogram, 0.5)
-
-        # Normalize the spectrogram by subtracting the mean and dividing by the standard deviation.
-        # A small value of 1e-10 is added to the denominator to prevent division by zero.
-        spectrogram = (spectrogram - np.mean(spectrogram)) / (np.std(spectrogram) + 1e-10)
-
-        return spectrogram
-
-    @staticmethod
-    def plot_raw_audio(wav_path: str, title:str = None, sr: int = 16000) -> None:
-        """Plot the raw audio of a WAV file
-
-        Args:
-            wav_path (str): Path to the WAV file.
-            sr (int, optional): Sample rate of the WAV file. Defaults to 16000.
-        """
-        # Load the wav file and store the audio data in the variable 'audio' and the sample rate in 'orig_sr'
-        audio, orig_sr = librosa.load(wav_path, sr=sr)
-
-        duration = len(audio) / orig_sr
-
-        time = np.linspace(0, duration, num=len(audio))
-
-        plt.figure(figsize=(15, 5))
-        plt.plot(time, audio)
-        plt.title(title) if title else plt.title('Audio Plot')
-        plt.ylabel('signal wave')
-        plt.xlabel('time (s)')
-        plt.tight_layout()
-        plt.show()
-
-    @staticmethod
-    def plot_spectrogram(spectrogram: np.ndarray, title:str = "", transpose: bool = True, invert: bool = True) -> None:
-        """Plot the spectrogram of a WAV file
-
-        Args:
-            spectrogram (np.ndarray): Spectrogram of the WAV file.
-            title (str, optional): Title of the plot. Defaults to None.
-            transpose (bool, optional): Transpose the spectrogram. Defaults to True.
-            invert (bool, optional): Invert the spectrogram. Defaults to True.
-        """
-        if transpose:
-            spectrogram = spectrogram.T
-        
-        if invert:
-            spectrogram = spectrogram[::-1]
-
-        plt.figure(figsize=(15, 5))
-        plt.imshow(spectrogram, aspect='auto', origin='lower')
-        plt.title(f'Spectrogram: {title}')
-        plt.xlabel('Time')
-        plt.ylabel('Frequency')
-        plt.colorbar()
-        plt.tight_layout()
-        plt.show()
-
-    def __call__(self, audio_path: str, label: typing.Any):
-        """
-        Extract the spectrogram and label of a WAV file.
-
-        Args:
-            audio_path (str): Path to the WAV file.
-            label (typing.Any): Label of the WAV file.
-
-        Returns:
-            Tuple[np.ndarray, typing.Any]: Spectrogram of the WAV file and its label.
-        """
+import os
+import cv2
+import typing
+import librosa
+import librosa.display
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotlib
+matplotlib.interactive(False)
+
+import logging
+logging.basicConfig(format='%(asctime)s %(levelname)s %(name)s: %(message)s')
+
+from . import Image
+
+class ImageReader:
+    """Read image with cv2 from path and return image and label"""
+    def __init__(self, method: int = cv2.IMREAD_COLOR, log_level: int = logging.INFO) -> None:
+        self._method = method
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(log_level)
+
+    def __call__(self, image_path: typing.Union[str, np.ndarray], label: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Read image with cv2 from path and return image and label
+        
+        Args:
+            image_path (typing.Union[str, np.ndarray]): Path to image or numpy array
+            label (Any): Label of image
+
+        Returns:
+            Image: Image object
+            Any: Label of image
+        """
+        if isinstance(image_path, str):
+            # check whether image_path exists
+            if not os.path.exists(image_path):
+                raise FileNotFoundError(f"Image {image_path} not found.")
+        elif isinstance(image_path, np.ndarray):
+            pass
+        else:
+            raise TypeError(f"Image {image_path} is not a string or numpy array.")
+
+        image = Image(image = image_path, method = self._method)
+        if image.image is None:
+            image = None
+            self.logger.warning(f"Image {image_path} could not be read, returning None.")
+
+        return image, label
+
+class WavReader:
+    """Read wav file with librosa and return audio and label
+    
+    Attributes:
+        frame_length (int): Length of the frames in samples.
+        frame_step (int): Step size between frames in samples.
+        fft_length (int): Number of FFT components.
+    """
+    def __init__(
+        self, 
+        frame_length: int=256, 
+        frame_step: int=160,
+        fft_length: int=384,
+        *args, **kwargs
+        ) -> None:
+        self.frame_length = frame_length
+        self.frame_step = frame_step
+        self.fft_length = fft_length
+
+    @staticmethod
+    def get_spectrogram(wav_path: str, frame_length: int, frame_step: int, fft_length: int) -> np.ndarray:
+        """Compute the spectrogram of a WAV file
+
+        Args:
+            wav_path (str): Path to the WAV file.
+            frame_length (int): Length of the frames in samples.
+            frame_step (int): Step size between frames in samples.
+            fft_length (int): Number of FFT components.
+
+        Returns:
+            np.ndarray: Spectrogram of the WAV file.
+        """
+        # Load the wav file and store the audio data in the variable 'audio' and the sample rate in 'orig_sr'
+        audio, orig_sr = librosa.load(wav_path) 
+
+        # Compute the Short Time Fourier Transform (STFT) of the audio data and store it in the variable 'spectrogram'
+        # The STFT is computed with a hop length of 'frame_step' samples, a window length of 'frame_length' samples, and 'fft_length' FFT components.
+        # The resulting spectrogram is also transposed for convenience
+        spectrogram = librosa.stft(audio, hop_length=frame_step, win_length=frame_length, n_fft=fft_length).T
+
+        # Take the absolute value of the spectrogram to obtain the magnitude spectrum
+        spectrogram = np.abs(spectrogram)
+
+        # Take the square root of the magnitude spectrum to obtain the log spectrogram
+        spectrogram = np.power(spectrogram, 0.5)
+
+        # Normalize the spectrogram by subtracting the mean and dividing by the standard deviation.
+        # A small value of 1e-10 is added to the denominator to prevent division by zero.
+        spectrogram = (spectrogram - np.mean(spectrogram)) / (np.std(spectrogram) + 1e-10)
+
+        return spectrogram
+
+    @staticmethod
+    def plot_raw_audio(wav_path: str, title:str = None, sr: int = 16000) -> None:
+        """Plot the raw audio of a WAV file
+
+        Args:
+            wav_path (str): Path to the WAV file.
+            sr (int, optional): Sample rate of the WAV file. Defaults to 16000.
+        """
+        # Load the wav file and store the audio data in the variable 'audio' and the sample rate in 'orig_sr'
+        audio, orig_sr = librosa.load(wav_path, sr=sr)
+
+        duration = len(audio) / orig_sr
+
+        time = np.linspace(0, duration, num=len(audio))
+
+        plt.figure(figsize=(15, 5))
+        plt.plot(time, audio)
+        plt.title(title) if title else plt.title('Audio Plot')
+        plt.ylabel('signal wave')
+        plt.xlabel('time (s)')
+        plt.tight_layout()
+        plt.show()
+
+    @staticmethod
+    def plot_spectrogram(spectrogram: np.ndarray, title:str = "", transpose: bool = True, invert: bool = True) -> None:
+        """Plot the spectrogram of a WAV file
+
+        Args:
+            spectrogram (np.ndarray): Spectrogram of the WAV file.
+            title (str, optional): Title of the plot. Defaults to None.
+            transpose (bool, optional): Transpose the spectrogram. Defaults to True.
+            invert (bool, optional): Invert the spectrogram. Defaults to True.
+        """
+        if transpose:
+            spectrogram = spectrogram.T
+        
+        if invert:
+            spectrogram = spectrogram[::-1]
+
+        plt.figure(figsize=(15, 5))
+        plt.imshow(spectrogram, aspect='auto', origin='lower')
+        plt.title(f'Spectrogram: {title}')
+        plt.xlabel('Time')
+        plt.ylabel('Frequency')
+        plt.colorbar()
+        plt.tight_layout()
+        plt.show()
+
+    def __call__(self, audio_path: str, label: typing.Any):
+        """
+        Extract the spectrogram and label of a WAV file.
+
+        Args:
+            audio_path (str): Path to the WAV file.
+            label (typing.Any): Label of the WAV file.
+
+        Returns:
+            Tuple[np.ndarray, typing.Any]: Spectrogram of the WAV file and its label.
+        """
         return self.get_spectrogram(audio_path, self.frame_length, self.frame_step, self.fft_length), label
```

### Comparing `mltu-1.0.5/mltu/tensorflow/callbacks.py` & `mltu-1.0.6/mltu/tensorflow/callbacks.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import os
-import tf2onnx
-import onnx
-from keras.callbacks import Callback
-
-import logging
-
-class Model2onnx(Callback):
-    """ Converts the model to onnx format after training is finished. """
-    def __init__(
-        self, 
-        saved_model_path: str, 
-        metadata: dict=None
-        ) -> None:
-        """ Converts the model to onnx format after training is finished.
-        Args:
-            saved_model_path (str): Path to the saved .h5 model.
-            metadata (dict, optional): Dictionary containing metadata to be added to the onnx model. Defaults to None.
-        """
-        super().__init__()
-        self.saved_model_path = saved_model_path
-        self.metadata = metadata
-
-    def on_train_end(self, logs=None):
-        self.model.load_weights(self.saved_model_path)
-        self.onnx_model_path = self.saved_model_path.replace(".h5", ".onnx")
-        tf2onnx.convert.from_keras(self.model, output_path=self.onnx_model_path)
-
-        if self.metadata and isinstance(self.metadata, dict):
-            # Load the ONNX model
-            onnx_model = onnx.load(self.onnx_model_path)
-
-            # Add the metadata dictionary to the model's metadata_props attribute
-            for key, value in self.metadata.items():
-                meta = onnx_model.metadata_props.add()
-                meta.key = key
-                meta.value = value
-
-            # Save the modified ONNX model
-            onnx.save(onnx_model, self.onnx_model_path)
-
-class TrainLogger(Callback):
-    """Logs training metrics to a file.
-    
-    Args:
-        log_path (str): Path to the directory where the log file will be saved.
-        log_file (str, optional): Name of the log file. Defaults to 'logs.log'.
-        logLevel (int, optional): Logging level. Defaults to logging.INFO.
-    """
-    def __init__(self, log_path: str, log_file: str='logs.log', logLevel=logging.INFO) -> None:
-        super().__init__()
-        self.log_path = log_path
-        self.log_file = log_file
-
-        if not os.path.exists(log_path):
-            os.mkdir(log_path)
-
-        self.logger = logging.getLogger()
-        self.logger.setLevel(logLevel)
-
-        self.formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-
-        self.file_handler = logging.FileHandler(os.path.join(self.log_path, self.log_file))
-        self.file_handler.setLevel(logLevel)
-        self.file_handler.setFormatter(self.formatter)
-
-        self.logger.addHandler(self.file_handler)
-
-    def on_epoch_end(self, epoch: int, logs: dict=None):
-        epoch_message = f"Epoch {epoch}; "
-        logs_message = "; ".join([f"{key}: {value}" for key, value in logs.items()])
+import os
+import tf2onnx
+import onnx
+from keras.callbacks import Callback
+
+import logging
+
+class Model2onnx(Callback):
+    """ Converts the model to onnx format after training is finished. """
+    def __init__(
+        self, 
+        saved_model_path: str, 
+        metadata: dict=None
+        ) -> None:
+        """ Converts the model to onnx format after training is finished.
+        Args:
+            saved_model_path (str): Path to the saved .h5 model.
+            metadata (dict, optional): Dictionary containing metadata to be added to the onnx model. Defaults to None.
+        """
+        super().__init__()
+        self.saved_model_path = saved_model_path
+        self.metadata = metadata
+
+    def on_train_end(self, logs=None):
+        self.model.load_weights(self.saved_model_path)
+        self.onnx_model_path = self.saved_model_path.replace(".h5", ".onnx")
+        tf2onnx.convert.from_keras(self.model, output_path=self.onnx_model_path)
+
+        if self.metadata and isinstance(self.metadata, dict):
+            # Load the ONNX model
+            onnx_model = onnx.load(self.onnx_model_path)
+
+            # Add the metadata dictionary to the model's metadata_props attribute
+            for key, value in self.metadata.items():
+                meta = onnx_model.metadata_props.add()
+                meta.key = key
+                meta.value = value
+
+            # Save the modified ONNX model
+            onnx.save(onnx_model, self.onnx_model_path)
+
+class TrainLogger(Callback):
+    """Logs training metrics to a file.
+    
+    Args:
+        log_path (str): Path to the directory where the log file will be saved.
+        log_file (str, optional): Name of the log file. Defaults to 'logs.log'.
+        logLevel (int, optional): Logging level. Defaults to logging.INFO.
+    """
+    def __init__(self, log_path: str, log_file: str='logs.log', logLevel=logging.INFO) -> None:
+        super().__init__()
+        self.log_path = log_path
+        self.log_file = log_file
+
+        if not os.path.exists(log_path):
+            os.mkdir(log_path)
+
+        self.logger = logging.getLogger()
+        self.logger.setLevel(logLevel)
+
+        self.formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+
+        self.file_handler = logging.FileHandler(os.path.join(self.log_path, self.log_file))
+        self.file_handler.setLevel(logLevel)
+        self.file_handler.setFormatter(self.formatter)
+
+        self.logger.addHandler(self.file_handler)
+
+    def on_epoch_end(self, epoch: int, logs: dict=None):
+        epoch_message = f"Epoch {epoch}; "
+        logs_message = "; ".join([f"{key}: {value}" for key, value in logs.items()])
         self.logger.info(epoch_message + logs_message)
```

### Comparing `mltu-1.0.5/mltu/tensorflow/metrics.py` & `mltu-1.0.6/mltu/tensorflow/metrics.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-import tensorflow as tf
-from keras.metrics import Metric
-
-class CWERMetric(tf.keras.metrics.Metric):
-    """A custom TensorFlow metric to compute the Character Error Rate (CER).
-    
-    Args:
-        padding_token: An integer representing the padding token in the input data.
-        name: (Optional) string name of the metric instance.
-        **kwargs: Additional keyword arguments.
-    """
-    def __init__(self, padding_token, name='CWER', **kwargs):
-        # Initialize the base Metric class
-        super(CWERMetric, self).__init__(name=name, **kwargs)
-        
-        # Initialize variables to keep track of the cumulative character/word error rates and counter
-        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
-        self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
-        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
-        
-        # Store the padding token as an attribute
-        self.padding_token = padding_token
-
-    def update_state(self, y_true, y_pred, sample_weight=None):
-        """Updates the state variables of the metric.
-
-        Args:
-            y_true: A tensor of true labels with shape (batch_size, sequence_length).
-            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
-            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
-        """
-        # Get the input shape and length
-        input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
-
-        # Decode the predicted labels using greedy decoding
-        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
-
-        # Convert the dense decode tensor to a sparse tensor
-        predicted_labels_sparse = tf.keras.backend.ctc_label_dense_to_sparse(decode_predicted[0], input_length)
-        
-        # Convert the dense true labels tensor to a sparse tensor and cast to int64
-        true_labels_sparse = tf.cast(tf.keras.backend.ctc_label_dense_to_sparse(y_true, input_length), "int64")
-
-        # Retain only the non-padding elements in the predicted labels tensor
-        predicted_labels_sparse = tf.sparse.retain(predicted_labels_sparse, tf.not_equal(predicted_labels_sparse.values, -1))
-        
-        # Retain only the non-padding elements in the true labels tensor
-        true_labels_sparse = tf.sparse.retain(true_labels_sparse, tf.not_equal(true_labels_sparse.values, self.padding_token))
-
-        # Calculate the normalized edit distance between the predicted labels and true labels tensors
-        distance = tf.edit_distance(predicted_labels_sparse, true_labels_sparse, normalize=True)
-
-        # Add the sum of the distance tensor to the cer_accumulator variable
-        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
-        
-        # Increment the batch_counter by the batch size
-        self.batch_counter.assign_add(len(y_true))
-
-        # Calculate the number of wrong words in batch and add to wer_accumulator variable
-        self.wer_accumulator.assign_add(tf.reduce_sum(tf.cast(tf.not_equal(distance, 0), tf.float32)))
-
-    def result(self):
-        """Computes and returns the metric result.
-
-        Returns:
-            A dictionary containing the CER and WER.
-        """
-        return {
-                "CER": tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32)),
-                "WER": tf.math.divide_no_nan(self.wer_accumulator, tf.cast(self.batch_counter, tf.float32))
-        }
-
-class CERMetric(tf.keras.metrics.Metric):
-    """A custom TensorFlow metric to compute the Character Error Rate (CER).
-    
-    Args:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-        **kwargs: Additional keyword arguments.
-    """
-    def __init__(self, vocabulary, name='CER', **kwargs):
-        # Initialize the base Metric class
-        super(CERMetric, self).__init__(name=name, **kwargs)
-        
-        # Initialize variables to keep track of the cumulative character/word error rates and counter
-        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
-        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
-        
-        # Store the vocabulary as an attribute
-        self.vocabulary = tf.constant(list(vocabulary))
-
-    @staticmethod
-    def get_cer(pred_decoded, y_true, vocab, padding=-1):
-        """ Calculates the character error rate (CER) between the predicted labels and true labels for a batch of input data.
-
-        Args:
-            pred_decoded (tf.Tensor): The predicted labels, with dtype=tf.int32, usually output from tf.keras.backend.ctc_decode
-            y_true (tf.Tensor): The true labels, with dtype=tf.int32
-            vocab (tf.Tensor): The vocabulary tensor, with dtype=tf.string
-            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
-
-        Returns:
-            tf.Tensor: The CER between the predicted labels and true labels
-        """
-        # Keep only valid indices in the predicted labels tensor, replacing invalid indices with padding token
-        vocab_length = tf.cast(tf.shape(vocab)[0], tf.int64)
-        valid_pred_indices = tf.less(pred_decoded, vocab_length)
-        valid_pred = tf.where(valid_pred_indices, pred_decoded, padding)
-
-        # Keep only valid indices in the true labels tensor, replacing invalid indices with padding token
-        y_true = tf.cast(y_true, tf.int64)
-        valid_true_indices = tf.less(y_true, vocab_length)
-        valid_true = tf.where(valid_true_indices, y_true, padding)
-
-        # Convert the valid predicted labels tensor to a sparse tensor
-        sparse_pred = tf.RaggedTensor.from_tensor(valid_pred, padding=padding).to_sparse()
-
-        # Convert the valid true labels tensor to a sparse tensor
-        sparse_true = tf.RaggedTensor.from_tensor(valid_true, padding=padding).to_sparse()
-
-        # Calculate the normalized edit distance between the sparse predicted labels tensor and sparse true labels tensor
-        distance = tf.edit_distance(sparse_pred, sparse_true, normalize=True)
-
-        return distance
-
-    def update_state(self, y_true, y_pred, sample_weight=None):
-        """Updates the state variables of the metric.
-
-        Args:
-            y_true: A tensor of true labels with shape (batch_size, sequence_length).
-            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
-            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
-        """
-        # Get the input shape and length
-        input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
-
-        # Decode the predicted labels using greedy decoding
-        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
-
-        # Calculate the normalized edit distance between the predicted labels and true labels tensors
-        distance = self.get_cer(decode_predicted[0], y_true, self.vocabulary)
-
-        # Add the sum of the distance tensor to the cer_accumulator variable
-        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
-        
-        # Increment the batch_counter by the batch size
-        self.batch_counter.assign_add(len(y_true))
-
-    def result(self):
-        """ Computes and returns the metric result.
-
-        Returns:
-            A TensorFlow float representing the CER (character error rate).
-        """
-        return tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32))
-
-
-class WERMetric(tf.keras.metrics.Metric):
-    """A custom TensorFlow metric to compute the Word Error Rate (WER).
-    
-    Attributes:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-        **kwargs: Additional keyword arguments.
-    """
-    def __init__(self, vocabulary: str, name='WER', **kwargs):
-        # Initialize the base Metric class
-        super(WERMetric, self).__init__(name=name, **kwargs)
-        
-        # Initialize variables to keep track of the cumulative character/word error rates and counter
-        self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
-        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
-        
-        # Store the vocabulary as an attribute
-        self.vocabulary = tf.constant(list(vocabulary))
-
-    @staticmethod
-    def preprocess_dense(dense_input: tf.Tensor, vocab: tf.Tensor, padding=-1) -> tf.SparseTensor:
-        """ Preprocess the dense input tensor to a sparse tensor with given vocabulary
-        
-        Args:
-            dense_input (tf.Tensor): The dense input tensor, dtype=tf.int32
-            vocab (tf.Tensor): The vocabulary tensor, dtype=tf.string
-            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
-
-        Returns:
-            tf.SparseTensor: The sparse tensor with given vocabulary
-        """
-        # Keep only the valid indices of the dense input tensor
-        vocab_length = tf.cast(tf.shape(vocab)[0], tf.int64)
-        dense_input = tf.cast(dense_input, tf.int64)
-        valid_indices = tf.less(dense_input, vocab_length)
-        valid_input = tf.where(valid_indices, dense_input, padding)
-
-        # Convert the valid input tensor to a ragged tensor with padding
-        input_ragged = tf.RaggedTensor.from_tensor(valid_input, padding=padding)
-
-        # Use the vocabulary tensor to get the strings corresponding to the indices in the ragged tensor
-        input_binary_chars = tf.gather(vocab, input_ragged)
-
-        # Join the binary character tensor along the sequence axis to get the input strings
-        input_strings = tf.strings.reduce_join(input_binary_chars, axis=1, separator='')
-
-        # Convert the input strings tensor to a sparse tensor
-        input_sparse_string = tf.strings.split(input_strings, sep=' ').to_sparse()
-
-        return input_sparse_string
-
-    @staticmethod
-    def get_wer(pred_decoded, y_true, vocab, padding=-1):
-        """ Calculate the normalized WER distance between the predicted labels and true labels tensors
-
-        Args:
-            pred_decoded (tf.Tensor): The predicted labels tensor, dtype=tf.int32. Usually output from tf.keras.backend.ctc_decode
-            y_true (tf.Tensor): The true labels tensor, dtype=tf.int32
-            vocab (tf.Tensor): The vocabulary tensor, dtype=tf.string
-
-        Returns:
-            tf.Tensor: The normalized WER distance between the predicted labels and true labels tensors
-        """
-        pred_sparse = WERMetric.preprocess_dense(pred_decoded, vocab, padding=padding)
-        true_sparse = WERMetric.preprocess_dense(y_true, vocab, padding=padding)
-
-        distance = tf.edit_distance(pred_sparse, true_sparse, normalize=True)
-
-        return distance
-
-    def update_state(self, y_true, y_pred, sample_weight=None):
-        """
-        """
-        # Get the input shape and length
-        input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
-
-        # Decode the predicted labels using greedy decoding
-        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
-
-        # Calculate the normalized edit distance between the predicted labels and true labels tensors
-        distance = self.get_wer(decode_predicted[0], y_true, self.vocabulary)
-
-        # Calculate the number of wrong words in batch and add to wer_accumulator variable
-        self.wer_accumulator.assign_add(tf.reduce_sum(tf.cast(distance, tf.float32)))
-
-        # Increment the batch_counter by the batch size
-        self.batch_counter.assign_add(len(y_true))
-
-    def result(self):
-        """Computes and returns the metric result.
-
-        Returns:
-            A TensorFlow float representing the WER (Word Error Rate).
-        """
+import tensorflow as tf
+from keras.metrics import Metric
+
+class CWERMetric(tf.keras.metrics.Metric):
+    """A custom TensorFlow metric to compute the Character Error Rate (CER).
+    
+    Args:
+        padding_token: An integer representing the padding token in the input data.
+        name: (Optional) string name of the metric instance.
+        **kwargs: Additional keyword arguments.
+    """
+    def __init__(self, padding_token, name='CWER', **kwargs):
+        # Initialize the base Metric class
+        super(CWERMetric, self).__init__(name=name, **kwargs)
+        
+        # Initialize variables to keep track of the cumulative character/word error rates and counter
+        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
+        self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
+        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
+        
+        # Store the padding token as an attribute
+        self.padding_token = padding_token
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        """Updates the state variables of the metric.
+
+        Args:
+            y_true: A tensor of true labels with shape (batch_size, sequence_length).
+            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
+            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
+        """
+        # Get the input shape and length
+        input_shape = tf.keras.backend.shape(y_pred)
+        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
+
+        # Decode the predicted labels using greedy decoding
+        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
+
+        # Convert the dense decode tensor to a sparse tensor
+        predicted_labels_sparse = tf.keras.backend.ctc_label_dense_to_sparse(decode_predicted[0], input_length)
+        
+        # Convert the dense true labels tensor to a sparse tensor and cast to int64
+        true_labels_sparse = tf.cast(tf.keras.backend.ctc_label_dense_to_sparse(y_true, input_length), "int64")
+
+        # Retain only the non-padding elements in the predicted labels tensor
+        predicted_labels_sparse = tf.sparse.retain(predicted_labels_sparse, tf.not_equal(predicted_labels_sparse.values, -1))
+        
+        # Retain only the non-padding elements in the true labels tensor
+        true_labels_sparse = tf.sparse.retain(true_labels_sparse, tf.not_equal(true_labels_sparse.values, self.padding_token))
+
+        # Calculate the normalized edit distance between the predicted labels and true labels tensors
+        distance = tf.edit_distance(predicted_labels_sparse, true_labels_sparse, normalize=True)
+
+        # Add the sum of the distance tensor to the cer_accumulator variable
+        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
+        
+        # Increment the batch_counter by the batch size
+        self.batch_counter.assign_add(len(y_true))
+
+        # Calculate the number of wrong words in batch and add to wer_accumulator variable
+        self.wer_accumulator.assign_add(tf.reduce_sum(tf.cast(tf.not_equal(distance, 0), tf.float32)))
+
+    def result(self):
+        """Computes and returns the metric result.
+
+        Returns:
+            A dictionary containing the CER and WER.
+        """
+        return {
+                "CER": tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32)),
+                "WER": tf.math.divide_no_nan(self.wer_accumulator, tf.cast(self.batch_counter, tf.float32))
+        }
+
+class CERMetric(tf.keras.metrics.Metric):
+    """A custom TensorFlow metric to compute the Character Error Rate (CER).
+    
+    Args:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+        **kwargs: Additional keyword arguments.
+    """
+    def __init__(self, vocabulary, name='CER', **kwargs):
+        # Initialize the base Metric class
+        super(CERMetric, self).__init__(name=name, **kwargs)
+        
+        # Initialize variables to keep track of the cumulative character/word error rates and counter
+        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
+        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
+        
+        # Store the vocabulary as an attribute
+        self.vocabulary = tf.constant(list(vocabulary))
+
+    @staticmethod
+    def get_cer(pred_decoded, y_true, vocab, padding=-1):
+        """ Calculates the character error rate (CER) between the predicted labels and true labels for a batch of input data.
+
+        Args:
+            pred_decoded (tf.Tensor): The predicted labels, with dtype=tf.int32, usually output from tf.keras.backend.ctc_decode
+            y_true (tf.Tensor): The true labels, with dtype=tf.int32
+            vocab (tf.Tensor): The vocabulary tensor, with dtype=tf.string
+            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
+
+        Returns:
+            tf.Tensor: The CER between the predicted labels and true labels
+        """
+        # Keep only valid indices in the predicted labels tensor, replacing invalid indices with padding token
+        vocab_length = tf.cast(tf.shape(vocab)[0], tf.int64)
+        valid_pred_indices = tf.less(pred_decoded, vocab_length)
+        valid_pred = tf.where(valid_pred_indices, pred_decoded, padding)
+
+        # Keep only valid indices in the true labels tensor, replacing invalid indices with padding token
+        y_true = tf.cast(y_true, tf.int64)
+        valid_true_indices = tf.less(y_true, vocab_length)
+        valid_true = tf.where(valid_true_indices, y_true, padding)
+
+        # Convert the valid predicted labels tensor to a sparse tensor
+        sparse_pred = tf.RaggedTensor.from_tensor(valid_pred, padding=padding).to_sparse()
+
+        # Convert the valid true labels tensor to a sparse tensor
+        sparse_true = tf.RaggedTensor.from_tensor(valid_true, padding=padding).to_sparse()
+
+        # Calculate the normalized edit distance between the sparse predicted labels tensor and sparse true labels tensor
+        distance = tf.edit_distance(sparse_pred, sparse_true, normalize=True)
+
+        return distance
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        """Updates the state variables of the metric.
+
+        Args:
+            y_true: A tensor of true labels with shape (batch_size, sequence_length).
+            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
+            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
+        """
+        # Get the input shape and length
+        input_shape = tf.keras.backend.shape(y_pred)
+        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
+
+        # Decode the predicted labels using greedy decoding
+        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
+
+        # Calculate the normalized edit distance between the predicted labels and true labels tensors
+        distance = self.get_cer(decode_predicted[0], y_true, self.vocabulary)
+
+        # Add the sum of the distance tensor to the cer_accumulator variable
+        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
+        
+        # Increment the batch_counter by the batch size
+        self.batch_counter.assign_add(len(y_true))
+
+    def result(self):
+        """ Computes and returns the metric result.
+
+        Returns:
+            A TensorFlow float representing the CER (character error rate).
+        """
+        return tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32))
+
+
+class WERMetric(tf.keras.metrics.Metric):
+    """A custom TensorFlow metric to compute the Word Error Rate (WER).
+    
+    Attributes:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+        **kwargs: Additional keyword arguments.
+    """
+    def __init__(self, vocabulary: str, name='WER', **kwargs):
+        # Initialize the base Metric class
+        super(WERMetric, self).__init__(name=name, **kwargs)
+        
+        # Initialize variables to keep track of the cumulative character/word error rates and counter
+        self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
+        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
+        
+        # Store the vocabulary as an attribute
+        self.vocabulary = tf.constant(list(vocabulary))
+
+    @staticmethod
+    def preprocess_dense(dense_input: tf.Tensor, vocab: tf.Tensor, padding=-1) -> tf.SparseTensor:
+        """ Preprocess the dense input tensor to a sparse tensor with given vocabulary
+        
+        Args:
+            dense_input (tf.Tensor): The dense input tensor, dtype=tf.int32
+            vocab (tf.Tensor): The vocabulary tensor, dtype=tf.string
+            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
+
+        Returns:
+            tf.SparseTensor: The sparse tensor with given vocabulary
+        """
+        # Keep only the valid indices of the dense input tensor
+        vocab_length = tf.cast(tf.shape(vocab)[0], tf.int64)
+        dense_input = tf.cast(dense_input, tf.int64)
+        valid_indices = tf.less(dense_input, vocab_length)
+        valid_input = tf.where(valid_indices, dense_input, padding)
+
+        # Convert the valid input tensor to a ragged tensor with padding
+        input_ragged = tf.RaggedTensor.from_tensor(valid_input, padding=padding)
+
+        # Use the vocabulary tensor to get the strings corresponding to the indices in the ragged tensor
+        input_binary_chars = tf.gather(vocab, input_ragged)
+
+        # Join the binary character tensor along the sequence axis to get the input strings
+        input_strings = tf.strings.reduce_join(input_binary_chars, axis=1, separator='')
+
+        # Convert the input strings tensor to a sparse tensor
+        input_sparse_string = tf.strings.split(input_strings, sep=' ').to_sparse()
+
+        return input_sparse_string
+
+    @staticmethod
+    def get_wer(pred_decoded, y_true, vocab, padding=-1):
+        """ Calculate the normalized WER distance between the predicted labels and true labels tensors
+
+        Args:
+            pred_decoded (tf.Tensor): The predicted labels tensor, dtype=tf.int32. Usually output from tf.keras.backend.ctc_decode
+            y_true (tf.Tensor): The true labels tensor, dtype=tf.int32
+            vocab (tf.Tensor): The vocabulary tensor, dtype=tf.string
+
+        Returns:
+            tf.Tensor: The normalized WER distance between the predicted labels and true labels tensors
+        """
+        pred_sparse = WERMetric.preprocess_dense(pred_decoded, vocab, padding=padding)
+        true_sparse = WERMetric.preprocess_dense(y_true, vocab, padding=padding)
+
+        distance = tf.edit_distance(pred_sparse, true_sparse, normalize=True)
+
+        return distance
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        """
+        """
+        # Get the input shape and length
+        input_shape = tf.keras.backend.shape(y_pred)
+        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
+
+        # Decode the predicted labels using greedy decoding
+        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
+
+        # Calculate the normalized edit distance between the predicted labels and true labels tensors
+        distance = self.get_wer(decode_predicted[0], y_true, self.vocabulary)
+
+        # Calculate the number of wrong words in batch and add to wer_accumulator variable
+        self.wer_accumulator.assign_add(tf.reduce_sum(tf.cast(distance, tf.float32)))
+
+        # Increment the batch_counter by the batch size
+        self.batch_counter.assign_add(len(y_true))
+
+    def result(self):
+        """Computes and returns the metric result.
+
+        Returns:
+            A TensorFlow float representing the WER (Word Error Rate).
+        """
         return tf.math.divide_no_nan(self.wer_accumulator, tf.cast(self.batch_counter, tf.float32))
```

### Comparing `mltu-1.0.5/mltu/tensorflow/model_utils.py` & `mltu-1.0.6/mltu/tensorflow/model_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import typing
-import tensorflow as tf
-from tensorflow import keras
-from keras import layers
-from keras.models import Model
-
-class CustomModel(Model):
-    """ Custom TensorFlow model for debugging training process purposes
-    """
-    def train_step(self, train_data):
-        # Unpack the data. Its structure depends on your model and
-        # on what you pass to `fit()`.
-        inputs, targets = train_data
-        with tf.GradientTape() as tape:
-            results = self(inputs, training=True)
-            loss = self.compiled_loss(targets, results, regularization_losses=self.losses)
-            gradients = tape.gradient(loss, self.trainable_weights)
-
-        # Applying the gradients on the model using the specified optimizer
-        self.optimizer.apply_gradients(zip(gradients, self.trainable_weights))
-
-        # Update the metrics.
-        # Metrics are configured in `compile()`.
-        self.compiled_metrics.update_state(targets, results)
-
-        return {m.name: m.result() for m in self.metrics}
-
-    def test_step(self, test_data):
-        inputs, targets = test_data
-        # Get prediction from model
-        results = self(inputs, training=False)
-
-        # Update the loss
-        self.compiled_loss(targets, results, regularization_losses=self.losses)
-
-        # Update the metrics
-        self.compiled_metrics.update_state(targets, results)
-
-        # Return a dict mapping metric names to current value.
-        # Note that it will include the loss (tracked in self.metrics).
-        return {m.name: m.result() for m in self.metrics}
-
-def activation_layer(layer, activation: str='relu', alpha: float=0.1) -> tf.Tensor:
-    """ Activation layer wrapper for LeakyReLU and ReLU activation functions
-    Args:
-        layer: tf.Tensor
-        activation: str, activation function name (default: 'relu')
-        alpha: float (LeakyReLU activation function parameter)
-    Returns:
-        tf.Tensor
-    """
-    if activation == 'relu':
-        layer = layers.ReLU()(layer)
-    elif activation == 'leaky_relu':
-        layer = layers.LeakyReLU(alpha=alpha)(layer)
-
-    return layer
-
-def residual_block(
-    x: tf.Tensor,
-    filter_num: int,
-    strides: typing.Union[int, list]=2, 
-    kernel_size: typing.Union[int, list]=3, 
-    skip_conv: bool=True, 
-    padding: str='same', 
-    kernel_initializer: str='he_uniform', 
-    activation: str='relu', 
-    dropout: float=0.2
-    ):
-    # Create skip connection tensor
-    x_skip = x
-
-    # Perform 1-st convolution
-    x = layers.Conv2D(filter_num, kernel_size, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x)
-    x = layers.BatchNormalization()(x)
-    x = activation_layer(x, activation=activation)
-
-    # Perform 2-nd convoluti
-    x = layers.Conv2D(filter_num, kernel_size, padding = padding, kernel_initializer=kernel_initializer)(x)
-    x = layers.BatchNormalization()(x)
-
-    # Perform 3-rd convolution if skip_conv is True, matchin the number of filters and the shape of the skip connection tensor
-    if skip_conv:
-        x_skip = layers.Conv2D(filter_num, 1, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x_skip)
-
-    # Add x and skip connection and apply activation function
-    x = layers.Add()([x, x_skip])     
-    x = activation_layer(x, activation=activation)
-
-    # Apply dropout
-    if dropout:
-        x = layers.Dropout(dropout)(x)
-
+import typing
+import tensorflow as tf
+from tensorflow import keras
+from keras import layers
+from keras.models import Model
+
+class CustomModel(Model):
+    """ Custom TensorFlow model for debugging training process purposes
+    """
+    def train_step(self, train_data):
+        # Unpack the data. Its structure depends on your model and
+        # on what you pass to `fit()`.
+        inputs, targets = train_data
+        with tf.GradientTape() as tape:
+            results = self(inputs, training=True)
+            loss = self.compiled_loss(targets, results, regularization_losses=self.losses)
+            gradients = tape.gradient(loss, self.trainable_weights)
+
+        # Applying the gradients on the model using the specified optimizer
+        self.optimizer.apply_gradients(zip(gradients, self.trainable_weights))
+
+        # Update the metrics.
+        # Metrics are configured in `compile()`.
+        self.compiled_metrics.update_state(targets, results)
+
+        return {m.name: m.result() for m in self.metrics}
+
+    def test_step(self, test_data):
+        inputs, targets = test_data
+        # Get prediction from model
+        results = self(inputs, training=False)
+
+        # Update the loss
+        self.compiled_loss(targets, results, regularization_losses=self.losses)
+
+        # Update the metrics
+        self.compiled_metrics.update_state(targets, results)
+
+        # Return a dict mapping metric names to current value.
+        # Note that it will include the loss (tracked in self.metrics).
+        return {m.name: m.result() for m in self.metrics}
+
+def activation_layer(layer, activation: str='relu', alpha: float=0.1) -> tf.Tensor:
+    """ Activation layer wrapper for LeakyReLU and ReLU activation functions
+    Args:
+        layer: tf.Tensor
+        activation: str, activation function name (default: 'relu')
+        alpha: float (LeakyReLU activation function parameter)
+    Returns:
+        tf.Tensor
+    """
+    if activation == 'relu':
+        layer = layers.ReLU()(layer)
+    elif activation == 'leaky_relu':
+        layer = layers.LeakyReLU(alpha=alpha)(layer)
+
+    return layer
+
+def residual_block(
+    x: tf.Tensor,
+    filter_num: int,
+    strides: typing.Union[int, list]=2, 
+    kernel_size: typing.Union[int, list]=3, 
+    skip_conv: bool=True, 
+    padding: str='same', 
+    kernel_initializer: str='he_uniform', 
+    activation: str='relu', 
+    dropout: float=0.2
+    ):
+    # Create skip connection tensor
+    x_skip = x
+
+    # Perform 1-st convolution
+    x = layers.Conv2D(filter_num, kernel_size, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x)
+    x = layers.BatchNormalization()(x)
+    x = activation_layer(x, activation=activation)
+
+    # Perform 2-nd convoluti
+    x = layers.Conv2D(filter_num, kernel_size, padding = padding, kernel_initializer=kernel_initializer)(x)
+    x = layers.BatchNormalization()(x)
+
+    # Perform 3-rd convolution if skip_conv is True, matchin the number of filters and the shape of the skip connection tensor
+    if skip_conv:
+        x_skip = layers.Conv2D(filter_num, 1, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x_skip)
+
+    # Add x and skip connection and apply activation function
+    x = layers.Add()([x, x_skip])     
+    x = activation_layer(x, activation=activation)
+
+    # Apply dropout
+    if dropout:
+        x = layers.Dropout(dropout)(x)
+
     return x
```

### Comparing `mltu-1.0.5/mltu/torch/callbacks.py` & `mltu-1.0.6/mltu/torch/callbacks.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,393 +1,393 @@
-import os
-import onnx
-import logging
-import numpy as np
-from datetime import datetime
-
-import torch.onnx
-from torch.utils.tensorboard import SummaryWriter
-
-class Callback:
-    """ Base class used to build new callbacks."""
-    def __init__(
-        self, 
-        monitor: str = "val_loss"
-    ) -> None:
-        self.monitor = monitor
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(logging.INFO)
-
-    def on_train_begin(self, logs=None):
-        pass
-
-    def on_train_end(self, logs=None):
-        pass
-
-    def on_train_batch_begin(self, batch: int, logs=None):
-        pass
-
-    def on_train_batch_end(self, batch: int, logs=None):
-        pass
-
-    def on_test_begin(self, logs=None):
-        pass
-
-    def on_test_end(self, logs=None):
-        pass
-
-    def on_test_batch_begin(self, batch: int, logs=None):
-        pass
-
-    def on_test_batch_end(self, batch: int, logs=None):
-        pass
-
-    def on_epoch_begin(self, epoch: int, logs=None):
-        pass
-
-    def on_epoch_end(self, epoch: int, logs=None):
-        pass
-
-    def on_batch_begin(self, batch: int, logs=None):
-        pass
-
-    def on_batch_end(self, batch: int, logs=None):
-        pass
-
-    def get_monitor_value(self, logs: dict):
-        logs = logs or {}
-        monitor_value = logs.get(self.monitor)
-        if monitor_value is None:
-            logging.warning(
-                "Early stopping conditioned on metric `%s` "
-                "which is not available. Available metrics are: %s",
-                self.monitor,
-                ",".join(list(logs.keys())),
-            )
-        return monitor_value
-
-class EarlyStopping(Callback):
-    def __init__(
-        self, 
-        monitor: str = "val_loss",
-        min_delta: float = 0.0, 
-        patience: int = 0, 
-        verbose: bool = False,
-        mode: str = "min",
-        ):
-        super(EarlyStopping, self).__init__()
-
-        self.monitor = monitor
-        self.min_delta = min_delta
-        self.patience = patience
-        self.verbose = verbose
-        self.mode = mode
-        self.wait = None
-        self.stopped_epoch = None
-        self.best = None
-
-        if self.mode not in ["min", "max", "max_equal", "min_equal"]:
-            raise ValueError(
-                "EarlyStopping mode %s is unknown, "
-                "please choose one of min, max, max_equal, min_equal" % self.mode
-            )
-        
-    def on_train_begin(self, logs=None):
-        self.wait = 0
-        self.stopped_epoch = 0
-        self.best = np.inf if self.mode == "min" or self.mode == "min_equal" else -np.Inf
-
-    def on_epoch_end(self, epoch: int, logs=None):
-        current = self.get_monitor_value(logs)
-        if current is None:
-            return
-
-        if self.mode == "min" and np.less(current, self.best - self.min_delta):
-            self.best = current
-            self.wait = 0
-        elif self.mode == "max" and np.greater(current, self.best + self.min_delta):
-            self.best = current
-            self.wait = 0
-        elif self.mode == "min_equal" and np.less_equal(current, self.best - self.min_delta):
-            self.best = current
-            self.wait = 0
-        elif self.mode == "max_equal" and np.greater_equal(current, self.best + self.min_delta):
-            self.best = current
-            self.wait = 0
-        else:
-            self.wait += 1
-            if self.wait >= self.patience:
-                self.stopped_epoch = epoch
-                self.model.stop_training = True
-
-    def on_train_end(self, logs=None):
-        if self.stopped_epoch > 0 and self.verbose:
-            self.logger.info(f"Epoch {self.stopped_epoch}: early stopping")
-
-def assign_mode(mode: str):
-    if mode not in ["min", "max", "max_equal", "min_equal"]:
-        raise ValueError(
-            "ModelCheckpoint mode %s is unknown, "
-            "please choose one of min, max, max_equal, min_equal" % mode
-        )
-
-    if mode == "min": return np.less
-    elif mode == "max": return np.greater
-    elif mode == "min_equal": return np.less_equal
-    elif mode == "max_equal": return np.greater_equal
-
-class ModelCheckpoint(Callback):
-    """ ModelCheckpoint callback to save the model after every epoch or the best model across all epochs."""
-    def __init__(
-        self, 
-        filepath: str,
-        monitor: str = "val_loss",
-        verbose: bool = False,
-        save_best_only: bool = True,
-        mode: str = "min",
-        ) -> None:
-        """ ModelCheckpoint callback to save the model after every epoch or the best model across all epochs
-        
-        Args:
-            filepath (str): path to save the model file
-            monitor (str, optional): metric to monitor. Defaults to "val_loss".
-            verbose (bool, optional): verbosity mode. Defaults to False.
-            save_best_only (bool, optional): if True, the latest best model according to the quantity monitored will not be overwritten. Defaults to True.
-            mode (str, optional): one of {min, max, max_equal, min_equal}. Defaults to "min".
-        """
-        super(ModelCheckpoint, self).__init__()
-
-        self.filepath = filepath
-        self.monitor = monitor
-        self.verbose = verbose
-        self.mode = mode
-        self.save_best_only = save_best_only
-        self.best = None
-
-        self.monitor_op = assign_mode(self.mode)
-        
-    def on_train_begin(self, logs=None):
-        self.best = np.inf if self.mode == "min" or self.mode == "min_equal" else -np.Inf
-
-        # create directory if not exist
-        if not os.path.exists(os.path.dirname(self.filepath)):
-            os.makedirs(os.path.dirname(self.filepath))
-
-    def on_epoch_end(self, epoch: int, logs=None):
-        current = self.get_monitor_value(logs)
-        if current is None:
-            return
-
-        if self.monitor_op(current, self.best):
-            previous = self.best
-            self.best = current
-            self.save_model(epoch, current, previous)
-        else:
-            if not self.save_best_only:
-                self.save_model(epoch, current, previous=None)
-
-    def save_model(self, epoch: int, best: float, previous: float = None):
-        """ Save model to filepath
-        
-        Args:
-            epoch (int): current epoch
-            best (float): current best value
-            previous (float, optional): previous best value. Defaults to None.
-        """
-        if self.verbose:
-            if previous is None:
-                self.logger.info(f"Epoch {epoch}: {self.monitor} got {best:.5f}, saving model to {self.filepath}")
-            else:
-                self.logger.info(f"Epoch {epoch}: {self.monitor} improved from {previous:.5f} to {best:.5f}, saving model to {self.filepath}")
-
-        self.model.save(self.filepath)
-
-
-class TensorBoard(Callback):
-    """ TensorBoard basic visualizations. """
-    def __init__(self, log_dir: str = "logs", comment: str = None):
-        """ TensorBoard basic visualizations.
-        
-        Args:
-            log_dir (str, optional): the path of the directory where to save the log files to be parsed by TensorBoard. Defaults to "logs".
-            comment (str, optional): comment to append to the default log_dir. Defaults to None.
-        """
-        super(TensorBoard, self).__init__()
-
-        self.log_dir = log_dir
-
-        self.writer = None
-        self.comment = str(comment) if not None else datetime.now().strftime("%Y%m%d-%H%M%S")
-
-    def on_train_begin(self, logs=None):
-        if self.writer is None:
-            self.writer = SummaryWriter(self.log_dir, comment=self.comment)
-
-    def update_lr(self, epoch: int):
-        for param_group in self.model.optimizer.param_groups:
-            self.writer.add_scalar("learning_rate", param_group["lr"], epoch)
-
-    def update_histogram(self, epoch: int):
-        for name, param in self.model.model.named_parameters():
-            self.writer.add_histogram(name, param.clone().cpu().data.numpy(), epoch)
-
-    def parse_key(self, key: str):
-        if key.startswith("val_"):
-            return f"{key[4:].capitalize()}/test"
-        else:
-            return f"{key.capitalize()}/train"
-
-    def on_epoch_end(self, epoch: int, logs=None):
-        logs = logs or {}
-        for key, value in logs.items():
-            self.writer.add_scalar(self.parse_key(key), value, epoch)
-
-        self.update_lr(epoch)
-        self.update_histogram(epoch)
-
-    def on_train_end(self, logs=None):
-        self.writer.close()
-
-
-class Model2onnx(Callback):
-    """Converts the model from PyTorch to ONNX format after training."""
-    def __init__(
-        self, 
-        saved_model_path: str,
-        input_shape: tuple,
-        export_params: bool=True,
-        opset_version: int=14,
-        do_constant_folding: bool=True,
-        input_names: list=['input'],
-        output_names: list=['output'],
-        dynamic_axes: dict={'input' : {0 : 'batch_size'}, 
-                            'output' : {0 : 'batch_size'}},
-        verbose: bool=False,
-        metadata: dict=None,
-        ) -> None:
-        """ Converts the model from PyTorch to ONNX format after training.
-
-        Args:
-            saved_model_path (str): path to the saved model
-            input_shape (tuple): input shape of the model
-            export_params (bool, optional): if True, all model parameters will be exported. Defaults to True.
-            opset_version (int, optional): the ONNX version to export the model to. Defaults to 14.
-            do_constant_folding (bool, optional): whether to execute constant folding for optimization. Defaults to True.
-            input_names (list, optional): the model's input names. Defaults to ['input'].
-            output_names (list, optional): the model's output names. Defaults to ['output'].
-            dynamic_axes (dict, optional): dictionary specifying dynamic axes. Defaults to {'input' : {0 : 'batch_size'}, 'output' : {0 : 'batch_size'}}.
-            verbose (bool, optional): if True, information about the conversion will be printed. Defaults to False.
-            metadata (dict, optional): dictionary containing model metadata. Defaults to None.
-        """
-        super().__init__()
-        self.saved_model_path = saved_model_path
-        self.input_shape = input_shape
-        self.export_params = export_params
-        self.opset_version = opset_version
-        self.do_constant_folding = do_constant_folding
-        self.input_names = input_names
-        self.output_names = output_names
-        self.dynamic_axes = dynamic_axes
-        self.verbose = verbose
-        self.metadata = metadata
-        
-        self.onnx_model_path = saved_model_path.replace(".pt", ".onnx")
-
-    def on_train_end(self, logs=None):
-        self.model.model.load_state_dict(torch.load(self.saved_model_path))
-
-        # place model on cpu
-        self.model.model.to("cpu")
-
-        # set the model to inference mode
-        self.model.model.eval()
-        
-        # convert the model to ONNX format
-        dummy_input = torch.randn(self.input_shape)
-
-        # Export the model
-        torch.onnx.export(
-            self.model.model,               
-            dummy_input,                         
-            self.onnx_model_path,   
-            export_params=self.export_params,        
-            opset_version=self.opset_version,          
-            do_constant_folding=self.do_constant_folding,  
-            input_names = self.input_names,   
-            output_names = self.output_names, 
-            dynamic_axes = self.dynamic_axes,
-            )
-        
-        if self.verbose:
-            self.logger.info(f"Model saved to {self.onnx_model_path}")
-
-        if self.metadata and isinstance(self.metadata, dict):
-            # Load the ONNX model
-            onnx_model = onnx.load(self.onnx_model_path)
-
-            # Add the metadata dictionary to the model's metadata_props attribute
-            for key, value in self.metadata.items():
-                meta = onnx_model.metadata_props.add()
-                meta.key = key
-                meta.value = value
-
-            # Save the modified ONNX model
-            onnx.save(onnx_model, self.onnx_model_path)
-
-class ReduceLROnPlateau(Callback):
-    """ Reduce learning rate when a metric has stopped improving.
-    Models often benefit from reducing the learning rate by a factor of 2-10 once learning stagnates.
-    This callback monitors a quantity and if no improvement is seen for a 'patience' number of epochs,
-    the learning rate is reduced.
-    """
-    def __init__(
-        self, 
-        monitor: str = "val_loss", 
-        factor: float = 0.1, 
-        patience: int = 10, 
-        min_lr: float = 1e-6, 
-        mode: str = "min",
-        verbose: int = False,
-        ) -> None:
-        """ Reduce learning rate when a metric has stopped improving.
-        
-        Args:
-            monitor (str, optional): quantity to be monitored. Defaults to "val_loss".
-            factor (float, optional): factor by which the learning rate will be reduced. Defaults to 0.1.
-            patience (int, optional): number of epochs with no improvement after which learning rate will be reduced. Defaults to 10.
-            min_lr (float, optional): lower bound on the learning rate. Defaults to 1e-6.
-            verbose (int, optional): verbosity mode. Defaults to 0.
-            mode (str, optional): one of {min, max, max_equal, min_equal}. Defaults to "min". 
-        """
-        super(ReduceLROnPlateau, self).__init__()
-
-        self.monitor = monitor
-        self.factor = factor
-        self.patience = patience
-        self.min_lr = min_lr
-        self.verbose = verbose
-        self.mode = mode
-
-        self.monitor_op = assign_mode(self.mode)
-
-    def on_train_begin(self, logs=None):
-        self.wait = 0
-        self.best = np.inf if self.mode == "min" or self.mode == "min_equal" else -np.Inf
-
-    def on_epoch_end(self, epoch: int, logs=None):
-        current = self.get_monitor_value(logs)
-        if current is None:
-            return
-        
-        if self.monitor_op(current, self.best):
-            self.best = current
-            self.wait = 0
-
-        else:
-            self.wait += 1
-            if self.wait >= self.patience:
-                self.wait = 0
-                current_lr = self.model.optimizer.param_groups[0]["lr"]
-                new_lr = max(current_lr * self.factor, self.min_lr)
-                self.model.optimizer.param_groups[0]["lr"] = new_lr
-                if self.verbose:
+import os
+import onnx
+import logging
+import numpy as np
+from datetime import datetime
+
+import torch.onnx
+from torch.utils.tensorboard import SummaryWriter
+
+class Callback:
+    """ Base class used to build new callbacks."""
+    def __init__(
+        self, 
+        monitor: str = "val_loss"
+    ) -> None:
+        self.monitor = monitor
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(logging.INFO)
+
+    def on_train_begin(self, logs=None):
+        pass
+
+    def on_train_end(self, logs=None):
+        pass
+
+    def on_train_batch_begin(self, batch: int, logs=None):
+        pass
+
+    def on_train_batch_end(self, batch: int, logs=None):
+        pass
+
+    def on_test_begin(self, logs=None):
+        pass
+
+    def on_test_end(self, logs=None):
+        pass
+
+    def on_test_batch_begin(self, batch: int, logs=None):
+        pass
+
+    def on_test_batch_end(self, batch: int, logs=None):
+        pass
+
+    def on_epoch_begin(self, epoch: int, logs=None):
+        pass
+
+    def on_epoch_end(self, epoch: int, logs=None):
+        pass
+
+    def on_batch_begin(self, batch: int, logs=None):
+        pass
+
+    def on_batch_end(self, batch: int, logs=None):
+        pass
+
+    def get_monitor_value(self, logs: dict):
+        logs = logs or {}
+        monitor_value = logs.get(self.monitor)
+        if monitor_value is None:
+            logging.warning(
+                "Early stopping conditioned on metric `%s` "
+                "which is not available. Available metrics are: %s",
+                self.monitor,
+                ",".join(list(logs.keys())),
+            )
+        return monitor_value
+
+class EarlyStopping(Callback):
+    def __init__(
+        self, 
+        monitor: str = "val_loss",
+        min_delta: float = 0.0, 
+        patience: int = 0, 
+        verbose: bool = False,
+        mode: str = "min",
+        ):
+        super(EarlyStopping, self).__init__()
+
+        self.monitor = monitor
+        self.min_delta = min_delta
+        self.patience = patience
+        self.verbose = verbose
+        self.mode = mode
+        self.wait = None
+        self.stopped_epoch = None
+        self.best = None
+
+        if self.mode not in ["min", "max", "max_equal", "min_equal"]:
+            raise ValueError(
+                "EarlyStopping mode %s is unknown, "
+                "please choose one of min, max, max_equal, min_equal" % self.mode
+            )
+        
+    def on_train_begin(self, logs=None):
+        self.wait = 0
+        self.stopped_epoch = 0
+        self.best = np.inf if self.mode == "min" or self.mode == "min_equal" else -np.Inf
+
+    def on_epoch_end(self, epoch: int, logs=None):
+        current = self.get_monitor_value(logs)
+        if current is None:
+            return
+
+        if self.mode == "min" and np.less(current, self.best - self.min_delta):
+            self.best = current
+            self.wait = 0
+        elif self.mode == "max" and np.greater(current, self.best + self.min_delta):
+            self.best = current
+            self.wait = 0
+        elif self.mode == "min_equal" and np.less_equal(current, self.best - self.min_delta):
+            self.best = current
+            self.wait = 0
+        elif self.mode == "max_equal" and np.greater_equal(current, self.best + self.min_delta):
+            self.best = current
+            self.wait = 0
+        else:
+            self.wait += 1
+            if self.wait >= self.patience:
+                self.stopped_epoch = epoch
+                self.model.stop_training = True
+
+    def on_train_end(self, logs=None):
+        if self.stopped_epoch > 0 and self.verbose:
+            self.logger.info(f"Epoch {self.stopped_epoch}: early stopping")
+
+def assign_mode(mode: str):
+    if mode not in ["min", "max", "max_equal", "min_equal"]:
+        raise ValueError(
+            "ModelCheckpoint mode %s is unknown, "
+            "please choose one of min, max, max_equal, min_equal" % mode
+        )
+
+    if mode == "min": return np.less
+    elif mode == "max": return np.greater
+    elif mode == "min_equal": return np.less_equal
+    elif mode == "max_equal": return np.greater_equal
+
+class ModelCheckpoint(Callback):
+    """ ModelCheckpoint callback to save the model after every epoch or the best model across all epochs."""
+    def __init__(
+        self, 
+        filepath: str,
+        monitor: str = "val_loss",
+        verbose: bool = False,
+        save_best_only: bool = True,
+        mode: str = "min",
+        ) -> None:
+        """ ModelCheckpoint callback to save the model after every epoch or the best model across all epochs
+        
+        Args:
+            filepath (str): path to save the model file
+            monitor (str, optional): metric to monitor. Defaults to "val_loss".
+            verbose (bool, optional): verbosity mode. Defaults to False.
+            save_best_only (bool, optional): if True, the latest best model according to the quantity monitored will not be overwritten. Defaults to True.
+            mode (str, optional): one of {min, max, max_equal, min_equal}. Defaults to "min".
+        """
+        super(ModelCheckpoint, self).__init__()
+
+        self.filepath = filepath
+        self.monitor = monitor
+        self.verbose = verbose
+        self.mode = mode
+        self.save_best_only = save_best_only
+        self.best = None
+
+        self.monitor_op = assign_mode(self.mode)
+        
+    def on_train_begin(self, logs=None):
+        self.best = np.inf if self.mode == "min" or self.mode == "min_equal" else -np.Inf
+
+        # create directory if not exist
+        if not os.path.exists(os.path.dirname(self.filepath)):
+            os.makedirs(os.path.dirname(self.filepath))
+
+    def on_epoch_end(self, epoch: int, logs=None):
+        current = self.get_monitor_value(logs)
+        if current is None:
+            return
+
+        if self.monitor_op(current, self.best):
+            previous = self.best
+            self.best = current
+            self.save_model(epoch, current, previous)
+        else:
+            if not self.save_best_only:
+                self.save_model(epoch, current, previous=None)
+
+    def save_model(self, epoch: int, best: float, previous: float = None):
+        """ Save model to filepath
+        
+        Args:
+            epoch (int): current epoch
+            best (float): current best value
+            previous (float, optional): previous best value. Defaults to None.
+        """
+        if self.verbose:
+            if previous is None:
+                self.logger.info(f"Epoch {epoch}: {self.monitor} got {best:.5f}, saving model to {self.filepath}")
+            else:
+                self.logger.info(f"Epoch {epoch}: {self.monitor} improved from {previous:.5f} to {best:.5f}, saving model to {self.filepath}")
+
+        self.model.save(self.filepath)
+
+
+class TensorBoard(Callback):
+    """ TensorBoard basic visualizations. """
+    def __init__(self, log_dir: str = "logs", comment: str = None):
+        """ TensorBoard basic visualizations.
+        
+        Args:
+            log_dir (str, optional): the path of the directory where to save the log files to be parsed by TensorBoard. Defaults to "logs".
+            comment (str, optional): comment to append to the default log_dir. Defaults to None.
+        """
+        super(TensorBoard, self).__init__()
+
+        self.log_dir = log_dir
+
+        self.writer = None
+        self.comment = str(comment) if not None else datetime.now().strftime("%Y%m%d-%H%M%S")
+
+    def on_train_begin(self, logs=None):
+        if self.writer is None:
+            self.writer = SummaryWriter(self.log_dir, comment=self.comment)
+
+    def update_lr(self, epoch: int):
+        for param_group in self.model.optimizer.param_groups:
+            self.writer.add_scalar("learning_rate", param_group["lr"], epoch)
+
+    def update_histogram(self, epoch: int):
+        for name, param in self.model.model.named_parameters():
+            self.writer.add_histogram(name, param.clone().cpu().data.numpy(), epoch)
+
+    def parse_key(self, key: str):
+        if key.startswith("val_"):
+            return f"{key[4:].capitalize()}/test"
+        else:
+            return f"{key.capitalize()}/train"
+
+    def on_epoch_end(self, epoch: int, logs=None):
+        logs = logs or {}
+        for key, value in logs.items():
+            self.writer.add_scalar(self.parse_key(key), value, epoch)
+
+        self.update_lr(epoch)
+        self.update_histogram(epoch)
+
+    def on_train_end(self, logs=None):
+        self.writer.close()
+
+
+class Model2onnx(Callback):
+    """Converts the model from PyTorch to ONNX format after training."""
+    def __init__(
+        self, 
+        saved_model_path: str,
+        input_shape: tuple,
+        export_params: bool=True,
+        opset_version: int=14,
+        do_constant_folding: bool=True,
+        input_names: list=['input'],
+        output_names: list=['output'],
+        dynamic_axes: dict={'input' : {0 : 'batch_size'}, 
+                            'output' : {0 : 'batch_size'}},
+        verbose: bool=False,
+        metadata: dict=None,
+        ) -> None:
+        """ Converts the model from PyTorch to ONNX format after training.
+
+        Args:
+            saved_model_path (str): path to the saved model
+            input_shape (tuple): input shape of the model
+            export_params (bool, optional): if True, all model parameters will be exported. Defaults to True.
+            opset_version (int, optional): the ONNX version to export the model to. Defaults to 14.
+            do_constant_folding (bool, optional): whether to execute constant folding for optimization. Defaults to True.
+            input_names (list, optional): the model's input names. Defaults to ['input'].
+            output_names (list, optional): the model's output names. Defaults to ['output'].
+            dynamic_axes (dict, optional): dictionary specifying dynamic axes. Defaults to {'input' : {0 : 'batch_size'}, 'output' : {0 : 'batch_size'}}.
+            verbose (bool, optional): if True, information about the conversion will be printed. Defaults to False.
+            metadata (dict, optional): dictionary containing model metadata. Defaults to None.
+        """
+        super().__init__()
+        self.saved_model_path = saved_model_path
+        self.input_shape = input_shape
+        self.export_params = export_params
+        self.opset_version = opset_version
+        self.do_constant_folding = do_constant_folding
+        self.input_names = input_names
+        self.output_names = output_names
+        self.dynamic_axes = dynamic_axes
+        self.verbose = verbose
+        self.metadata = metadata
+        
+        self.onnx_model_path = saved_model_path.replace(".pt", ".onnx")
+
+    def on_train_end(self, logs=None):
+        self.model.model.load_state_dict(torch.load(self.saved_model_path))
+
+        # place model on cpu
+        self.model.model.to("cpu")
+
+        # set the model to inference mode
+        self.model.model.eval()
+        
+        # convert the model to ONNX format
+        dummy_input = torch.randn(self.input_shape)
+
+        # Export the model
+        torch.onnx.export(
+            self.model.model,               
+            dummy_input,                         
+            self.onnx_model_path,   
+            export_params=self.export_params,        
+            opset_version=self.opset_version,          
+            do_constant_folding=self.do_constant_folding,  
+            input_names = self.input_names,   
+            output_names = self.output_names, 
+            dynamic_axes = self.dynamic_axes,
+            )
+        
+        if self.verbose:
+            self.logger.info(f"Model saved to {self.onnx_model_path}")
+
+        if self.metadata and isinstance(self.metadata, dict):
+            # Load the ONNX model
+            onnx_model = onnx.load(self.onnx_model_path)
+
+            # Add the metadata dictionary to the model's metadata_props attribute
+            for key, value in self.metadata.items():
+                meta = onnx_model.metadata_props.add()
+                meta.key = key
+                meta.value = value
+
+            # Save the modified ONNX model
+            onnx.save(onnx_model, self.onnx_model_path)
+
+class ReduceLROnPlateau(Callback):
+    """ Reduce learning rate when a metric has stopped improving.
+    Models often benefit from reducing the learning rate by a factor of 2-10 once learning stagnates.
+    This callback monitors a quantity and if no improvement is seen for a 'patience' number of epochs,
+    the learning rate is reduced.
+    """
+    def __init__(
+        self, 
+        monitor: str = "val_loss", 
+        factor: float = 0.1, 
+        patience: int = 10, 
+        min_lr: float = 1e-6, 
+        mode: str = "min",
+        verbose: int = False,
+        ) -> None:
+        """ Reduce learning rate when a metric has stopped improving.
+        
+        Args:
+            monitor (str, optional): quantity to be monitored. Defaults to "val_loss".
+            factor (float, optional): factor by which the learning rate will be reduced. Defaults to 0.1.
+            patience (int, optional): number of epochs with no improvement after which learning rate will be reduced. Defaults to 10.
+            min_lr (float, optional): lower bound on the learning rate. Defaults to 1e-6.
+            verbose (int, optional): verbosity mode. Defaults to 0.
+            mode (str, optional): one of {min, max, max_equal, min_equal}. Defaults to "min". 
+        """
+        super(ReduceLROnPlateau, self).__init__()
+
+        self.monitor = monitor
+        self.factor = factor
+        self.patience = patience
+        self.min_lr = min_lr
+        self.verbose = verbose
+        self.mode = mode
+
+        self.monitor_op = assign_mode(self.mode)
+
+    def on_train_begin(self, logs=None):
+        self.wait = 0
+        self.best = np.inf if self.mode == "min" or self.mode == "min_equal" else -np.Inf
+
+    def on_epoch_end(self, epoch: int, logs=None):
+        current = self.get_monitor_value(logs)
+        if current is None:
+            return
+        
+        if self.monitor_op(current, self.best):
+            self.best = current
+            self.wait = 0
+
+        else:
+            self.wait += 1
+            if self.wait >= self.patience:
+                self.wait = 0
+                current_lr = self.model.optimizer.param_groups[0]["lr"]
+                new_lr = max(current_lr * self.factor, self.min_lr)
+                self.model.optimizer.param_groups[0]["lr"] = new_lr
+                if self.verbose:
                     self.logger.info(f"Epoch {epoch}: reducing learning rate to {new_lr}.")
```

### Comparing `mltu-1.0.5/mltu/torch/dataProvider.py` & `mltu-1.0.6/mltu/torch/dataProvider.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import os
-import typing
-import numpy as np
-import pandas as pd
-import concurrent.futures
-
-from ..augmentors import Augmentor
-from ..transformers import Transformer
-from ..dataProvider import DataProvider
-
-class DataProvider(DataProvider):
-    """ DataProvider for PyTorch with multiprocessing and multithreading support.
-    """
-    def __init__(
-            self, 
-            dataset: typing.Union[str, list, pd.DataFrame],
-            data_preprocessors: typing.List[typing.Callable] = None,
-            batch_size: int = 4,
-            shuffle: bool = True,
-            initial_epoch: int = 1,
-            augmentors: typing.List[Augmentor] = None,
-            transformers: typing.List[Transformer] = None,
-            skip_validation: bool = True,
-            limit: int = None,
-            use_cache: bool = False,
-            workers: int = os.cpu_count(),
-            use_multiprocessing: bool = False,
-        ):
-        """ Standardised object for providing data to a model while training.
-
-        Args:
-            dataset (str, list, pd.DataFrame): Path to dataset, list of data or pandas dataframe of data.
-            data_preprocessors (list): List of data preprocessors. (e.g. [read image, read audio, etc.])
-            batch_size (int): The number of samples to include in each batch. Defaults to 4.
-            shuffle (bool): Whether to shuffle the data. Defaults to True.
-            initial_epoch (int): The initial epoch. Defaults to 1.
-            augmentors (list, optional): List of augmentor functions. Defaults to None.
-            transformers (list, optional): List of transformer functions. Defaults to None.
-            skip_validation (bool, optional): Whether to skip validation. Defaults to True.
-            limit (int, optional): Limit the number of samples in the dataset. Defaults to None.
-            use_cache (bool, optional): Whether to cache the dataset. Defaults to False.
-            workers (int, optional): Number of workers to use for multiprocessing or multithreading. Defaults to os.cpu_count().
-            use_multiprocessing (bool, optional): Whether to use multiprocessing or multithreading. Defaults to multithreading (False).
-        """
-        super(DataProvider, self).__init__(dataset=dataset, data_preprocessors=data_preprocessors, batch_size=batch_size, 
-                                           shuffle=shuffle, initial_epoch=initial_epoch, augmentors=augmentors, transformers=transformers, 
-                                           skip_validation=skip_validation, limit=limit, use_cache=use_cache)
-        self.workers = workers
-        self.use_multiprocessing = use_multiprocessing
-        self._executor = None
-
-    def start_executor(self) -> None:
-        """ Start the executor for multiprocessing or multithreading"""
-        if self.use_multiprocessing:
-            self._executor = concurrent.futures.ProcessPoolExecutor(max_workers=min(self._batch_size, self.workers))
-        self._executor = concurrent.futures.ThreadPoolExecutor(max_workers=min(self._batch_size, self.workers))
-
-    def __getitem__(self, index: int):
-        """ Returns a batch of processed data by index
-        
-        Args:
-            index (int): index of batch
-            
-        Returns:
-            tuple: batch of data and batch of annotations
-        """
-
-        dataset_batch = self.get_batch_annotations(index)
-
-        if self._executor is None:
-            self.start_executor()
-
-        batch_data, batch_annotations = [], []
-        for data, annotation in self._executor.map(self.process_data, dataset_batch):
-            if data is None or annotation is None:
-                continue
-            batch_data.append(data)
-            batch_annotations.append(annotation)
-
+import os
+import typing
+import numpy as np
+import pandas as pd
+import concurrent.futures
+
+from ..augmentors import Augmentor
+from ..transformers import Transformer
+from ..dataProvider import DataProvider
+
+class DataProvider(DataProvider):
+    """ DataProvider for PyTorch with multiprocessing and multithreading support.
+    """
+    def __init__(
+            self, 
+            dataset: typing.Union[str, list, pd.DataFrame],
+            data_preprocessors: typing.List[typing.Callable] = None,
+            batch_size: int = 4,
+            shuffle: bool = True,
+            initial_epoch: int = 1,
+            augmentors: typing.List[Augmentor] = None,
+            transformers: typing.List[Transformer] = None,
+            skip_validation: bool = True,
+            limit: int = None,
+            use_cache: bool = False,
+            workers: int = os.cpu_count(),
+            use_multiprocessing: bool = False,
+        ):
+        """ Standardised object for providing data to a model while training.
+
+        Args:
+            dataset (str, list, pd.DataFrame): Path to dataset, list of data or pandas dataframe of data.
+            data_preprocessors (list): List of data preprocessors. (e.g. [read image, read audio, etc.])
+            batch_size (int): The number of samples to include in each batch. Defaults to 4.
+            shuffle (bool): Whether to shuffle the data. Defaults to True.
+            initial_epoch (int): The initial epoch. Defaults to 1.
+            augmentors (list, optional): List of augmentor functions. Defaults to None.
+            transformers (list, optional): List of transformer functions. Defaults to None.
+            skip_validation (bool, optional): Whether to skip validation. Defaults to True.
+            limit (int, optional): Limit the number of samples in the dataset. Defaults to None.
+            use_cache (bool, optional): Whether to cache the dataset. Defaults to False.
+            workers (int, optional): Number of workers to use for multiprocessing or multithreading. Defaults to os.cpu_count().
+            use_multiprocessing (bool, optional): Whether to use multiprocessing or multithreading. Defaults to multithreading (False).
+        """
+        super(DataProvider, self).__init__(dataset=dataset, data_preprocessors=data_preprocessors, batch_size=batch_size, 
+                                           shuffle=shuffle, initial_epoch=initial_epoch, augmentors=augmentors, transformers=transformers, 
+                                           skip_validation=skip_validation, limit=limit, use_cache=use_cache)
+        self.workers = workers
+        self.use_multiprocessing = use_multiprocessing
+        self._executor = None
+
+    def start_executor(self) -> None:
+        """ Start the executor for multiprocessing or multithreading"""
+        if self.use_multiprocessing:
+            self._executor = concurrent.futures.ProcessPoolExecutor(max_workers=min(self._batch_size, self.workers))
+        self._executor = concurrent.futures.ThreadPoolExecutor(max_workers=min(self._batch_size, self.workers))
+
+    def __getitem__(self, index: int):
+        """ Returns a batch of processed data by index
+        
+        Args:
+            index (int): index of batch
+            
+        Returns:
+            tuple: batch of data and batch of annotations
+        """
+
+        dataset_batch = self.get_batch_annotations(index)
+
+        if self._executor is None:
+            self.start_executor()
+
+        batch_data, batch_annotations = [], []
+        for data, annotation in self._executor.map(self.process_data, dataset_batch):
+            if data is None or annotation is None:
+                continue
+            batch_data.append(data)
+            batch_annotations.append(annotation)
+
         return np.array(batch_data), np.array(batch_annotations)
```

### Comparing `mltu-1.0.5/mltu/torch/handlers.py` & `mltu-1.0.6/mltu/torch/handlers.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import typing
-
-from .metrics import Metric
-from .callbacks import Callback
-
-class MetricsHandler:
-    """ Metrics handler class for training and testing loops"""
-    def __init__(self, metrics: typing.List[Metric]):
-        self.metrics = metrics
-
-        # Validate metrics
-        if not all(isinstance(m, Metric) for m in self.metrics):
-            raise TypeError("all items in the metrics argument must be of type Metric (Check mltu.metrics.metrics.py for more information)")
-        
-        self.train_results_dict = {'loss': None}
-        self.train_results_dict.update({metric.name: None for metric in self.metrics})
-        
-        self.val_results_dict = {'val_loss': None}
-        self.val_results_dict.update({"val_" + metric.name: None for metric in self.metrics})
-
-    def update(self, target, output):
-        for metric in self.metrics:
-            metric.update(output, target)
-
-    def reset(self):
-        for metric in self.metrics:
-            metric.reset()
-
-    def results(self, loss, train: bool=True):
-        if train:
-            self.train_results_dict['loss'] = loss
-            for metric in self.metrics:
-                self.train_results_dict[metric.name] = metric.result()
-            return self.train_results_dict
-        
-        self.val_results_dict['val_loss'] = loss
-        for metric in self.metrics:
-            self.val_results_dict["val_" + metric.name] = metric.result()  
-        return self.val_results_dict
-    
-    def description(self, epoch: int=None, train: bool=True):
-        epoch_desc = f"Epoch {epoch} - " if epoch is not None else "          "
-        dict = self.train_results_dict if train else self.val_results_dict
-        
-        return epoch_desc + " - ".join([f"{k}: {v:.4f}" for k, v in dict.items()])
-    
-
-class CallbacksHandler:
-    """ Callbacks handler class for training and testing loops"""
-    def __init__(self, model, callbacks: typing.List[Callback]):
-        self.callbacks = callbacks
-
-        # Validate callbacks
-        if not all(isinstance(c, Callback) for c in self.callbacks):
-            raise TypeError("all items in the callbacks argument must be of type Callback (Check mltu.torch.callbacks.py for more information)")
-        
-        for callback in self.callbacks:
-            callback.model = model
-        
-    def on_train_begin(self, logs=None):
-        for callback in self.callbacks:
-            callback.on_train_begin(logs)
-
-    def on_train_end(self, logs=None):
-        for callback in self.callbacks:
-            callback.on_train_end(logs)
-
-    def on_epoch_begin(self, epoch, logs=None):
-        for callback in self.callbacks:
-            callback.on_epoch_begin(epoch, logs)
-
-    def on_epoch_end(self, epoch, logs=None):
-        for callback in self.callbacks:
-            callback.on_epoch_end(epoch, logs)
-
-    def on_test_begin(self, logs=None):
-        for callback in self.callbacks:
-            callback.on_test_begin(logs)
-
-    def on_test_end(self, logs=None):
-        for callback in self.callbacks:
-            callback.on_test_end(logs)
-
-    def on_batch_begin(self, batch: int, logs=None, train: bool=True):
-        for callback in self.callbacks:
-            callback.on_batch_begin(batch, logs)
-
-            if train:
-                callback.on_train_batch_begin(batch, logs)
-            else:
-                callback.on_test_batch_begin(batch, logs)
-
-    def on_batch_end(self, batch: int, logs=None, train: bool=True):
-        for callback in self.callbacks:
-            callback.on_batch_end(batch, logs)
-
-            if train:
-                callback.on_train_batch_end(batch, logs)
-            else:
+import typing
+
+from .metrics import Metric
+from .callbacks import Callback
+
+class MetricsHandler:
+    """ Metrics handler class for training and testing loops"""
+    def __init__(self, metrics: typing.List[Metric]):
+        self.metrics = metrics
+
+        # Validate metrics
+        if not all(isinstance(m, Metric) for m in self.metrics):
+            raise TypeError("all items in the metrics argument must be of type Metric (Check mltu.metrics.metrics.py for more information)")
+        
+        self.train_results_dict = {'loss': None}
+        self.train_results_dict.update({metric.name: None for metric in self.metrics})
+        
+        self.val_results_dict = {'val_loss': None}
+        self.val_results_dict.update({"val_" + metric.name: None for metric in self.metrics})
+
+    def update(self, target, output):
+        for metric in self.metrics:
+            metric.update(output, target)
+
+    def reset(self):
+        for metric in self.metrics:
+            metric.reset()
+
+    def results(self, loss, train: bool=True):
+        if train:
+            self.train_results_dict['loss'] = loss
+            for metric in self.metrics:
+                self.train_results_dict[metric.name] = metric.result()
+            return self.train_results_dict
+        
+        self.val_results_dict['val_loss'] = loss
+        for metric in self.metrics:
+            self.val_results_dict["val_" + metric.name] = metric.result()  
+        return self.val_results_dict
+    
+    def description(self, epoch: int=None, train: bool=True):
+        epoch_desc = f"Epoch {epoch} - " if epoch is not None else "          "
+        dict = self.train_results_dict if train else self.val_results_dict
+        
+        return epoch_desc + " - ".join([f"{k}: {v:.4f}" for k, v in dict.items()])
+    
+
+class CallbacksHandler:
+    """ Callbacks handler class for training and testing loops"""
+    def __init__(self, model, callbacks: typing.List[Callback]):
+        self.callbacks = callbacks
+
+        # Validate callbacks
+        if not all(isinstance(c, Callback) for c in self.callbacks):
+            raise TypeError("all items in the callbacks argument must be of type Callback (Check mltu.torch.callbacks.py for more information)")
+        
+        for callback in self.callbacks:
+            callback.model = model
+        
+    def on_train_begin(self, logs=None):
+        for callback in self.callbacks:
+            callback.on_train_begin(logs)
+
+    def on_train_end(self, logs=None):
+        for callback in self.callbacks:
+            callback.on_train_end(logs)
+
+    def on_epoch_begin(self, epoch, logs=None):
+        for callback in self.callbacks:
+            callback.on_epoch_begin(epoch, logs)
+
+    def on_epoch_end(self, epoch, logs=None):
+        for callback in self.callbacks:
+            callback.on_epoch_end(epoch, logs)
+
+    def on_test_begin(self, logs=None):
+        for callback in self.callbacks:
+            callback.on_test_begin(logs)
+
+    def on_test_end(self, logs=None):
+        for callback in self.callbacks:
+            callback.on_test_end(logs)
+
+    def on_batch_begin(self, batch: int, logs=None, train: bool=True):
+        for callback in self.callbacks:
+            callback.on_batch_begin(batch, logs)
+
+            if train:
+                callback.on_train_batch_begin(batch, logs)
+            else:
+                callback.on_test_batch_begin(batch, logs)
+
+    def on_batch_end(self, batch: int, logs=None, train: bool=True):
+        for callback in self.callbacks:
+            callback.on_batch_end(batch, logs)
+
+            if train:
+                callback.on_train_batch_end(batch, logs)
+            else:
                 callback.on_test_batch_end(batch, logs)
```

### Comparing `mltu-1.0.5/mltu/torch/metrics.py` & `mltu-1.0.6/mltu/torch/metrics.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-import torch
-import typing
-import numpy as np
-from itertools import groupby
-
-from mltu.utils.text_utils import get_cer, get_wer
-
-
-class Metric:
-    """ Base class for all metrics"""
-    def __init__(self, name: str) -> None:
-        """ Initialize metric with name
-
-        Args:
-            name (str): name of metric
-        """
-        self.name = name
-
-    def reset(self):
-        """ Reset metric state to initial values and return metric value"""
-        self.__init__()
-
-    def update(self, output: torch.Tensor, target: torch.Tensor):
-        """ Update metric state with new data
-        
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        pass
-
-    def result(self):
-        """ Return metric value"""
-        pass
-
-
-class Accuracy(Metric):
-    """ Accuracy metric class
-    
-    Args:
-        name (str, optional): name of metric. Defaults to 'accuracy'.
-    """
-    def __init__(self, name='accuracy') -> None:
-        super(Accuracy, self).__init__(name=name)
-        self.correct = 0
-        self.total = 0
-
-    def update(self, output: torch.Tensor, target: torch.Tensor):
-        """ Update metric state with new data
-
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        _, predicted = torch.max(output.data, 1)
-        self.total += target.size(0)
-        self.correct += (predicted == target).sum().item()
-
-    def result(self):
-        """ Return metric value"""
-        return self.correct / self.total
-
-
-class CERMetric(Metric):
-    """A custom PyTorch metric to compute the Character Error Rate (CER).
-    
-    Args:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-
-    # TODO: implement everything in Torch to avoid converting to numpy
-    """
-    def __init__(
-        self, 
-        vocabulary: typing.Union[str, list],
-        name: str='CER'
-    ) -> None:
-        super(CERMetric, self).__init__(name=name)
-        self.vocabulary = vocabulary
-        self.reset()
-
-    def reset(self):
-        """ Reset metric state to initial values"""
-        self.cer = 0
-        self.counter = 0
-
-    def update(self, output: torch.Tensor, target: torch.Tensor) -> None:
-        """ Update metric state with new data
-
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        # convert to numpy
-        output = output.detach().cpu().numpy()
-        target = target.detach().cpu().numpy()
-        # use argmax to find the index of the highest probability
-        argmax_preds = np.argmax(output, axis=-1)
-        
-        # use groupby to find continuous same indexes
-        grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
-
-        # convert indexes to strings
-        output_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in grouped_preds]
-        target_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in target]
-
-        cer = get_cer(output_texts, target_texts)
-
-        self.cer += cer
-        self.counter += 1
-
-    def result(self) -> float:
-        """ Return metric value"""
-        return self.cer / self.counter
-    
-
-class WERMetric(Metric):
-    """A custom PyTorch metric to compute the Word Error Rate (WER).
-    
-    Args:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-
-    # TODO: implement everything in Torch to avoid converting to numpy
-    """
-    def __init__(
-        self, 
-        vocabulary: typing.Union[str, list],
-        name: str='WER'
-    ) -> None:
-        super(WERMetric, self).__init__(name=name)
-        self.vocabulary = vocabulary
-        self.reset()
-
-    def reset(self):
-        """ Reset metric state to initial values"""
-        self.wer = 0
-        self.counter = 0
-
-    def update(self, output: torch.Tensor, target: torch.Tensor) -> None:
-        """ Update metric state with new data
-
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        # convert to numpy
-        output = output.detach().cpu().numpy()
-        target = target.detach().cpu().numpy()
-        # use argmax to find the index of the highest probability
-        argmax_preds = np.argmax(output, axis=-1)
-        
-        # use groupby to find continuous same indexes
-        grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
-
-        # convert indexes to strings
-        output_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in grouped_preds]
-        target_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in target]
-
-        wer = get_wer(output_texts, target_texts)
-
-        self.wer += wer
-        self.counter += 1
-
-    def result(self) -> float:
-        """ Return metric value"""
+import torch
+import typing
+import numpy as np
+from itertools import groupby
+
+from mltu.utils.text_utils import get_cer, get_wer
+
+
+class Metric:
+    """ Base class for all metrics"""
+    def __init__(self, name: str) -> None:
+        """ Initialize metric with name
+
+        Args:
+            name (str): name of metric
+        """
+        self.name = name
+
+    def reset(self):
+        """ Reset metric state to initial values and return metric value"""
+        self.__init__()
+
+    def update(self, output: torch.Tensor, target: torch.Tensor):
+        """ Update metric state with new data
+        
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        pass
+
+    def result(self):
+        """ Return metric value"""
+        pass
+
+
+class Accuracy(Metric):
+    """ Accuracy metric class
+    
+    Args:
+        name (str, optional): name of metric. Defaults to 'accuracy'.
+    """
+    def __init__(self, name='accuracy') -> None:
+        super(Accuracy, self).__init__(name=name)
+        self.correct = 0
+        self.total = 0
+
+    def update(self, output: torch.Tensor, target: torch.Tensor):
+        """ Update metric state with new data
+
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        _, predicted = torch.max(output.data, 1)
+        self.total += target.size(0)
+        self.correct += (predicted == target).sum().item()
+
+    def result(self):
+        """ Return metric value"""
+        return self.correct / self.total
+
+
+class CERMetric(Metric):
+    """A custom PyTorch metric to compute the Character Error Rate (CER).
+    
+    Args:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+
+    # TODO: implement everything in Torch to avoid converting to numpy
+    """
+    def __init__(
+        self, 
+        vocabulary: typing.Union[str, list],
+        name: str='CER'
+    ) -> None:
+        super(CERMetric, self).__init__(name=name)
+        self.vocabulary = vocabulary
+        self.reset()
+
+    def reset(self):
+        """ Reset metric state to initial values"""
+        self.cer = 0
+        self.counter = 0
+
+    def update(self, output: torch.Tensor, target: torch.Tensor) -> None:
+        """ Update metric state with new data
+
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        # convert to numpy
+        output = output.detach().cpu().numpy()
+        target = target.detach().cpu().numpy()
+        # use argmax to find the index of the highest probability
+        argmax_preds = np.argmax(output, axis=-1)
+        
+        # use groupby to find continuous same indexes
+        grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
+
+        # convert indexes to strings
+        output_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in grouped_preds]
+        target_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in target]
+
+        cer = get_cer(output_texts, target_texts)
+
+        self.cer += cer
+        self.counter += 1
+
+    def result(self) -> float:
+        """ Return metric value"""
+        return self.cer / self.counter
+    
+
+class WERMetric(Metric):
+    """A custom PyTorch metric to compute the Word Error Rate (WER).
+    
+    Args:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+
+    # TODO: implement everything in Torch to avoid converting to numpy
+    """
+    def __init__(
+        self, 
+        vocabulary: typing.Union[str, list],
+        name: str='WER'
+    ) -> None:
+        super(WERMetric, self).__init__(name=name)
+        self.vocabulary = vocabulary
+        self.reset()
+
+    def reset(self):
+        """ Reset metric state to initial values"""
+        self.wer = 0
+        self.counter = 0
+
+    def update(self, output: torch.Tensor, target: torch.Tensor) -> None:
+        """ Update metric state with new data
+
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        # convert to numpy
+        output = output.detach().cpu().numpy()
+        target = target.detach().cpu().numpy()
+        # use argmax to find the index of the highest probability
+        argmax_preds = np.argmax(output, axis=-1)
+        
+        # use groupby to find continuous same indexes
+        grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
+
+        # convert indexes to strings
+        output_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in grouped_preds]
+        target_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in target]
+
+        wer = get_wer(output_texts, target_texts)
+
+        self.wer += wer
+        self.counter += 1
+
+    def result(self) -> float:
+        """ Return metric value"""
         return self.wer / self.counter
```

### Comparing `mltu-1.0.5/mltu/torch/model.py` & `mltu-1.0.6/mltu/torch/model.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-import torch
-import typing
-import numpy as np
-from tqdm import tqdm
-
-from .metrics import Metric
-from .callbacks import Callback
-from .dataProvider import DataProvider
-from .handlers import MetricsHandler, CallbacksHandler
-
-def toTorch(data: np.ndarray, target: np.ndarray) -> typing.Tuple[torch.Tensor, torch.Tensor]:
-    """ Check if data is of type torch.Tensor, if not convert it to torch.Tensor
-
-    Args:
-        data (np.ndarray): data to be converted
-        target (np.ndarray): target to be converted
-
-    Returns:
-        typing.Tuple[torch.Tensor, torch.Tensor]: converted data and target
-    """
-    if not isinstance(data, torch.Tensor):
-        data = torch.from_numpy(data)
-
-    if not isinstance(target, torch.Tensor):
-        target = torch.from_numpy(target)
-
-    if data.dtype != torch.float32:
-        data = data.float()
-
-    return data, target
-
-class Model:
-    """ Model class for training and testing PyTorch neural networks"""
-    def __init__(
-        self, 
-        model: torch.nn.Module, 
-        optimizer: torch.optim.Optimizer, 
-        loss: typing.Callable,
-        metrics: typing.List[Metric] = [],
-        ):
-        """ Initialize model class
-
-        Attributes:
-            model (torch.nn.Module): PyTorch neural network
-            optimizer (torch.optim.Optimizer): PyTorch optimizer
-            loss (typing.Callable): loss function
-            metrics (typing.List[Metric], optional): list of metrics. Defaults to [].
-        """
-        self.model = model
-        self.optimizer = optimizer
-        self.loss = loss
-
-        self.metrics = MetricsHandler(metrics)
-
-        self.stop_training = False
-        # get device on which model is running
-        self._device = next(self.model.parameters()).device
-
-        self.validate()
-
-    def validate(self):
-        """ Validate model, optimizer"""
-        if not isinstance(self.model, torch.nn.Module):
-            raise TypeError("model argument must be a torch.nn.Module")
-        
-        if not isinstance(self.optimizer, torch.optim.Optimizer):
-            raise TypeError("optimizer argument must be a torch.optim.Optimizer")
-        
-    def toDevice(self, data: np.ndarray, target: np.ndarray) -> typing.Tuple[torch.Tensor, torch.Tensor]:
-        """ Check if data is on the same device as model, if not move it to the device
-
-        Args:
-            data (np.ndarray): data to be moved
-            target (np.ndarray): target to be moved
-
-        Returns:
-            typing.Tuple[torch.Tensor, torch.Tensor]: moved data and target
-        """
-        if data.device != self._device:
-            data = data.to(self._device)
-
-        if target.device != self._device:
-            target = target.to(self._device)
-
-        return data, target
-
-    def train_step(
-        self, 
-        data: typing.Union[np.ndarray, torch.Tensor], 
-        target: typing.Union[np.ndarray, torch.Tensor]
-        ) -> torch.Tensor:
-        """ Perform one training step
-
-        Args:
-            data (typing.Union[np.ndarray, torch.Tensor]): training data
-            target (typing.Union[np.ndarray, torch.Tensor]): training target
-
-        Returns:
-            torch.Tensor: loss
-        """
-        self.optimizer.zero_grad()
-        output = self.model(data)
-        loss = self.loss(output, target)
-        loss.backward()
-        self.optimizer.step()
-        torch.cuda.synchronize() # synchronize after each forward and backward pass
-
-        self.metrics.update(target, output)
-
-        return loss
-    
-    def test_step(
-        self, 
-        data: typing.Union[np.ndarray, torch.Tensor], 
-        target: typing.Union[np.ndarray, torch.Tensor]
-        ) -> torch.Tensor:
-        """ Perform one validation step
-
-        Args:
-            data (typing.Union[np.ndarray, torch.Tensor]): validation data
-            target (typing.Union[np.ndarray, torch.Tensor]): validation target
-
-        Returns:
-            torch.Tensor: loss
-        """
-        output = self.model(data)
-        loss = self.loss(output, target)
-
-        self.metrics.update(target, output)
-
-        return loss
-    
-    def train(self, dataProvider: DataProvider):
-        """ Perform one training epoch
-        
-        Args:
-            dataProvider (DataProvider): data provider for training data
-
-        Returns:
-            dict: training results
-        """
-        # set model to training mode
-        self.model.train()
-
-        loss_sum = 0
-        pbar = tqdm(dataProvider, total=len(dataProvider))
-        for step, (data, target) in enumerate(pbar, start=1):
-            self.callbacks.on_batch_begin(step, logs=None, train=True)
-
-            data, target = self.toDevice(*toTorch(data, target))
-            loss = self.train_step(data, target)
-            loss_sum += loss.item()
-            loss_mean = loss_sum / step
-
-            # get training results of one step
-            logs = self.metrics.results(loss_mean, train=True)
-            description = self.metrics.description(epoch=self._epoch, train=True)
-
-            # update progress bar description
-            pbar.set_description(description)
-
-            self.callbacks.on_batch_end(step, logs=logs, train=True)
-
-        # reset metrics after each training epoch
-        self.metrics.reset()
-
-        # call on_epoch_end of data provider
-        dataProvider.on_epoch_end()
-
-        return logs
-
-    def test(self, dataProvider: DataProvider):
-        """ Perform one validation epoch
-
-        Args:
-            dataProvider (DataProvider): data provider for validation data
-
-        Returns:
-            dict: validation results
-        """
-        # set model to evaluation mode
-        self.model.eval()
-        loss_sum = 0
-        pbar = tqdm(dataProvider, total=len(dataProvider))
-        for step, (data, target) in enumerate(pbar, start=1):
-            self.callbacks.on_batch_begin(step, logs=None, train=False)
-
-            data, target = self.toDevice(*toTorch(data, target))
-            loss = self.test_step(data, target)
-            loss_sum += loss.item()
-            loss_mean = loss_sum / step
-
-            # get testing results of one step
-            logs = self.metrics.results(loss_mean, train=False)
-            description = self.metrics.description(train=False)
-
-            # update progress bar description
-            pbar.set_description(description)
-
-            self.callbacks.on_batch_end(step, logs=logs, train=False)
-
-        # reset metrics after each test epoch
-        self.metrics.reset()
-
-        # call on_epoch_end of data provider
-        dataProvider.on_epoch_end()
-
-        return logs
-    
-    def save(self, path: str):
-        """ Save model state dict to file
-
-        Args:
-            path (str): path to file
-        """
-        torch.save(self.model.state_dict(), path)
-    
-    def fit(
-        self, 
-        train_dataProvider: DataProvider, 
-        test_dataProvider: DataProvider, 
-        epochs: int, 
-        initial_epoch:int = 1, 
-        callbacks: typing.List[Callback] = []
-        ) -> dict:
-        """ Train model for a given number of epochs
-        
-        Args:
-            train_dataProvider (DataProvider): data provider for training data
-            test_dataProvider (DataProvider): data provider for validation data
-            epochs (int): number of epochs
-            initial_epoch (int, optional): initial epoch. Defaults to 1.
-            callbacks (typing.List[Callback], optional): list of callbacks. Defaults to [].
-
-        Returns:
-            dict: training results
-        """
-        self._epoch = initial_epoch
-        self.callbacks = CallbacksHandler(self, callbacks)
-        self.callbacks.on_train_begin()
-        for epoch in range(initial_epoch, initial_epoch + epochs):
-            self.callbacks.on_epoch_begin(epoch)
-
-            train_logs = self.train(train_dataProvider)
-            val_logs = self.test(test_dataProvider)
-
-            logs = {**train_logs, **val_logs}
-            self.callbacks.on_epoch_end(epoch, logs=logs)
-
-            if self.stop_training:
-                break
-
-            self._epoch += 1
-
-        self.callbacks.on_train_end(logs)
-
+import torch
+import typing
+import numpy as np
+from tqdm import tqdm
+
+from .metrics import Metric
+from .callbacks import Callback
+from .dataProvider import DataProvider
+from .handlers import MetricsHandler, CallbacksHandler
+
+def toTorch(data: np.ndarray, target: np.ndarray) -> typing.Tuple[torch.Tensor, torch.Tensor]:
+    """ Check if data is of type torch.Tensor, if not convert it to torch.Tensor
+
+    Args:
+        data (np.ndarray): data to be converted
+        target (np.ndarray): target to be converted
+
+    Returns:
+        typing.Tuple[torch.Tensor, torch.Tensor]: converted data and target
+    """
+    if not isinstance(data, torch.Tensor):
+        data = torch.from_numpy(data)
+
+    if not isinstance(target, torch.Tensor):
+        target = torch.from_numpy(target)
+
+    if data.dtype != torch.float32:
+        data = data.float()
+
+    return data, target
+
+class Model:
+    """ Model class for training and testing PyTorch neural networks"""
+    def __init__(
+        self, 
+        model: torch.nn.Module, 
+        optimizer: torch.optim.Optimizer, 
+        loss: typing.Callable,
+        metrics: typing.List[Metric] = [],
+        ):
+        """ Initialize model class
+
+        Attributes:
+            model (torch.nn.Module): PyTorch neural network
+            optimizer (torch.optim.Optimizer): PyTorch optimizer
+            loss (typing.Callable): loss function
+            metrics (typing.List[Metric], optional): list of metrics. Defaults to [].
+        """
+        self.model = model
+        self.optimizer = optimizer
+        self.loss = loss
+
+        self.metrics = MetricsHandler(metrics)
+
+        self.stop_training = False
+        # get device on which model is running
+        self._device = next(self.model.parameters()).device
+
+        self.validate()
+
+    def validate(self):
+        """ Validate model, optimizer"""
+        if not isinstance(self.model, torch.nn.Module):
+            raise TypeError("model argument must be a torch.nn.Module")
+        
+        if not isinstance(self.optimizer, torch.optim.Optimizer):
+            raise TypeError("optimizer argument must be a torch.optim.Optimizer")
+        
+    def toDevice(self, data: np.ndarray, target: np.ndarray) -> typing.Tuple[torch.Tensor, torch.Tensor]:
+        """ Check if data is on the same device as model, if not move it to the device
+
+        Args:
+            data (np.ndarray): data to be moved
+            target (np.ndarray): target to be moved
+
+        Returns:
+            typing.Tuple[torch.Tensor, torch.Tensor]: moved data and target
+        """
+        if data.device != self._device:
+            data = data.to(self._device)
+
+        if target.device != self._device:
+            target = target.to(self._device)
+
+        return data, target
+
+    def train_step(
+        self, 
+        data: typing.Union[np.ndarray, torch.Tensor], 
+        target: typing.Union[np.ndarray, torch.Tensor]
+        ) -> torch.Tensor:
+        """ Perform one training step
+
+        Args:
+            data (typing.Union[np.ndarray, torch.Tensor]): training data
+            target (typing.Union[np.ndarray, torch.Tensor]): training target
+
+        Returns:
+            torch.Tensor: loss
+        """
+        self.optimizer.zero_grad()
+        output = self.model(data)
+        loss = self.loss(output, target)
+        loss.backward()
+        self.optimizer.step()
+        torch.cuda.synchronize() # synchronize after each forward and backward pass
+
+        self.metrics.update(target, output)
+
+        return loss
+    
+    def test_step(
+        self, 
+        data: typing.Union[np.ndarray, torch.Tensor], 
+        target: typing.Union[np.ndarray, torch.Tensor]
+        ) -> torch.Tensor:
+        """ Perform one validation step
+
+        Args:
+            data (typing.Union[np.ndarray, torch.Tensor]): validation data
+            target (typing.Union[np.ndarray, torch.Tensor]): validation target
+
+        Returns:
+            torch.Tensor: loss
+        """
+        output = self.model(data)
+        loss = self.loss(output, target)
+
+        self.metrics.update(target, output)
+
+        return loss
+    
+    def train(self, dataProvider: DataProvider):
+        """ Perform one training epoch
+        
+        Args:
+            dataProvider (DataProvider): data provider for training data
+
+        Returns:
+            dict: training results
+        """
+        # set model to training mode
+        self.model.train()
+
+        loss_sum = 0
+        pbar = tqdm(dataProvider, total=len(dataProvider))
+        for step, (data, target) in enumerate(pbar, start=1):
+            self.callbacks.on_batch_begin(step, logs=None, train=True)
+
+            data, target = self.toDevice(*toTorch(data, target))
+            loss = self.train_step(data, target)
+            loss_sum += loss.item()
+            loss_mean = loss_sum / step
+
+            # get training results of one step
+            logs = self.metrics.results(loss_mean, train=True)
+            description = self.metrics.description(epoch=self._epoch, train=True)
+
+            # update progress bar description
+            pbar.set_description(description)
+
+            self.callbacks.on_batch_end(step, logs=logs, train=True)
+
+        # reset metrics after each training epoch
+        self.metrics.reset()
+
+        # call on_epoch_end of data provider
+        dataProvider.on_epoch_end()
+
+        return logs
+
+    def test(self, dataProvider: DataProvider):
+        """ Perform one validation epoch
+
+        Args:
+            dataProvider (DataProvider): data provider for validation data
+
+        Returns:
+            dict: validation results
+        """
+        # set model to evaluation mode
+        self.model.eval()
+        loss_sum = 0
+        pbar = tqdm(dataProvider, total=len(dataProvider))
+        for step, (data, target) in enumerate(pbar, start=1):
+            self.callbacks.on_batch_begin(step, logs=None, train=False)
+
+            data, target = self.toDevice(*toTorch(data, target))
+            loss = self.test_step(data, target)
+            loss_sum += loss.item()
+            loss_mean = loss_sum / step
+
+            # get testing results of one step
+            logs = self.metrics.results(loss_mean, train=False)
+            description = self.metrics.description(train=False)
+
+            # update progress bar description
+            pbar.set_description(description)
+
+            self.callbacks.on_batch_end(step, logs=logs, train=False)
+
+        # reset metrics after each test epoch
+        self.metrics.reset()
+
+        # call on_epoch_end of data provider
+        dataProvider.on_epoch_end()
+
+        return logs
+    
+    def save(self, path: str):
+        """ Save model state dict to file
+
+        Args:
+            path (str): path to file
+        """
+        torch.save(self.model.state_dict(), path)
+    
+    def fit(
+        self, 
+        train_dataProvider: DataProvider, 
+        test_dataProvider: DataProvider, 
+        epochs: int, 
+        initial_epoch:int = 1, 
+        callbacks: typing.List[Callback] = []
+        ) -> dict:
+        """ Train model for a given number of epochs
+        
+        Args:
+            train_dataProvider (DataProvider): data provider for training data
+            test_dataProvider (DataProvider): data provider for validation data
+            epochs (int): number of epochs
+            initial_epoch (int, optional): initial epoch. Defaults to 1.
+            callbacks (typing.List[Callback], optional): list of callbacks. Defaults to [].
+
+        Returns:
+            dict: training results
+        """
+        self._epoch = initial_epoch
+        self.callbacks = CallbacksHandler(self, callbacks)
+        self.callbacks.on_train_begin()
+        for epoch in range(initial_epoch, initial_epoch + epochs):
+            self.callbacks.on_epoch_begin(epoch)
+
+            train_logs = self.train(train_dataProvider)
+            val_logs = self.test(test_dataProvider)
+
+            logs = {**train_logs, **val_logs}
+            self.callbacks.on_epoch_end(epoch, logs=logs)
+
+            if self.stop_training:
+                break
+
+            self._epoch += 1
+
+        self.callbacks.on_train_end(logs)
+
         return logs
```

### Comparing `mltu-1.0.5/mltu/transformers.py` & `mltu-1.0.6/mltu/transformers.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-import cv2
-import typing
-import numpy as np
-
-from . import Image
-
-import logging
-logging.basicConfig(format='%(asctime)s %(levelname)s %(name)s: %(message)s')
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
-
-
-class Transformer:
-    def __init__(self, log_level: int = logging.INFO) -> None:
-        self._log_level = log_level
-
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(logging.INFO)
-
-    def __call__(self, data: typing.Any, label: typing.Any, *args, **kwargs):
-        raise NotImplementedError
-
-
-class ExpandDims(Transformer):
-    def __init__(self, axis: int=-1):
-        self.axis = axis
-
-    def __call__(self, data: np.ndarray, label: np.ndarray):
-        return np.expand_dims(data, self.axis), label
-
-class ImageResizer(Transformer):
-    """Resize image to (width, height)
-    
-    Attributes:
-        width (int): Width of image
-        height (int): Height of image
-        keep_aspect_ratio (bool): Whether to keep aspect ratio of image
-        padding_color (typing.Tuple[int]): Color to pad image
-    """
-    def __init__(
-        self, 
-        width: int, 
-        height: int, 
-        keep_aspect_ratio: bool=False, 
-        padding_color: typing.Tuple[int]=(0, 0, 0)
-        ) -> None:
-        self._width = width
-        self._height = height
-        self._keep_aspect_ratio = keep_aspect_ratio
-        self._padding_color = padding_color
-
-    @staticmethod
-    def resize_maintaining_aspect_ratio(image: np.ndarray, width_target: int, height_target: int, padding_color: typing.Tuple[int]=(0, 0, 0)) -> np.ndarray:
-        """ Resize image maintaining aspect ratio and pad with padding_color.
-
-        Args:
-            image (np.ndarray): Image to resize
-            width_target (int): Target width
-            height_target (int): Target height
-            padding_color (typing.Tuple[int]): Color to pad image
-
-        Returns:
-            np.ndarray: Resized image
-        """
-        height, width = image.shape[:2]
-        ratio = min(width_target / width, height_target / height)
-        new_w, new_h = int(width * ratio), int(height * ratio)
-
-        resized_image = cv2.resize(image, (new_w, new_h))
-        delta_w = width_target - new_w
-        delta_h = height_target - new_h
-        top, bottom = delta_h//2, delta_h-(delta_h//2)
-        left, right = delta_w//2, delta_w-(delta_w//2)
-
-        new_image = cv2.copyMakeBorder(resized_image, top, bottom, left, right, cv2.BORDER_CONSTANT, value=padding_color)
-
-        return new_image
-
-    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        # Maintains aspect ratio and resizes with padding.
-        image_numpy = image.numpy()
-        if self._keep_aspect_ratio:
-            image_numpy = self.resize_maintaining_aspect_ratio(image.numpy(), self._width, self._height, self._padding_color)
-
-            # TODO - Fix this
-            # if isinstance(label, np.ndarray):
-            #     label = self.resize_maintaining_aspect_ratio(label, self._width, self._height, self._padding_color)
-
-        else:   
-            # Resizes without maintaining aspect ratio.
-            image_numpy = cv2.resize(image_numpy, (self._width, self._height))
-
-        image.update(image_numpy)
-
-        return image, label
-
-class LabelIndexer(Transformer):
-    """Convert label to index by vocab
-    
-    Attributes:
-        vocab (typing.List[str]): List of characters in vocab
-    """
-    def __init__(
-        self, 
-        vocab: typing.List[str]
-        ) -> None:
-        self.vocab = vocab
-
-    def __call__(self, data: np.ndarray, label: np.ndarray):
-        return data, np.array([self.vocab.index(l) for l in label if l in self.vocab])
-
-class LabelPadding(Transformer):
-    """Pad label to max_word_length
-    
-    Attributes:
-        max_word_length (int): Maximum length of label
-        padding_value (int): Value to pad
-    """
-    def __init__(
-        self, 
-        max_word_length: int, 
-        padding_value: int
-        ) -> None:
-        self.max_word_length = max_word_length
-        self.padding_value = padding_value
-
-    def __call__(self, data: np.ndarray, label: np.ndarray):
-        return data, np.pad(label, (0, self.max_word_length - len(label)), 'constant', constant_values=self.padding_value)
-
-class SpectrogramPadding(Transformer):
-    """Pad spectrogram to max_spectrogram_length
-    
-    Attributes:
-        max_spectrogram_length (int): Maximum length of spectrogram
-        padding_value (int): Value to pad
-    """
-    def __init__(
-        self, 
-        max_spectrogram_length: int, 
-        padding_value: int
-        ) -> None:
-        self.max_spectrogram_length = max_spectrogram_length
-        self.padding_value = padding_value
-
-    def __call__(self, spectrogram: np.ndarray, label: np.ndarray):
-        padded_spectrogram = np.pad(spectrogram, ((self.max_spectrogram_length - spectrogram.shape[0], 0),(0,0)), mode='constant', constant_values=self.padding_value)
-
-        return padded_spectrogram, label
-
-class ImageShowCV2(Transformer):
-    """Show image for visual inspection
-    """
-    def __init__(
-        self, 
-        verbose: bool=True, 
-        log_level: int = logging.INFO,
-        name: str = 'Image'
-        ) -> None:
-        """
-        Args:
-            verbose (bool): Whether to log label
-            log_level (int): Logging level (default: logging.INFO)
-            name (str): Name of window to show image
-        """
-        super(ImageShowCV2, self).__init__(log_level=log_level)
-        self.verbose = verbose
-        self.name = name
-
-    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Show image for visual inspection
-
-        Args:
-            data (np.ndarray): Image data
-            label (np.ndarray): Label data
-        
-        Returns:
-            data (np.ndarray): Image data
-            label (np.ndarray): Label data (unchanged)
-        """
-        if self.verbose:
-            if isinstance(label, (str, int, float)):
-                self.logger.info(f'Label: {label}')
-
-        cv2.imshow(self.name, image.numpy())
-        cv2.waitKey(0)
-        cv2.destroyAllWindows()
-
+import cv2
+import typing
+import numpy as np
+
+from . import Image
+
+import logging
+logging.basicConfig(format='%(asctime)s %(levelname)s %(name)s: %(message)s')
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+
+
+class Transformer:
+    def __init__(self, log_level: int = logging.INFO) -> None:
+        self._log_level = log_level
+
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(logging.INFO)
+
+    def __call__(self, data: typing.Any, label: typing.Any, *args, **kwargs):
+        raise NotImplementedError
+
+
+class ExpandDims(Transformer):
+    def __init__(self, axis: int=-1):
+        self.axis = axis
+
+    def __call__(self, data: np.ndarray, label: np.ndarray):
+        return np.expand_dims(data, self.axis), label
+
+class ImageResizer(Transformer):
+    """Resize image to (width, height)
+    
+    Attributes:
+        width (int): Width of image
+        height (int): Height of image
+        keep_aspect_ratio (bool): Whether to keep aspect ratio of image
+        padding_color (typing.Tuple[int]): Color to pad image
+    """
+    def __init__(
+        self, 
+        width: int, 
+        height: int, 
+        keep_aspect_ratio: bool=False, 
+        padding_color: typing.Tuple[int]=(0, 0, 0)
+        ) -> None:
+        self._width = width
+        self._height = height
+        self._keep_aspect_ratio = keep_aspect_ratio
+        self._padding_color = padding_color
+
+    @staticmethod
+    def resize_maintaining_aspect_ratio(image: np.ndarray, width_target: int, height_target: int, padding_color: typing.Tuple[int]=(0, 0, 0)) -> np.ndarray:
+        """ Resize image maintaining aspect ratio and pad with padding_color.
+
+        Args:
+            image (np.ndarray): Image to resize
+            width_target (int): Target width
+            height_target (int): Target height
+            padding_color (typing.Tuple[int]): Color to pad image
+
+        Returns:
+            np.ndarray: Resized image
+        """
+        height, width = image.shape[:2]
+        ratio = min(width_target / width, height_target / height)
+        new_w, new_h = int(width * ratio), int(height * ratio)
+
+        resized_image = cv2.resize(image, (new_w, new_h))
+        delta_w = width_target - new_w
+        delta_h = height_target - new_h
+        top, bottom = delta_h//2, delta_h-(delta_h//2)
+        left, right = delta_w//2, delta_w-(delta_w//2)
+
+        new_image = cv2.copyMakeBorder(resized_image, top, bottom, left, right, cv2.BORDER_CONSTANT, value=padding_color)
+
+        return new_image
+
+    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        # Maintains aspect ratio and resizes with padding.
+        image_numpy = image.numpy()
+        if self._keep_aspect_ratio:
+            image_numpy = self.resize_maintaining_aspect_ratio(image.numpy(), self._width, self._height, self._padding_color)
+
+            # TODO - Fix this
+            # if isinstance(label, np.ndarray):
+            #     label = self.resize_maintaining_aspect_ratio(label, self._width, self._height, self._padding_color)
+
+        else:   
+            # Resizes without maintaining aspect ratio.
+            image_numpy = cv2.resize(image_numpy, (self._width, self._height))
+
+        image.update(image_numpy)
+
+        return image, label
+
+class LabelIndexer(Transformer):
+    """Convert label to index by vocab
+    
+    Attributes:
+        vocab (typing.List[str]): List of characters in vocab
+    """
+    def __init__(
+        self, 
+        vocab: typing.List[str]
+        ) -> None:
+        self.vocab = vocab
+
+    def __call__(self, data: np.ndarray, label: np.ndarray):
+        return data, np.array([self.vocab.index(l) for l in label if l in self.vocab])
+
+class LabelPadding(Transformer):
+    """Pad label to max_word_length
+    
+    Attributes:
+        max_word_length (int): Maximum length of label
+        padding_value (int): Value to pad
+    """
+    def __init__(
+        self, 
+        max_word_length: int, 
+        padding_value: int
+        ) -> None:
+        self.max_word_length = max_word_length
+        self.padding_value = padding_value
+
+    def __call__(self, data: np.ndarray, label: np.ndarray):
+        return data, np.pad(label, (0, self.max_word_length - len(label)), 'constant', constant_values=self.padding_value)
+
+class SpectrogramPadding(Transformer):
+    """Pad spectrogram to max_spectrogram_length
+    
+    Attributes:
+        max_spectrogram_length (int): Maximum length of spectrogram
+        padding_value (int): Value to pad
+    """
+    def __init__(
+        self, 
+        max_spectrogram_length: int, 
+        padding_value: int
+        ) -> None:
+        self.max_spectrogram_length = max_spectrogram_length
+        self.padding_value = padding_value
+
+    def __call__(self, spectrogram: np.ndarray, label: np.ndarray):
+        padded_spectrogram = np.pad(spectrogram, ((self.max_spectrogram_length - spectrogram.shape[0], 0),(0,0)), mode='constant', constant_values=self.padding_value)
+
+        return padded_spectrogram, label
+
+class ImageShowCV2(Transformer):
+    """Show image for visual inspection
+    """
+    def __init__(
+        self, 
+        verbose: bool=True, 
+        log_level: int = logging.INFO,
+        name: str = 'Image'
+        ) -> None:
+        """
+        Args:
+            verbose (bool): Whether to log label
+            log_level (int): Logging level (default: logging.INFO)
+            name (str): Name of window to show image
+        """
+        super(ImageShowCV2, self).__init__(log_level=log_level)
+        self.verbose = verbose
+        self.name = name
+
+    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Show image for visual inspection
+
+        Args:
+            data (np.ndarray): Image data
+            label (np.ndarray): Label data
+        
+        Returns:
+            data (np.ndarray): Image data
+            label (np.ndarray): Label data (unchanged)
+        """
+        if self.verbose:
+            if isinstance(label, (str, int, float)):
+                self.logger.info(f'Label: {label}')
+
+        cv2.imshow(self.name, image.numpy())
+        cv2.waitKey(0)
+        cv2.destroyAllWindows()
+
         return image, label
```

### Comparing `mltu-1.0.5/mltu/utils/text_utils.py` & `mltu-1.0.6/mltu/utils/text_utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import typing
-import numpy as np
-from itertools import groupby
-    
-def ctc_decoder(predictions: np.ndarray, chars: typing.Union[str, list]) -> typing.List[str]:
-    ''' CTC greedy decoder for predictions
-    
-    Args:
-        predictions (np.ndarray): predictions from model
-        chars (typing.Union[str, list]): list of characters
-
-    Returns:
-        typing.List[str]: list of words
-    '''
-    # use argmax to find the index of the highest probability
-    argmax_preds = np.argmax(predictions, axis=-1)
-    
-    # use groupby to find continuous same indexes
-    grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
-
-    # convert indexes to chars
-    texts = ["".join([chars[k] for k in group if k < len(chars)]) for group in grouped_preds]
-
-    return texts
-
-
-def edit_distance(prediction_tokens: typing.List[str], reference_tokens: typing.List[str]) -> int:
-    """ Standard dynamic programming algorithm to compute the Levenshtein Edit Distance Algorithm
-
-    Args:
-        prediction_tokens: A tokenized predicted sentence
-        reference_tokens: A tokenized reference sentence
-    Returns:
-        Edit distance between the predicted sentence and the reference sentence
-    """
-    # Initialize a matrix to store the edit distances
-    dp = [[0] * (len(reference_tokens) + 1) for _ in range(len(prediction_tokens) + 1)]
-
-    # Fill the first row and column with the number of insertions needed
-    for i in range(len(prediction_tokens) + 1):
-        dp[i][0] = i
-    
-    dp[0] = [j for j in range(len(reference_tokens) + 1)]
-
-    # Iterate through the prediction and reference tokens
-    for i, p_tok in enumerate(prediction_tokens):
-        for j, r_tok in enumerate(reference_tokens):
-            # If the tokens are the same, the edit distance is the same as the previous entry
-            if p_tok == r_tok:
-                dp[i+1][j+1] = dp[i][j]
-            # If the tokens are different, the edit distance is the minimum of the previous entries plus 1
-            else:
-                dp[i+1][j+1] = min(dp[i][j+1], dp[i+1][j], dp[i][j]) + 1
-
-    # Return the final entry in the matrix as the edit distance     
-    return dp[-1][-1]
-
-def get_cer(
-    preds: typing.Union[str, typing.List[str]],
-    target: typing.Union[str, typing.List[str]],
-    ) -> float:
-    """ Update the cer score with the current set of references and predictions.
-
-    Args:
-        preds (typing.Union[str, typing.List[str]]): list of predicted sentences
-        target (typing.Union[str, typing.List[str]]): list of target words
-
-    Returns:
-        Character error rate score
-    """
-    if isinstance(preds, str):
-        preds = [preds]
-    if isinstance(target, str):
-        target = [target]
-
-    total, errors = 0, 0
-    for pred_tokens, tgt_tokens in zip(preds, target):
-        errors += edit_distance(list(pred_tokens), list(tgt_tokens))
-        total += len(tgt_tokens)
-
-    if total == 0:
-        return 0.0
-
-    cer = errors / total
-
-    return cer
-
-def get_wer(
-    preds: typing.Union[str, typing.List[str]],
-    target: typing.Union[str, typing.List[str]],
-    ) -> float:
-    """ Update the wer score with the current set of references and predictions.
-
-    Args:
-        target (typing.Union[str, typing.List[str]]): string of target sentence or list of target words
-        preds (typing.Union[str, typing.List[str]]): string of predicted sentence or list of predicted words
-
-    Returns:
-        Word error rate score
-    """
-    if isinstance(preds, str):
-        preds = preds.split()
-    if isinstance(target, str):
-        target = target.split()
-
-    errors = edit_distance(preds, target)
-    total_words = len(target)
-
-    if total_words == 0:
-        return 0.0
-
-    return errors / total_words
-
-if __name__ == '__main__':
-    c1 = 'ROKAS'
-    c2 = 'ROKAZ '
-
-    w1 = 'ROKAS GOOD BOY'
-    w2 = 'ROKAZ IS A GOOD BOY'
-
-    cer = get_cer(c1, c2)
-    wer = get_wer(w1, w2)
-
+import typing
+import numpy as np
+from itertools import groupby
+    
+def ctc_decoder(predictions: np.ndarray, chars: typing.Union[str, list]) -> typing.List[str]:
+    ''' CTC greedy decoder for predictions
+    
+    Args:
+        predictions (np.ndarray): predictions from model
+        chars (typing.Union[str, list]): list of characters
+
+    Returns:
+        typing.List[str]: list of words
+    '''
+    # use argmax to find the index of the highest probability
+    argmax_preds = np.argmax(predictions, axis=-1)
+    
+    # use groupby to find continuous same indexes
+    grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
+
+    # convert indexes to chars
+    texts = ["".join([chars[k] for k in group if k < len(chars)]) for group in grouped_preds]
+
+    return texts
+
+
+def edit_distance(prediction_tokens: typing.List[str], reference_tokens: typing.List[str]) -> int:
+    """ Standard dynamic programming algorithm to compute the Levenshtein Edit Distance Algorithm
+
+    Args:
+        prediction_tokens: A tokenized predicted sentence
+        reference_tokens: A tokenized reference sentence
+    Returns:
+        Edit distance between the predicted sentence and the reference sentence
+    """
+    # Initialize a matrix to store the edit distances
+    dp = [[0] * (len(reference_tokens) + 1) for _ in range(len(prediction_tokens) + 1)]
+
+    # Fill the first row and column with the number of insertions needed
+    for i in range(len(prediction_tokens) + 1):
+        dp[i][0] = i
+    
+    dp[0] = [j for j in range(len(reference_tokens) + 1)]
+
+    # Iterate through the prediction and reference tokens
+    for i, p_tok in enumerate(prediction_tokens):
+        for j, r_tok in enumerate(reference_tokens):
+            # If the tokens are the same, the edit distance is the same as the previous entry
+            if p_tok == r_tok:
+                dp[i+1][j+1] = dp[i][j]
+            # If the tokens are different, the edit distance is the minimum of the previous entries plus 1
+            else:
+                dp[i+1][j+1] = min(dp[i][j+1], dp[i+1][j], dp[i][j]) + 1
+
+    # Return the final entry in the matrix as the edit distance     
+    return dp[-1][-1]
+
+def get_cer(
+    preds: typing.Union[str, typing.List[str]],
+    target: typing.Union[str, typing.List[str]],
+    ) -> float:
+    """ Update the cer score with the current set of references and predictions.
+
+    Args:
+        preds (typing.Union[str, typing.List[str]]): list of predicted sentences
+        target (typing.Union[str, typing.List[str]]): list of target words
+
+    Returns:
+        Character error rate score
+    """
+    if isinstance(preds, str):
+        preds = [preds]
+    if isinstance(target, str):
+        target = [target]
+
+    total, errors = 0, 0
+    for pred_tokens, tgt_tokens in zip(preds, target):
+        errors += edit_distance(list(pred_tokens), list(tgt_tokens))
+        total += len(tgt_tokens)
+
+    if total == 0:
+        return 0.0
+
+    cer = errors / total
+
+    return cer
+
+def get_wer(
+    preds: typing.Union[str, typing.List[str]],
+    target: typing.Union[str, typing.List[str]],
+    ) -> float:
+    """ Update the wer score with the current set of references and predictions.
+
+    Args:
+        target (typing.Union[str, typing.List[str]]): string of target sentence or list of target words
+        preds (typing.Union[str, typing.List[str]]): string of predicted sentence or list of predicted words
+
+    Returns:
+        Word error rate score
+    """
+    if isinstance(preds, str):
+        preds = preds.split()
+    if isinstance(target, str):
+        target = target.split()
+
+    errors = edit_distance(preds, target)
+    total_words = len(target)
+
+    if total_words == 0:
+        return 0.0
+
+    return errors / total_words
+
+if __name__ == '__main__':
+    c1 = 'ROKAS'
+    c2 = 'ROKAZ '
+
+    w1 = 'ROKAS GOOD BOY'
+    w2 = 'ROKAZ IS A GOOD BOY'
+
+    cer = get_cer(c1, c2)
+    wer = get_wer(w1, w2)
+
     print(wer)
```

### Comparing `mltu-1.0.5/mltu.egg-info/PKG-INFO` & `mltu-1.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,26 @@
-Metadata-Version: 2.1
-Name: mltu
-Version: 1.0.5
-Summary: Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch
-Home-page: https://pylessons.com/
-Author: PyLessons
-Author-email: pythonlessons0@gmail.com
-Project-URL: Source, https://github.com/pythonlessons/mltu/
-Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-License-File: LICENSE
-
-# MLTU - Machine Learning Training Utilities
-Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
-<p align="center">
-  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
-</p>
-
-# Installation:
-To use MLTU in your own project, you can install it from PyPI:
-```bash
-pip install mltu
-```
-When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
-```bash
-pip install mltu==0.1.3
-```
-Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
-
-# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
-1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
-2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
-3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
-4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
-5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
-6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
-7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
-8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
+# MLTU - Machine Learning Training Utilities
+Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
+<p align="center">
+  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
+</p>
+
+# Installation:
+To use MLTU in your own project, you can install it from PyPI:
+```bash
+pip install mltu
+```
+When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
+```bash
+pip install mltu==0.1.3
+```
+Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
+
+# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
+1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
+2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
+3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
+4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
+5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
+6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
+7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
+8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
```

### Comparing `mltu-1.0.5/mltu.egg-info/SOURCES.txt` & `mltu-1.0.6/mltu.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -26,9 +26,8 @@
 mltu/torch/callbacks.py
 mltu/torch/dataProvider.py
 mltu/torch/handlers.py
 mltu/torch/losses.py
 mltu/torch/metrics.py
 mltu/torch/model.py
 mltu/utils/__init__.py
-mltu/utils/text_utils.py
-tests/test_text_utils.py
+mltu/utils/text_utils.py
```

### Comparing `mltu-1.0.5/setup.py` & `mltu-1.0.6/setup.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import os
-from setuptools import setup
-
-DIR = os.path.abspath(os.path.dirname(__file__))
-
-with open(os.path.join(DIR, 'README.md')) as fh:
-    long_description = fh.read()
-
-with open(os.path.join(DIR, 'requirements.txt')) as fh:
-    requirements = fh.read().splitlines()
-
-def get_version(initpath: str) -> str:
-    """ Get from the init of the source code the version string
-
-    Params:
-        initpath (str): path to the init file of the python package relative to the setup file
-
-    Returns:
-        str: The version string in the form 0.0.1
-    """
-
-    path = os.path.join(os.path.dirname(__file__), initpath)
-
-    with open(path, "r") as handle:
-        for line in handle.read().splitlines():
-            if line.startswith("__version__"):
-                return line.split("=")[1].strip().strip("\"'")
-        else:
-            raise RuntimeError("Unable to find version string.")
-
-setup(
-    name = 'mltu',
-    version = get_version("mltu/__init__.py"),
-    long_description = long_description,
-    long_description_content_type = 'text/markdown',
-    url='https://pylessons.com/',
-    author='PyLessons',
-    author_email='pythonlessons0@gmail.com',
-    install_requires=requirements,
-    extras_require={
-        'gpu': ['onnxruntime-gpu'],
-    },
-    python_requires='>=3',
-    packages = ['mltu', 'mltu.utils', 'mltu.torch', 'mltu.tensorflow', 'mltu.annotations'],
-    include_package_data=True,
-    project_urls={
-        'Source': 'https://github.com/pythonlessons/mltu/',
-        'Tracker': 'https://github.com/pythonlessons/mltu/issues',
-    },
-    description="Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch",
+import os
+from setuptools import setup
+
+DIR = os.path.abspath(os.path.dirname(__file__))
+
+with open(os.path.join(DIR, 'README.md')) as fh:
+    long_description = fh.read()
+
+with open(os.path.join(DIR, 'requirements.txt')) as fh:
+    requirements = fh.read().splitlines()
+
+def get_version(initpath: str) -> str:
+    """ Get from the init of the source code the version string
+
+    Params:
+        initpath (str): path to the init file of the python package relative to the setup file
+
+    Returns:
+        str: The version string in the form 0.0.1
+    """
+
+    path = os.path.join(os.path.dirname(__file__), initpath)
+
+    with open(path, "r") as handle:
+        for line in handle.read().splitlines():
+            if line.startswith("__version__"):
+                return line.split("=")[1].strip().strip("\"'")
+        else:
+            raise RuntimeError("Unable to find version string.")
+
+setup(
+    name = 'mltu',
+    version = get_version("mltu/__init__.py"),
+    long_description = long_description,
+    long_description_content_type = 'text/markdown',
+    url='https://pylessons.com/',
+    author='PyLessons',
+    author_email='pythonlessons0@gmail.com',
+    install_requires=requirements,
+    extras_require={
+        'gpu': ['onnxruntime-gpu'],
+    },
+    python_requires='>=3',
+    packages = ['mltu', 'mltu.utils', 'mltu.torch', 'mltu.tensorflow', 'mltu.annotations'],
+    include_package_data=True,
+    project_urls={
+        'Source': 'https://github.com/pythonlessons/mltu/',
+        'Tracker': 'https://github.com/pythonlessons/mltu/issues',
+    },
+    description="Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch",
 )
```

