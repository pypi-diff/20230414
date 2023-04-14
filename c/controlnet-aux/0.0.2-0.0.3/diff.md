# Comparing `tmp/controlnet_aux-0.0.2.tar.gz` & `tmp/controlnet_aux-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlnet_aux-0.0.2.tar", last modified: Tue Apr 11 17:36:28 2023, max compression
+gzip compressed data, was "controlnet_aux-0.0.3.tar", last modified: Fri Apr 14 17:21:27 2023, max compression
```

## Comparing `controlnet_aux-0.0.2.tar` & `controlnet_aux-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,103 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1574 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      670 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/README.md
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8604 2023-04-11 17:33:24.000000 controlnet_aux-0.0.2/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.839497 controlnet_aux-0.0.2/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      189 2023-04-11 17:23:50.000000 controlnet_aux-0.0.2/src/controlnet_aux/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/canny/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      502 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/canny/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/hed/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7586 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/hed/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2272 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/api.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/blocks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/dpt_depth.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/midas_net.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/midas_net_custom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2026 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    24134 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3156 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10883 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/body.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3389 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/hand.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8387 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/util.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3742 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1574 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1212 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      107 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2958 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2054 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/README.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8636 2023-04-14 17:12:42.000000 controlnet_aux-0.0.3/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      394 2023-04-14 15:41:51.000000 controlnet_aux-0.0.3/src/controlnet_aux/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/canny/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      547 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/canny/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/hed/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7726 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/hed/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/lineart/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5057 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/lineart/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/lineart_anime/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7574 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/lineart_anime/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2618 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/api.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/blocks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/dpt_depth.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/midas_net.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    24134 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2517 2023-04-14 17:15:46.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      597 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/NNET.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:17.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2980 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/baseline.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:28.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10480 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/decoder.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:38.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2428 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5993 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       89 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3000 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3113 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9187 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4760 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2690 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2294 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4549 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3350 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12093 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    26514 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    59925 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2833 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15009 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      707 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       22 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2730 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5821 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2932 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      843 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4905 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1737 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6632 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1060 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5703 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/submodules.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:29.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7570 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/losses.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6725 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5233 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10883 2023-04-14 09:59:01.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/body.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15314 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/face.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6530 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/hand.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7934 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/pidi/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2952 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/pidi/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    21794 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/pidi/model.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/shuffle/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3468 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/shuffle/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3742 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2958 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4410 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      120 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/top_level.txt
```

### Comparing `controlnet_aux-0.0.2/setup.py` & `controlnet_aux-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,16 @@
     "importlib_metadata",
     "opencv-python",
     "matplotlib",
     "scipy",
     "huggingface_hub",
     "einops",
     "timm",
-    "torchvision"
+    "torchvision",
+    "scikit-image"
 ]
 
 # this is a lookup table with items like:
 #
 # tokenizers: "huggingface-hub==0.8.0"
 # packaging: "packaging"
 #
@@ -159,34 +160,32 @@
         print(f"updating {target}")
         with open(target, "w", encoding="utf-8", newline="\n") as f:
             f.write("\n".join(content))
 
 
 extras = {}
 
