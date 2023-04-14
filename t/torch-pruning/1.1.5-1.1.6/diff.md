# Comparing `tmp/torch-pruning-1.1.5.tar.gz` & `tmp/torch-pruning-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-pruning-1.1.5.tar", last modified: Sun Apr  9 09:07:01 2023, max compression
+gzip compressed data, was "torch-pruning-1.1.6.tar", last modified: Fri Apr 14 18:02:57 2023, max compression
```

## Comparing `torch-pruning-1.1.5.tar` & `torch-pruning-1.1.6.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.789480 torch-pruning-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-09 09:07:01.789480 torch-pruning-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:07:01.789480 torch-pruning-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_backward.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_customized_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_dependency_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_dependency_lenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_fully_connected_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_interactive_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_multiple_inputs_and_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_pruning_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_unwrapped_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/torch_pruning/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    36317 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/torch_pruning/pruner/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/batchnorm_scale_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/group_norm_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/magnitude_based_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/metapruner.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.789480 torch-pruning-1.1.5/torch_pruning/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/utils/op_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/torch_pruning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:02:57.574589 torch-pruning-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-04-14 18:02:57.574589 torch-pruning-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:02:57.574589 torch-pruning-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:02:57.570588 torch-pruning-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_backward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_concat_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_customized_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_dependency_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_dependency_lenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_fully_connected_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_interactive_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_multiple_inputs_and_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_pruning_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/tests/test_unwrapped_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:02:57.570588 torch-pruning-1.1.6/torch_pruning/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41422 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:02:57.570588 torch-pruning-1.1.6/torch_pruning/pruner/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/pruner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:02:57.570588 torch-pruning-1.1.6/torch_pruning/pruner/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/pruner/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/pruner/algorithms/batchnorm_scale_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/pruner/algorithms/group_norm_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/pruner/algorithms/magnitude_based_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/pruner/algorithms/metapruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/pruner/algorithms/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/pruner/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:02:57.574589 torch-pruning-1.1.6/torch_pruning/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/utils/op_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-14 18:02:48.000000 torch-pruning-1.1.6/torch_pruning/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:02:57.570588 torch-pruning-1.1.6/torch_pruning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-04-14 18:02:57.000000 torch-pruning-1.1.6/torch_pruning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 18:02:57.000000 torch-pruning-1.1.6/torch_pruning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:02:57.000000 torch-pruning-1.1.6/torch_pruning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 18:02:57.000000 torch-pruning-1.1.6/torch_pruning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 18:02:57.000000 torch-pruning-1.1.6/torch_pruning.egg-info/top_level.txt
```

### Comparing `torch-pruning-1.1.5/LICENSE` & `torch-pruning-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/PKG-INFO` & `torch-pruning-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-pruning
-Version: 1.1.5
+Version: 1.1.6
 Summary: Structural Pruning for Model Acceleration.
 Home-page: https://github.com/VainF/Torch-Pruning
 Author: Gongfan Fang
 Author-email: gongfan@u.nus.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,30 +15,33 @@
 <div align="center"> <h1>Torch-Pruning <br> <h3>Towards Any Structural Pruning<h3> </h1> </div>
 <div align="center">
 <img src="assets/intro.png" width="50%">
 </div>
 
 <p align="center">
   <a href="https://github.com/VainF/Torch-Pruning/actions"><img src="https://img.shields.io/badge/tests-passing-9c27b0.svg" alt="Test Status"></a>
-  <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8.1%20%7C%202.0.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
+  <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8 %20%7C%201.12 %20%7C%202.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-4caf50.svg" alt="License"></a>
   <a href="https://pepy.tech/project/Torch-Pruning"><img src="https://pepy.tech/badge/Torch-Pruning?color=2196f3" alt="Downloads"></a>
-  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.4-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.6-3f51b5.svg" alt="Latest Version"></a>
   <a href="https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
   <a href="https://arxiv.org/abs/2301.12900" target="_blank"><img src="https://img.shields.io/badge/arXiv-2301.12900-009688.svg" alt="arXiv"></a>
 </p>
 
 
 [[中文README | README in Chinese]](README_CN.md)
 
 Torch-Pruning (TP) is a versatile library for Structural Network Pruning with the following features:
