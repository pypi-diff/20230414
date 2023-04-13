# Comparing `tmp/manim-ml-0.0.8.tar.gz` & `tmp/manim-ml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim-ml-0.0.8.tar", last modified: Thu Apr 14 05:16:59 2022, max compression
+gzip compressed data, was "manim-ml-0.0.9.tar", last modified: Fri May  6 03:37:05 2022, max compression
```

## Comparing `manim-ml-0.0.8.tar` & `manim-ml-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 alechelbling   (501) staff       (20)        0 2022-04-14 05:16:59.503588 manim-ml-0.0.8/
--rw-r--r--   0 alechelbling   (501) staff       (20)     1069 2022-03-28 04:34:00.000000 manim-ml-0.0.8/LICENSE.md
--rw-r--r--   0 alechelbling   (501) staff       (20)     3447 2022-04-14 05:16:59.503685 manim-ml-0.0.8/PKG-INFO
-drwxr-xr-x   0 alechelbling   (501) staff       (20)        0 2022-04-14 05:16:59.500122 manim-ml-0.0.8/manim_ml/
--rw-r--r--   0 alechelbling   (501) staff       (20)        0 2022-02-06 03:46:43.000000 manim-ml-0.0.8/manim_ml/__init__.py
--rw-r--r--   0 alechelbling   (501) staff       (20)      779 2022-04-09 23:04:54.000000 manim-ml-0.0.8/manim_ml/image.py
--rw-r--r--   0 alechelbling   (501) staff       (20)       46 2022-04-02 23:20:30.000000 manim-ml-0.0.8/manim_ml/manifold.py
--rw-r--r--   0 alechelbling   (501) staff       (20)      399 2022-04-02 23:20:30.000000 manim-ml-0.0.8/manim_ml/one_to_one_sync.py
--rw-r--r--   0 alechelbling   (501) staff       (20)     1167 2022-04-02 23:20:30.000000 manim-ml-0.0.8/manim_ml/util.py
-drwxr-xr-x   0 alechelbling   (501) staff       (20)        0 2022-04-14 05:16:59.503392 manim-ml-0.0.8/manim_ml.egg-info/
--rw-r--r--   0 alechelbling   (501) staff       (20)     3447 2022-04-14 05:16:59.000000 manim-ml-0.0.8/manim_ml.egg-info/PKG-INFO
--rw-r--r--   0 alechelbling   (501) staff       (20)      268 2022-04-14 05:16:59.000000 manim-ml-0.0.8/manim_ml.egg-info/SOURCES.txt
--rw-r--r--   0 alechelbling   (501) staff       (20)        1 2022-04-14 05:16:59.000000 manim-ml-0.0.8/manim_ml.egg-info/dependency_links.txt
--rw-r--r--   0 alechelbling   (501) staff       (20)        9 2022-04-14 05:16:59.000000 manim-ml-0.0.8/manim_ml.egg-info/top_level.txt
--rw-r--r--   0 alechelbling   (501) staff       (20)        0 2022-03-28 17:57:52.000000 manim-ml-0.0.8/pyproject.toml
--rw-r--r--   0 alechelbling   (501) staff       (20)      632 2022-04-14 05:16:59.504016 manim-ml-0.0.8/setup.cfg
+drwxr-xr-x   0 alechelbling   (501) staff       (20)        0 2022-05-06 03:37:05.051108 manim-ml-0.0.9/
+-rw-r--r--   0 alechelbling   (501) staff       (20)     1069 2022-03-28 04:34:00.000000 manim-ml-0.0.9/LICENSE.md
+-rw-r--r--   0 alechelbling   (501) staff       (20)     3480 2022-05-06 03:37:05.051178 manim-ml-0.0.9/PKG-INFO
+drwxr-xr-x   0 alechelbling   (501) staff       (20)        0 2022-05-06 03:37:05.050206 manim-ml-0.0.9/manim_ml/
+-rw-r--r--   0 alechelbling   (501) staff       (20)        0 2022-04-19 03:37:54.000000 manim-ml-0.0.9/manim_ml/__init__.py
+-rw-r--r--   0 alechelbling   (501) staff       (20)     1731 2022-04-27 04:45:23.000000 manim-ml-0.0.9/manim_ml/image.py
+-rw-r--r--   0 alechelbling   (501) staff       (20)     2022 2022-04-25 01:27:41.000000 manim-ml-0.0.9/manim_ml/list_group.py
+-rw-r--r--   0 alechelbling   (501) staff       (20)       46 2022-04-02 23:20:30.000000 manim-ml-0.0.9/manim_ml/manifold.py
+-rw-r--r--   0 alechelbling   (501) staff       (20)      399 2022-04-02 23:20:30.000000 manim-ml-0.0.9/manim_ml/one_to_one_sync.py
+-rw-r--r--   0 alechelbling   (501) staff       (20)     4030 2022-04-26 19:48:47.000000 manim-ml-0.0.9/manim_ml/probability.py
+drwxr-xr-x   0 alechelbling   (501) staff       (20)        0 2022-05-06 03:37:05.050989 manim-ml-0.0.9/manim_ml.egg-info/
+-rw-r--r--   0 alechelbling   (501) staff       (20)     3480 2022-05-06 03:37:04.000000 manim-ml-0.0.9/manim_ml.egg-info/PKG-INFO
+-rw-r--r--   0 alechelbling   (501) staff       (20)      298 2022-05-06 03:37:05.000000 manim-ml-0.0.9/manim_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 alechelbling   (501) staff       (20)        1 2022-05-06 03:37:04.000000 manim-ml-0.0.9/manim_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 alechelbling   (501) staff       (20)        9 2022-05-06 03:37:05.000000 manim-ml-0.0.9/manim_ml.egg-info/top_level.txt
+-rw-r--r--   0 alechelbling   (501) staff       (20)        0 2022-03-28 17:57:52.000000 manim-ml-0.0.9/pyproject.toml
+-rw-r--r--   0 alechelbling   (501) staff       (20)      632 2022-05-06 03:37:05.051437 manim-ml-0.0.9/setup.cfg
```

### Comparing `manim-ml-0.0.8/LICENSE.md` & `manim-ml-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `manim-ml-0.0.8/PKG-INFO` & `manim-ml-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-ml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Machine Learning Animations in python using Manim
 Home-page: https://github.com/helblazer811/ManimMachineLearning
 Author: Alec Helbling
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/helblazer811/ManimMachineLearning/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -43,51 +43,48 @@
 
 ## Examples
 
 Checkout the ```examples``` directory for some example videos with source code. 
 
 ### Neural Networks
 
-This is a visualization of a Neural Network made using ManimML. It has a Pytorch style list of layers that can be composed in arbitrary order. The following video is made with the code from below.  
+This is a visualization of a Variational Autoencoder made using ManimML. It has a Pytorch style list of layers that can be composed in arbitrary order. The following video is made with the code from below.  
 
-<img src="examples/media/ImageNeuralNetworkScene.gif">
+<img src="examples/media/VAEScene.gif">
 
 ```python