-
-extras = {}
-
 install_requires = [
     deps["torch"],
     deps["importlib_metadata"],
     deps["huggingface_hub"],
     deps["scipy"],
     deps["opencv-python"],
     deps["filelock"],
     deps["numpy"],
     deps["Pillow"],
     deps["einops"],
     deps["torchvision"],
     deps["timm"],
+    deps["scikit-image"],
 ]
 
 setup(
     name="controlnet_aux",
-    version="0.0.2",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.0.3",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Human Pose",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
```

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/hed/__init__.py` & `controlnet_aux-0.0.3/src/controlnet_aux/hed/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,19 @@
 
 class HEDdetector:
     def __init__(self, netNetwork):
         self.netNetwork = netNetwork.eval()
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
-        filename = filename or "annotator/ckpts/network-bsds500.pth"
+        if pretrained_model_or_path == "lllyasviel/ControlNet":
+            filename = filename or "annotator/ckpts/network-bsds500.pth"
+        else:
+            filename = filename or "network-bsds500.pth"
+
         model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         netNetwork = Network(model_path)
 
         return cls(netNetwork)
 
     def __call__(self, input_image, detect_resolution=512, image_resolution=512, return_pil=True, scribble=False):
```

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/__init__.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,42 @@
 from huggingface_hub import hf_hub_download
 from einops import rearrange
 from .api import MiDaSInference
 from ..util import HWC3
 
 class MidasDetector:
     def __init__(self, model_type="dpt_hybrid", model_path=None):
-        self.model = MiDaSInference(model_type=model_type, model_path=model_path).cuda()
+        self.model = MiDaSInference(model_type=model_type, model_path=model_path)
+        if torch.cuda.is_available():
+            self.model = self.model.cuda()
 
         
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, model_type="dpt_hybrid", filename=None, cache_dir=None):
-        filename = filename or "annotator/ckpts/dpt_hybrid-midas-501f0c75.pt"
+        if pretrained_model_or_path == "lllyasviel/ControlNet":
+            filename = filename or "annotator/ckpts/dpt_hybrid-midas-501f0c75.pt"
+        else:
+            filename = filename or "dpt_hybrid-midas-501f0c75.pt"
+
         model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
         return cls(model_type=model_type, model_path=model_path)
         
     def __call__(self, input_image, a=np.pi * 2.0, bg_th=0.1):
         
         input_type = "np"
         if isinstance(input_image, Image.Image):
             input_image = np.array(input_image)
             input_type = "pil"
             
         input_image = HWC3(input_image)
         image_depth = input_image
         with torch.no_grad():
-            image_depth = torch.from_numpy(image_depth).float().cuda()
+            image_depth = torch.from_numpy(image_depth).float()
+            if torch.cuda.is_available():
+                image_depth = image_depth.cuda()
             image_depth = image_depth / 127.5 - 1.0
             image_depth = rearrange(image_depth, 'h w c -> 1 c h w')
             depth = self.model(image_depth)[0]
 
             depth_pt = depth.clone()
             depth_pt -= torch.min(depth_pt)
             depth_pt /= torch.max(depth_pt)
@@ -48,10 +56,11 @@
             y[depth_pt < bg_th] = 0
             normal = np.stack([x, y, z], axis=2)
             normal /= np.sum(normal ** 2.0, axis=2, keepdims=True) ** 0.5
             normal_image = (normal * 127.5 + 127.5).clip(0, 255).astype(np.uint8)
         
         if input_type == "pil":
             depth_image = Image.fromarray(depth_image)
+            depth_image = depth_image.convert("RGB")
             normal_image = Image.fromarray(normal_image)
         
-        return depth_image, normal_image
+        return depth_image
```

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/api.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/blocks.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/dpt_depth.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/midas_net.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/midas_net_custom.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/transforms.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/vit.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/midas/utils.py` & `controlnet_aux-0.0.3/src/controlnet_aux/midas/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/mlsd/__init__.py` & `controlnet_aux-0.0.3/src/controlnet_aux/mlsd/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 
 class MLSDdetector:
     def __init__(self, model):
         self.model = model.eval()
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
-        filename = filename or "annotator/ckpts/mlsd_large_512_fp32.pth"
+        if pretrained_model_or_path == "lllyasviel/ControlNet":
+            filename = filename or "annotator/ckpts/mlsd_large_512_fp32.pth"
+        else:
+            filename = filename or "mlsd_large_512_fp32.pth"
+
         model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         model = MobileV2_MLSD_Large()
         model.load_state_dict(torch.load(model_path), strict=True)
 
         return cls(model)
```

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/mlsd/utils.py` & `controlnet_aux-0.0.3/src/controlnet_aux/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/open_pose/body.py` & `controlnet_aux-0.0.3/src/controlnet_aux/open_pose/body.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/open_pose/model.py` & `controlnet_aux-0.0.3/src/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.2/src/controlnet_aux/util.py` & `controlnet_aux-0.0.3/src/controlnet_aux/util.py`

 * *Files identical despite different names*