-* **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
-* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
+* **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *[LLaMA](https://github.com/horseee/LLaMA-Pruning), [Vision Transformers](benchmarks/prunability), [Yolov7, yolov8](benchmarks/prunability), FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
+* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **81/85=95.3%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
+
+### Update:
+* 2023.04.10 [**Structural Pruning for LLaMA**](https://github.com/horseee/LLaMA-Pruning)
 
 For more technical details, please refer to our CVPR'23 paper:
 > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/2301.12900)   
 > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong), [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://sites.google.com/site/sitexinchaowang/)   
 
 Please do not hesitate to open a [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue](https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems with the library or the paper. 
 
@@ -49,27 +52,31 @@
 - [x] Supported modules: Conv, Linear, Normalization, Transposed Conv, PReLU, Embedding, MultiheadAttention, nn.Parameters and [customized modules](tests/test_customized_layer.py).
 - [x] Supported operations: split, concatenation, skip connection, flatten, reshape, view, all element-wise ops, etc.
 - [x] [Low-level pruning functions](torch_pruning/pruner/function.py)
 - [x] [Benchmarks](benchmarks) and [tutorials](tutorials)
 - [x] A [resource list](practical_structural_pruning.md) for practical structrual pruning.
 
 ### **TODO List:**
-- [ ] A benchmark for [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility (**77/85=90.6%**, :heavy_check_mark:) and [timm](https://github.com/huggingface/pytorch-image-models) compatibility.
+- [ ] A strong baseline pruner with bags of tricks from existing methods.
+- [ ] A benchmark for [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility (**81/85=95.3%**, :heavy_check_mark:) and [timm](https://github.com/huggingface/pytorch-image-models) compatibility.
 - [ ] More Detectors (We are working on the pruning of YOLO series such as YOLOv7 :heavy_check_mark:, YOLOv8)
 - [ ] Pruning from Scratch / at Initialization.
-- [ ] Language, Speech and Generative Models.
+- [ ] Language (e.g., [LLaMA](https://github.com/horseee/LLaMA-Pruning):heavy_check_mark:), Speech and Generative Models.
 - [ ] More high-level pruners like [FisherPruner](https://arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243), etc.
 - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin Transformers, PoolFormers.
 - [ ] Block/Layer/Depth Pruning
 - [ ] Pruning benchmarks for CIFAR, ImageNet and COCO.
 
 ## Installation
+
+TP is compatible with Pytorch 1.x and 2.x. **PyTorch 1.12.1 is recommended!**
+
 ```bash
-pip install torch-pruning # v1.1.4
+pip install torch-pruning # v1.1.6
 ```
 or
 ```bash
 git clone https://github.com/VainF/Torch-Pruning.git # recommended
 ```
 
 ## Quickstart
@@ -295,7 +302,8 @@
 @article{fang2023depgraph,
   title={DepGraph: Towards Any Structural Pruning},
   author={Fang, Gongfan and Ma, Xinyin and Song, Mingli and Mi, Michael Bi and Wang, Xinchao},
   journal={The IEEE/CVF Conference on Computer Vision and Pattern Recognition},
   year={2023}
 }
 ```
+
```

#### html2text {}

```diff
@@ -1,33 +1,36 @@
-Metadata-Version: 2.1 Name: torch-pruning Version: 1.1.5 Summary: Structural
+Metadata-Version: 2.1 Name: torch-pruning Version: 1.1.6 Summary: Structural
 Pruning for Model Acceleration. Home-page: https://github.com/VainF/Torch-
 Pruning Author: Gongfan Fang Author-email: gongfan@u.nus.edu Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** Torch-Pruning
                      Towards Any Structural Pruning ******
                               [assets/intro.png]
 [Test_Status] [Tested_PyTorch_Versions] [License] [Downloads] [Latest_Version]
                             [Open_In_Colab] [arXiv]
 [[ä¸­æREADME | README in Chinese]](README_CN.md) Torch-Pruning (TP) is a
 versatile library for Structural Network Pruning with the following features: *
 **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide
-range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN,
-SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet,
-FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/
-tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through
-masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to
-physically remove coupled parameters (channels) from models. * **Reproducible
-[Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/
-prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of
-the models from Torchvision 0.13.1. Try this [Colab Demo](https://
-colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing)
-for quick start. For more technical details, please refer to our CVPR'23 paper:
-> [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
+range of neural networks, including *[LLaMA](https://github.com/horseee/LLaMA-
+Pruning), [Vision Transformers](benchmarks/prunability), [Yolov7, yolov8]
+(benchmarks/prunability), FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t,
+ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from
+[torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/
+pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning
+employs a (non-deep) graph algorithm called DepGraph to physically remove
+coupled parameters (channels) from models. * **Reproducible [Performance
+Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):**
+Currently, TP is able to prune approximately **81/85=95.3%** of the models from
+Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/
+drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start. ###
+Update: * 2023.04.10 [**Structural Pruning for LLaMA**](https://github.com/
+horseee/LLaMA-Pruning) For more technical details, please refer to our CVPR'23
+paper: > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
 2301.12900) > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://
 horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong),
 [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://
 sites.google.com/site/sitexinchaowang/) Please do not hesitate to open a
 [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue]
 (https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems
 with the library or the paper. ### **Features:** - [x] Structural (Channel)
@@ -42,27 +45,30 @@
 Graph Tracing and Dependency Modeling. - [x] Supported modules: Conv, Linear,
 Normalization, Transposed Conv, PReLU, Embedding, MultiheadAttention,
 nn.Parameters and [customized modules](tests/test_customized_layer.py). - [x]
 Supported operations: split, concatenation, skip connection, flatten, reshape,
 view, all element-wise ops, etc. - [x] [Low-level pruning functions]
 (torch_pruning/pruner/function.py) - [x] [Benchmarks](benchmarks) and
 [tutorials](tutorials) - [x] A [resource list](practical_structural_pruning.md)
-for practical structrual pruning. ### **TODO List:** - [ ] A benchmark for
+for practical structrual pruning. ### **TODO List:** - [ ] A strong baseline
+pruner with bags of tricks from existing methods. - [ ] A benchmark for
 [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility
-(**77/85=90.6%**, :heavy_check_mark:) and [timm](https://github.com/
+(**81/85=95.3%**, :heavy_check_mark:) and [timm](https://github.com/
 huggingface/pytorch-image-models) compatibility. - [ ] More Detectors (We are
 working on the pruning of YOLO series such as YOLOv7 :heavy_check_mark:,
-YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language, Speech
+YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language (e.g.,
+[LLaMA](https://github.com/horseee/LLaMA-Pruning):heavy_check_mark:), Speech
 and Generative Models. - [ ] More high-level pruners like [FisherPruner](https:
 //arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243),
 etc. - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin
 Transformers, PoolFormers. - [ ] Block/Layer/Depth Pruning - [ ] Pruning
-benchmarks for CIFAR, ImageNet and COCO. ## Installation ```bash pip install
-torch-pruning # v1.1.4 ``` or ```bash git clone https://github.com/VainF/Torch-
+benchmarks for CIFAR, ImageNet and COCO. ## Installation TP is compatible with
+Pytorch 1.x and 2.x. **PyTorch 1.12.1 is recommended!** ```bash pip install
+torch-pruning # v1.1.6 ``` or ```bash git clone https://github.com/VainF/Torch-
 Pruning.git # recommended ``` ## Quickstart Here we provide a quick start for
 Torch-Pruning. More explained details can be found in [tutorals](./tutorials/
 ) ### 0. How It Works In structural pruning, **a ``Group`` constitutes the
 minimal prunable unit within deep networks**. Each group typically comprises
 several interdependent parameters that must be removed simultaneously to
 maintain the integrity of the resulting structures. However, deep networks
 often present complex dependencies among parameters, making structural pruning
```

### Comparing `torch-pruning-1.1.5/README.md` & `torch-pruning-1.1.6/torch_pruning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,47 @@
+Metadata-Version: 2.1
+Name: torch-pruning
+Version: 1.1.6
+Summary: Structural Pruning for Model Acceleration.
+Home-page: https://github.com/VainF/Torch-Pruning
+Author: Gongfan Fang
+Author-email: gongfan@u.nus.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center"> <h1>Torch-Pruning <br> <h3>Towards Any Structural Pruning<h3> </h1> </div>
 <div align="center">
 <img src="assets/intro.png" width="50%">
 </div>
 
 <p align="center">
   <a href="https://github.com/VainF/Torch-Pruning/actions"><img src="https://img.shields.io/badge/tests-passing-9c27b0.svg" alt="Test Status"></a>
-  <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8.1%20%7C%202.0.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
+  <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8 %20%7C%201.12 %20%7C%202.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-4caf50.svg" alt="License"></a>
   <a href="https://pepy.tech/project/Torch-Pruning"><img src="https://pepy.tech/badge/Torch-Pruning?color=2196f3" alt="Downloads"></a>
-  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.4-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.6-3f51b5.svg" alt="Latest Version"></a>
   <a href="https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
   <a href="https://arxiv.org/abs/2301.12900" target="_blank"><img src="https://img.shields.io/badge/arXiv-2301.12900-009688.svg" alt="arXiv"></a>
 </p>
 
 
 [[中文README | README in Chinese]](README_CN.md)
 
 Torch-Pruning (TP) is a versatile library for Structural Network Pruning with the following features:
-* **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
-* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
+* **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *[LLaMA](https://github.com/horseee/LLaMA-Pruning), [Vision Transformers](benchmarks/prunability), [Yolov7, yolov8](benchmarks/prunability), FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
+* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **81/85=95.3%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
+
+### Update:
+* 2023.04.10 [**Structural Pruning for LLaMA**](https://github.com/horseee/LLaMA-Pruning)
 
 For more technical details, please refer to our CVPR'23 paper:
 > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/2301.12900)   
 > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong), [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://sites.google.com/site/sitexinchaowang/)   
 
 Please do not hesitate to open a [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue](https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems with the library or the paper. 
 
@@ -35,27 +52,31 @@
 - [x] Supported modules: Conv, Linear, Normalization, Transposed Conv, PReLU, Embedding, MultiheadAttention, nn.Parameters and [customized modules](tests/test_customized_layer.py).
 - [x] Supported operations: split, concatenation, skip connection, flatten, reshape, view, all element-wise ops, etc.
 - [x] [Low-level pruning functions](torch_pruning/pruner/function.py)
 - [x] [Benchmarks](benchmarks) and [tutorials](tutorials)
 - [x] A [resource list](practical_structural_pruning.md) for practical structrual pruning.
 
 ### **TODO List:**
-- [ ] A benchmark for [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility (**77/85=90.6%**, :heavy_check_mark:) and [timm](https://github.com/huggingface/pytorch-image-models) compatibility.
+- [ ] A strong baseline pruner with bags of tricks from existing methods.
+- [ ] A benchmark for [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility (**81/85=95.3%**, :heavy_check_mark:) and [timm](https://github.com/huggingface/pytorch-image-models) compatibility.
 - [ ] More Detectors (We are working on the pruning of YOLO series such as YOLOv7 :heavy_check_mark:, YOLOv8)
 - [ ] Pruning from Scratch / at Initialization.
-- [ ] Language, Speech and Generative Models.
+- [ ] Language (e.g., [LLaMA](https://github.com/horseee/LLaMA-Pruning):heavy_check_mark:), Speech and Generative Models.
 - [ ] More high-level pruners like [FisherPruner](https://arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243), etc.
 - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin Transformers, PoolFormers.
 - [ ] Block/Layer/Depth Pruning
 - [ ] Pruning benchmarks for CIFAR, ImageNet and COCO.
 
 ## Installation
+
+TP is compatible with Pytorch 1.x and 2.x. **PyTorch 1.12.1 is recommended!**
+
 ```bash
-pip install torch-pruning # v1.1.4
+pip install torch-pruning # v1.1.6
 ```
 or
 ```bash
 git clone https://github.com/VainF/Torch-Pruning.git # recommended
 ```
 
 ## Quickstart
@@ -281,7 +302,8 @@
 @article{fang2023depgraph,
   title={DepGraph: Towards Any Structural Pruning},
   author={Fang, Gongfan and Ma, Xinyin and Song, Mingli and Mi, Michael Bi and Wang, Xinchao},
   journal={The IEEE/CVF Conference on Computer Vision and Pattern Recognition},
   year={2023}
 }
 ```
+
```

#### html2text {}

```diff
@@ -1,27 +1,36 @@
+Metadata-Version: 2.1 Name: torch-pruning Version: 1.1.6 Summary: Structural
+Pruning for Model Acceleration. Home-page: https://github.com/VainF/Torch-
+Pruning Author: Gongfan Fang Author-email: gongfan@u.nus.edu Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE
                              ****** Torch-Pruning
                      Towards Any Structural Pruning ******
                               [assets/intro.png]
 [Test_Status] [Tested_PyTorch_Versions] [License] [Downloads] [Latest_Version]
                             [Open_In_Colab] [arXiv]
 [[ä¸­æREADME | README in Chinese]](README_CN.md) Torch-Pruning (TP) is a
 versatile library for Structural Network Pruning with the following features: *
 **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide
-range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN,
-SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet,
-FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/
-tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through
-masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to
-physically remove coupled parameters (channels) from models. * **Reproducible
-[Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/
-prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of
-the models from Torchvision 0.13.1. Try this [Colab Demo](https://
-colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing)
-for quick start. For more technical details, please refer to our CVPR'23 paper:
-> [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
+range of neural networks, including *[LLaMA](https://github.com/horseee/LLaMA-
+Pruning), [Vision Transformers](benchmarks/prunability), [Yolov7, yolov8]
+(benchmarks/prunability), FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t,
+ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from
+[torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/
+pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning
+employs a (non-deep) graph algorithm called DepGraph to physically remove
+coupled parameters (channels) from models. * **Reproducible [Performance
+Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):**
+Currently, TP is able to prune approximately **81/85=95.3%** of the models from
+Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/
+drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start. ###
+Update: * 2023.04.10 [**Structural Pruning for LLaMA**](https://github.com/
+horseee/LLaMA-Pruning) For more technical details, please refer to our CVPR'23
+paper: > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
 2301.12900) > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://
 horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong),
 [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://
 sites.google.com/site/sitexinchaowang/) Please do not hesitate to open a
 [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue]
 (https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems
 with the library or the paper. ### **Features:** - [x] Structural (Channel)
@@ -36,27 +45,30 @@
 Graph Tracing and Dependency Modeling. - [x] Supported modules: Conv, Linear,
 Normalization, Transposed Conv, PReLU, Embedding, MultiheadAttention,
 nn.Parameters and [customized modules](tests/test_customized_layer.py). - [x]
 Supported operations: split, concatenation, skip connection, flatten, reshape,
 view, all element-wise ops, etc. - [x] [Low-level pruning functions]
 (torch_pruning/pruner/function.py) - [x] [Benchmarks](benchmarks) and
 [tutorials](tutorials) - [x] A [resource list](practical_structural_pruning.md)
-for practical structrual pruning. ### **TODO List:** - [ ] A benchmark for
+for practical structrual pruning. ### **TODO List:** - [ ] A strong baseline
+pruner with bags of tricks from existing methods. - [ ] A benchmark for
 [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility
-(**77/85=90.6%**, :heavy_check_mark:) and [timm](https://github.com/
+(**81/85=95.3%**, :heavy_check_mark:) and [timm](https://github.com/
 huggingface/pytorch-image-models) compatibility. - [ ] More Detectors (We are
 working on the pruning of YOLO series such as YOLOv7 :heavy_check_mark:,
-YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language, Speech
+YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language (e.g.,
+[LLaMA](https://github.com/horseee/LLaMA-Pruning):heavy_check_mark:), Speech
 and Generative Models. - [ ] More high-level pruners like [FisherPruner](https:
 //arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243),
 etc. - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin
 Transformers, PoolFormers. - [ ] Block/Layer/Depth Pruning - [ ] Pruning
-benchmarks for CIFAR, ImageNet and COCO. ## Installation ```bash pip install
-torch-pruning # v1.1.4 ``` or ```bash git clone https://github.com/VainF/Torch-
+benchmarks for CIFAR, ImageNet and COCO. ## Installation TP is compatible with
+Pytorch 1.x and 2.x. **PyTorch 1.12.1 is recommended!** ```bash pip install
+torch-pruning # v1.1.6 ``` or ```bash git clone https://github.com/VainF/Torch-
 Pruning.git # recommended ``` ## Quickstart Here we provide a quick start for
 Torch-Pruning. More explained details can be found in [tutorals](./tutorials/
 ) ### 0. How It Works In structural pruning, **a ``Group`` constitutes the
 minimal prunable unit within deep networks**. Each group typically comprises
 several interdependent parameters that must be removed simultaneously to
 maintain the integrity of the resulting structures. However, deep networks
 often present complex dependencies among parameters, making structural pruning
```

### Comparing `torch-pruning-1.1.5/setup.py` & `torch-pruning-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="torch-pruning",
-    version="v1.1.5",
+    version="v1.1.6",
     author="Gongfan Fang",
     author_email="gongfan@u.nus.edu",
     description="Structural Pruning for Model Acceleration.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VainF/Torch-Pruning",
     packages=setuptools.find_packages(),
```

### Comparing `torch-pruning-1.1.5/tests/test_backward.py` & `torch-pruning-1.1.6/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_customized_layer.py` & `torch-pruning-1.1.6/tests/test_customized_layer.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_dependency_graph.py` & `torch-pruning-1.1.6/tests/test_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_dependency_lenet.py` & `torch-pruning-1.1.6/tests/test_dependency_lenet.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_fully_connected_layers.py` & `torch-pruning-1.1.6/tests/test_fully_connected_layers.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_importance.py` & `torch-pruning-1.1.6/tests/test_importance.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_interactive_pruner.py` & `torch-pruning-1.1.6/tests/test_interactive_pruner.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_multiple_inputs_and_outputs.py` & `torch-pruning-1.1.6/tests/test_multiple_inputs_and_outputs.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_pruner.py` & `torch-pruning-1.1.6/tests/test_pruner.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_pruning_fn.py` & `torch-pruning-1.1.6/tests/test_pruning_fn.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_reshape.py` & `torch-pruning-1.1.6/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/tests/test_unwrapped_parameters.py` & `torch-pruning-1.1.6/tests/test_unwrapped_parameters.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/torch_pruning/_helpers.py` & `torch-pruning-1.1.6/torch_pruning/_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/torch_pruning/dependency.py` & `torch-pruning-1.1.6/torch_pruning/dependency.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,28 @@
             return str(self.module)
         else:
             fmt = self._name
             if self.type != ops.OPTYPE.PARAMETER:
                 fmt += " ({})".format(str(self.module))
             return fmt
 
-    def add_input(self, node):
-        if node not in self.inputs:
+    def add_input(self, node, allow_dumplicated=False):
+        #if node not in self.inputs:
+        if allow_dumplicated is True:
             self.inputs.append(node)
+        else:
+            if node not in self.inputs:
+                self.inputs.append(node)
 
-    def add_output(self, node):
-        if node not in self.outputs:
+    def add_output(self, node, allow_dumplicated=False):
+        if allow_dumplicated is True:
             self.outputs.append(node)
+        else:
+            if node not in self.outputs:
+                self.outputs.append(node)
 
     def __repr__(self):
         return "<Node: ({})>".format(self.name)
 
     def __str__(self):
         return "<Node: ({})>".format(self.name)
 
@@ -80,29 +87,28 @@
 class Dependency(Edge):
     def __init__(
         self,
         trigger: typing.Callable,
         handler: typing.Callable,
         source: Node,
         target: Node,
-        index_mapping: typing.Callable = None,
     ):
         """Layer dependency (Edge of DepGraph) in structral neural network pruning. 
         Args:
             trigger (Callable): a pruning function that triggers this dependency
             handler (Callable): a pruning function that can fix the broken dependency
             source (Node): the source node pruned by the trigger function
             target (Node): the target node pruned by the handler function
             index_mapping (Callable): a callable function for index mapping
         """
         self.trigger = trigger
         self.handler = handler
         self.source = source
         self.target = target
-        self.index_mapping = index_mapping
+        self.index_mapping = [None, None]
 
     def __call__(self, idxs: list):
         self.handler.__self__.pruning_dim = self.target.pruning_dim
         result = self.handler(
             self.target.module,
             idxs,
         )
@@ -257,14 +263,15 @@
         self.REGISTERED_PRUNERS.update(_dummy_pruners)
         self.CUSTOMIZED_PRUNERS = {}
         self.IGNORED_LAYERS = []
 
         # cache
         self._in_channel_pruning_fn = set([p.prune_in_channels for p in self.REGISTERED_PRUNERS.values() if p is not None] + [p.prune_in_channels for p in self.CUSTOMIZED_PRUNERS.values() if p is not None])
         self._out_channel_pruning_fn = set([p.prune_out_channels for p in self.REGISTERED_PRUNERS.values() if p is not None] + [p.prune_out_channels for p in self.CUSTOMIZED_PRUNERS.values() if p is not None])
+        self._op_id = 0
 
     def build_dependency(
         self,
         model: torch.nn.Module,
         example_inputs: typing.Union[torch.Tensor, typing.Sequence],
         forward_fn: typing.Callable[[
             torch.nn.Module, typing.Union[torch.Tensor, typing.Sequence]], torch.Tensor] = None,
@@ -340,14 +347,17 @@
         # Build computational graph by tracing.
         self.module2node = self._trace(
             model, example_inputs, forward_fn, output_transform=output_transform
         )
 
         # Build dependency graph
         self._build_dependency(self.module2node)
+        
+        # Init Shape information
+        self._init_shape_information()
 
         # Update index mapping for torch.cat/split/chunck/...
         self.update_index_mapping()
         return self
 
     def register_customized_layer(
         self,
@@ -418,31 +428,33 @@
         group = Group()
         #  the user pruning operation
         root_node = self.module2node[module]
         group.add_dep(
             Dependency(pruning_fn, pruning_fn,
                        source=root_node, target=root_node), idxs
         )
-
         visited_node = set()
 
         def _fix_dependency_graph_non_recursive(dep, idxs):
             processing_stack = [(dep, idxs)]
             while len(processing_stack) > 0:
                 dep, idxs = processing_stack.pop(-1)
                 node, fn = dep.target, dep.handler
                 visited_node.add(node)
-
+                #print(dep)
+                #print(node.dependencies)
                 for new_dep in node.dependencies:
                     if new_dep.is_triggered_by(fn):
-                        new_indices = (
-                            new_dep.index_mapping(idxs)
-                            if new_dep.index_mapping is not None
-                            else idxs
-                        )
+                        new_indices = idxs
+                        for mapping in new_dep.index_mapping:
+                            if mapping is not None:
+                                new_indices = mapping(new_indices)
+                                #print(new_dep, new_dep.index_mapping)
+                                #print(len(new_indices), new_indices)
+                        #print()
                         if len(new_indices) == 0:
                             continue
                         if (new_dep.target in visited_node) and group.has_pruning_op(
                             new_dep, new_indices
                         ):
                             continue
                         else:
@@ -459,15 +471,15 @@
             merged_group.add_and_merge(dep, idxs)
         merged_group._DG = self
         return merged_group
 
     def get_all_groups(self, ignored_layers=[], root_module_types=(ops.TORCH_CONV, ops.TORCH_LINEAR)):
         visited_layers = []
         ignored_layers = ignored_layers+self.IGNORED_LAYERS
-        for m in self.module2node.keys():
+        for m in list(self.module2node.keys()):
             if m in ignored_layers:
                 continue
 
             if not isinstance(m, tuple(root_module_types)):
                 continue
 
             pruner = self.get_pruner_of_module(m)
@@ -521,33 +533,38 @@
         p.pruning_dim = pruning_dim
         if p is None:
             return None
         return p.get_in_channels(module)
 
     def _infer_out_channels_recursively(self, node: Node):
         """ infer the number of output channels recursively
-        """
+        """     
         ch = self.get_out_channels(node)
         if ch is None:
             ch = 0
             for in_node in node.inputs:
                 if node.type == ops.OPTYPE.CONCAT:
                     sub_ch = self._infer_out_channels_recursively(in_node)
                     if sub_ch is None:
                         return None
                     ch += sub_ch
                 else:
-                    ch = self._infer_out_channels_recursively(in_node)
+                    if in_node.type == ops.OPTYPE.SPLIT and in_node.module.split_sizes is not None:
+                        for i, split_out_node in enumerate(in_node.outputs):
+                            if split_out_node == node:
+                                ch = in_node.module.split_sizes[i]
+                    else:
+                        ch = self._infer_out_channels_recursively(in_node)
             if ch == 0:
                 return None
         return ch
 
     def _infer_in_channels_recursively(self, node: Node):
         """ infer the number of input channels recursively
-        """
+        """         
         ch = self.get_in_channels(node)
         if ch is None:
             ch = 0
             for out_node in node.outputs:
                 if node.type == ops.OPTYPE.SPLIT:
                     sub_ch = self._infer_in_channels_recursively(out_node)
                     if sub_ch is None:
@@ -675,29 +692,34 @@
 
             # 1. link grad_fns and modules
             if module is None:  # a new module
                 if not hasattr(grad_fn, "name"):
                     # we treat all unknwon modules as element-wise operations by default,
                     # which does not modify the #dimension/#channel of features.
                     # If you have some customized layers, please register it with DependencyGraph.register_customized_layer
-                    module = ops._ElementWiseOp("Unknown")
+                    module = ops._ElementWiseOp(self._op_id ,"Unknown")
+                    self._op_id+=1
                     if self.verbose:
                         warnings.warn(
                             "[Warning] Unknown operation {} encountered, which will be handled as an element-wise op".format(
                                 str(grad_fn))
                         )
                 elif "catbackward" in grad_fn.name().lower():
-                    module = ops._ConcatOp()
+                    module = ops._ConcatOp(self._op_id)
+                    self._op_id+=1
                 elif "split" in grad_fn.name().lower():
-                    module = ops._SplitOp()
+                    module = ops._SplitOp(self._op_id)
+                    self._op_id+=1
                 elif "view" in grad_fn.name().lower() or 'reshape' in grad_fn.name().lower():
-                    module = ops._ReshapeOp()
+                    module = ops._ReshapeOp(self._op_id)
+                    self._op_id+=1
                 else:
                     # treate other ops as element-wise ones, like Add, Sub, Div, Mul.
-                    module = ops._ElementWiseOp(grad_fn.name())
+                    module = ops._ElementWiseOp(self._op_id, grad_fn.name())
+                    self._op_id+=1
                 gradfn2module[grad_fn] = module
 
             # 2. link modules and nodes
             if module not in module2node:
                 node = Node(
                     module=module,
                     grad_fn=grad_fn,
@@ -711,18 +733,20 @@
             else:
                 node = module2node[module]
             return node
 
         # non-recursive construction of computational graph
         processing_stack = [grad_fn_root]
         visited = set()
+        visited_as_output_node = set()
         while len(processing_stack) > 0:
             grad_fn = processing_stack.pop(-1)
             if grad_fn in visited:
                 continue
+            
             node = create_node_if_not_exists(grad_fn=grad_fn)
             if hasattr(grad_fn, "next_functions"):
                 for f in grad_fn.next_functions:
                     if f[0] is not None:
                         if (
                             hasattr(f[0], "name")
                             and "accumulategrad" in f[0].name().lower()
@@ -732,37 +756,84 @@
                                 if f[0].variable is p:
                                     is_unwrapped_param = True
                                     gradfn2module[f[0]] = p
                                     self._module2name[p] = "UnwrappedParameter_{} ({})".format(j, p.shape)
                             if not is_unwrapped_param:
                                 continue
                         input_node = create_node_if_not_exists(f[0])
-                        node.add_input(input_node)
-                        input_node.add_output(node)
+
+                        #allow_dumplicated = False
+
+                        # TODO: support duplicated concat/split like torch.cat([x, x], dim=1)
+                        # The following implementation is can achieve this but will introduce some bugs. 
+                        # will be fixed in the future version
+                        #if node.type == ops.OPTYPE.CONCAT:
+                        #    allow_dumplicated = (node not in visited_as_output_node)
+                        #    node.add_input(input_node, allow_dumplicated=allow_dumplicated)
+                        #    input_node.add_output(node, allow_dumplicated=allow_dumplicated)
+                        #    print(node, node.inputs)
+                        #elif input_node.type == ops.OPTYPE.SPLIT:
+                        #    allow_dumplicated = (node not in visited_as_output_node)
+                        #    node.add_input(input_node, allow_dumplicated=allow_dumplicated)
+                        #    input_node.add_output(node, allow_dumplicated=allow_dumplicated)
+                        #else:
+                        node.add_input(input_node, allow_dumplicated=False)
+                        input_node.add_output(node, allow_dumplicated=False)
+
                         processing_stack.append(f[0])
             visited.add(grad_fn)
+            visited_as_output_node.add(node)
         
         for (param, dim) in self.unwrapped_parameters:
             module2node[param].pruning_dim = dim
         return module2node
 
     def update_index_mapping(self):
         """ update all index mapping after pruning
-        """
+        """       
+        # update index mapping
         for module, node in self.module2node.items():
-            #if node.type == ops.OPTYPE.LINEAR:
-                # for Conv-Flatten-Linear (e.g., VGG)
-            #    self._update_flatten_index_mapping(node)
-            if node.type == ops.OPTYPE.RESHAPE:
-                self._update_reshape_index_mapping(node)
             if node.type == ops.OPTYPE.CONCAT:
                 self._update_concat_index_mapping(node)
             if node.type == ops.OPTYPE.SPLIT:
                 self._update_split_index_mapping(node)
+            if node.type == ops.OPTYPE.RESHAPE:
+                self._update_reshape_index_mapping(node)
 
+    def _init_shape_information(self):
+        for module, node in self.module2node.items():
+            
+            if node.type == ops.OPTYPE.SPLIT:
+                grad_fn = node.grad_fn
+                if hasattr(grad_fn, '_saved_self_sizes'):
+                    if hasattr(grad_fn, '_saved_split_sizes') and hasattr(grad_fn, '_saved_dim') :
+                        if grad_fn._saved_dim != 1:
+                            continue
+                        chs = list(grad_fn._saved_split_sizes)
+                        node.module.split_sizes = chs
+                    elif hasattr(grad_fn, '_saved_split_size') and hasattr(grad_fn, '_saved_dim'):
+                        if grad_fn._saved_dim != 1:
+                            continue
+                        chs = [grad_fn._saved_split_size for _ in range(len(node.outputs))]
+                        node.module.split_sizes = chs
+                    offsets = [0]
+                    for i in range(len(chs)):
+                        offsets.append(offsets[i] + chs[i])
+                    node.module.offsets = offsets
+                else: # legency version
+                    chs = []
+                    for n in node.outputs:
+                        chs.append(self._infer_in_channels_recursively(n))
+                    offsets = [0]
+                    for ch in chs:
+                        if ch is None: continue
+                        offsets.append(offsets[-1] + ch)
+                    node.module.split_sizes = chs
+                    node.module.offsets = offsets
+                                                
     def _update_flatten_index_mapping(self, fc_node: Node):
         if fc_node.type != ops.OPTYPE.LINEAR:
             return
         fc_in_features = fc_node.module.in_features
         feature_channels = 0
         for n in fc_node.inputs:
             feature_channels = self._infer_out_channels_recursively(n)
@@ -773,20 +844,20 @@
         ):  # the first layer: https://github.com/VainF/Torch-Pruning/issues/21
             return
         stride = fc_in_features // feature_channels
         if stride > 1 and fc_in_features % feature_channels == 0:
             for in_node in fc_node.inputs:
                 for dep in fc_node.dependencies:
                     if dep.target == in_node:
-                        dep.index_mapping = _helpers._FlattenIndexMapping(
+                        dep.index_mapping[0] = _helpers._FlattenIndexMapping(
                             stride=stride, reverse=True
                         )
                 for dep in in_node.dependencies:
                     if dep.target == fc_node:
-                        dep.index_mapping = _helpers._FlattenIndexMapping(
+                        dep.index_mapping[0] = _helpers._FlattenIndexMapping(
                             stride=stride, reverse=False
                         )
 
     def _update_reshape_index_mapping(self, reshape_node: Node):
         
         # Only Supports 2D/4D tensors
         # TODO: Better support for reshape/view/flatten
@@ -819,87 +890,120 @@
         
         # Flatten
         #print(reshape_node.grad_fn._saved_self_sizes, in_channels, out_channels)
         if out_channels > in_channels:
              for in_node in reshape_node.inputs:
                 for dep in reshape_node.dependencies:
                     if dep.target == in_node:
-                        dep.index_mapping = _helpers._FlattenIndexMapping(
+                        dep.index_mapping[0] = _helpers._FlattenIndexMapping(
                             stride=out_channels // in_channels, reverse=True
                         )
 
                 for dep in in_node.dependencies:
                     if dep.target == reshape_node:
-                        dep.index_mapping = _helpers._FlattenIndexMapping(
+                        dep.index_mapping[0] = _helpers._FlattenIndexMapping(
                             stride=out_channels // in_channels, reverse=False
                         )
         else: # 1D -> 2D
             for out_node in reshape_node.outputs:
                 for dep in reshape_node.dependencies:
                     if dep.target == out_node:
-                        dep.index_mapping = _helpers._FlattenIndexMapping(
+                        dep.index_mapping[0] = _helpers._FlattenIndexMapping(
                             stride=in_channels // out_channels, reverse=True
                         )
 
                 for dep in out_node.dependencies:
                     if dep.target == reshape_node:
-                        dep.index_mapping = _helpers._FlattenIndexMapping(
+                        dep.index_mapping[0] = _helpers._FlattenIndexMapping(
                             stride=in_channels // out_channels, reverse=False
                         )
         #print(in_channels, out_channels)
         #print(reshape_node.grad_fn._saved_self_sizes)
         #print('------')
         
     def _update_concat_index_mapping(self, cat_node: Node):
         if cat_node.type != ops.OPTYPE.CONCAT:
             return
-        chs = []
-        for n in cat_node.inputs:
-            chs.append(self._infer_out_channels_recursively(n))
+        
+        if cat_node.module.concat_sizes is not None:
+            chs = cat_node.module.concat_sizes
+        else:
+            chs = []
+            for n in cat_node.inputs:
+                chs.append(self.infer_channels(n, cat_node))
+            cat_node.module.concat_sizes = chs
+            
         offsets = [0]
         for ch in chs:
             offsets.append(offsets[-1] + ch)
         cat_node.module.offsets = offsets
 
         # no transform if the concat dim is different from the feature dim
+        # TODO: make the messy for loop more efficient
+        addressed_dep = []
         for i, in_node in enumerate(cat_node.inputs):
             for dep in cat_node.dependencies:
+                if any((dep is d) for d in addressed_dep): continue
                 if dep.target == in_node:
                     if cat_node.enable_index_mapping:
-                        dep.index_mapping = _helpers._ConcatIndexMapping(
+                        dep.index_mapping[1] = _helpers._ConcatIndexMapping(
                             offset=offsets[i: i + 2], reverse=True
                         )
-
+                        addressed_dep.append(dep)
+                        break
+                        
+        addressed_dep = []
+        for i, in_node in enumerate(cat_node.inputs):
             for dep in in_node.dependencies:
+                if any((dep is d) for d in addressed_dep): continue
                 if dep.target == cat_node:
                     if cat_node.enable_index_mapping:
-                        dep.index_mapping = _helpers._ConcatIndexMapping(
+                        dep.index_mapping[1] = _helpers._ConcatIndexMapping(
                             offset=offsets[i: i + 2], reverse=False
                         )
-
+                        addressed_dep.append(dep)
+                        break
+    
+        
     def _update_split_index_mapping(self, split_node: Node):
         if split_node.type != ops.OPTYPE.SPLIT:
             return
-        chs = []
-        for n in split_node.outputs:
-            chs.append(self._infer_in_channels_recursively(n))
-
-        offsets = [0]
-        for ch in chs:
-            if ch is None: return
-            offsets.append(offsets[-1] + ch)
-        split_node.module.offsets = offsets
 
+        offsets = split_node.module.offsets
+        if offsets is None:
+            return
+        addressed_dep = []
         for i, out_node in enumerate(split_node.outputs):
             for dep in split_node.dependencies:
+                if any((dep is d) for d in addressed_dep): continue
                 if dep.target == out_node:
                     if split_node.enable_index_mapping:
-                        dep.index_mapping = _helpers._SplitIndexMapping(
+                        dep.index_mapping[0] = (_helpers._SplitIndexMapping(
                             offset=offsets[i: i + 2], reverse=False
-                        )
-
+                        ))
+                        addressed_dep.append(dep)
+                        break
+        
+        addressed_dep = []
+        for i, out_node in enumerate(split_node.outputs):
             for dep in out_node.dependencies:
                 if dep.target == split_node:
+                    if any((dep is d) for d in addressed_dep): continue
                     if split_node.enable_index_mapping:
-                        dep.index_mapping = _helpers._SplitIndexMapping(
+                        dep.index_mapping[0] = (_helpers._SplitIndexMapping(
                             offset=offsets[i: i + 2], reverse=True
-                        )
+                        ))
+                        addressed_dep.append(dep)
+                        break
+
+    def infer_channels(self, node_1, node_2):
+        if node_1.type == ops.OPTYPE.SPLIT:
+            for i, n in enumerate(node_1.outputs):
+                if n == node_2:
+                    return node_1.module.split_sizes[i]
+        return self._infer_out_channels_recursively(node_1)
+
+        
+
+
+
+
```

### Comparing `torch-pruning-1.1.5/torch_pruning/importance.py` & `torch-pruning-1.1.6/torch_pruning/importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             raise NotImplementedError
         return group_imp
 
     @torch.no_grad()
     def __call__(self, group, ch_groups=1):
         group_imp = []
         #Get group norm
-        #print(group)
+        #print(group.details())
         for dep, idxs in group:
             idxs.sort()
             layer = dep.target.module
             prune_fn = dep.handler
             # Conv out_channels
             if prune_fn in [
                 function.prune_conv_out_channels,
```

### Comparing `torch-pruning-1.1.5/torch_pruning/pruner/algorithms/batchnorm_scale_pruner.py` & `torch-pruning-1.1.6/torch_pruning/pruner/algorithms/batchnorm_scale_pruner.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/torch_pruning/pruner/algorithms/group_norm_pruner.py` & `torch-pruning-1.1.6/torch_pruning/pruner/algorithms/group_norm_pruner.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/torch_pruning/pruner/algorithms/metapruner.py` & `torch-pruning-1.1.6/torch_pruning/pruner/algorithms/metapruner.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
                 n_pruned = current_channels - int(
                     self.layer_init_out_ch[module] *
                     (1 - target_sparsity)
                 )
 
                 if self.round_to:
                     n_pruned = n_pruned - (n_pruned % self.round_to)
-
+    
                 if n_pruned <= 0:
                     continue
                 if ch_groups > 1:
                     imp = imp[:len(imp)//ch_groups]
                 imp_argsort = torch.argsort(imp)
                 pruning_idxs = imp_argsort[:(n_pruned//ch_groups)]
                 if ch_groups > 1:
@@ -251,15 +251,15 @@
         n_pruned = len(imp) - int(
             self.initial_total_channels *
             (1 - target_sparsity)
         )
         if n_pruned <= 0:
             return
         topk_imp, _ = torch.topk(imp, k=n_pruned, largest=False)
-
+        
         # global pruning through thresholding
         thres = topk_imp[-1]
         for group, ch_groups, imp in global_importance:
             module = group[0][0].target.module
             pruning_fn = group[0][0].handler
             pruning_indices = (imp <= thres).nonzero().view(-1)
             if ch_groups > 1:
```

### Comparing `torch-pruning-1.1.5/torch_pruning/pruner/function.py` & `torch-pruning-1.1.6/torch_pruning/pruner/function.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/torch_pruning/utils/op_counter.py` & `torch-pruning-1.1.6/torch_pruning/utils/op_counter.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/torch_pruning/utils/utils.py` & `torch-pruning-1.1.6/torch_pruning/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.5/torch_pruning.egg-info/PKG-INFO` & `torch-pruning-1.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,33 @@
-Metadata-Version: 2.1
-Name: torch-pruning
-Version: 1.1.5
-Summary: Structural Pruning for Model Acceleration.
-Home-page: https://github.com/VainF/Torch-Pruning
-Author: Gongfan Fang
-Author-email: gongfan@u.nus.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center"> <h1>Torch-Pruning <br> <h3>Towards Any Structural Pruning<h3> </h1> </div>
 <div align="center">
 <img src="assets/intro.png" width="50%">
 </div>
 
 <p align="center">
   <a href="https://github.com/VainF/Torch-Pruning/actions"><img src="https://img.shields.io/badge/tests-passing-9c27b0.svg" alt="Test Status"></a>
-  <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8.1%20%7C%202.0.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
+  <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8 %20%7C%201.12 %20%7C%202.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-4caf50.svg" alt="License"></a>
   <a href="https://pepy.tech/project/Torch-Pruning"><img src="https://pepy.tech/badge/Torch-Pruning?color=2196f3" alt="Downloads"></a>
-  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.4-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.6-3f51b5.svg" alt="Latest Version"></a>
   <a href="https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
   <a href="https://arxiv.org/abs/2301.12900" target="_blank"><img src="https://img.shields.io/badge/arXiv-2301.12900-009688.svg" alt="arXiv"></a>
 </p>
 
 
 [[中文README | README in Chinese]](README_CN.md)
 
 Torch-Pruning (TP) is a versatile library for Structural Network Pruning with the following features:
-* **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
-* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
+* **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *[LLaMA](https://github.com/horseee/LLaMA-Pruning), [Vision Transformers](benchmarks/prunability), [Yolov7, yolov8](benchmarks/prunability), FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
+* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **81/85=95.3%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
+
+### Update:
+* 2023.04.10 [**Structural Pruning for LLaMA**](https://github.com/horseee/LLaMA-Pruning)
 
 For more technical details, please refer to our CVPR'23 paper:
 > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/2301.12900)   
 > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong), [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://sites.google.com/site/sitexinchaowang/)   
 
 Please do not hesitate to open a [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue](https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems with the library or the paper. 
 
@@ -49,27 +38,31 @@
 - [x] Supported modules: Conv, Linear, Normalization, Transposed Conv, PReLU, Embedding, MultiheadAttention, nn.Parameters and [customized modules](tests/test_customized_layer.py).
 - [x] Supported operations: split, concatenation, skip connection, flatten, reshape, view, all element-wise ops, etc.
 - [x] [Low-level pruning functions](torch_pruning/pruner/function.py)
 - [x] [Benchmarks](benchmarks) and [tutorials](tutorials)
 - [x] A [resource list](practical_structural_pruning.md) for practical structrual pruning.
 
 ### **TODO List:**
-- [ ] A benchmark for [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility (**77/85=90.6%**, :heavy_check_mark:) and [timm](https://github.com/huggingface/pytorch-image-models) compatibility.
+- [ ] A strong baseline pruner with bags of tricks from existing methods.
+- [ ] A benchmark for [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility (**81/85=95.3%**, :heavy_check_mark:) and [timm](https://github.com/huggingface/pytorch-image-models) compatibility.
 - [ ] More Detectors (We are working on the pruning of YOLO series such as YOLOv7 :heavy_check_mark:, YOLOv8)
 - [ ] Pruning from Scratch / at Initialization.
-- [ ] Language, Speech and Generative Models.
+- [ ] Language (e.g., [LLaMA](https://github.com/horseee/LLaMA-Pruning):heavy_check_mark:), Speech and Generative Models.
 - [ ] More high-level pruners like [FisherPruner](https://arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243), etc.
 - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin Transformers, PoolFormers.
 - [ ] Block/Layer/Depth Pruning
 - [ ] Pruning benchmarks for CIFAR, ImageNet and COCO.
 
 ## Installation
+
+TP is compatible with Pytorch 1.x and 2.x. **PyTorch 1.12.1 is recommended!**
+
 ```bash
-pip install torch-pruning # v1.1.4
+pip install torch-pruning # v1.1.6
 ```
 or
 ```bash
 git clone https://github.com/VainF/Torch-Pruning.git # recommended
 ```
 
 ## Quickstart
@@ -295,7 +288,8 @@
 @article{fang2023depgraph,
   title={DepGraph: Towards Any Structural Pruning},
   author={Fang, Gongfan and Ma, Xinyin and Song, Mingli and Mi, Michael Bi and Wang, Xinchao},
   journal={The IEEE/CVF Conference on Computer Vision and Pattern Recognition},
   year={2023}
 }
 ```
+
```

#### html2text {}

```diff
@@ -1,33 +1,30 @@
-Metadata-Version: 2.1 Name: torch-pruning Version: 1.1.5 Summary: Structural
-Pruning for Model Acceleration. Home-page: https://github.com/VainF/Torch-
-Pruning Author: Gongfan Fang Author-email: gongfan@u.nus.edu Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE
                              ****** Torch-Pruning
                      Towards Any Structural Pruning ******
                               [assets/intro.png]
 [Test_Status] [Tested_PyTorch_Versions] [License] [Downloads] [Latest_Version]
                             [Open_In_Colab] [arXiv]
 [[ä¸­æREADME | README in Chinese]](README_CN.md) Torch-Pruning (TP) is a
 versatile library for Structural Network Pruning with the following features: *
 **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide
-range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN,
-SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet,
-FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/
-tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through
-masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to
-physically remove coupled parameters (channels) from models. * **Reproducible
-[Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/
-prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of
-the models from Torchvision 0.13.1. Try this [Colab Demo](https://
-colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing)
-for quick start. For more technical details, please refer to our CVPR'23 paper:
-> [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
+range of neural networks, including *[LLaMA](https://github.com/horseee/LLaMA-
+Pruning), [Vision Transformers](benchmarks/prunability), [Yolov7, yolov8]
+(benchmarks/prunability), FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t,
+ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from
+[torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/
+pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning
+employs a (non-deep) graph algorithm called DepGraph to physically remove
+coupled parameters (channels) from models. * **Reproducible [Performance
+Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):**
+Currently, TP is able to prune approximately **81/85=95.3%** of the models from
+Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/
+drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start. ###
+Update: * 2023.04.10 [**Structural Pruning for LLaMA**](https://github.com/
+horseee/LLaMA-Pruning) For more technical details, please refer to our CVPR'23
+paper: > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
 2301.12900) > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://
 horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong),
 [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://
 sites.google.com/site/sitexinchaowang/) Please do not hesitate to open a
 [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue]
 (https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems
 with the library or the paper. ### **Features:** - [x] Structural (Channel)
@@ -42,27 +39,30 @@
 Graph Tracing and Dependency Modeling. - [x] Supported modules: Conv, Linear,
 Normalization, Transposed Conv, PReLU, Embedding, MultiheadAttention,
 nn.Parameters and [customized modules](tests/test_customized_layer.py). - [x]
 Supported operations: split, concatenation, skip connection, flatten, reshape,
 view, all element-wise ops, etc. - [x] [Low-level pruning functions]
 (torch_pruning/pruner/function.py) - [x] [Benchmarks](benchmarks) and
 [tutorials](tutorials) - [x] A [resource list](practical_structural_pruning.md)
-for practical structrual pruning. ### **TODO List:** - [ ] A benchmark for
+for practical structrual pruning. ### **TODO List:** - [ ] A strong baseline
+pruner with bags of tricks from existing methods. - [ ] A benchmark for
 [Torchvision](https://pytorch.org/vision/stable/models.html) compatibility
-(**77/85=90.6%**, :heavy_check_mark:) and [timm](https://github.com/
+(**81/85=95.3%**, :heavy_check_mark:) and [timm](https://github.com/
 huggingface/pytorch-image-models) compatibility. - [ ] More Detectors (We are
 working on the pruning of YOLO series such as YOLOv7 :heavy_check_mark:,
-YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language, Speech
+YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language (e.g.,
+[LLaMA](https://github.com/horseee/LLaMA-Pruning):heavy_check_mark:), Speech
 and Generative Models. - [ ] More high-level pruners like [FisherPruner](https:
 //arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243),
 etc. - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin
 Transformers, PoolFormers. - [ ] Block/Layer/Depth Pruning - [ ] Pruning
-benchmarks for CIFAR, ImageNet and COCO. ## Installation ```bash pip install
-torch-pruning # v1.1.4 ``` or ```bash git clone https://github.com/VainF/Torch-
+benchmarks for CIFAR, ImageNet and COCO. ## Installation TP is compatible with
+Pytorch 1.x and 2.x. **PyTorch 1.12.1 is recommended!** ```bash pip install
+torch-pruning # v1.1.6 ``` or ```bash git clone https://github.com/VainF/Torch-
 Pruning.git # recommended ``` ## Quickstart Here we provide a quick start for
 Torch-Pruning. More explained details can be found in [tutorals](./tutorials/
 ) ### 0. How It Works In structural pruning, **a ``Group`` constitutes the
 minimal prunable unit within deep networks**. Each group typically comprises
 several interdependent parameters that must be removed simultaneously to
 maintain the integrity of the resulting structures. However, deep networks
 often present complex dependencies among parameters, making structural pruning
```

### Comparing `torch-pruning-1.1.5/torch_pruning.egg-info/SOURCES.txt` & `torch-pruning-1.1.6/torch_pruning.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 LICENSE
 README.md
 setup.py
 tests/test_backward.py
+tests/test_concat.py
+tests/test_concat_split.py
 tests/test_customized_layer.py
 tests/test_dependency_graph.py
 tests/test_dependency_lenet.py
 tests/test_fully_connected_layers.py
 tests/test_importance.py
 tests/test_interactive_pruner.py
 tests/test_multiple_inputs_and_outputs.py
 tests/test_pruner.py
 tests/test_pruning_fn.py
 tests/test_reshape.py
+tests/test_split.py
 tests/test_unwrapped_parameters.py
 torch_pruning/__init__.py
 torch_pruning/_helpers.py
 torch_pruning/dependency.py
 torch_pruning/importance.py
 torch_pruning/ops.py
 torch_pruning.egg-info/PKG-INFO
```