-from manim import *
-from manim_ml.neural_network.layers import FeedForwardLayer, ImageLayer
-from manim_ml.neural_network.neural_network import NeuralNetwork
-from PIL import Image
-import numpy as np
-
-class ImageNeuralNetworkScene(Scene):
+class VariationalAutoencoderScene(Scene):
 
     def construct(self):
+        embedding_layer = EmbeddingLayer(dist_theme="ellipse").scale(2)
+        
         image = Image.open('images/image.jpeg')
         numpy_image = np.asarray(image)
         # Make nn
-        layers = [
-            ImageLayer(numpy_image, height=1.0),
-            FeedForwardLayer(3), 
+        neural_network = NeuralNetwork([
+            ImageLayer(numpy_image, height=1.4),
             FeedForwardLayer(5),
-            FeedForwardLayer(3)
-        ]
-        nn = NeuralNetwork(layers)
-        # Center the nn
-        nn.move_to(ORIGIN)
-        self.add(nn)
-        # Play animation
-        self.play(nn.make_forward_pass_animation())
-```
+            FeedForwardLayer(3),
+            embedding_layer,
+            FeedForwardLayer(3),
+            FeedForwardLayer(5),
+            ImageLayer(numpy_image, height=1.4),
+        ], layer_spacing=0.1)
 
+        neural_network.scale(1.3)
 
-### Variational Autoencoders
+        self.play(Create(neural_network))
+        self.play(neural_network.make_forward_pass_animation(run_time=15))
+```
 
-This is a visualization of a Variational Autoencoder. 
+### Generative Adversarial Network
 
-<img src="examples/media/VAEScene.gif">
+This is a visualization of a Generative Adversarial Network made using ManimML. 
+
+<img src="examples/media/GANScene.gif">
 
 ### VAE Disentanglement 
 
 This is a visualization of disentanglement with a Variational Autoencoder
 
 <img src="examples/media/DisentanglementScene.gif">
```

### Comparing `manim-ml-0.0.8/manim_ml.egg-info/PKG-INFO` & `manim-ml-0.0.9/manim_ml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-ml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Machine Learning Animations in python using Manim
 Home-page: https://github.com/helblazer811/ManimMachineLearning
 Author: Alec Helbling
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/helblazer811/ManimMachineLearning/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -43,51 +43,48 @@
 
 ## Examples
 
 Checkout the ```examples``` directory for some example videos with source code. 
 
 ### Neural Networks
 
-This is a visualization of a Neural Network made using ManimML. It has a Pytorch style list of layers that can be composed in arbitrary order. The following video is made with the code from below.  
+This is a visualization of a Variational Autoencoder made using ManimML. It has a Pytorch style list of layers that can be composed in arbitrary order. The following video is made with the code from below.  
 
-<img src="examples/media/ImageNeuralNetworkScene.gif">
+<img src="examples/media/VAEScene.gif">
 
 ```python
-from manim import *
-from manim_ml.neural_network.layers import FeedForwardLayer, ImageLayer
-from manim_ml.neural_network.neural_network import NeuralNetwork
-from PIL import Image
-import numpy as np
-
-class ImageNeuralNetworkScene(Scene):
+class VariationalAutoencoderScene(Scene):
 
     def construct(self):
+        embedding_layer = EmbeddingLayer(dist_theme="ellipse").scale(2)
+        
         image = Image.open('images/image.jpeg')
         numpy_image = np.asarray(image)
         # Make nn
-        layers = [
-            ImageLayer(numpy_image, height=1.0),
-            FeedForwardLayer(3), 
+        neural_network = NeuralNetwork([
+            ImageLayer(numpy_image, height=1.4),
             FeedForwardLayer(5),
-            FeedForwardLayer(3)
-        ]
-        nn = NeuralNetwork(layers)
-        # Center the nn
-        nn.move_to(ORIGIN)
-        self.add(nn)
-        # Play animation
-        self.play(nn.make_forward_pass_animation())
-```
+            FeedForwardLayer(3),
+            embedding_layer,
+            FeedForwardLayer(3),
+            FeedForwardLayer(5),
+            ImageLayer(numpy_image, height=1.4),
+        ], layer_spacing=0.1)
 
+        neural_network.scale(1.3)
 
-### Variational Autoencoders
+        self.play(Create(neural_network))
+        self.play(neural_network.make_forward_pass_animation(run_time=15))
+```
 
-This is a visualization of a Variational Autoencoder. 
+### Generative Adversarial Network
 
-<img src="examples/media/VAEScene.gif">
+This is a visualization of a Generative Adversarial Network made using ManimML. 
+
+<img src="examples/media/GANScene.gif">
 
 ### VAE Disentanglement 
 
 This is a visualization of disentanglement with a Variational Autoencoder
 
 <img src="examples/media/DisentanglementScene.gif">
```

### Comparing `manim-ml-0.0.8/setup.cfg` & `manim-ml-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = manim-ml
-version = 0.0.8
+version = 0.0.9
 author = Alec Helbling
 description = Machine Learning Animations in python using Manim
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/helblazer811/ManimMachineLearning
 project_urls = 
 	Bug Tracker = https://github.com/helblazer811/ManimMachineLearning/issues
```

