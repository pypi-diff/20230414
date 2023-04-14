# Comparing `tmp/returnn-1.20230413.93323.tar.gz` & `tmp/returnn-1.20230414.110554.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230413.93323.tar", last modified: Thu Apr 13 07:48:21 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230414.110554.tar", last modified: Fri Apr 14 09:19:10 2023, max compression
```

## Comparing `returnn-1.20230413.93323.tar` & `returnn-1.20230414.110554.tar`

### file list

```diff
@@ -1,413 +1,420 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 07:48:01.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27146 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    94908 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   154798 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151442 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   585656 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28438 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144505 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 09:19:09.000000 returnn-1.20230414.110554/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 09:18:51.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-14 09:18:53.000000 returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29013 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95121 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154892 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151442 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   585656 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30653 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 09:19:09.000000 returnn-1.20230414.110554/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-14 09:19:09.000000 returnn-1.20230414.110554/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:19:09.000000 returnn-1.20230414.110554/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 09:19:09.000000 returnn-1.20230414.110554/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:19:10.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-14 09:18:50.000000 returnn-1.20230414.110554/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230413.93323/.gitignore` & `returnn-1.20230414.110554/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/.gitmodules` & `returnn-1.20230414.110554/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/CHANGELOG.md` & `returnn-1.20230414.110554/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/CODEOWNERS` & `returnn-1.20230414.110554/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/CONTRIBUTING.md` & `returnn-1.20230414.110554/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/LICENSE` & `returnn-1.20230414.110554/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/MANIFEST.in` & `returnn-1.20230414.110554/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/PKG-INFO` & `returnn-1.20230414.110554/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230413.93323
+Version: 1.20230414.110554
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230413.93323/README.rst` & `returnn-1.20230414.110554/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/__init__.py` & `returnn-1.20230414.110554/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/12AX.cluster_map` & `returnn-1.20230414.110554/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-fwd.config` & `returnn-1.20230414.110554/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-horovod-mpi.py` & `returnn-1.20230414.110554/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230414.110554/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-hyper-param-tuning.config` & `returnn-1.20230414.110554/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-iter-dataset.py` & `returnn-1.20230414.110554/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-list-devices.py` & `returnn-1.20230414.110554/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-lua-torch-layer.config` & `returnn-1.20230414.110554/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230414.110554/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-returnn-as-framework.py` & `returnn-1.20230414.110554/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-rf.config` & `returnn-1.20230414.110554/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-rhn-enwik8.config` & `returnn-1.20230414.110554/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-sprint-interface.py` & `returnn-1.20230414.110554/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-att-copy.config` & `returnn-1.20230414.110554/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-attention.config` & `returnn-1.20230414.110554/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230414.110554/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230414.110554/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-enc-dec.config` & `returnn-1.20230414.110554/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230414.110554/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230414.110554/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230414.110554/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230414.110554/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230414.110554/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230414.110554/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230414.110554/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230414.110554/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230414.110554/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230414.110554/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-rec-self-att.config` & `returnn-1.20230414.110554/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230414.110554/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230414.110554/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230414.110554/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-torch.config` & `returnn-1.20230414.110554/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230414.110554/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/demo.sh` & `returnn-1.20230414.110554/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230414.110554/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230414.110554/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230414.110554/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/README.txt` & `returnn-1.20230414.110554/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/config_demo` & `returnn-1.20230414.110554/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230414.110554/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/config_real` & `returnn-1.20230414.110554/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230414.110554/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/decode.py` & `returnn-1.20230414.110554/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230414.110554/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230414.110554/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230414.110554/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230414.110554/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230414.110554/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230414.110554/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230414.110554/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230414.110554/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230414.110554/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230414.110554/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/__init__.py` & `returnn-1.20230414.110554/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/__main__.py` & `returnn-1.20230414.110554/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/__old_mod_loader__.py` & `returnn-1.20230414.110554/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/__setup__.py` & `returnn-1.20230414.110554/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/config.py` & `returnn-1.20230414.110554/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/audio.py` & `returnn-1.20230414.110554/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/basic.py` & `returnn-1.20230414.110554/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/bundle_file.py` & `returnn-1.20230414.110554/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/cached.py` & `returnn-1.20230414.110554/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/cached2.py` & `returnn-1.20230414.110554/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/generating.py` & `returnn-1.20230414.110554/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/hdf.py` & `returnn-1.20230414.110554/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/lm.py` & `returnn-1.20230414.110554/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/map.py` & `returnn-1.20230414.110554/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/meta.py` & `returnn-1.20230414.110554/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/multi_proc.py` & `returnn-1.20230414.110554/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/normalization_data.py` & `returnn-1.20230414.110554/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/numpy_dump.py` & `returnn-1.20230414.110554/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/raw_wav.py` & `returnn-1.20230414.110554/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/sprint.py` & `returnn-1.20230414.110554/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/stereo.py` & `returnn-1.20230414.110554/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230414.110554/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/datasets/util/vocabulary.py` & `returnn-1.20230414.110554/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/engine/base.py` & `returnn-1.20230414.110554/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/engine/batch.py` & `returnn-1.20230414.110554/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230414.110554/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230414.110554/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230414.110554/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230414.110554/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/graph_editor/edit.py` & `returnn-1.20230414.110554/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230414.110554/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/graph_editor/select.py` & `returnn-1.20230414.110554/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230414.110554/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/graph_editor/transform.py` & `returnn-1.20230414.110554/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/extern/graph_editor/util.py` & `returnn-1.20230414.110554/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/__init__.py` & `returnn-1.20230414.110554/returnn/frontend/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,28 +10,35 @@
 
 # Not necessarily all here, but the most common ones.
 # (Take PyTorch `torch.nn` as a reference.)
 
 # Some most come first here when others directly use it,
 # e.g. `rf.Module` as a baseclass.
 from .module import *
+from .state import *
 
+# Now the rest, in alphabetical order.
 from .array_ import *
+from .attention import *
 from .cond import *
 from .const import *
+from .container import *
 from .dims import *
 from .dropout import *
 from .dtype import *
+from .gradient import *
 from .linear import *
 from .loss import *
 from .math_ import *
 from .matmul import *
+from .normalization import *
 from .parameter import *
 from .rand import *
 from .reduce import *
 from .run_ctx import *
-from .state import *
 from .types import *
 
+# Modules not in the main namespace but in sub namespaces.
 from . import init
 
+# And some functions from the internal backend API.
 from ._backend import select_backend_torch, select_backend_returnn_layers_tf
```

### Comparing `returnn-1.20230413.93323/returnn/frontend/_backend.py` & `returnn-1.20230414.110554/returnn/frontend/_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -238,14 +238,22 @@
         res = tensor.copy_template()
         res.dtype = dtype
         # noinspection PyProtectedMember
         res.raw_tensor = tensor._raw_backend.cast_raw(tensor.raw_tensor, dtype)
         return res
 
     @staticmethod
+    def stop_gradient(tensor: Tensor) -> Tensor:
+        """
+        :param tensor:
+        :return: tensor with stopped gradient
+        """
+        raise NotImplementedError
+
+    @staticmethod
     def merge_dims(
         source: Tensor,
         *,
         dims: Sequence[Dim],
         out_dim: Optional[Dim] = None,
     ) -> Tuple[Tensor, Dim]:
         """
@@ -275,14 +283,43 @@
         :param dims:
         :param pad_to_multiples:
         :param pad_value:
         :return: source with axis replaced by dims
         """
         raise NotImplementedError
 
+    @staticmethod
+    def split(source: Tensor, *, axis: Dim, out_dims: Sequence[Dim]) -> Tuple[Tensor, ...]:
+        """
+        Split the input on the specified axis (by default feature).
+        Basically a wrapper around tf.split.
+
+        :param source: {..., axis}
+        :param axis: some static axis
+        :param out_dims: list of dims where sum(out_dims) == axis
+        :return: tuple of tensors, same amount as out_dims,
+            with the same shape as source, but with the specified axis replaced by the out_dims
+        """
+        raise NotImplementedError
+
+    @staticmethod
+    def cum_concat_step(source: Tensor, *, prev_accum: Tensor, axis: Dim, out_spatial_dim: Dim) -> Tensor:
+        """
+        Concatenates all previous frames over a time-axis.
+        See RETURNN :class:`CumConcatLayer` for details.
+
+        :param source: same dims as prev_accum except for the accum axis
+        :param prev_accum: previous accumulated tensor, shape {..., axis}
+        :param axis: the axis to accumulate over
+        :param out_spatial_dim: the spatial dim of the output will be this dim. like axis+1.
+        :return: accumulated. accumulated shape {..., out_spatial_dim},
+            same shape as prev_accum with axis replaced by out_spatial_dim.
+        """
+        raise NotImplementedError
+
     # Restrict the possible activation function names,
     # to not get unexpected behavior,
     # or unwanted incompatibilities.
     _AllowedActivationFuncs = {
         "exp",
         "expm1",
         "log",
@@ -426,27 +463,35 @@
         Rather, the logic to create placeholders should be done elsewhere.
         """
         raise Exception("create_placeholder not supported by backend")
 
     @staticmethod
     def create_parameter_raw(tensor: rf.Parameter) -> T:
         """
-        :return: parameter
+        :return: parameter (by default trainable)
         """
         raise NotImplementedError
 
     @staticmethod
     def set_parameter_initial_value(param: rf.Parameter, value: Union[None, Tensor, rf.RawTensorTypes]) -> None:
         """
         :param param: parameter
         :param value: initial value
         """
         raise NotImplementedError
 
     @staticmethod
+    def set_parameter_trainable(param: rf.Parameter, trainable: bool) -> None:
+        """
+        :param param: parameter
+        :param trainable: whether the parameter should be trainable
+        """
+        raise NotImplementedError
+
+    @staticmethod
     def runtime_sanity_checks(tensor: Tensor) -> Any:
         """
         Checks whether the tensor.raw_tensor is consistent with the tensor metadata.
 
         In graph-based frameworks (TF graph), we return some operation here.
         In eager frameworks, we would not return anything but instead directly perform the checks.
         """
@@ -627,14 +672,16 @@
         :param source:
         :param in_dim:
         :param out_dim:
         :return: source with in_dim replaced by out_dim.
         """
         # This default implementation works fine as long as the backend
         # does not have special treatments of Tensor and dim tags itself (like TF net dict backend).
+        if not out_dim.is_dim_known():
+            out_dim.copy_from(in_dim)
         out = source.copy_template_replace_dim_tag(axis=source.get_axis_from_description(in_dim), new_dim_tag=out_dim)
         out.raw_tensor = source.raw_tensor
         return out
 
     _AllowedReduceModes = {"sum", "max", "min", "mean", "logsumexp", "any", "all", "argmin", "argmax"}
 
     @staticmethod
```

### Comparing `returnn-1.20230413.93323/returnn/frontend/_numpy_backend.py` & `returnn-1.20230414.110554/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/_utils.py` & `returnn-1.20230414.110554/returnn/frontend/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,10 +117,26 @@
         else:
             raise TypeError(f"invalid type for allow_broadcast_all_sources: {type(allow_broadcast_all_sources)}")
     if dim_order:
         all_dims.sort(key=lambda d: dim_order.index(d) if d in dim_order else len(dim_order))
     if res_dtype is None:
         res_dtype = src_dtype
     out = Tensor(name, dims=all_dims, dtype=res_dtype)
+    out.feature_dim = res_feature_dim(a, b)
     a = a.copy_compatible_to(out, check_dtype=False, check_sparse=False)
     b = b.copy_compatible_to(out, check_dtype=False, check_sparse=False)
     return out, a, b
+
+
+def res_feature_dim(a: Tensor, b: Tensor) -> Optional[Dim]:
+    """
+    :param a:
+    :param b:
+    :return: feature dim if consistent or None
+    """
+    if a.feature_dim and not b.feature_dim:
+        return a.feature_dim
+    if b.feature_dim and not a.feature_dim:
+        return b.feature_dim
+    if a.feature_dim and b.feature_dim and a.feature_dim == b.feature_dim:
+        return a.feature_dim
+    return None
```

### Comparing `returnn-1.20230413.93323/returnn/frontend/array_.py` & `returnn-1.20230414.110554/returnn/frontend/array_.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,26 @@
 from returnn.tensor import Tensor, Dim
 import returnn.frontend as rf
 from ._backend import Backend, global_backend, get_backend_by_raw_tensor_type
 from .types import RawTensorTypes
 
 T = TypeVar("T")
 
-__all__ = ["convert_to_tensor", "constant", "cast", "merge_dims", "split_dims", "masked_select", "pack", "gather"]
+__all__ = [
+    "convert_to_tensor",
+    "constant",
+    "cast",
+    "merge_dims",
+    "split_dims",
+    "split",
+    "cum_concat_step",
+    "masked_select",
+    "pack",
+    "gather",
+]
 
 
 def convert_to_tensor(
     value: Union[Tensor, T, RawTensorTypes],
     *,
     dims: Sequence[Dim] = None,
     dtype: Optional[str] = None,
@@ -150,14 +161,52 @@
     """
     # noinspection PyProtectedMember
     return source._raw_backend.split_dims(
         source, axis=axis, dims=dims, pad_to_multiples=pad_to_multiples, pad_value=pad_value
     )
 
 
+def split(source: Tensor, *, axis: Dim, out_dims: Sequence[Dim]) -> Tuple[Tensor, ...]:
+    """
+    Split the input on the specified axis (by default feature).
+    Basically a wrapper around tf.split.
+
+    :param source: {..., axis}
+    :param axis: some static axis
+    :param out_dims: list of dims where sum(out_dims) == axis
+    :return: tuple of tensors, same amount as out_dims,
+        with the same shape as source, but with the specified axis replaced by the out_dims
+    """
+    # noinspection PyProtectedMember
+    return source._raw_backend.split(source, axis=axis, out_dims=out_dims)
+
+
+def cum_concat_step(
+    source: Tensor, *, prev_accum: Tensor, axis: Dim, out_spatial_dim: Optional[Dim] = None
+) -> Tuple[Tensor, Dim]:
+    """
+    Concatenates all previous frames over a time-axis.
+    See RETURNN :class:`CumConcatLayer` for details.
+
+    :param source: same dims as prev_accum except for the accum axis
+    :param prev_accum: previous accumulated tensor, shape {..., axis}
+    :param axis: the axis to accumulate over
+    :param out_spatial_dim: if given, the spatial dim of the output will be this dim. axis+1.
+    :return: (accumulated, out_spatial_dim). accumulated shape {..., out_spatial_dim},
+        same shape as prev_accum with axis replaced by out_spatial_dim.
+    """
+    if not out_spatial_dim:
+        out_spatial_dim = axis + 1
+    # noinspection PyProtectedMember
+    return (
+        source._raw_backend.cum_concat_step(source, prev_accum=prev_accum, axis=axis, out_spatial_dim=out_spatial_dim),
+        out_spatial_dim,
+    )
+
+
 def masked_select(
     tensor: Tensor, *, mask: Tensor, dims: Sequence[Dim], out_dim: Optional[Dim] = None
 ) -> Tuple[Tensor, Dim]:
     """
     :param tensor:
     :param mask:
     :param dims: the order of the dims defines the format. those dims should be exactly the dims of the mask.
```

### Comparing `returnn-1.20230413.93323/returnn/frontend/cond.py` & `returnn-1.20230414.110554/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/const.py` & `returnn-1.20230414.110554/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/dims.py` & `returnn-1.20230414.110554/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/dropout.py` & `returnn-1.20230414.110554/returnn/frontend/dropout.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
     Applies dropout.
 
     Dropout will only be applied during training (unless you set on_forward=True).
 
     When dropout is applied, the output will be scaled by 1/dropout.
 
-    :param nn.Tensor source:
+    :param source:
     :param drop_prob: 0.0 means to apply no dropout. 100% would mask everything.
         For every value in the tensor, the probability of it being dropped
         is drawn independently given this probability.
         The broadcasted axes are those not specified in ``axis``.
     :param axis: axis to apply dropout on. multiple axes can be specified.
         This defines the set of axes where the dropout mask is not broadcasted to.
         (RETURNN also has the ``noise_shape`` option but the ``axis`` option provides the same functionality.)
@@ -38,16 +38,25 @@
     keep_prob = 1.0 - drop_prob
     if isinstance(axis, Dim):
         noise_dims = (axis,)
     else:
         noise_dims = axis
     if not set(noise_dims).issubset(source.dims):
         raise ValueError(f"dropout axis {axis} not in source {source}")
+
+    if isinstance(keep_prob, (float, int)) and not 0 < keep_prob <= 1:
+        raise ValueError("keep_prob must be a scalar tensor or a float in the " "range (0, 1], got %g" % keep_prob)
+
+    # Do nothing if we know keep_prob == 1
+    if isinstance(keep_prob, (float, int)) and keep_prob == 1:
+        return source
+
     if on_forward:
         return _dropout(source, keep_prob, noise_dims=noise_dims)
+
     return rf.cond(
         pred=rf.get_run_ctx().train_flag,
         true_fn=lambda: _dropout(source, keep_prob, noise_dims=noise_dims),
         false_fn=lambda: source,
     )
 
 
@@ -67,21 +76,14 @@
 
     :param x:
     :param keep_prob:
     :param noise_dims: other dims would broadcast
     :param seed: passed on to :func:`random` for the mask
     :param bool apply_correction_factor:
     """
-    assert isinstance(x, Tensor)
-    if isinstance(keep_prob, (float, int)) and not 0 < keep_prob <= 1:
-        raise ValueError("keep_prob must be a scalar tensor or a float in the " "range (0, 1], got %g" % keep_prob)
-    # Do nothing if we know keep_prob == 1
-    if isinstance(keep_prob, (float, int)) and keep_prob == 1:
-        return x
-
     # uniform [keep_prob, 1.0 + keep_prob)
     random_tensor = keep_prob + rf.random_uniform(dims=noise_dims, seed=seed, dtype=x.dtype, minval=0.0, maxval=1.0)
     # 0. if [keep_prob, 1.0) and 1. if [1.0, 1.0 + keep_prob)
     binary_tensor = rf.floor(random_tensor)
     if apply_correction_factor:
         # Apply the factor on binary_tensor, because that is potentially smaller than x.
         # Use `*(1/p)` instead of `/p` because that might be faster in some cases.
```

### Comparing `returnn-1.20230413.93323/returnn/frontend/dtype.py` & `returnn-1.20230414.110554/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/init.py` & `returnn-1.20230414.110554/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/linear.py` & `returnn-1.20230414.110554/returnn/frontend/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __call__(self, source: Tensor) -> Tensor:
         if not isinstance(source, Tensor):
             raise TypeError(f"{self}: source must be a Tensor but got {type(source)}")
         if self.in_dim not in source.dims_set:
             raise ValueError(f"{self}: input {source} does not have in_dim {self.in_dim}")
         out = rf.matmul(source, self.weight, reduce=self.in_dim)
+        out.feature_dim = self.out_dim
         if self.with_bias:
             out += self.bias
         return out
 
 
 class Embedding(rf.Module):
     """
```

### Comparing `returnn-1.20230413.93323/returnn/frontend/loss.py` & `returnn-1.20230414.110554/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/math_.py` & `returnn-1.20230414.110554/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/matmul.py` & `returnn-1.20230414.110554/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/module.py` & `returnn-1.20230414.110554/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/parameter.py` & `returnn-1.20230414.110554/returnn/frontend/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,22 @@
             dtype=dtype or (rf.get_default_float_dtype() if not sparse_dim else rf.get_default_array_index_dtype()),
             sparse_dim=sparse_dim,
         )
         if raw_tensor is not None:
             self.raw_tensor = raw_tensor
         else:
             self.raw_tensor = _global_backend.create_parameter_raw(self)
-        if auxiliary and trainable is None:
-            trainable = False
-        self._trainable = trainable
+        self._trainable = None  # type: Optional[bool]
         self._auxiliary = auxiliary
         self._non_critical_for_restore = non_critical_for_restore
         self._weight_decay = weight_decay
         self._initial = None  # type: Optional[rf.init.ParamInitType]
-        self.initial = initial
+
+        self.trainable = trainable  # use setter
+        self.initial = initial  # use setter
 
     def __copy__(self):
         # Should return new copy. https://github.com/rwth-i6/returnn_common/pull/215#issuecomment-1269651064
         # Note that the values are *not* copied, but rather it will use the same param init scheme.
         res = type(self)(
             dims=self.dims,
             dtype=self.dtype,
@@ -131,16 +131,19 @@
 
     @property
     def trainable(self) -> Optional[bool]:
         """trainable"""
         return self._trainable
 
     @trainable.setter
-    def trainable(self, value: Optional[bool]):
-        self._trainable = value
+    def trainable(self, trainable: Optional[bool]):
+        self._trainable = trainable
+        if trainable is None:
+            trainable = not self.auxiliary
+        self._raw_backend.set_parameter_trainable(self, trainable)
 
     @property
     def auxiliary(self) -> bool:
         """auxiliary"""
         return self._auxiliary
 
     @auxiliary.setter
```

### Comparing `returnn-1.20230413.93323/returnn/frontend/rand.py` & `returnn-1.20230414.110554/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/reduce.py` & `returnn-1.20230414.110554/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/run_ctx.py` & `returnn-1.20230414.110554/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/state.py` & `returnn-1.20230414.110554/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/frontend/types.py` & `returnn-1.20230414.110554/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/import_/common.py` & `returnn-1.20230414.110554/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/import_/git.py` & `returnn-1.20230414.110554/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/import_/import_.py` & `returnn-1.20230414.110554/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/learning_rate_control.py` & `returnn-1.20230414.110554/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/log.py` & `returnn-1.20230414.110554/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/native_op.cpp` & `returnn-1.20230414.110554/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/native_op.py` & `returnn-1.20230414.110554/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/pretrain.py` & `returnn-1.20230414.110554/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/sprint/cache.py` & `returnn-1.20230414.110554/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/sprint/control.py` & `returnn-1.20230414.110554/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/sprint/error_signals.py` & `returnn-1.20230414.110554/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/sprint/extern_interface.py` & `returnn-1.20230414.110554/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/sprint/interface.py` & `returnn-1.20230414.110554/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tensor/_dim_extra.py` & `returnn-1.20230414.110554/returnn/tensor/_dim_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1474,14 +1474,21 @@
                     if base.batch and base.batch == self.batch and base.control_flow_ctx == self.control_flow_ctx:
                         self.dyn_size_ext = base.dyn_size_ext.copy_template(name="%s:size" % self_base.description)
                 elif base.is_batch_dim():
                     self.dyn_size_ext = _t.Tensor(
                         name="%s:batch" % self_base.description, shape=(), dtype="int32", batch_dim_axis=None
                     )
 
+    def copy_from(self: Dim, other: Dim):
+        """define"""
+        self.size = other.size
+        self.capacity = other.capacity
+        self.dyn_size_ext = other.dyn_size_ext
+        self.derive_from(other)
+
     @classmethod
     def get_existing_tag_from_collection(cls, other, tags, is_equal_opts=None):
         """
         :param Dim other:
         :param list[Dim]|tuple[Dim]|set[Dim] tags:
         :param dict[str]|None is_equal_opts: passed to Dim.is_equal
         :rtype: Dim|None
```

### Comparing `returnn-1.20230413.93323/returnn/tensor/_tensor_extra.py` & `returnn-1.20230414.110554/returnn/tensor/_tensor_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -2664,21 +2664,23 @@
         else:
             assert self.batch_dim_axis == 0
             assert self.time_dim_axis == 1
             return backend.sequence_mask_raw(dyn_seq_len, batch_major=True)
 
     def get_sequence_mask_broadcast(self: Tensor, axis=None) -> _t.RawTensorType:
         """
-        :param int|None axis:
+        :param Dim|int|None axis:
         :return: seq mask of shape ((batch,time) or (time,batch)) + (1,)s for remaining dims
           if BT or TB major, and axis is T or None.
           In general compatible to placeholder, i.e. same ndim, with broadcast dims.
           We assert here that the axis is dynamic (:func:`is_axis_dynamic`), i.e. we have the size.
         :rtype: tf.Tensor
         """
+        if isinstance(axis, Dim):
+            axis = self.get_axis_from_description(axis)
         if axis is None:
             assert self.time_dim_axis is not None
             axis = self.time_dim_axis
         if axis < 0:
             assert axis + self.batch_ndim > 0
             axis += self.batch_ndim
         assert 0 <= axis < self.batch_ndim
```

### Comparing `returnn-1.20230413.93323/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230414.110554/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230414.110554/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230414.110554/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tensor/dim.py` & `returnn-1.20230414.110554/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tensor/marked_dim.py` & `returnn-1.20230414.110554/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tensor/tensor.py` & `returnn-1.20230414.110554/returnn/tensor/tensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,22 +39,23 @@
 class Tensor(_TensorMixin, _TensorOpOverloadsMixin, Generic[RawTensorType]):
     """
     Represents a tensor, in a frame-agnostic way. See the module docstring.
     """
 
     size_dtype = "int32"
 
-    __slots__ = ("name", "_dims", "dtype", "sparse_dim", "_feature_dim_axis", "_raw_tensor", "version", "_extra")
+    __slots__ = ("name", "_dims", "dtype", "sparse_dim", "_raw_tensor", "_feature_dim_axis", "version", "_extra")
 
     name: str
     _dims: Tuple[Dim, ...]
     dtype: str
     sparse_dim: Optional[Dim]
-    _feature_dim_axis: Optional[Union[int, NotSpecified]]
     _raw_tensor: Optional[RawTensorType]
+
+    _feature_dim_axis: Optional[Union[int, NotSpecified]]  # https://github.com/rwth-i6/returnn/issues/1273
     version: int
     _extra: Optional[_TensorExtra]
 
     def __init__(
         self,
         name: str,
         dims: Optional[Sequence[Dim]] = None,
@@ -163,17 +164,28 @@
         """
         self._raw_tensor = value
         self.sanity_check(assume_complete=False)
 
     @property
     def feature_dim(self) -> Optional[Dim]:
         """
-        :return: self.dims[self.feature_dim_axis] or None
+        :return: self.dims[self.feature_dim_axis] or None.
+            See https://github.com/rwth-i6/returnn/issues/1273 for some discussion.
         """
         # first fast paths
         if self._feature_dim_axis is None:
             return None
         if isinstance(self._feature_dim_axis, int):
             return self._dims[self._feature_dim_axis]
         if self.feature_dim_axis is None:
             return None
         return self._dims[self.feature_dim_axis]
+
+    @feature_dim.setter
+    def feature_dim(self, value: Optional[Dim]):
+        """
+        :param value:
+        """
+        if value is None:
+            self._feature_dim_axis = None
+            return
+        self._feature_dim_axis = self.get_axis_from_description(value, allow_int=False)
```

### Comparing `returnn-1.20230413.93323/returnn/tensor/tensor_dict.py` & `returnn-1.20230414.110554/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/compat.py` & `returnn-1.20230414.110554/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/data_pipeline.py` & `returnn-1.20230414.110554/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/distributed.py` & `returnn-1.20230414.110554/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/engine.py` & `returnn-1.20230414.110554/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230414.110554/returnn/tf/frontend_layers/_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,19 @@
 
     @staticmethod
     def cast(tensor: Tensor, dtype: str) -> Tensor:
         """cast"""
         return rfl.make_layer({"class": "cast", "from": tensor, "dtype": dtype}, name="cast")
 
     @staticmethod
+    def stop_gradient(tensor: Tensor) -> Tensor:
+        """stop grad"""
+        return rfl.make_layer({"class": "scaled_grad", "from": tensor, "scale": 0}, name="stop_gradient")
+
+    @staticmethod
     def merge_dims(
         source: Tensor,
         *,
         dims: Sequence[Dim],
         out_dim: Optional[Dim] = None,
     ) -> Tuple[Tensor, Dim]:
         """
@@ -171,14 +176,46 @@
             args["pad_value"] = pad_value
         args = {key: value for (key, value) in args.items() if value is not NotSpecified}
         return rfl.make_layer(
             {"class": "split_dims", "from": source, "axis": axis, "dims": dims, **args}, name="split_dims"
         )
 
     @staticmethod
+    def split(source: Tensor, *, axis: Dim, out_dims: Sequence[Dim]) -> Tuple[Tensor, ...]:
+        """split"""
+        res = rfl.make_layer({"class": "split", "from": source, "axis": axis, "out_dims": out_dims}, name="split")
+
+        src_axis_int = source.get_axis_from_description(axis)
+        # noinspection PyProtectedMember
+        return tuple(
+            rfl._get_sub_layer(
+                layer=res,
+                name=str(i),
+                data=source.copy_template_replace_dim_tag(
+                    axis=src_axis_int, new_dim_tag=dim, name=f"{source.name}/split:{i}:{dim.description}"
+                ),
+            )
+            for i, dim in enumerate(out_dims)
+        )
+
+    @staticmethod
+    def cum_concat_step(source: Tensor, *, prev_accum: Tensor, axis: Dim, out_spatial_dim: Dim) -> Tensor:
+        """cum_concat_step"""
+        return rfl.make_layer(
+            {
+                "class": "cum_concat",
+                "from": source,
+                "state": {"state": prev_accum},
+                "out_spatial_dim": out_spatial_dim,
+                "axis": axis,
+            },
+            name="cum_concat",
+        )
+
+    @staticmethod
     def activation(tensor: Tensor, func: str) -> Tensor:
         """activation"""
         return rfl.make_layer({"class": "activation", "activation": func, "from": tensor}, name=func)
 
     @staticmethod
     def activation_raw(raw_tensor: Layer, func: str) -> Layer:
         """activation"""
@@ -266,14 +303,23 @@
                 param.raw_tensor.debug_layer.output.placeholder = var
             else:
                 var = param.raw_tensor.debug_layer.output.placeholder
                 assert isinstance(var, tf.Variable)
                 var.assign(value_tf)
 
     @staticmethod
+    def set_parameter_trainable(param: rf.Parameter, trainable: bool) -> None:
+        """set parameter trainable"""
+        if trainable:
+            # pop it, as it's the default
+            param.raw_tensor.layer_dict.pop("trainable", None)
+        else:
+            param.raw_tensor.layer_dict["trainable"] = False
+
+    @staticmethod
     def convert_to_tensor(
         value: Union[Tensor, Layer, RawTensorTypes],
         *,
         dims: Sequence[Dim],
         dtype: str,
         sparse_dim: Optional[Dim] = None,
         name: Optional[str] = None,
@@ -392,18 +438,19 @@
         """
         try:
             ReturnnLayersBackend._random_journal_replay_enabled = True
             ReturnnLayersBackend._random_journal_replay_idx = 0
             ReturnnLayersBackend._random_journal = journal
             yield
         finally:
-            assert ReturnnLayersBackend._random_journal_replay_idx == len(journal)
+            final_replay_idx = ReturnnLayersBackend._random_journal_replay_idx
             ReturnnLayersBackend._random_journal_replay_enabled = False
             ReturnnLayersBackend._random_journal_replay_idx = 0
             ReturnnLayersBackend._random_journal = None
+        assert final_replay_idx == len(journal)
 
     _random_journal_replay_enabled = False
     _random_journal_replay_idx = 0
     _random_journal = None  # type: Optional[Sequence[Dict[str, Any]]]
 
     @staticmethod
     def random(
@@ -426,15 +473,21 @@
     ) -> Tensor:
         """random"""
         if ReturnnLayersBackend._random_journal_replay_enabled:
             idx = ReturnnLayersBackend._random_journal_replay_idx
             ReturnnLayersBackend._random_journal_replay_idx += 1
             elem = ReturnnLayersBackend._random_journal[idx]
             assert isinstance(elem, dict)
-            assert elem["dims"] == dims
+            # Different calls might create their own dims, so we cannot directly compare dim tags for equality.
+            assert len(elem["dims"]) == len(dims)
+            # We still check static dimension equality.
+            for dim_journal, dim_tf in zip(elem["dims"], dims):
+                assert (
+                    dim_journal.dimension == dim_tf.dimension
+                ), f"random with dims {dims} does not match random journal replay\n{elem!r}"
             assert elem["dtype"] == dtype
             assert elem["sparse_dim"] == sparse_dim
             assert elem["distribution"] == distribution
             assert rfl.Layer.inner_control_flow() is None  # not implemented yet
             return rfl.make_layer(
                 {
                     "class": "eval",
```

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230414.110554/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230414.110554/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230414.110554/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230414.110554/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230414.110554/returnn/tf/frontend_layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,14 +617,20 @@
             child.tensor = data
         assert child.tensor is data
         if data.raw_tensor is None:
             data.raw_tensor = child
         assert data.raw_tensor is child
         return child
 
+    def get_child_tensor(self, name: str, *, data: Tensor) -> Tensor[Layer]:
+        """
+        Get child layer ref. Makes sure it exists.
+        """
+        return self.get_child_with_tensor(name, data=data).tensor
+
     def __enter__(self):
         self._maybe_init_default_root()
         self._stack.append(self)
         from returnn.util.better_exchook import get_current_frame
 
         frame = get_current_frame()
         self._enter_stack_frames = set()
```

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230414.110554/returnn/tf/frontend_layers/make_layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from tensorflow.python.util import nest
 from returnn.tensor import Tensor, batch_dim
 from returnn.tf.util.data import BatchInfo
 from .. import frontend_layers as rfl
 from . import dims as _dims
 
 
+__all__ = ["make_layer", "_get_sub_layer", "register_extern_data"]
+
+
 def make_layer(
     layer_dict: rfl.LayerDictRaw,
     *,
     name: Optional[Union[str, rfl.Layer]] = None,
     out: Optional[Tensor] = None,
     predefined_out_data: Optional[Tensor] = None,
     name_ctx_ignore_top_stack_frames: int = 0,
@@ -107,14 +110,32 @@
         # noinspection PyProtectedMember
         _dims._register_dim_deps_when_novel(tag, [layer])
     # Debug out. Similar as RETURNN template log. Maybe put this behind a flag? Anyway, useful for now.
     print(layer)
     return layer
 
 
+def _get_sub_layer(layer: Tensor[rfl.Layer], name: str, *, data: Tensor) -> Tensor:
+    """
+    Like the "{layer}/{name}" syntax in RETURNN.
+    Normally this should only be needed for internal usage.
+    """
+    out = layer.raw_tensor.get_child_tensor(name, data=data)
+    if rfl.is_debug_eager_mode_enabled():
+        assert layer.raw_tensor.debug_layer
+        import returnn.tf.layers.base
+
+        assert isinstance(layer.raw_tensor.debug_layer, returnn.tf.layers.base.LayerBase)
+        sub_layer = layer.raw_tensor.debug_layer.get_sub_layer(name)
+        assert sub_layer and sub_layer.output.dim_tags == out.data.dim_tags
+        out.raw_tensor.debug_layer = sub_layer
+        out.data = sub_layer.output
+    return out
+
+
 def _tensor_from_layer_dict(layer_dict: rfl.LayerDictRaw, *, layer: rfl.Layer) -> Tensor[rfl.Layer]:
     """
     Use RETURNN layer_class.get_out_data_from_opts to get the :class:`Data`.
     For this function, we need to set up some dummy network and dummy source layers.
     """
     from returnn.tf.network import TFNetwork, ExternData
     from returnn.tf.layers.base import InternalLayer, LayerBase
```

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230414.110554/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230414.110554/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/horovod.py` & `returnn-1.20230414.110554/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230414.110554/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/layers/base.py` & `returnn-1.20230414.110554/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/layers/basic.py` & `returnn-1.20230414.110554/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/layers/rec.py` & `returnn-1.20230414.110554/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/layers/segmental_model.py` & `returnn-1.20230414.110554/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/layers/signal_processing.py` & `returnn-1.20230414.110554/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/native_op.py` & `returnn-1.20230414.110554/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/network.py` & `returnn-1.20230414.110554/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/sprint.py` & `returnn-1.20230414.110554/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/updater.py` & `returnn-1.20230414.110554/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/util/basic.py` & `returnn-1.20230414.110554/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/util/data.py` & `returnn-1.20230414.110554/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/util/ken_lm.py` & `returnn-1.20230414.110554/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/tf/util/open_fst.py` & `returnn-1.20230414.110554/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/torch/data/pipeline.py` & `returnn-1.20230414.110554/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230414.110554/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/torch/data/tensor_utils.py` & `returnn-1.20230414.110554/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/torch/engine.py` & `returnn-1.20230414.110554/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/torch/frontend/_backend.py` & `returnn-1.20230414.110554/returnn/torch/frontend/_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 from typing import Optional, Union, Any, Sequence, Tuple, List, Dict
 import contextlib
 import torch
 import numpy
 
 from returnn.tensor import Tensor, Dim
-from returnn.util.basic import prod, NotSpecified
+from returnn.util.basic import prod, NotSpecified, get_global_inf_value
 
 # noinspection PyProtectedMember
 from returnn.frontend._backend import Backend
 from returnn.frontend import RawTensorTypes
 import returnn.frontend as rf
 
 
@@ -128,14 +128,21 @@
 
     @staticmethod
     def cast_raw(raw_tensor: torch.Tensor, dtype: str) -> torch.Tensor:
         """cast"""
         return raw_tensor.to(dtype=TorchBackend.as_dtype_raw(dtype))
 
     @staticmethod
+    def stop_gradient(tensor: Tensor) -> Tensor:
+        """stop grad"""
+        out = tensor.copy()
+        out.raw_tensor = out.raw_tensor.detach()
+        return out
+
+    @staticmethod
     def merge_dims(
         source: Tensor,
         *,
         dims: Sequence[Dim],
         out_dim: Optional[Dim] = None,
     ) -> Tuple[Tensor, Dim]:
         """
@@ -190,14 +197,47 @@
             dims=out_dims,
             dtype=source.dtype,
             sparse_dim=source.sparse_dim,
             raw_tensor=out_raw,
         )
 
     @staticmethod
+    def split(source: Tensor, *, axis: Dim, out_dims: Sequence[Dim]) -> Tuple[Tensor, ...]:
+        """split"""
+        src_axis_int = source.get_axis_from_description(axis)
+        out_raw_list = torch.split(
+            source.raw_tensor,
+            split_size_or_sections=[d.get_dim_value() for d in out_dims],
+            dim=src_axis_int,
+        )
+        out_tuple = tuple(
+            source.copy_template_replace_dim_tag(
+                axis=src_axis_int, new_dim_tag=dim, name=f"{source.name}/split:{i}:{dim.description}"
+            )
+            for i, dim in enumerate(out_dims)
+        )
+        for i, out in enumerate(out_tuple):
+            out.raw_tensor = out_raw_list[i]
+        return out_tuple
+
+    @staticmethod
+    def cum_concat_step(source: Tensor, *, prev_accum: Tensor, axis: Dim, out_spatial_dim: Dim) -> Tensor:
+        """cum concat step"""
+        out = prev_accum.copy_template_replace_dim_tag(
+            axis=prev_accum.get_axis_from_description(axis),
+            new_dim_tag=out_spatial_dim,
+            name=f"{source.name}/cum_concat_step",
+        )
+        source_ = source.copy_compatible_to(prev_accum)
+        out.raw_tensor = torch.cat(
+            (prev_accum.raw_tensor, source_.raw_tensor), dim=prev_accum.get_axis_from_description(axis)
+        )
+        return out
+
+    @staticmethod
     def activation_raw(raw_tensor: torch.Tensor, func: str) -> torch.Tensor:
         """
         :param raw_tensor:
         :param func: e.g. "tanh"
         :return: raw tensor after activation
         """
         assert func in Backend._AllowedActivationFuncs
@@ -213,27 +253,35 @@
     def softmax(tensor: Tensor, *, axis: Dim) -> Tensor:
         """
         :param tensor:
         :param axis:
         :return: softmax over axis
         """
         out = tensor.copy_template("softmax")
-        assert not axis.need_masking(), "not implemented"
+        if axis.need_masking():
+            tensor = tensor.copy()
+            mask = tensor.get_sequence_mask_broadcast(axis=axis)
+            inf_value = get_global_inf_value()
+            tensor.raw_tensor = torch.where(mask, tensor.raw_tensor, -inf_value)
         out.raw_tensor = torch.softmax(tensor.raw_tensor, dim=tensor.dims.index(axis))
         return out
 
     @staticmethod
     def log_softmax(tensor: Tensor, *, axis: Dim) -> Tensor:
         """
         :param tensor:
         :param axis:
         :return: log_softmax over axis
         """
         out = tensor.copy_template("log_softmax")
-        assert not axis.need_masking(), "not implemented"
+        if axis.need_masking():
+            tensor = tensor.copy()
+            mask = tensor.get_sequence_mask_broadcast(axis=axis)
+            inf_value = get_global_inf_value()
+            tensor.raw_tensor = torch.where(mask, tensor.raw_tensor, -inf_value)
         out.raw_tensor = torch.log_softmax(tensor.raw_tensor, dim=tensor.dims.index(axis))
         return out
 
     @staticmethod
     def softmax_cross_entropy_with_logits(*, logits: Tensor, targets: Tensor, axis: Dim):
         """
         Efficient cross entropy. For PyTorch this is actually the default cross entropy function.
@@ -314,14 +362,21 @@
             with torch.no_grad():
                 raw_param[:] = value.raw_tensor
         else:
             with torch.no_grad():
                 raw_param[:] = value
 
     @staticmethod
+    def set_parameter_trainable(param: rf.Parameter, trainable: bool) -> None:
+        """set trainable"""
+        raw_param = param.raw_tensor
+        assert isinstance(raw_param, torch.nn.Parameter)
+        raw_param.requires_grad = trainable
+
+    @staticmethod
     def compare_raw(a: torch.Tensor, kind: str, b: torch.Tensor) -> torch.Tensor:
         """
         :param a:
         :param kind: "equal", "less", "less_equal", "greater", "greater_equal", "not_equal"
         :param b:
         :return: a `kind` b
         """
```

### Comparing `returnn-1.20230413.93323/returnn/torch/frontend/_rand.py` & `returnn-1.20230414.110554/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/torch/frontend/bridge.py` & `returnn-1.20230414.110554/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/torch/updater.py` & `returnn-1.20230414.110554/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/basic.py` & `returnn-1.20230414.110554/returnn/util/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -6847,2186 +6847,2212 @@
 0001abe0: 2068 7664 2e72 616e 6b28 2920 213d 2030   hvd.rank() != 0
 0001abf0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
 0001ac00: 7475 726e 2046 616c 7365 0a20 2020 2069  turn False.    i
 0001ac10: 6620 636f 6e66 6967 2e69 735f 7472 7565  f config.is_true
 0001ac20: 2822 6472 795f 7275 6e22 293a 0a20 2020  ("dry_run"):.   
 0001ac30: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
 0001ac40: 650a 2020 2020 7265 7475 726e 2054 7275  e.    return Tru
-0001ac50: 650a 0a0a 636c 6173 7320 4e61 7469 7665  e...class Native
-0001ac60: 436f 6465 436f 6d70 696c 6572 286f 626a  CodeCompiler(obj
-0001ac70: 6563 7429 3a0a 2020 2020 2222 220a 2020  ect):.    """.  
-0001ac80: 2020 4865 6c70 6572 2063 6c61 7373 2074    Helper class t
-0001ac90: 6f20 636f 6d70 696c 6520 6e61 7469 7665  o compile native
-0001aca0: 2043 2f43 2b2b 2063 6f64 6520 6f6e 2d74   C/C++ code on-t
-0001acb0: 6865 2d66 6c79 2e0a 2020 2020 2222 220a  he-fly..    """.
-0001acc0: 0a20 2020 2043 6163 6865 4469 724e 616d  .    CacheDirNam
-0001acd0: 6520 3d20 2272 6574 7572 6e6e 5f6e 6174  e = "returnn_nat
-0001ace0: 6976 6522 0a20 2020 2043 6f6c 6c65 6374  ive".    Collect
-0001acf0: 6564 436f 6d70 696c 6572 7320 3d20 4e6f  edCompilers = No
-0001ad00: 6e65 2020 2320 7479 7065 3a20 7479 7069  ne  # type: typi
-0001ad10: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0001ad20: 6e67 2e4c 6973 745b 4e61 7469 7665 436f  ng.List[NativeCo
-0001ad30: 6465 436f 6d70 696c 6572 5d5d 0a0a 2020  deCompiler]]..  
-0001ad40: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-0001ad50: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0001ad60: 2020 2020 2020 6261 7365 5f6e 616d 652c        base_name,
-0001ad70: 0a20 2020 2020 2020 2063 6f64 655f 7665  .        code_ve
-0001ad80: 7273 696f 6e2c 0a20 2020 2020 2020 2063  rsion,.        c
-0001ad90: 6f64 652c 0a20 2020 2020 2020 2069 735f  ode,.        is_
-0001ada0: 6370 703d 5472 7565 2c0a 2020 2020 2020  cpp=True,.      
-0001adb0: 2020 635f 6d61 6372 6f5f 6465 6669 6e65    c_macro_define
-0001adc0: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-0001add0: 6c64 5f66 6c61 6773 3d4e 6f6e 652c 0a20  ld_flags=None,. 
-0001ade0: 2020 2020 2020 2069 6e63 6c75 6465 5f70         include_p
-0001adf0: 6174 6873 3d28 292c 0a20 2020 2020 2020  aths=(),.       
-0001ae00: 2069 6e63 6c75 6465 5f64 6570 733d 4e6f   include_deps=No
-0001ae10: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
-0001ae20: 6963 5f76 6572 7369 6f6e 5f6e 616d 653d  ic_version_name=
-0001ae30: 4e6f 6e65 2c0a 2020 2020 2020 2020 7368  None,.        sh
-0001ae40: 6f75 6c64 5f63 6c65 616e 7570 5f6f 6c64  ould_cleanup_old
-0001ae50: 5f61 6c6c 3d54 7275 652c 0a20 2020 2020  _all=True,.     
-0001ae60: 2020 2073 686f 756c 645f 636c 6561 6e75     should_cleanu
-0001ae70: 705f 6f6c 645f 6d79 6469 723d 4661 6c73  p_old_mydir=Fals
-0001ae80: 652c 0a20 2020 2020 2020 2075 7365 5f63  e,.        use_c
-0001ae90: 7878 3131 5f61 6269 3d46 616c 7365 2c0a  xx11_abi=False,.
-0001aea0: 2020 2020 2020 2020 6c6f 675f 7374 7265          log_stre
-0001aeb0: 616d 3d4e 6f6e 652c 0a20 2020 2020 2020  am=None,.       
-0001aec0: 2076 6572 626f 7365 3d46 616c 7365 2c0a   verbose=False,.
-0001aed0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-0001aee0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-0001aef0: 6d20 7374 7220 6261 7365 5f6e 616d 653a  m str base_name:
-0001af00: 2062 6173 6520 6e61 6d65 2066 6f72 2074   base name for t
-0001af10: 6865 206d 6f64 756c 652c 2065 2e67 2e20  he module, e.g. 
-0001af20: 227a 6572 6f5f 6f75 7422 0a20 2020 2020  "zero_out".     
-0001af30: 2020 203a 7061 7261 6d20 696e 747c 7475     :param int|tu
-0001af40: 706c 655b 696e 745d 2063 6f64 655f 7665  ple[int] code_ve
-0001af50: 7273 696f 6e3a 2063 6865 636b 2066 6f72  rsion: check for
-0001af60: 2074 6865 2063 6163 6865 2077 6865 7468   the cache wheth
-0001af70: 6572 2074 6f20 7265 7573 650a 2020 2020  er to reuse.    
-0001af80: 2020 2020 3a70 6172 616d 2073 7472 2063      :param str c
-0001af90: 6f64 653a 2074 6865 2073 6f75 7263 6520  ode: the source 
-0001afa0: 636f 6465 2069 7473 656c 660a 2020 2020  code itself.    
-0001afb0: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-0001afc0: 6973 5f63 7070 3a20 6966 2046 616c 7365  is_cpp: if False
-0001afd0: 2c20 4320 6973 2061 7373 756d 6564 0a20  , C is assumed. 
-0001afe0: 2020 2020 2020 203a 7061 7261 6d20 6469         :param di
-0001aff0: 6374 5b73 7472 2c73 7472 7c69 6e74 7c4e  ct[str,str|int|N
-0001b000: 6f6e 655d 7c4e 6f6e 6520 635f 6d61 6372  one]|None c_macr
-0001b010: 6f5f 6465 6669 6e65 733a 2065 2e67 2e20  o_defines: e.g. 
-0001b020: 7b22 5445 4e53 4f52 464c 4f57 223a 2031  {"TENSORFLOW": 1
-0001b030: 7d0a 2020 2020 2020 2020 3a70 6172 616d  }.        :param
-0001b040: 206c 6973 745b 7374 725d 7c4e 6f6e 6520   list[str]|None 
-0001b050: 6c64 5f66 6c61 6773 3a20 652e 672e 205b  ld_flags: e.g. [
-0001b060: 222d 6c62 6c61 7322 5d0a 2020 2020 2020  "-lblas"].      
-0001b070: 2020 3a70 6172 616d 206c 6973 745b 7374    :param list[st
-0001b080: 725d 7c74 7570 6c65 5b73 7472 5d20 696e  r]|tuple[str] in
-0001b090: 636c 7564 655f 7061 7468 733a 0a20 2020  clude_paths:.   
-0001b0a0: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
-0001b0b0: 5b73 7472 5d7c 4e6f 6e65 2069 6e63 6c75  [str]|None inclu
-0001b0c0: 6465 5f64 6570 733a 2069 6620 7072 6f76  de_deps: if prov
-0001b0d0: 6964 6564 2061 6e64 2061 6e20 6578 6973  ided and an exis
-0001b0e0: 7469 6e67 206c 6962 2066 696c 652c 0a20  ting lib file,. 
-0001b0f0: 2020 2020 2020 2020 2020 2077 6520 7769             we wi
-0001b100: 6c6c 2063 6865 636b 2069 6620 616e 7920  ll check if any 
-0001b110: 6465 7065 6e64 656e 6379 2069 7320 6e65  dependency is ne
-0001b120: 7765 720a 2020 2020 2020 2020 2020 2020  wer.            
-0001b130: 616e 6420 7765 206e 6565 6420 746f 2072  and we need to r
-0001b140: 6563 6f6d 7069 6c65 2e20 7765 2063 6f75  ecompile. we cou
-0001b150: 6c64 2061 6c73 6f20 646f 2069 7420 6175  ld also do it au
-0001b160: 746f 6d61 7469 6361 6c6c 7920 7669 6120  tomatically via 
-0001b170: 2d4d 4420 6275 7420 7468 6174 2073 6565  -MD but that see
-0001b180: 6d73 206f 7665 726b 696c 6c20 616e 6420  ms overkill and 
-0001b190: 746f 6f20 736c 6f77 2e0a 2020 2020 2020  too slow..      
-0001b1a0: 2020 3a70 6172 616d 2073 7472 7c4e 6f6e    :param str|Non
-0001b1b0: 6520 7374 6174 6963 5f76 6572 7369 6f6e  e static_version
-0001b1c0: 5f6e 616d 653a 206e 6f72 6d61 6c6c 792c  _name: normally,
-0001b1d0: 2077 6520 7573 6520 2e2e 2e2f 6261 7365   we use .../base
-0001b1e0: 5f6e 616d 652f 6861 7368 2061 7320 7468  _name/hash as th
-0001b1f0: 6520 6469 720a 2020 2020 2020 2020 2020  e dir.          
-0001b200: 2020 6275 7420 7468 6973 2077 6f75 6c64    but this would
-0001b210: 2075 7365 202e 2e2e 2f62 6173 655f 6e61   use .../base_na
-0001b220: 6d65 2f73 7461 7469 635f 7665 7273 696f  me/static_versio
-0001b230: 6e5f 6e61 6d65 2e0a 2020 2020 2020 2020  n_name..        
-0001b240: 3a70 6172 616d 2062 6f6f 6c20 7368 6f75  :param bool shou
-0001b250: 6c64 5f63 6c65 616e 7570 5f6f 6c64 5f61  ld_cleanup_old_a
-0001b260: 6c6c 3a20 7768 6574 6865 7220 7765 2073  ll: whether we s
-0001b270: 686f 756c 6420 6c6f 6f6b 2069 6e20 7468  hould look in th
-0001b280: 6520 6361 6368 6520 6469 720a 2020 2020  e cache dir.    
-0001b290: 2020 2020 2020 2020 616e 6420 6368 6563          and chec
-0001b2a0: 6b20 616c 6c20 6f70 7320 6966 2077 6520  k all ops if we 
-0001b2b0: 6361 6e20 6465 6c65 7465 2073 6f6d 6520  can delete some 
-0001b2c0: 6f6c 6420 6f6e 6573 2077 6869 6368 2061  old ones which a
-0001b2d0: 7265 206f 6c64 6572 2074 6861 6e20 736f  re older than so
-0001b2e0: 6d65 206c 696d 6974 0a20 2020 2020 2020  me limit.       
-0001b2f0: 2020 2020 2028 7365 6c66 2e5f 636c 6561       (self._clea
-0001b300: 6e75 705f 7469 6d65 5f6c 696d 6974 5f64  nup_time_limit_d
-0001b310: 6179 7329 0a20 2020 2020 2020 203a 7061  ays).        :pa
-0001b320: 7261 6d20 626f 6f6c 2073 686f 756c 645f  ram bool should_
-0001b330: 636c 6561 6e75 705f 6f6c 645f 6d79 6469  cleanup_old_mydi
-0001b340: 723a 2077 6865 7468 6572 2077 6520 7368  r: whether we sh
-0001b350: 6f75 6c64 2064 656c 6574 6520 6f75 7220  ould delete our 
-0001b360: 6f70 2064 6972 2062 6566 6f72 6520 7765  op dir before we
-0001b370: 2063 6f6d 7069 6c65 2074 6865 7265 2e0a   compile there..
-0001b380: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-0001b390: 7970 696e 672e 5465 7874 494f 7c4e 6f6e  yping.TextIO|Non
-0001b3a0: 6520 6c6f 675f 7374 7265 616d 3a20 6669  e log_stream: fi
-0001b3b0: 6c65 2073 7472 6561 6d20 666f 7220 7072  le stream for pr
-0001b3c0: 696e 7420 7374 6174 656d 656e 7473 0a20  int statements. 
-0001b3d0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
-0001b3e0: 6f6c 2076 6572 626f 7365 3a20 6265 2073  ol verbose: be s
-0001b3f0: 6c69 6768 746c 7920 6d6f 7265 2076 6572  lightly more ver
-0001b400: 626f 7365 0a20 2020 2020 2020 2022 2222  bose.        """
-0001b410: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0001b420: 2e43 6f6c 6c65 6374 6564 436f 6d70 696c  .CollectedCompil
-0001b430: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-0001b440: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001b450: 662e 436f 6c6c 6563 7465 6443 6f6d 7069  f.CollectedCompi
-0001b460: 6c65 7273 2e61 7070 656e 6428 7365 6c66  lers.append(self
-0001b470: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-0001b480: 6572 626f 7365 203d 2076 6572 626f 7365  erbose = verbose
-0001b490: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
-0001b4a0: 6368 655f 6469 7220 3d20 2225 732f 2573  che_dir = "%s/%s
-0001b4b0: 2220 2520 2867 6574 5f63 6163 6865 5f64  " % (get_cache_d
-0001b4c0: 6972 2829 2c20 7365 6c66 2e43 6163 6865  ir(), self.Cache
-0001b4d0: 4469 724e 616d 6529 0a20 2020 2020 2020  DirName).       
-0001b4e0: 2073 656c 662e 5f69 6e63 6c75 6465 5f70   self._include_p
-0001b4f0: 6174 6873 203d 206c 6973 7428 696e 636c  aths = list(incl
-0001b500: 7564 655f 7061 7468 7329 0a20 2020 2020  ude_paths).     
-0001b510: 2020 2073 656c 662e 6261 7365 5f6e 616d     self.base_nam
-0001b520: 6520 3d20 6261 7365 5f6e 616d 650a 2020  e = base_name.  
-0001b530: 2020 2020 2020 7365 6c66 2e63 6f64 655f        self.code_
-0001b540: 7665 7273 696f 6e20 3d20 636f 6465 5f76  version = code_v
-0001b550: 6572 7369 6f6e 0a20 2020 2020 2020 2073  ersion.        s
-0001b560: 656c 662e 636f 6465 203d 2063 6f64 650a  elf.code = code.
-0001b570: 2020 2020 2020 2020 7365 6c66 2e69 735f          self.is_
-0001b580: 6370 7020 3d20 6973 5f63 7070 0a20 2020  cpp = is_cpp.   
-0001b590: 2020 2020 2073 656c 662e 635f 6d61 6372       self.c_macr
-0001b5a0: 6f5f 6465 6669 6e65 7320 3d20 7b6b 3a20  o_defines = {k: 
-0001b5b0: 7620 666f 7220 6b2c 2076 2069 6e20 2863  v for k, v in (c
-0001b5c0: 5f6d 6163 726f 5f64 6566 696e 6573 206f  _macro_defines o
-0001b5d0: 7220 7b7d 292e 6974 656d 7328 2920 6966  r {}).items() if
-0001b5e0: 2076 2069 7320 6e6f 7420 4e6f 6e65 7d0a   v is not None}.
-0001b5f0: 2020 2020 2020 2020 7365 6c66 2e6c 645f          self.ld_
-0001b600: 666c 6167 7320 3d20 6c64 5f66 6c61 6773  flags = ld_flags
-0001b610: 206f 7220 5b5d 0a20 2020 2020 2020 2073   or [].        s
-0001b620: 656c 662e 696e 636c 7564 655f 6465 7073  elf.include_deps
-0001b630: 203d 2069 6e63 6c75 6465 5f64 6570 730a   = include_deps.
-0001b640: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0001b650: 7469 635f 7665 7273 696f 6e5f 6e61 6d65  tic_version_name
-0001b660: 203d 2073 7461 7469 635f 7665 7273 696f   = static_versio
-0001b670: 6e5f 6e61 6d65 0a20 2020 2020 2020 2073  n_name.        s
-0001b680: 656c 662e 5f63 6f64 655f 6861 7368 203d  elf._code_hash =
-0001b690: 2073 656c 662e 5f6d 616b 655f 636f 6465   self._make_code
-0001b6a0: 5f68 6173 6828 290a 2020 2020 2020 2020  _hash().        
-0001b6b0: 7365 6c66 2e5f 696e 666f 5f64 6963 7420  self._info_dict 
-0001b6c0: 3d20 7365 6c66 2e5f 6d61 6b65 5f69 6e66  = self._make_inf
-0001b6d0: 6f5f 6469 6374 2829 0a20 2020 2020 2020  o_dict().       
-0001b6e0: 2073 656c 662e 5f68 6173 6820 3d20 7365   self._hash = se
-0001b6f0: 6c66 2e5f 6d61 6b65 5f68 6173 6828 290a  lf._make_hash().
-0001b700: 2020 2020 2020 2020 7365 6c66 2e5f 6374          self._ct
-0001b710: 7970 6573 5f6c 6962 203d 204e 6f6e 650a  ypes_lib = None.
-0001b720: 2020 2020 2020 2020 6966 2073 686f 756c          if shoul
-0001b730: 645f 636c 6561 6e75 705f 6f6c 645f 616c  d_cleanup_old_al
-0001b740: 6c3a 0a20 2020 2020 2020 2020 2020 2073  l:.            s
-0001b750: 656c 662e 5f63 6c65 616e 7570 5f6f 6c64  elf._cleanup_old
-0001b760: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0001b770: 5f73 686f 756c 645f 636c 6561 6e75 705f  _should_cleanup_
-0001b780: 6f6c 645f 6d79 6469 7220 3d20 7368 6f75  old_mydir = shou
-0001b790: 6c64 5f63 6c65 616e 7570 5f6f 6c64 5f6d  ld_cleanup_old_m
-0001b7a0: 7964 6972 0a20 2020 2020 2020 2073 656c  ydir.        sel
-0001b7b0: 662e 7573 655f 6378 7831 315f 6162 6920  f.use_cxx11_abi 
-0001b7c0: 3d20 7573 655f 6378 7831 315f 6162 690a  = use_cxx11_abi.
-0001b7d0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-0001b7e0: 675f 7374 7265 616d 203d 206c 6f67 5f73  g_stream = log_s
-0001b7f0: 7472 6561 6d0a 2020 2020 2020 2020 6966  tream.        if
-0001b800: 2073 656c 662e 7665 7262 6f73 653a 0a20   self.verbose:. 
-0001b810: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0001b820: 2822 2573 3a20 2572 2220 2520 2873 656c  ("%s: %r" % (sel
-0001b830: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
-0001b840: 6d65 5f5f 2c20 7365 6c66 292c 2066 696c  me__, self), fil
-0001b850: 653d 6c6f 675f 7374 7265 616d 290a 0a20  e=log_stream).. 
-0001b860: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
-0001b870: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-0001b880: 6574 7572 6e20 223c 2573 2025 7220 696e  eturn "<%s %r in
-0001b890: 2025 723e 2220 2520 2873 656c 662e 5f5f   %r>" % (self.__
-0001b8a0: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
-0001b8b0: 2c20 7365 6c66 2e62 6173 655f 6e61 6d65  , self.base_name
-0001b8c0: 2c20 7365 6c66 2e5f 6d6f 645f 7061 7468  , self._mod_path
-0001b8d0: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-0001b8e0: 0a20 2020 2064 6566 205f 6d6f 645f 7061  .    def _mod_pa
-0001b8f0: 7468 2873 656c 6629 3a0a 2020 2020 2020  th(self):.      
-0001b900: 2020 7265 7475 726e 2022 2573 2f25 732f    return "%s/%s/
-0001b910: 2573 2220 2520 2873 656c 662e 6361 6368  %s" % (self.cach
-0001b920: 655f 6469 722c 2073 656c 662e 6261 7365  e_dir, self.base
-0001b930: 5f6e 616d 652c 2073 656c 662e 7374 6174  _name, self.stat
-0001b940: 6963 5f76 6572 7369 6f6e 5f6e 616d 6520  ic_version_name 
-0001b950: 6f72 2073 656c 662e 5f68 6173 685b 3a31  or self._hash[:1
-0001b960: 305d 290a 0a20 2020 2040 7072 6f70 6572  0])..    @proper
-0001b970: 7479 0a20 2020 2064 6566 205f 696e 666f  ty.    def _info
-0001b980: 5f66 696c 656e 616d 6528 7365 6c66 293a  _filename(self):
-0001b990: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001b9a0: 2225 732f 696e 666f 2e70 7922 2025 2028  "%s/info.py" % (
-0001b9b0: 7365 6c66 2e5f 6d6f 645f 7061 7468 2c29  self._mod_path,)
-0001b9c0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0001b9d0: 2020 2020 6465 6620 5f73 6f5f 6669 6c65      def _so_file
-0001b9e0: 6e61 6d65 2873 656c 6629 3a0a 2020 2020  name(self):.    
-0001b9f0: 2020 2020 7265 7475 726e 2022 2573 2f25      return "%s/%
-0001ba00: 732e 736f 2220 2520 2873 656c 662e 5f6d  s.so" % (self._m
-0001ba10: 6f64 5f70 6174 682c 2073 656c 662e 6261  od_path, self.ba
-0001ba20: 7365 5f6e 616d 6529 0a0a 2020 2020 4070  se_name)..    @p
-0001ba30: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0001ba40: 5f63 5f66 696c 656e 616d 6528 7365 6c66  _c_filename(self
-0001ba50: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-0001ba60: 6c66 2e69 735f 6370 703a 0a20 2020 2020  lf.is_cpp:.     
-0001ba70: 2020 2020 2020 2072 6574 7572 6e20 2225         return "%
-0001ba80: 732f 2573 2e63 6322 2025 2028 7365 6c66  s/%s.cc" % (self
-0001ba90: 2e5f 6d6f 645f 7061 7468 2c20 7365 6c66  ._mod_path, self
-0001baa0: 2e62 6173 655f 6e61 6d65 290a 2020 2020  .base_name).    
-0001bab0: 2020 2020 7265 7475 726e 2022 2573 2f25      return "%s/%
-0001bac0: 732e 6322 2025 2028 7365 6c66 2e5f 6d6f  s.c" % (self._mo
-0001bad0: 645f 7061 7468 2c20 7365 6c66 2e62 6173  d_path, self.bas
-0001bae0: 655f 6e61 6d65 290a 0a20 2020 205f 636c  e_name)..    _cl
-0001baf0: 6561 6e75 705f 7469 6d65 5f6c 696d 6974  eanup_time_limit
-0001bb00: 5f64 6179 7320 3d20 3630 0a0a 2020 2020  _days = 60..    
-0001bb10: 6465 6620 5f63 6c65 616e 7570 5f6f 6c64  def _cleanup_old
-0001bb20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001bb30: 6d6f 645f 7061 7468 203d 2073 656c 662e  mod_path = self.
-0001bb40: 5f6d 6f64 5f70 6174 6820 2023 202e 2e2e  _mod_path  # ...
-0001bb50: 2f62 6173 655f 6e61 6d65 2f68 6173 680a  /base_name/hash.
-0001bb60: 2020 2020 2020 2020 6261 7365 5f6d 6f64          base_mod
-0001bb70: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0001bb80: 6469 726e 616d 6528 6d6f 645f 7061 7468  dirname(mod_path
-0001bb90: 2920 2023 202e 2e2e 2f62 6173 655f 6e61  )  # .../base_na
-0001bba0: 6d65 0a20 2020 2020 2020 206d 795f 6d6f  me.        my_mo
-0001bbb0: 645f 7061 7468 5f6e 616d 6520 3d20 6f73  d_path_name = os
-0001bbc0: 2e70 6174 682e 6261 7365 6e61 6d65 286d  .path.basename(m
-0001bbd0: 6f64 5f70 6174 6829 0a20 2020 2020 2020  od_path).       
-0001bbe0: 2069 6620 6e6f 7420 6f73 2e70 6174 682e   if not os.path.
-0001bbf0: 6578 6973 7473 2862 6173 655f 6d6f 645f  exists(base_mod_
-0001bc00: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
-0001bc10: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0001bc20: 2020 696d 706f 7274 2074 696d 650a 0a20    import time.. 
-0001bc30: 2020 2020 2020 2063 6c65 616e 7570 5f74         cleanup_t
-0001bc40: 696d 655f 6c69 6d69 745f 7365 6373 203d  ime_limit_secs =
-0001bc50: 2073 656c 662e 5f63 6c65 616e 7570 5f74   self._cleanup_t
-0001bc60: 696d 655f 6c69 6d69 745f 6461 7973 202a  ime_limit_days *
-0001bc70: 2032 3420 2a20 3630 202a 2036 300a 2020   24 * 60 * 60.  
-0001bc80: 2020 2020 2020 666f 7220 7020 696e 206f        for p in o
-0001bc90: 732e 6c69 7374 6469 7228 6261 7365 5f6d  s.listdir(base_m
-0001bca0: 6f64 5f70 6174 6829 3a0a 2020 2020 2020  od_path):.      
-0001bcb0: 2020 2020 2020 6966 2070 203d 3d20 6d79        if p == my
-0001bcc0: 5f6d 6f64 5f70 6174 685f 6e61 6d65 3a0a  _mod_path_name:.
-0001bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bce0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0001bcf0: 2020 2020 2066 756c 6c5f 6469 725f 7061       full_dir_pa
-0001bd00: 7468 203d 2022 2573 2f25 7322 2025 2028  th = "%s/%s" % (
-0001bd10: 6261 7365 5f6d 6f64 5f70 6174 682c 2070  base_mod_path, p
-0001bd20: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001bd30: 206e 6f74 206f 732e 7061 7468 2e69 7364   not os.path.isd
-0001bd40: 6972 2866 756c 6c5f 6469 725f 7061 7468  ir(full_dir_path
-0001bd50: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001bd60: 2020 2063 6f6e 7469 6e75 6520 2023 2069     continue  # i
-0001bd70: 676e 6f72 6520 666f 7220 6e6f 770a 2020  gnore for now.  
-0001bd80: 2020 2020 2020 2020 2020 6c6f 636b 203d            lock =
-0001bd90: 204c 6f63 6b46 696c 6528 6675 6c6c 5f64   LockFile(full_d
-0001bda0: 6972 5f70 6174 6829 0a20 2020 2020 2020  ir_path).       
-0001bdb0: 2020 2020 2069 6620 6c6f 636b 2e69 735f       if lock.is_
-0001bdc0: 6c6f 636b 6564 2829 3a0a 2020 2020 2020  locked():.      
-0001bdd0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0001bde0: 7565 0a20 2020 2020 2020 2020 2020 206c  ue.            l
-0001bdf0: 6f63 6b2e 6d61 7962 655f 7265 6d6f 7665  ock.maybe_remove
-0001be00: 5f6f 6c64 5f6c 6f63 6b66 696c 6528 290a  _old_lockfile().
-0001be10: 2020 2020 2020 2020 2020 2020 696e 666f              info
-0001be20: 5f70 6174 6820 3d20 2225 732f 696e 666f  _path = "%s/info
-0001be30: 2e70 7922 2025 2066 756c 6c5f 6469 725f  .py" % full_dir_
-0001be40: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-0001be50: 2069 6620 6e6f 7420 6f73 2e70 6174 682e   if not os.path.
-0001be60: 6578 6973 7473 2869 6e66 6f5f 7061 7468  exists(info_path
-0001be70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001be80: 2020 2073 656c 662e 5f63 6c65 616e 7570     self._cleanup
-0001be90: 5f6f 6c64 5f70 6174 6828 6675 6c6c 5f64  _old_path(full_d
-0001bea0: 6972 5f70 6174 682c 2072 6561 736f 6e3d  ir_path, reason=
-0001beb0: 2263 6f72 7275 7074 2064 6972 2c20 6d69  "corrupt dir, mi
-0001bec0: 7373 696e 6720 696e 666f 2e70 7922 290a  ssing info.py").
-0001bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bee0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0001bef0: 2020 2020 2073 6f5f 7061 7468 203d 2022       so_path = "
-0001bf00: 2573 2f25 732e 736f 2220 2520 2866 756c  %s/%s.so" % (ful
-0001bf10: 6c5f 6469 725f 7061 7468 2c20 7365 6c66  l_dir_path, self
-0001bf20: 2e62 6173 655f 6e61 6d65 290a 2020 2020  .base_name).    
-0001bf30: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
-0001bf40: 732e 7061 7468 2e65 7869 7374 7328 736f  s.path.exists(so
-0001bf50: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
-0001bf60: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
-0001bf70: 6561 6e75 705f 6f6c 645f 7061 7468 2866  eanup_old_path(f
-0001bf80: 756c 6c5f 6469 725f 7061 7468 2c20 7265  ull_dir_path, re
-0001bf90: 6173 6f6e 3d22 636f 7272 7570 7420 6469  ason="corrupt di
-0001bfa0: 722c 206d 6973 7369 6e67 2073 6f22 290a  r, missing so").
-0001bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfc0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0001bfd0: 2020 2020 2064 7420 3d20 7469 6d65 2e74       dt = time.t
-0001bfe0: 696d 6528 2920 2d20 6f73 2e70 6174 682e  ime() - os.path.
-0001bff0: 6765 746d 7469 6d65 2873 6f5f 7061 7468  getmtime(so_path
-0001c000: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001c010: 2064 7420 3e20 636c 6561 6e75 705f 7469   dt > cleanup_ti
-0001c020: 6d65 5f6c 696d 6974 5f73 6563 733a 0a20  me_limit_secs:. 
-0001c030: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001c040: 656c 662e 5f63 6c65 616e 7570 5f6f 6c64  elf._cleanup_old
-0001c050: 5f70 6174 6828 6675 6c6c 5f64 6972 5f70  _path(full_dir_p
-0001c060: 6174 682c 2072 6561 736f 6e3d 2225 7320  ath, reason="%s 
-0001c070: 6f6c 6422 2025 2068 6d73 2864 7429 290a  old" % hms(dt)).
-0001c080: 0a20 2020 2064 6566 205f 636c 6561 6e75  .    def _cleanu
-0001c090: 705f 6f6c 645f 7061 7468 2873 656c 662c  p_old_path(self,
-0001c0a0: 2070 2c20 7265 6173 6f6e 293a 0a20 2020   p, reason):.   
-0001c0b0: 2020 2020 2070 7269 6e74 2822 2573 2064       print("%s d
-0001c0c0: 656c 6574 6520 6f6c 642c 2025 733a 2025  elete old, %s: %
-0001c0d0: 7322 2025 2028 7365 6c66 2e5f 5f63 6c61  s" % (self.__cla
-0001c0e0: 7373 5f5f 2e5f 5f6e 616d 655f 5f2c 2072  ss__.__name__, r
-0001c0f0: 6561 736f 6e2c 2070 2929 0a20 2020 2020  eason, p)).     
-0001c100: 2020 2061 7373 6572 7420 6f73 2e70 6174     assert os.pat
-0001c110: 682e 6578 6973 7473 2870 290a 2020 2020  h.exists(p).    
-0001c120: 2020 2020 696d 706f 7274 2073 6875 7469      import shuti
-0001c130: 6c0a 0a20 2020 2020 2020 2074 7279 3a0a  l..        try:.
-0001c140: 2020 2020 2020 2020 2020 2020 7368 7574              shut
-0001c150: 696c 2e72 6d74 7265 6528 7029 0a20 2020  il.rmtree(p).   
-0001c160: 2020 2020 2065 7863 6570 7420 4f53 4572       except OSEr
-0001c170: 726f 7220 6173 2065 7863 3a0a 2020 2020  ror as exc:.    
-0001c180: 2020 2020 2020 2020 7072 696e 7428 2225          print("%
-0001c190: 7320 6465 6c65 7465 2065 7863 6570 7469  s delete excepti
-0001c1a0: 6f6e 2028 2573 292e 2057 696c 6c20 6967  on (%s). Will ig
-0001c1b0: 6e6f 7265 2061 6e64 2074 7279 2074 6f20  nore and try to 
-0001c1c0: 636f 6e74 696e 7565 2061 6e79 7761 792e  continue anyway.
-0001c1d0: 2220 2520 2873 656c 662e 5f5f 636c 6173  " % (self.__clas
-0001c1e0: 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20 6578  s__.__name__, ex
-0001c1f0: 6329 290a 0a20 2020 2064 6566 205f 6c6f  c))..    def _lo
-0001c200: 6164 5f69 6e66 6f28 7365 6c66 293a 0a20  ad_info(self):. 
-0001c210: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001c220: 2020 203a 7274 7970 653a 2064 6963 745b     :rtype: dict[
-0001c230: 7374 725d 7c4e 6f6e 650a 2020 2020 2020  str]|None.      
-0001c240: 2020 2222 220a 2020 2020 2020 2020 6669    """.        fi
-0001c250: 6c65 6e61 6d65 203d 2073 656c 662e 5f69  lename = self._i
-0001c260: 6e66 6f5f 6669 6c65 6e61 6d65 0a20 2020  nfo_filename.   
-0001c270: 2020 2020 2069 6620 6e6f 7420 6f73 2e70       if not os.p
-0001c280: 6174 682e 6578 6973 7473 2866 696c 656e  ath.exists(filen
-0001c290: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
-0001c2a0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-0001c2b0: 2020 2020 2020 7320 3d20 6f70 656e 2866        s = open(f
-0001c2c0: 696c 656e 616d 6529 2e72 6561 6428 290a  ilename).read().
-0001c2d0: 2020 2020 2020 2020 7265 7320 3d20 6576          res = ev
-0001c2e0: 616c 2873 290a 2020 2020 2020 2020 6173  al(s).        as
-0001c2f0: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
-0001c300: 7265 732c 2064 6963 7429 0a20 2020 2020  res, dict).     
-0001c310: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
-0001c320: 2020 205f 7265 6c65 7661 6e74 5f69 6e66     _relevant_inf
-0001c330: 6f5f 6b65 7973 203d 2028 2263 6f64 655f  o_keys = ("code_
-0001c340: 7665 7273 696f 6e22 2c20 2263 6f64 655f  version", "code_
-0001c350: 6861 7368 222c 2022 635f 6d61 6372 6f5f  hash", "c_macro_
-0001c360: 6465 6669 6e65 7322 2c20 226c 645f 666c  defines", "ld_fl
-0001c370: 6167 7322 2c20 2263 6f6d 7069 6c65 725f  ags", "compiler_
-0001c380: 6269 6e22 290a 0a20 2020 2064 6566 205f  bin")..    def _
-0001c390: 6d61 6b65 5f69 6e66 6f5f 6469 6374 2873  make_info_dict(s
-0001c3a0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0001c3b0: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
-0001c3c0: 3a20 6469 6374 5b73 7472 5d0a 2020 2020  : dict[str].    
-0001c3d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0001c3e0: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-0001c3f0: 2020 2020 2022 6261 7365 5f6e 616d 6522       "base_name"
-0001c400: 3a20 7365 6c66 2e62 6173 655f 6e61 6d65  : self.base_name
-0001c410: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
-0001c420: 6e63 6c75 6465 5f70 6174 6873 223a 2073  nclude_paths": s
-0001c430: 656c 662e 5f69 6e63 6c75 6465 5f70 6174  elf._include_pat
-0001c440: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
-0001c450: 2263 6f64 655f 7665 7273 696f 6e22 3a20  "code_version": 
-0001c460: 7365 6c66 2e63 6f64 655f 7665 7273 696f  self.code_versio
-0001c470: 6e2c 0a20 2020 2020 2020 2020 2020 2022  n,.            "
-0001c480: 636f 6465 5f68 6173 6822 3a20 7365 6c66  code_hash": self
-0001c490: 2e5f 636f 6465 5f68 6173 682c 0a20 2020  ._code_hash,.   
-0001c4a0: 2020 2020 2020 2020 2022 635f 6d61 6372           "c_macr
-0001c4b0: 6f5f 6465 6669 6e65 7322 3a20 7365 6c66  o_defines": self
-0001c4c0: 2e63 5f6d 6163 726f 5f64 6566 696e 6573  .c_macro_defines
-0001c4d0: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-0001c4e0: 645f 666c 6167 7322 3a20 7365 6c66 2e6c  d_flags": self.l
-0001c4f0: 645f 666c 6167 732c 0a20 2020 2020 2020  d_flags,.       
-0001c500: 2020 2020 2022 636f 6d70 696c 6572 5f62       "compiler_b
-0001c510: 696e 223a 2073 656c 662e 5f67 6574 5f63  in": self._get_c
-0001c520: 6f6d 7069 6c65 725f 6269 6e28 292c 0a20  ompiler_bin(),. 
-0001c530: 2020 2020 2020 207d 0a0a 2020 2020 6465         }..    de
-0001c540: 6620 5f6d 616b 655f 636f 6465 5f68 6173  f _make_code_has
-0001c550: 6828 7365 6c66 293a 0a20 2020 2020 2020  h(self):.       
-0001c560: 2069 6d70 6f72 7420 6861 7368 6c69 620a   import hashlib.
-0001c570: 0a20 2020 2020 2020 2068 203d 2068 6173  .        h = has
-0001c580: 686c 6962 2e6d 6435 2829 0a20 2020 2020  hlib.md5().     
-0001c590: 2020 2068 2e75 7064 6174 6528 7365 6c66     h.update(self
-0001c5a0: 2e63 6f64 652e 656e 636f 6465 2822 7574  .code.encode("ut
-0001c5b0: 6638 2229 290a 2020 2020 2020 2020 7265  f8")).        re
-0001c5c0: 7475 726e 2068 2e68 6578 6469 6765 7374  turn h.hexdigest
-0001c5d0: 2829 0a0a 2020 2020 6465 6620 5f6d 616b  ()..    def _mak
-0001c5e0: 655f 6861 7368 2873 656c 6629 3a0a 2020  e_hash(self):.  
-0001c5f0: 2020 2020 2020 696d 706f 7274 2068 6173        import has
-0001c600: 686c 6962 0a0a 2020 2020 2020 2020 6820  hlib..        h 
-0001c610: 3d20 6861 7368 6c69 622e 6d64 3528 290a  = hashlib.md5().
-0001c620: 2020 2020 2020 2020 682e 7570 6461 7465          h.update
-0001c630: 2822 7b22 2e65 6e63 6f64 6528 2275 7466  ("{".encode("utf
-0001c640: 3822 2929 0a20 2020 2020 2020 2066 6f72  8")).        for
-0001c650: 206b 6579 2069 6e20 7365 6c66 2e5f 7265   key in self._re
-0001c660: 6c65 7661 6e74 5f69 6e66 6f5f 6b65 7973  levant_info_keys
-0001c670: 3a0a 2020 2020 2020 2020 2020 2020 682e  :.            h.
-0001c680: 7570 6461 7465 2828 2225 733a 7b25 737d  update(("%s:{%s}
-0001c690: 2220 2520 286b 6579 2c20 7365 6c66 2e5f  " % (key, self._
-0001c6a0: 696e 666f 5f64 6963 745b 6b65 795d 2929  info_dict[key]))
-0001c6b0: 2e65 6e63 6f64 6528 2275 7466 3822 2929  .encode("utf8"))
-0001c6c0: 0a20 2020 2020 2020 2068 2e75 7064 6174  .        h.updat
-0001c6d0: 6528 227d 222e 656e 636f 6465 2822 7574  e("}".encode("ut
-0001c6e0: 6638 2229 290a 2020 2020 2020 2020 7265  f8")).        re
-0001c6f0: 7475 726e 2068 2e68 6578 6469 6765 7374  turn h.hexdigest
-0001c700: 2829 0a0a 2020 2020 6465 6620 5f73 6176  ()..    def _sav
-0001c710: 655f 696e 666f 2873 656c 6629 3a0a 2020  e_info(self):.  
-0001c720: 2020 2020 2020 6669 6c65 6e61 6d65 203d        filename =
-0001c730: 2073 656c 662e 5f69 6e66 6f5f 6669 6c65   self._info_file
-0001c740: 6e61 6d65 0a20 2020 2020 2020 2077 6974  name.        wit
-0001c750: 6820 6f70 656e 2866 696c 656e 616d 652c  h open(filename,
-0001c760: 2022 7722 2920 6173 2066 3a0a 2020 2020   "w") as f:.    
-0001c770: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-0001c780: 2225 735c 6e22 2025 2062 6574 7465 725f  "%s\n" % better_
-0001c790: 7265 7072 2873 656c 662e 5f69 6e66 6f5f  repr(self._info_
-0001c7a0: 6469 6374 2929 0a0a 2020 2020 6465 6620  dict))..    def 
-0001c7b0: 5f6e 6565 645f 7265 636f 6d70 696c 6528  _need_recompile(
-0001c7c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0001c7d0: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
-0001c7e0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-0001c7f0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-0001c800: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
-0001c810: 7328 7365 6c66 2e5f 736f 5f66 696c 656e  s(self._so_filen
-0001c820: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
-0001c830: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0001c840: 2020 2020 2020 6966 2073 656c 662e 696e        if self.in
-0001c850: 636c 7564 655f 6465 7073 3a0a 2020 2020  clude_deps:.    
-0001c860: 2020 2020 2020 2020 736f 5f6d 7469 6d65          so_mtime
-0001c870: 203d 206f 732e 7061 7468 2e67 6574 6d74   = os.path.getmt
-0001c880: 696d 6528 7365 6c66 2e5f 736f 5f66 696c  ime(self._so_fil
-0001c890: 656e 616d 6529 0a20 2020 2020 2020 2020  ename).         
-0001c8a0: 2020 2066 6f72 2066 6e20 696e 2073 656c     for fn in sel
-0001c8b0: 662e 696e 636c 7564 655f 6465 7073 3a0a  f.include_deps:.
-0001c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8d0: 6966 206f 732e 7061 7468 2e67 6574 6d74  if os.path.getmt
-0001c8e0: 696d 6528 666e 2920 3e20 736f 5f6d 7469  ime(fn) > so_mti
-0001c8f0: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
-0001c900: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0001c910: 7275 650a 2020 2020 2020 2020 6f6c 645f  rue.        old_
-0001c920: 696e 666f 203d 2073 656c 662e 5f6c 6f61  info = self._loa
-0001c930: 645f 696e 666f 2829 0a20 2020 2020 2020  d_info().       
-0001c940: 206e 6577 5f69 6e66 6f20 3d20 7365 6c66   new_info = self
-0001c950: 2e5f 6d61 6b65 5f69 6e66 6f5f 6469 6374  ._make_info_dict
-0001c960: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
-0001c970: 7420 6f6c 645f 696e 666f 3a0a 2020 2020  t old_info:.    
-0001c980: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0001c990: 7275 650a 2020 2020 2020 2020 2320 5468  rue.        # Th
-0001c9a0: 6520 6861 7368 2061 6c72 6561 6479 206d  e hash already m
-0001c9b0: 6174 6368 6564 2062 7574 2076 6572 7920  atched but very 
-0001c9c0: 756e 6c69 6b65 6c79 2c20 7468 6973 2063  unlikely, this c
-0001c9d0: 6f75 6c64 2062 6520 6120 636f 6c6c 6973  ould be a collis
-0001c9e0: 696f 6e2e 0a20 2020 2020 2020 2023 2041  ion..        # A
-0001c9f0: 6e79 7761 792c 206a 7573 7420 646f 2074  nyway, just do t
-0001ca00: 6869 7320 7665 7279 2063 6865 6170 2063  his very cheap c
-0001ca10: 6865 636b 2e0a 2020 2020 2020 2020 666f  heck..        fo
-0001ca20: 7220 6b65 7920 696e 2073 656c 662e 5f72  r key in self._r
-0001ca30: 656c 6576 616e 745f 696e 666f 5f6b 6579  elevant_info_key
-0001ca40: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-0001ca50: 6620 6b65 7920 6e6f 7420 696e 206f 6c64  f key not in old
-0001ca60: 5f69 6e66 6f3a 0a20 2020 2020 2020 2020  _info:.         
-0001ca70: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001ca80: 7565 0a20 2020 2020 2020 2020 2020 2069  ue.            i
-0001ca90: 6620 6f6c 645f 696e 666f 5b6b 6579 5d20  f old_info[key] 
-0001caa0: 213d 206e 6577 5f69 6e66 6f5b 6b65 795d  != new_info[key]
-0001cab0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001cac0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0001cad0: 2020 2020 2020 2320 4966 206e 6f20 636f        # If no co
-0001cae0: 6465 2076 6572 7369 6f6e 2069 7320 7072  de version is pr
-0001caf0: 6f76 6964 6564 2c20 7765 2063 6f75 6c64  ovided, we could
-0001cb00: 2061 6c73 6f20 6368 6563 6b20 7468 6520   also check the 
-0001cb10: 636f 6465 2069 7473 656c 6620 6e6f 772e  code itself now.
-0001cb20: 0a20 2020 2020 2020 2023 2042 7574 2049  .        # But I
-0001cb30: 2074 6869 6e6b 2074 6869 7320 6973 206f   think this is o
-0001cb40: 7665 726b 696c 6c2e 0a20 2020 2020 2020  verkill..       
-0001cb50: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-0001cb60: 2020 2064 6566 205f 6d61 7962 655f 636f     def _maybe_co
-0001cb70: 6d70 696c 6528 7365 6c66 293a 0a20 2020  mpile(self):.   
-0001cb80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001cb90: 204f 6e20 7375 6363 6573 7366 756c 2072   On successful r
-0001cba0: 6574 7572 6e2c 2073 656c 662e 5f73 6f5f  eturn, self._so_
-0001cbb0: 6669 6c65 6e61 6d65 2073 686f 756c 6420  filename should 
-0001cbc0: 6578 6973 7420 616e 6420 6265 2075 702d  exist and be up-
-0001cbd0: 746f 2d64 6174 652e 0a20 2020 2020 2020  to-date..       
-0001cbe0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-0001cbf0: 6e6f 7420 7365 6c66 2e5f 6e65 6564 5f72  not self._need_r
-0001cc00: 6563 6f6d 7069 6c65 2829 3a0a 2020 2020  ecompile():.    
-0001cc10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001cc20: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-0001cc30: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-0001cc40: 2573 3a20 4e6f 206e 6565 6420 746f 2072  %s: No need to r
-0001cc50: 6563 6f6d 7069 6c65 3a20 2573 2220 2520  ecompile: %s" % 
-0001cc60: 2873 656c 662e 5f5f 636c 6173 735f 5f2e  (self.__class__.
-0001cc70: 5f5f 6e61 6d65 5f5f 2c20 7365 6c66 2e5f  __name__, self._
-0001cc80: 736f 5f66 696c 656e 616d 6529 290a 2020  so_filename)).  
-0001cc90: 2020 2020 2020 2020 2020 2320 546f 7563            # Touc
-0001cca0: 6820 6974 2073 6f20 7468 6174 2077 6520  h it so that we 
-0001ccb0: 6361 6e20 7365 6520 7468 6174 2077 6520  can see that we 
-0001ccc0: 7573 6564 2069 7420 7265 6365 6e74 6c79  used it recently
-0001ccd0: 2e0a 2020 2020 2020 2020 2020 2020 6f73  ..            os
-0001cce0: 2e75 7469 6d65 2873 656c 662e 5f69 6e66  .utime(self._inf
-0001ccf0: 6f5f 6669 6c65 6e61 6d65 2c20 4e6f 6e65  o_filename, None
-0001cd00: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0001cd10: 7475 726e 0a20 2020 2020 2020 206c 6f63  turn.        loc
-0001cd20: 6b20 3d20 4c6f 636b 4669 6c65 2873 656c  k = LockFile(sel
-0001cd30: 662e 5f6d 6f64 5f70 6174 6829 0a20 2020  f._mod_path).   
-0001cd40: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0001cd50: 2e5f 6e65 6564 5f72 6563 6f6d 7069 6c65  ._need_recompile
-0001cd60: 2829 3a20 2023 2063 6865 636b 2061 6761  ():  # check aga
-0001cd70: 696e 0a20 2020 2020 2020 2020 2020 2069  in.            i
-0001cd80: 6620 7365 6c66 2e76 6572 626f 7365 3a0a  f self.verbose:.
-0001cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cda0: 7072 696e 7428 2225 733a 204e 6f20 6e65  print("%s: No ne
-0001cdb0: 6564 2074 6f20 7265 636f 6d70 696c 6520  ed to recompile 
-0001cdc0: 6166 7465 7220 7765 2077 6169 7465 643a  after we waited:
-0001cdd0: 2025 7322 2025 2028 7365 6c66 2e5f 5f63   %s" % (self.__c
-0001cde0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f2c  lass__.__name__,
-0001cdf0: 2073 656c 662e 5f73 6f5f 6669 6c65 6e61   self._so_filena
-0001ce00: 6d65 2929 0a20 2020 2020 2020 2020 2020  me)).           
-0001ce10: 206f 732e 7574 696d 6528 7365 6c66 2e5f   os.utime(self._
-0001ce20: 696e 666f 5f66 696c 656e 616d 652c 204e  info_filename, N
-0001ce30: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
-0001ce40: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0001ce50: 6966 2073 656c 662e 5f73 686f 756c 645f  if self._should_
-0001ce60: 636c 6561 6e75 705f 6f6c 645f 6d79 6469  cleanup_old_mydi
-0001ce70: 7220 616e 6420 6e6f 7420 6c6f 636b 2e69  r and not lock.i
-0001ce80: 735f 6c6f 636b 6564 2829 3a0a 2020 2020  s_locked():.    
-0001ce90: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-0001cea0: 7468 2e65 7869 7374 7328 7365 6c66 2e5f  th.exists(self._
-0001ceb0: 6d6f 645f 7061 7468 293a 0a20 2020 2020  mod_path):.     
-0001cec0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001ced0: 5f63 6c65 616e 7570 5f6f 6c64 5f70 6174  _cleanup_old_pat
-0001cee0: 6828 7365 6c66 2e5f 6d6f 645f 7061 7468  h(self._mod_path
-0001cef0: 2c20 7265 6173 6f6e 3d22 6e65 6564 2072  , reason="need r
-0001cf00: 6563 6f6d 7069 6c65 2229 0a20 2020 2020  ecompile").     
-0001cf10: 2020 2077 6974 6820 6c6f 636b 3a0a 2020     with lock:.  
-0001cf20: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0001cf30: 6d61 7962 655f 636f 6d70 696c 655f 696e  maybe_compile_in
-0001cf40: 6e65 7228 290a 0a20 2020 2064 6566 205f  ner()..    def _
-0001cf50: 6765 745f 636f 6d70 696c 6572 5f62 696e  get_compiler_bin
-0001cf60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001cf70: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
-0001cf80: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-0001cf90: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-0001cfa0: 656c 662e 6973 5f63 7070 3a0a 2020 2020  elf.is_cpp:.    
-0001cfb0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-0001cfc0: 672b 2b22 0a20 2020 2020 2020 2072 6574  g++".        ret
-0001cfd0: 7572 6e20 2267 6363 220a 0a20 2020 2064  urn "gcc"..    d
-0001cfe0: 6566 205f 7472 616e 7366 6f72 6d5f 636f  ef _transform_co
-0001cff0: 6d70 696c 6572 5f6f 7074 7328 7365 6c66  mpiler_opts(self
-0001d000: 2c20 6f70 7473 293a 0a20 2020 2020 2020  , opts):.       
-0001d010: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-0001d020: 7261 6d20 6c69 7374 5b73 7472 5d20 6f70  ram list[str] op
-0001d030: 7473 3a0a 2020 2020 2020 2020 3a72 7479  ts:.        :rty
-0001d040: 7065 3a20 6c69 7374 5b73 7472 5d0a 2020  pe: list[str].  
-0001d050: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001d060: 2020 7265 7475 726e 206f 7074 730a 0a20    return opts.. 
-0001d070: 2020 2064 6566 205f 6578 7472 615f 636f     def _extra_co
-0001d080: 6d6d 6f6e 5f6f 7074 7328 7365 6c66 293a  mmon_opts(self):
-0001d090: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001d0a0: 2020 2020 203a 7274 7970 653a 206c 6973       :rtype: lis
-0001d0b0: 745b 7374 725d 0a20 2020 2020 2020 2022  t[str].        "
-0001d0c0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-0001d0d0: 6c66 2e69 735f 6370 703a 0a20 2020 2020  lf.is_cpp:.     
-0001d0e0: 2020 2020 2020 2072 6574 7572 6e20 5b22         return ["
-0001d0f0: 2d73 7464 3d63 2b2b 3131 225d 0a20 2020  -std=c++11"].   
-0001d100: 2020 2020 2072 6574 7572 6e20 5b5d 0a0a       return []..
-0001d110: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-0001d120: 0a20 2020 2064 6566 205f 7472 616e 7366  .    def _transf
-0001d130: 6f72 6d5f 6c64 5f66 6c61 6728 636c 732c  orm_ld_flag(cls,
-0001d140: 206f 7074 293a 0a20 2020 2020 2020 2022   opt):.        "
-0001d150: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-0001d160: 6d20 7374 7220 6f70 743a 0a20 2020 2020  m str opt:.     
-0001d170: 2020 203a 7274 7970 653a 2073 7472 0a20     :rtype: str. 
-0001d180: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001d190: 2020 2069 6620 7379 732e 706c 6174 666f     if sys.platfo
-0001d1a0: 726d 203d 3d20 2264 6172 7769 6e22 3a0a  rm == "darwin":.
-0001d1b0: 2020 2020 2020 2020 2020 2020 2320 4974              # It
-0001d1c0: 2073 6565 6d73 2073 6f6d 6520 7665 7273   seems some vers
-0001d1d0: 696f 6e73 206f 6620 4d61 634f 5320 6c64  ions of MacOS ld
-0001d1e0: 2063 616e 6e6f 7420 6861 6e64 6c65 2074   cannot handle t
-0001d1f0: 6865 2060 2d6c 3a66 696c 656e 616d 6560  he `-l:filename`
-0001d200: 2061 7267 756d 656e 7420 636f 7272 6563   argument correc
-0001d210: 746c 792e 0a20 2020 2020 2020 2020 2020  tly..           
-0001d220: 2023 2045 2e67 2e20 5465 6e73 6f72 466c   # E.g. TensorFl
-0001d230: 6f77 2031 2e31 3420 696e 636f 7272 6563  ow 1.14 incorrec
-0001d240: 746c 7920 7573 6573 2074 6869 732e 0a20  tly uses this.. 
-0001d250: 2020 2020 2020 2020 2020 2023 2068 7474             # htt
-0001d260: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0001d270: 7465 6e73 6f72 666c 6f77 2f74 656e 736f  tensorflow/tenso
-0001d280: 7266 6c6f 772f 6973 7375 6573 2f33 3035  rflow/issues/305
-0001d290: 3634 0a20 2020 2020 2020 2020 2020 2069  64.            i
-0001d2a0: 6620 6f70 742e 7374 6172 7473 7769 7468  f opt.startswith
-0001d2b0: 2822 2d6c 3a6c 6962 2229 2061 6e64 206f  ("-l:lib") and o
-0001d2c0: 7074 2e65 6e64 7377 6974 6828 222e 6479  pt.endswith(".dy
-0001d2d0: 6c69 6222 293a 0a20 2020 2020 2020 2020  lib"):.         
-0001d2e0: 2020 2020 2020 2072 6574 7572 6e20 222d         return "-
-0001d2f0: 6c25 7322 2025 206f 7074 5b6c 656e 2822  l%s" % opt[len("
-0001d300: 2d6c 3a6c 6962 2229 203a 202d 6c65 6e28  -l:lib") : -len(
-0001d310: 222e 6479 6c69 6222 295d 0a20 2020 2020  ".dylib")].     
-0001d320: 2020 2072 6574 7572 6e20 6f70 740a 0a20     return opt.. 
-0001d330: 2020 2064 6566 205f 6d61 7962 655f 636f     def _maybe_co
-0001d340: 6d70 696c 655f 696e 6e65 7228 7365 6c66  mpile_inner(self
-0001d350: 293a 0a20 2020 2020 2020 2023 2044 6972  ):.        # Dir
-0001d360: 6563 746f 7279 2073 686f 756c 6420 6265  ectory should be
-0001d370: 2063 7265 6174 6564 2062 7920 7468 6520   created by the 
-0001d380: 6c6f 636b 696e 6720 6d65 6368 616e 6973  locking mechanis
-0001d390: 6d2e 0a20 2020 2020 2020 2061 7373 6572  m..        asser
-0001d3a0: 7420 6f73 2e70 6174 682e 6578 6973 7473  t os.path.exists
-0001d3b0: 2873 656c 662e 5f6d 6f64 5f70 6174 6829  (self._mod_path)
-0001d3c0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-0001d3d0: 656e 2873 656c 662e 5f63 5f66 696c 656e  en(self._c_filen
-0001d3e0: 616d 652c 2022 7722 2920 6173 2066 3a0a  ame, "w") as f:.
-0001d3f0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-0001d400: 6974 6528 7365 6c66 2e63 6f64 6529 0a20  ite(self.code). 
-0001d410: 2020 2020 2020 2063 6f6d 6d6f 6e5f 6f70         common_op
-0001d420: 7473 203d 205b 222d 7368 6172 6564 222c  ts = ["-shared",
-0001d430: 2022 2d4f 3222 5d0a 2020 2020 2020 2020   "-O2"].        
-0001d440: 636f 6d6d 6f6e 5f6f 7074 7320 2b3d 2073  common_opts += s
-0001d450: 656c 662e 5f65 7874 7261 5f63 6f6d 6d6f  elf._extra_commo
-0001d460: 6e5f 6f70 7473 2829 0a20 2020 2020 2020  n_opts().       
-0001d470: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
-0001d480: 203d 3d20 2264 6172 7769 6e22 3a0a 2020   == "darwin":.  
-0001d490: 2020 2020 2020 2020 2020 636f 6d6d 6f6e            common
-0001d4a0: 5f6f 7074 7320 2b3d 205b 222d 756e 6465  _opts += ["-unde
-0001d4b0: 6669 6e65 6422 2c20 2264 796e 616d 6963  fined", "dynamic
-0001d4c0: 5f6c 6f6f 6b75 7022 5d0a 2020 2020 2020  _lookup"].      
-0001d4d0: 2020 666f 7220 696e 636c 7564 655f 7061    for include_pa
-0001d4e0: 7468 2069 6e20 7365 6c66 2e5f 696e 636c  th in self._incl
-0001d4f0: 7564 655f 7061 7468 733a 0a20 2020 2020  ude_paths:.     
-0001d500: 2020 2020 2020 2063 6f6d 6d6f 6e5f 6f70         common_op
-0001d510: 7473 202b 3d20 5b22 2d49 222c 2069 6e63  ts += ["-I", inc
-0001d520: 6c75 6465 5f70 6174 685d 0a20 2020 2020  lude_path].     
-0001d530: 2020 2063 6f6d 7069 6c65 725f 6f70 7473     compiler_opts
-0001d540: 203d 205b 222d 6650 4943 222c 2022 2d76   = ["-fPIC", "-v
-0001d550: 225d 0a20 2020 2020 2020 2063 6f6d 6d6f  "].        commo
-0001d560: 6e5f 6f70 7473 202b 3d20 7365 6c66 2e5f  n_opts += self._
-0001d570: 7472 616e 7366 6f72 6d5f 636f 6d70 696c  transform_compil
-0001d580: 6572 5f6f 7074 7328 636f 6d70 696c 6572  er_opts(compiler
-0001d590: 5f6f 7074 7329 0a20 2020 2020 2020 2063  _opts).        c
-0001d5a0: 6f6d 6d6f 6e5f 6f70 7473 202b 3d20 5b22  ommon_opts += ["
-0001d5b0: 2d44 5f47 4c49 4243 5858 5f55 5345 5f43  -D_GLIBCXX_USE_C
-0001d5c0: 5858 3131 5f41 4249 3d25 6922 2025 2028  XX11_ABI=%i" % (
-0001d5d0: 3120 6966 2073 656c 662e 7573 655f 6378  1 if self.use_cx
-0001d5e0: 7831 315f 6162 6920 656c 7365 2030 295d  x11_abi else 0)]
-0001d5f0: 0a20 2020 2020 2020 2063 6f6d 6d6f 6e5f  .        common_
-0001d600: 6f70 7473 202b 3d20 5b22 2d44 2573 3d25  opts += ["-D%s=%
-0001d610: 7322 2025 2069 7465 6d20 666f 7220 6974  s" % item for it
-0001d620: 656d 2069 6e20 736f 7274 6564 2873 656c  em in sorted(sel
-0001d630: 662e 635f 6d61 6372 6f5f 6465 6669 6e65  f.c_macro_define
-0001d640: 732e 6974 656d 7328 2929 5d0a 2020 2020  s.items())].    
-0001d650: 2020 2020 636f 6d6d 6f6e 5f6f 7074 7320      common_opts 
-0001d660: 2b3d 205b 222d 6722 5d0a 2020 2020 2020  += ["-g"].      
-0001d670: 2020 6f70 7473 203d 2063 6f6d 6d6f 6e5f    opts = common_
-0001d680: 6f70 7473 202b 205b 7365 6c66 2e5f 635f  opts + [self._c_
-0001d690: 6669 6c65 6e61 6d65 2c20 222d 6f22 2c20  filename, "-o", 
-0001d6a0: 7365 6c66 2e5f 736f 5f66 696c 656e 616d  self._so_filenam
-0001d6b0: 655d 0a20 2020 2020 2020 206f 7074 7320  e].        opts 
-0001d6c0: 2b3d 206c 6973 7428 6d61 7028 7365 6c66  += list(map(self
-0001d6d0: 2e5f 7472 616e 7366 6f72 6d5f 6c64 5f66  ._transform_ld_f
-0001d6e0: 6c61 672c 2073 656c 662e 6c64 5f66 6c61  lag, self.ld_fla
-0001d6f0: 6773 2929 0a20 2020 2020 2020 2063 6d64  gs)).        cmd
-0001d700: 5f62 696e 203d 2073 656c 662e 5f67 6574  _bin = self._get
-0001d710: 5f63 6f6d 7069 6c65 725f 6269 6e28 290a  _compiler_bin().
-0001d720: 2020 2020 2020 2020 636d 645f 6172 6773          cmd_args
-0001d730: 203d 205b 636d 645f 6269 6e5d 202b 206f   = [cmd_bin] + o
-0001d740: 7074 730a 2020 2020 2020 2020 6672 6f6d  pts.        from
-0001d750: 2073 7562 7072 6f63 6573 7320 696d 706f   subprocess impo
-0001d760: 7274 2050 6f70 656e 2c20 5049 5045 2c20  rt Popen, PIPE, 
-0001d770: 5354 444f 5554 2c20 4361 6c6c 6564 5072  STDOUT, CalledPr
-0001d780: 6f63 6573 7345 7272 6f72 0a0a 2020 2020  ocessError..    
-0001d790: 2020 2020 7072 696e 7428 2225 7320 6361      print("%s ca
-0001d7a0: 6c6c 3a20 2573 2220 2520 2873 656c 662e  ll: %s" % (self.
-0001d7b0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
-0001d7c0: 5f5f 2c20 2220 222e 6a6f 696e 2863 6d64  __, " ".join(cmd
-0001d7d0: 5f61 7267 7329 292c 2066 696c 653d 7365  _args)), file=se
-0001d7e0: 6c66 2e5f 6c6f 675f 7374 7265 616d 290a  lf._log_stream).
-0001d7f0: 2020 2020 2020 2020 7072 6f63 203d 2050          proc = P
-0001d800: 6f70 656e 2863 6d64 5f61 7267 732c 2063  open(cmd_args, c
-0001d810: 7764 3d73 656c 662e 5f6d 6f64 5f70 6174  wd=self._mod_pat
-0001d820: 682c 2073 7464 6f75 743d 5049 5045 2c20  h, stdout=PIPE, 
-0001d830: 7374 6465 7272 3d53 5444 4f55 5429 0a20  stderr=STDOUT). 
-0001d840: 2020 2020 2020 2073 7464 6f75 742c 2073         stdout, s
-0001d850: 7464 6572 7220 3d20 7072 6f63 2e63 6f6d  tderr = proc.com
-0001d860: 6d75 6e69 6361 7465 2829 0a20 2020 2020  municate().     
-0001d870: 2020 2061 7373 6572 7420 7374 6465 7272     assert stderr
-0001d880: 2069 7320 4e6f 6e65 2020 2320 7368 6f75   is None  # shou
-0001d890: 6c64 206f 6e6c 7920 6861 7665 2073 7464  ld only have std
-0001d8a0: 6f75 740a 2020 2020 2020 2020 6966 2070  out.        if p
-0001d8b0: 726f 632e 7265 7475 726e 636f 6465 2021  roc.returncode !
-0001d8c0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0001d8d0: 2070 7269 6e74 2822 2573 3a20 2573 2066   print("%s: %s f
-0001d8e0: 6169 6c65 642e 2220 2520 2873 656c 662e  ailed." % (self.
-0001d8f0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
-0001d900: 5f5f 2c20 636d 645f 6269 6e29 290a 2020  __, cmd_bin)).  
-0001d910: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0001d920: 224f 7269 6769 6e61 6c20 7374 646f 7574  "Original stdout
-0001d930: 2f73 7464 6572 723a 2229 0a20 2020 2020  /stderr:").     
-0001d940: 2020 2020 2020 2070 7269 6e74 2873 7464         print(std
-0001d950: 6f75 742e 6465 636f 6465 2822 7574 6638  out.decode("utf8
-0001d960: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-0001d970: 7072 696e 7428 290a 2020 2020 2020 2020  print().        
-0001d980: 2020 2020 6966 2063 6d64 5f62 696e 2e65      if cmd_bin.e
-0001d990: 6e64 7377 6974 6828 222f 6e76 6363 2229  ndswith("/nvcc")
-0001d9a0: 2061 6e64 2062 2265 7272 6f72 3a20 636f   and b"error: co
-0001d9b0: 6e73 7465 7870 7220 6675 6e63 7469 6f6e  nstexpr function
-0001d9c0: 2072 6574 7572 6e20 6973 206e 6f6e 2d63   return is non-c
-0001d9d0: 6f6e 7374 616e 7422 2069 6e20 7374 646f  onstant" in stdo
-0001d9e0: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
-0001d9f0: 2020 2020 7072 696e 7428 2254 6869 7320      print("This 
-0001da00: 6d69 6768 7420 6265 2074 6865 2065 7272  might be the err
-0001da10: 6f72 3a20 6874 7470 733a 2f2f 6769 7468  or: https://gith
-0001da20: 7562 2e63 6f6d 2f74 656e 736f 7266 6c6f  ub.com/tensorflo
-0001da30: 772f 7465 6e73 6f72 666c 6f77 2f69 7373  w/tensorflow/iss
-0001da40: 7565 732f 3232 3736 3622 290a 2020 2020  ues/22766").    
-0001da50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0001da60: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0001da70: 6966 2063 6d64 5f62 696e 2e65 6e64 7377  if cmd_bin.endsw
-0001da80: 6974 6828 222f 6e76 6363 2229 2061 6e64  ith("/nvcc") and
-0001da90: 2062 2267 6363 2076 6572 7369 6f6e 7320   b"gcc versions 
-0001daa0: 6c61 7465 7220 7468 616e 2220 696e 2073  later than" in s
-0001dab0: 7464 6f75 743a 0a20 2020 2020 2020 2020  tdout:.         
-0001dac0: 2020 2020 2020 2070 7269 6e74 2822 596f         print("Yo
-0001dad0: 7572 2047 4343 2076 6572 7369 6f6e 206d  ur GCC version m
-0001dae0: 6967 6874 2062 6520 746f 6f20 6e65 772e  ight be too new.
-0001daf0: 2054 6869 7320 6973 2061 2070 726f 626c   This is a probl
-0001db00: 656d 2077 6974 6820 736f 6d65 206e 7663  em with some nvc
-0001db10: 6320 7665 7273 696f 6e73 2e22 290a 2020  c versions.").  
-0001db20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0001db30: 696e 7428 290a 2020 2020 2020 2020 2020  int().          
-0001db40: 2020 7261 6973 6520 4361 6c6c 6564 5072    raise CalledPr
-0001db50: 6f63 6573 7345 7272 6f72 2872 6574 7572  ocessError(retur
-0001db60: 6e63 6f64 653d 7072 6f63 2e72 6574 7572  ncode=proc.retur
-0001db70: 6e63 6f64 652c 2063 6d64 3d63 6d64 5f61  ncode, cmd=cmd_a
-0001db80: 7267 7329 0a20 2020 2020 2020 2061 7373  rgs).        ass
-0001db90: 6572 7420 6f73 2e70 6174 682e 6578 6973  ert os.path.exis
-0001dba0: 7473 2873 656c 662e 5f73 6f5f 6669 6c65  ts(self._so_file
-0001dbb0: 6e61 6d65 290a 2020 2020 2020 2020 7769  name).        wi
-0001dbc0: 7468 206f 7065 6e28 2225 732f 636f 6d70  th open("%s/comp
-0001dbd0: 696c 652e 6c6f 6722 2025 2073 656c 662e  ile.log" % self.
-0001dbe0: 5f6d 6f64 5f70 6174 682c 2022 7762 2229  _mod_path, "wb")
-0001dbf0: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
-0001dc00: 2020 2069 6620 7365 6c66 2e76 6572 626f     if self.verbo
-0001dc10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001dc20: 2020 2020 7072 696e 7428 2225 733a 2077      print("%s: w
-0001dc30: 7269 7465 2063 6f6d 7069 6c65 206c 6f67  rite compile log
-0001dc40: 2074 6f3a 2025 7322 2025 2028 7365 6c66   to: %s" % (self
-0001dc50: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-0001dc60: 655f 5f2c 2066 2e6e 616d 6529 290a 2020  e__, f.name)).  
-0001dc70: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-0001dc80: 6528 2822 2b20 2573 5c6e 2220 2520 2220  e(("+ %s\n" % " 
-0001dc90: 222e 6a6f 696e 2863 6d64 5f61 7267 7329  ".join(cmd_args)
-0001dca0: 292e 656e 636f 6465 2822 7574 6638 2229  ).encode("utf8")
-0001dcb0: 290a 2020 2020 2020 2020 2020 2020 662e  ).            f.
-0001dcc0: 7772 6974 6528 7374 646f 7574 290a 2020  write(stdout).  
-0001dcd0: 2020 2020 2020 7365 6c66 2e5f 7361 7665        self._save
-0001dce0: 5f69 6e66 6f28 290a 2020 2020 2020 2020  _info().        
-0001dcf0: 6173 7365 7274 206e 6f74 2073 656c 662e  assert not self.
-0001dd00: 5f6e 6565 645f 7265 636f 6d70 696c 6528  _need_recompile(
-0001dd10: 290a 0a20 2020 2064 6566 206c 6f61 645f  )..    def load_
-0001dd20: 6c69 625f 6374 7970 6573 2873 656c 6629  lib_ctypes(self)
-0001dd30: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0001dd40: 2020 2020 2020 3a72 7479 7065 3a20 6374        :rtype: ct
-0001dd50: 7970 6573 2e43 444c 4c0a 2020 2020 2020  ypes.CDLL.      
-0001dd60: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0001dd70: 2073 656c 662e 5f63 7479 7065 735f 6c69   self._ctypes_li
-0001dd80: 623a 0a20 2020 2020 2020 2020 2020 2072  b:.            r
-0001dd90: 6574 7572 6e20 7365 6c66 2e5f 6374 7970  eturn self._ctyp
-0001dda0: 6573 5f6c 6962 0a20 2020 2020 2020 2073  es_lib.        s
-0001ddb0: 656c 662e 5f6d 6179 6265 5f63 6f6d 7069  elf._maybe_compi
-0001ddc0: 6c65 2829 0a20 2020 2020 2020 2069 6d70  le().        imp
-0001ddd0: 6f72 7420 6374 7970 6573 0a0a 2020 2020  ort ctypes..    
-0001dde0: 2020 2020 7365 6c66 2e5f 6374 7970 6573      self._ctypes
-0001ddf0: 5f6c 6962 203d 2063 7479 7065 732e 6364  _lib = ctypes.cd
-0001de00: 6c6c 2e4c 6f61 644c 6962 7261 7279 2873  ll.LoadLibrary(s
-0001de10: 656c 662e 5f73 6f5f 6669 6c65 6e61 6d65  elf._so_filename
-0001de20: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0001de30: 2073 656c 662e 5f63 7479 7065 735f 6c69   self._ctypes_li
-0001de40: 620a 0a20 2020 2064 6566 2067 6574 5f6c  b..    def get_l
-0001de50: 6962 5f66 696c 656e 616d 6528 7365 6c66  ib_filename(self
-0001de60: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0001de70: 2020 2020 2020 203a 7274 7970 653a 2073         :rtype: s
-0001de80: 7472 0a20 2020 2020 2020 2022 2222 0a20  tr.        """. 
-0001de90: 2020 2020 2020 2073 656c 662e 5f6d 6179         self._may
-0001dea0: 6265 5f63 6f6d 7069 6c65 2829 0a20 2020  be_compile().   
-0001deb0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001dec0: 2e5f 736f 5f66 696c 656e 616d 650a 0a0a  ._so_filename...
-0001ded0: 2320 5365 6520 3a66 756e 633a 606d 6179  # See :func:`may
-0001dee0: 6265 5f72 6573 7461 7274 5f72 6574 7572  be_restart_retur
-0001def0: 6e6e 5f77 6974 685f 6174 666f 726b 5f70  nn_with_atfork_p
-0001df00: 6174 6368 6020 6265 6c6f 7720 666f 7220  atch` below for 
-0001df10: 7768 7920 796f 7520 6d69 6768 7420 7761  why you might wa
-0001df20: 6e74 2074 6f20 7573 6520 7468 6973 2e0a  nt to use this..
-0001df30: 5f63 5f63 6f64 655f 7061 7463 685f 6174  _c_code_patch_at
-0001df40: 666f 726b 203d 2022 2222 0a23 6465 6669  fork = """.#defi
-0001df50: 6e65 205f 474e 555f 534f 5552 4345 0a23  ne _GNU_SOURCE.#
-0001df60: 696e 636c 7564 6520 3c73 6368 6564 2e68  include <sched.h
-0001df70: 3e0a 2369 6e63 6c75 6465 203c 7369 676e  >.#include <sign
-0001df80: 616c 2e68 3e0a 2369 6e63 6c75 6465 203c  al.h>.#include <
-0001df90: 7379 732f 7379 7363 616c 6c2e 683e 0a23  sys/syscall.h>.#
-0001dfa0: 696e 636c 7564 6520 3c73 7464 696f 2e68  include <stdio.h
-0001dfb0: 3e0a 2369 6e63 6c75 6465 203c 7374 646c  >.#include <stdl
-0001dfc0: 6962 2e68 3e0a 2369 6e63 6c75 6465 203c  ib.h>.#include <
-0001dfd0: 756e 6973 7464 2e68 3e0a 0a2f 2f20 6874  unistd.h>..// ht
-0001dfe0: 7470 733a 2f2f 7374 6163 6b6f 7665 7266  tps://stackoverf
-0001dff0: 6c6f 772e 636f 6d2f 7175 6573 7469 6f6e  low.com/question
-0001e000: 732f 3436 3834 3534 3936 2f6c 642d 7072  s/46845496/ld-pr
-0001e010: 656c 6f61 642d 616e 642d 6c69 6e6b 6167  eload-and-linkag
-0001e020: 650a 2f2f 2068 7474 7073 3a2f 2f73 7461  e.// https://sta
-0001e030: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f71  ckoverflow.com/q
-0001e040: 7565 7374 696f 6e73 2f34 3638 3130 3539  uestions/4681059
-0001e050: 372f 666f 726b 6578 6563 2d77 6974 686f  7/forkexec-witho
-0001e060: 7574 2d61 7466 6f72 6b2d 6861 6e64 6c65  ut-atfork-handle
-0001e070: 7273 0a0a 696e 7420 7074 6872 6561 645f  rs..int pthread_
-0001e080: 6174 666f 726b 2876 6f69 6420 282a 7072  atfork(void (*pr
-0001e090: 6570 6172 6529 2876 6f69 6429 2c20 766f  epare)(void), vo
-0001e0a0: 6964 2028 2a70 6172 656e 7429 2876 6f69  id (*parent)(voi
-0001e0b0: 6429 2c20 766f 6964 2028 2a63 6869 6c64  d), void (*child
-0001e0c0: 2928 766f 6964 2929 207b 0a20 2070 7269  )(void)) {.  pri
-0001e0d0: 6e74 6628 2249 676e 6f72 696e 6720 7074  ntf("Ignoring pt
-0001e0e0: 6872 6561 645f 6174 666f 726b 2063 616c  hread_atfork cal
-0001e0f0: 6c21 5c5c 6e22 293b 0a20 2066 666c 7573  l!\\n");.  fflus
-0001e100: 6828 7374 646f 7574 293b 0a20 2072 6574  h(stdout);.  ret
-0001e110: 7572 6e20 303b 0a7d 0a0a 696e 7420 5f5f  urn 0;.}..int __
-0001e120: 7265 6769 7374 6572 5f61 7466 6f72 6b28  register_atfork(
-0001e130: 766f 6964 2028 2a70 7265 7061 7265 2928  void (*prepare)(
-0001e140: 766f 6964 292c 2076 6f69 6420 282a 7061  void), void (*pa
-0001e150: 7265 6e74 2928 766f 6964 292c 2076 6f69  rent)(void), voi
-0001e160: 6420 282a 6368 696c 6429 2876 6f69 6429  d (*child)(void)
-0001e170: 2920 7b0a 2020 7072 696e 7466 2822 4967  ) {.  printf("Ig
-0001e180: 6e6f 7269 6e67 205f 5f72 6567 6973 7465  noring __registe
-0001e190: 725f 6174 666f 726b 2063 616c 6c21 5c5c  r_atfork call!\\
-0001e1a0: 6e22 293b 0a20 2066 666c 7573 6828 7374  n");.  fflush(st
-0001e1b0: 646f 7574 293b 0a20 2072 6574 7572 6e20  dout);.  return 
-0001e1c0: 303b 0a7d 0a0a 2f2f 2041 6e6f 7468 6572  0;.}..// Another
-0001e1d0: 2077 6179 2074 6f20 6967 6e6f 7265 2061   way to ignore a
-0001e1e0: 7466 6f72 6b20 6861 6e64 6c65 7273 3a20  tfork handlers: 
-0001e1f0: 4f76 6572 7269 6465 2066 6f72 6b2e 0a23  Override fork..#
-0001e200: 6966 6465 6620 5f5f 6c69 6e75 785f 5f20  ifdef __linux__ 
-0001e210: 2f2f 206f 6e6c 7920 776f 726b 7320 6f6e  // only works on
-0001e220: 204c 696e 7578 2063 7572 7265 6e74 6c79   Linux currently
-0001e230: 0a70 6964 5f74 2066 6f72 6b28 766f 6964  .pid_t fork(void
-0001e240: 2920 7b0a 2020 7265 7475 726e 2073 7973  ) {.  return sys
-0001e250: 6361 6c6c 2853 5953 5f63 6c6f 6e65 2c20  call(SYS_clone, 
-0001e260: 5349 4743 484c 442c 2030 293b 0a7d 0a23  SIGCHLD, 0);.}.#
-0001e270: 656e 6469 660a 0a5f 5f61 7474 7269 6275  endif..__attribu
-0001e280: 7465 5f5f 2828 636f 6e73 7472 7563 746f  te__((constructo
-0001e290: 7229 290a 766f 6964 2070 6174 6368 5f61  r)).void patch_a
-0001e2a0: 7466 6f72 6b5f 696e 6974 2829 207b 0a20  tfork_init() {. 
-0001e2b0: 2073 6574 656e 7628 225f 5f52 4554 5552   setenv("__RETUR
-0001e2c0: 4e4e 5f41 5446 4f52 4b5f 5041 5443 4845  NN_ATFORK_PATCHE
-0001e2d0: 4422 2c20 2231 222c 2031 293b 0a7d 0a22  D", "1", 1);.}."
-0001e2e0: 2222 0a0a 0a64 6566 2067 6574 5f70 6174  ""...def get_pat
-0001e2f0: 6368 5f61 7466 6f72 6b5f 6c69 6228 293a  ch_atfork_lib():
-0001e300: 0a20 2020 2022 2222 0a20 2020 203a 7265  .    """.    :re
-0001e310: 7475 726e 3a20 7061 7468 2074 6f20 6f75  turn: path to ou
-0001e320: 7220 7061 7463 685f 6174 666f 726b 206c  r patch_atfork l
-0001e330: 6962 2e20 7365 6520 3a66 756e 633a 606d  ib. see :func:`m
-0001e340: 6179 6265 5f72 6573 7461 7274 5f72 6574  aybe_restart_ret
-0001e350: 7572 6e6e 5f77 6974 685f 6174 666f 726b  urnn_with_atfork
-0001e360: 5f70 6174 6368 600a 2020 2020 3a72 7479  _patch`.    :rty
-0001e370: 7065 3a20 7374 720a 2020 2020 2222 220a  pe: str.    """.
-0001e380: 2020 2020 6e61 7469 7665 203d 204e 6174      native = Nat
-0001e390: 6976 6543 6f64 6543 6f6d 7069 6c65 7228  iveCodeCompiler(
-0001e3a0: 6261 7365 5f6e 616d 653d 2270 6174 6368  base_name="patch
-0001e3b0: 5f61 7466 6f72 6b22 2c20 636f 6465 5f76  _atfork", code_v
-0001e3c0: 6572 7369 6f6e 3d32 2c20 636f 6465 3d5f  ersion=2, code=_
-0001e3d0: 635f 636f 6465 5f70 6174 6368 5f61 7466  c_code_patch_atf
-0001e3e0: 6f72 6b2c 2069 735f 6370 703d 4661 6c73  ork, is_cpp=Fals
-0001e3f0: 6529 0a20 2020 2066 6e20 3d20 6e61 7469  e).    fn = nati
-0001e400: 7665 2e67 6574 5f6c 6962 5f66 696c 656e  ve.get_lib_filen
-0001e410: 616d 6528 290a 2020 2020 7265 7475 726e  ame().    return
-0001e420: 2066 6e0a 0a0a 6465 6620 7265 7374 6172   fn...def restar
-0001e430: 745f 7265 7475 726e 6e28 293a 0a20 2020  t_returnn():.   
-0001e440: 2022 2222 0a20 2020 2052 6573 7461 7274   """.    Restart
-0001e450: 7320 5245 5455 524e 4e2e 0a20 2020 2022  s RETURNN..    "
-0001e460: 2222 0a20 2020 206c 6f67 2e66 6c75 7368  "".    log.flush
-0001e470: 2829 0a20 2020 2073 7973 2e73 7464 6f75  ().    sys.stdou
-0001e480: 742e 666c 7573 6828 290a 2020 2020 7379  t.flush().    sy
-0001e490: 732e 7374 6465 7272 2e66 6c75 7368 2829  s.stderr.flush()
-0001e4a0: 0a20 2020 2023 2068 7474 7073 3a2f 2f73  .    # https://s
-0001e4b0: 7461 636b 6f76 6572 666c 6f77 2e63 6f6d  tackoverflow.com
-0001e4c0: 2f71 7565 7374 696f 6e73 2f37 3233 3335  /questions/72335
-0001e4d0: 3930 342f 7369 6d70 6c65 2d77 6179 2d74  904/simple-way-t
-0001e4e0: 6f2d 7265 7374 6172 742d 6170 706c 6963  o-restart-applic
-0001e4f0: 6174 696f 6e0a 2020 2020 636c 6f73 655f  ation.    close_
-0001e500: 616c 6c5f 6664 735f 6578 6365 7074 287b  all_fds_except({
-0001e510: 302c 2031 2c20 327d 290a 2020 2020 6f73  0, 1, 2}).    os
-0001e520: 2e65 7865 6376 2873 7973 2e65 7865 6375  .execv(sys.execu
-0001e530: 7461 626c 652c 205b 7379 732e 6578 6563  table, [sys.exec
-0001e540: 7574 6162 6c65 5d20 2b20 7379 732e 6172  utable] + sys.ar
-0001e550: 6776 290a 2020 2020 7261 6973 6520 4578  gv).    raise Ex
-0001e560: 6365 7074 696f 6e28 2272 6573 7461 7274  ception("restart
-0001e570: 5f72 6574 7572 6e6e 3a20 6578 6563 7620  _returnn: execv 
-0001e580: 6661 696c 6564 2229 0a0a 0a64 6566 206d  failed")...def m
-0001e590: 6179 6265 5f72 6573 7461 7274 5f72 6574  aybe_restart_ret
-0001e5a0: 7572 6e6e 5f77 6974 685f 6174 666f 726b  urnn_with_atfork
-0001e5b0: 5f70 6174 6368 2829 3a0a 2020 2020 2222  _patch():.    ""
-0001e5c0: 220a 2020 2020 5768 6174 2077 6520 7761  ".    What we wa
-0001e5d0: 6e74 3a20 7375 6270 726f 6365 7373 2e50  nt: subprocess.P
-0001e5e0: 6f70 656e 2074 6f20 616c 7761 7973 2077  open to always w
-0001e5f0: 6f72 6b2e 0a20 2020 2050 726f 626c 656d  ork..    Problem
-0001e600: 3a20 4974 2075 7365 7320 666f 726b 2b65  : It uses fork+e
-0001e610: 7865 6320 696e 7465 726e 616c 6c79 2069  xec internally i
-0001e620: 6e20 7375 6270 726f 6365 7373 5f66 6f72  n subprocess_for
-0001e630: 6b5f 6578 6563 2c20 7669 6120 5f70 6f73  k_exec, via _pos
-0001e640: 6978 7375 6270 726f 6365 7373 2e66 6f72  ixsubprocess.for
-0001e650: 6b5f 6578 6563 2e0a 2020 2020 5468 6174  k_exec..    That
-0001e660: 2069 7320 6120 7072 6f62 6c65 6d20 6265   is a problem be
-0001e670: 6361 7573 6520 666f 726b 2063 616e 2074  cause fork can t
-0001e680: 7269 6767 6572 2061 6e79 2061 7466 6f72  rigger any atfor
-0001e690: 6b20 6861 6e64 6c65 7273 2072 6567 6973  k handlers regis
-0001e6a0: 7465 7265 6420 7669 6120 7074 6872 6561  tered via pthrea
-0001e6b0: 645f 6174 666f 726b 2c0a 2020 2020 616e  d_atfork,.    an
-0001e6c0: 6420 7468 6f73 6520 6361 6e20 6372 6173  d those can cras
-0001e6d0: 682f 6465 6164 6c6f 636b 2069 6e20 736f  h/deadlock in so
-0001e6e0: 6d65 2063 6173 6573 2e0a 0a20 2020 2068  me cases...    h
-0001e6f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0001e700: 6d2f 7465 6e73 6f72 666c 6f77 2f74 656e  m/tensorflow/ten
-0001e710: 736f 7266 6c6f 772f 6973 7375 6573 2f31  sorflow/issues/1
-0001e720: 3338 3032 0a20 2020 2068 7474 7073 3a2f  3802.    https:/
-0001e730: 2f67 6974 6875 622e 636f 6d2f 7869 616e  /github.com/xian
-0001e740: 7969 2f4f 7065 6e42 4c41 532f 6973 7375  yi/OpenBLAS/issu
-0001e750: 6573 2f32 3430 0a20 2020 2068 7474 7073  es/240.    https
-0001e760: 3a2f 2f74 7261 632e 7361 6765 6d61 7468  ://trac.sagemath
-0001e770: 2e6f 7267 2f74 6963 6b65 742f 3232 3032  .org/ticket/2202
-0001e780: 310a 2020 2020 6874 7470 733a 2f2f 6275  1.    https://bu
-0001e790: 6773 2e70 7974 686f 6e2e 6f72 672f 6973  gs.python.org/is
-0001e7a0: 7375 6533 3138 3134 0a20 2020 2068 7474  sue31814.    htt
-0001e7b0: 7073 3a2f 2f73 7461 636b 6f76 6572 666c  ps://stackoverfl
-0001e7c0: 6f77 2e63 6f6d 2f71 7565 7374 696f 6e73  ow.com/questions
-0001e7d0: 2f34 3638 3435 3439 362f 6c64 2d70 7265  /46845496/ld-pre
-0001e7e0: 6c6f 6164 2d61 6e64 2d6c 696e 6b61 6765  load-and-linkage
-0001e7f0: 0a20 2020 2068 7474 7073 3a2f 2f73 7461  .    https://sta
-0001e800: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f71  ckoverflow.com/q
-0001e810: 7565 7374 696f 6e73 2f34 3638 3130 3539  uestions/4681059
-0001e820: 372f 666f 726b 6578 6563 2d77 6974 686f  7/forkexec-witho
-0001e830: 7574 2d61 7466 6f72 6b2d 6861 6e64 6c65  ut-atfork-handle
-0001e840: 7273 0a0a 2020 2020 5468 6520 736f 6c75  rs..    The solu
-0001e850: 7469 6f6e 2068 6572 653a 204a 7573 7420  tion here: Just 
-0001e860: 6f76 6572 7269 6465 2070 7468 7265 6164  override pthread
-0001e870: 5f61 7466 6f72 6b2c 2076 6961 204c 445f  _atfork, via LD_
-0001e880: 5052 454c 4f41 442e 0a20 2020 204e 6f74  PRELOAD..    Not
-0001e890: 6520 7468 6174 2069 6e20 736f 6d65 2063  e that in some c
-0001e8a0: 6173 6573 2c20 7468 6973 2069 7320 6e6f  ases, this is no
-0001e8b0: 7420 656e 6f75 6768 2028 7365 6520 7468  t enough (see th
-0001e8c0: 6520 534f 2064 6973 6375 7373 696f 6e29  e SO discussion)
-0001e8d0: 2c0a 2020 2020 736f 2077 6520 616c 736f  ,.    so we also
-0001e8e0: 206f 7665 7277 7269 7465 2066 6f72 6b20   overwrite fork 
-0001e8f0: 6974 7365 6c66 2e0a 2020 2020 5365 6520  itself..    See 
-0001e900: 616c 736f 2074 6573 7473 2f74 6573 745f  also tests/test_
-0001e910: 666f 726b 5f65 7865 632e 7079 2066 6f72  fork_exec.py for
-0001e920: 2061 2064 656d 6f2e 0a20 2020 2022 2222   a demo..    """
-0001e930: 0a20 2020 2069 6620 6f73 2e65 6e76 6972  .    if os.envir
-0001e940: 6f6e 2e67 6574 2822 5f5f 5245 5455 524e  on.get("__RETURN
-0001e950: 4e5f 4154 464f 524b 5f50 4154 4348 4544  N_ATFORK_PATCHED
-0001e960: 2229 203d 3d20 2231 223a 0a20 2020 2020  ") == "1":.     
-0001e970: 2020 2070 7269 6e74 2822 5275 6e6e 696e     print("Runnin
-0001e980: 6720 7769 7468 2070 6174 6368 6564 2061  g with patched a
-0001e990: 7466 6f72 6b2e 2229 0a20 2020 2020 2020  tfork.").       
-0001e9a0: 2072 6574 7572 6e0a 2020 2020 6966 206f   return.    if o
-0001e9b0: 732e 656e 7669 726f 6e2e 6765 7428 225f  s.environ.get("_
-0001e9c0: 5f52 4554 5552 4e4e 5f54 5259 5f41 5446  _RETURNN_TRY_ATF
-0001e9d0: 4f52 4b5f 5041 5443 4845 4422 2920 3d3d  ORK_PATCHED") ==
-0001e9e0: 2022 3122 3a0a 2020 2020 2020 2020 7072   "1":.        pr
-0001e9f0: 696e 7428 2250 6174 6368 696e 6720 6174  int("Patching at
-0001ea00: 666f 726b 2064 6964 206e 6f74 2077 6f72  fork did not wor
-0001ea10: 6b21 2057 696c 6c20 636f 6e74 696e 7565  k! Will continue
-0001ea20: 2061 6e79 7761 792e 2229 0a20 2020 2020   anyway.").     
-0001ea30: 2020 2072 6574 7572 6e0a 2020 2020 6c69     return.    li
-0001ea40: 6220 3d20 6765 745f 7061 7463 685f 6174  b = get_patch_at
-0001ea50: 666f 726b 5f6c 6962 2829 0a20 2020 2065  fork_lib().    e
-0001ea60: 6e76 203d 206f 732e 656e 7669 726f 6e2e  nv = os.environ.
-0001ea70: 636f 7079 2829 0a20 2020 2065 6e76 5b22  copy().    env["
-0001ea80: 4459 4c44 5f49 4e53 4552 545f 4c49 4252  DYLD_INSERT_LIBR
-0001ea90: 4152 4945 5322 2069 6620 7379 732e 706c  ARIES" if sys.pl
-0001eaa0: 6174 666f 726d 203d 3d20 2264 6172 7769  atform == "darwi
-0001eab0: 6e22 2065 6c73 6520 224c 445f 5052 454c  n" else "LD_PREL
-0001eac0: 4f41 4422 5d20 3d20 6c69 620a 2020 2020  OAD"] = lib.    
-0001ead0: 656e 765b 225f 5f52 4554 5552 4e4e 5f54  env["__RETURNN_T
-0001eae0: 5259 5f41 5446 4f52 4b5f 5041 5443 4845  RY_ATFORK_PATCHE
-0001eaf0: 4422 5d20 3d20 2231 220a 2020 2020 7072  D"] = "1".    pr
-0001eb00: 696e 7428 2252 6573 7461 7274 696e 6720  int("Restarting 
-0001eb10: 5265 7475 726e 6e20 7769 7468 2061 7466  Returnn with atf
-0001eb20: 6f72 6b20 7061 7463 682e 2e2e 222c 2073  ork patch...", s
-0001eb30: 7973 2e65 7865 6375 7461 626c 652c 2073  ys.executable, s
-0001eb40: 7973 2e61 7267 7629 0a20 2020 2073 7973  ys.argv).    sys
-0001eb50: 2e73 7464 6f75 742e 666c 7573 6828 290a  .stdout.flush().
-0001eb60: 2020 2020 6f73 2e65 7865 6376 7065 2873      os.execvpe(s
-0001eb70: 7973 2e65 7865 6375 7461 626c 652c 205b  ys.executable, [
-0001eb80: 7379 732e 6578 6563 7574 6162 6c65 5d20  sys.executable] 
-0001eb90: 2b20 7379 732e 6172 6776 2c20 656e 7629  + sys.argv, env)
-0001eba0: 0a20 2020 2070 7269 6e74 2822 6578 6563  .    print("exec
-0001ebb0: 7670 6520 6469 6420 6e6f 7420 776f 726b  vpe did not work
-0001ebc0: 3f22 290a 0a0a 6465 6620 636c 6f73 655f  ?")...def close_
-0001ebd0: 616c 6c5f 6664 735f 6578 6365 7074 2865  all_fds_except(e
-0001ebe0: 7863 6570 745f 6664 7329 3a0a 2020 2020  xcept_fds):.    
-0001ebf0: 2222 220a 2020 2020 4361 6c6c 7320 6f73  """.    Calls os
-0001ec00: 2e63 6c6f 7365 7261 6e67 6520 6578 6365  .closerange exce
-0001ec10: 7074 2066 6f72 2074 6865 2067 6976 656e  pt for the given
-0001ec20: 2066 6473 2e0a 2020 2020 436f 6465 2061   fds..    Code a
-0001ec30: 646f 7074 6564 2061 6e64 2065 7874 656e  dopted and exten
-0001ec40: 6465 6420 6672 6f6d 206d 756c 7469 7072  ded from multipr
-0001ec50: 6f63 6573 7369 6e67 2e75 7469 6c2e 636c  ocessing.util.cl
-0001ec60: 6f73 655f 616c 6c5f 6664 735f 6578 6365  ose_all_fds_exce
-0001ec70: 7074 2e0a 0a20 2020 203a 7061 7261 6d20  pt...    :param 
-0001ec80: 7479 7069 6e67 2e43 6f6c 6c65 6374 696f  typing.Collectio
-0001ec90: 6e5b 696e 745d 2065 7863 6570 745f 6664  n[int] except_fd
-0001eca0: 733a 2075 7375 616c 6c79 2061 7420 6c65  s: usually at le
-0001ecb0: 6173 7420 7b30 2c31 2c32 7d0a 2020 2020  ast {0,1,2}.    
-0001ecc0: 2222 220a 2020 2020 2320 6e6f 696e 7370  """.    # noinsp
-0001ecd0: 6563 7469 6f6e 2050 7942 726f 6164 4578  ection PyBroadEx
-0001ece0: 6365 7074 696f 6e0a 2020 2020 7472 793a  ception.    try:
-0001ecf0: 0a20 2020 2020 2020 206d 6178 5f66 6420  .        max_fd 
-0001ed00: 3d20 6f73 2e73 7973 636f 6e66 2822 5343  = os.sysconf("SC
-0001ed10: 5f4f 5045 4e5f 4d41 5822 290a 2020 2020  _OPEN_MAX").    
-0001ed20: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0001ed30: 3a0a 2020 2020 2020 2020 6d61 785f 6664  :.        max_fd
-0001ed40: 203d 2032 3536 0a0a 2020 2020 6578 6365   = 256..    exce
-0001ed50: 7074 5f66 6473 203d 2073 6f72 7465 6428  pt_fds = sorted(
-0001ed60: 6c69 7374 2865 7863 6570 745f 6664 7329  list(except_fds)
-0001ed70: 202b 205b 2d31 2c20 6d61 785f 6664 5d29   + [-1, max_fd])
-0001ed80: 0a20 2020 2061 7373 6572 7420 6578 6365  .    assert exce
-0001ed90: 7074 5f66 6473 5b30 5d20 3d3d 202d 3120  pt_fds[0] == -1 
-0001eda0: 616e 6420 6578 6365 7074 5f66 6473 5b2d  and except_fds[-
-0001edb0: 315d 203d 3d20 6d61 785f 6664 2c20 2266  1] == max_fd, "f
-0001edc0: 6420 696e 7661 6c69 6422 0a0a 2020 2020  d invalid"..    
-0001edd0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-0001ede0: 656e 2865 7863 6570 745f 6664 7329 202d  en(except_fds) -
-0001edf0: 2031 293a 0a20 2020 2020 2020 2069 6620   1):.        if 
-0001ee00: 6578 6365 7074 5f66 6473 5b69 5d20 2b20  except_fds[i] + 
-0001ee10: 3120 3c20 6578 6365 7074 5f66 6473 5b69  1 < except_fds[i
-0001ee20: 202b 2031 5d3a 0a20 2020 2020 2020 2020   + 1]:.         
-0001ee30: 2020 206f 732e 636c 6f73 6572 616e 6765     os.closerange
-0001ee40: 2865 7863 6570 745f 6664 735b 695d 202b  (except_fds[i] +
-0001ee50: 2031 2c20 6578 6365 7074 5f66 6473 5b69   1, except_fds[i
-0001ee60: 202b 2031 5d29 0a0a 0a63 6c61 7373 2053   + 1])...class S
-0001ee70: 7461 7473 3a0a 2020 2020 2222 220a 2020  tats:.    """.  
-0001ee80: 2020 436f 6c6c 6563 7473 206d 6561 6e20    Collects mean 
-0001ee90: 616e 6420 7661 7269 616e 6365 2c20 7275  and variance, ru
-0001eea0: 6e6e 696e 6720 6176 6572 6167 652e 0a0a  nning average...
-0001eeb0: 2020 2020 6874 7470 733a 2f2f 656e 2e77      https://en.w
-0001eec0: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-0001eed0: 692f 416c 676f 7269 7468 6d73 5f66 6f72  i/Algorithms_for
-0001eee0: 5f63 616c 6375 6c61 7469 6e67 5f76 6172  _calculating_var
-0001eef0: 6961 6e63 650a 2020 2020 2222 220a 0a20  iance.    """.. 
-0001ef00: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0001ef10: 7365 6c66 2c20 666f 726d 6174 5f73 7472  self, format_str
-0001ef20: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0001ef30: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-0001ef40: 616d 204e 6f6e 657c 2828 666c 6f61 747c  am None|((float|
-0001ef50: 6e75 6d70 792e 6e64 6172 7261 7929 2d3e  numpy.ndarray)->
-0001ef60: 7374 7229 2066 6f72 6d61 745f 7374 723a  str) format_str:
-0001ef70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001ef80: 2020 2020 2073 656c 662e 666f 726d 6174       self.format
-0001ef90: 5f73 7472 203d 2066 6f72 6d61 745f 7374  _str = format_st
-0001efa0: 7220 6f72 2073 7472 0a20 2020 2020 2020  r or str.       
-0001efb0: 2073 656c 662e 6d65 616e 203d 2030 2e30   self.mean = 0.0
-0001efc0: 0a20 2020 2020 2020 2073 656c 662e 6d65  .        self.me
-0001efd0: 616e 5f73 7120 3d20 302e 300a 2020 2020  an_sq = 0.0.    
-0001efe0: 2020 2020 7365 6c66 2e76 6172 203d 2030      self.var = 0
-0001eff0: 2e30 0a20 2020 2020 2020 2073 656c 662e  .0.        self.
-0001f000: 6d69 6e20 3d20 4e6f 6e65 0a20 2020 2020  min = None.     
-0001f010: 2020 2073 656c 662e 6d61 7820 3d20 4e6f     self.max = No
-0001f020: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-0001f030: 746f 7461 6c5f 6461 7461 5f6c 656e 203d  total_data_len =
-0001f040: 2030 0a20 2020 2020 2020 2073 656c 662e   0.        self.
-0001f050: 6e75 6d5f 7365 7173 203d 2030 0a0a 2020  num_seqs = 0..  
-0001f060: 2020 6465 6620 5f5f 7374 725f 5f28 7365    def __str__(se
-0001f070: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-0001f080: 7365 6c66 2e6e 756d 5f73 6571 7320 3e20  self.num_seqs > 
-0001f090: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
-0001f0a0: 6620 7365 6c66 2e6e 756d 5f73 6571 7320  f self.num_seqs 
-0001f0b0: 3d3d 2073 656c 662e 746f 7461 6c5f 6461  == self.total_da
-0001f0c0: 7461 5f6c 656e 3a0a 2020 2020 2020 2020  ta_len:.        
-0001f0d0: 2020 2020 2020 2020 6578 7472 615f 7374          extra_st
-0001f0e0: 7220 3d20 2261 7667 5f64 6174 615f 6c65  r = "avg_data_le
-0001f0f0: 6e3d 3122 0a20 2020 2020 2020 2020 2020  n=1".           
-0001f100: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001f110: 2020 2020 2020 2065 7874 7261 5f73 7472         extra_str
-0001f120: 203d 2022 746f 7461 6c5f 6461 7461 5f6c   = "total_data_l
-0001f130: 656e 3d25 692c 2061 7667 5f64 6174 615f  en=%i, avg_data_
-0001f140: 6c65 6e3d 2566 2220 2520 280a 2020 2020  len=%f" % (.    
-0001f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f160: 7365 6c66 2e74 6f74 616c 5f64 6174 615f  self.total_data_
-0001f170: 6c65 6e2c 0a20 2020 2020 2020 2020 2020  len,.           
-0001f180: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-0001f190: 656c 662e 746f 7461 6c5f 6461 7461 5f6c  elf.total_data_l
-0001f1a0: 656e 2920 2f20 7365 6c66 2e6e 756d 5f73  en) / self.num_s
-0001f1b0: 6571 732c 0a20 2020 2020 2020 2020 2020  eqs,.           
-0001f1c0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0001f1d0: 2020 2072 6574 7572 6e20 2253 7461 7473     return "Stats
-0001f1e0: 286d 6561 6e3d 2573 2c20 7374 645f 6465  (mean=%s, std_de
-0001f1f0: 763d 2573 2c20 6d69 6e3d 2573 2c20 6d61  v=%s, min=%s, ma
-0001f200: 783d 2573 2c20 6e75 6d5f 7365 7173 3d25  x=%s, num_seqs=%
-0001f210: 692c 2025 7329 2220 2520 280a 2020 2020  i, %s)" % (.    
-0001f220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001f230: 2e66 6f72 6d61 745f 7374 7228 7365 6c66  .format_str(self
-0001f240: 2e67 6574 5f6d 6561 6e28 2929 2c0a 2020  .get_mean()),.  
-0001f250: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001f260: 6c66 2e66 6f72 6d61 745f 7374 7228 7365  lf.format_str(se
-0001f270: 6c66 2e67 6574 5f73 7464 5f64 6576 2829  lf.get_std_dev()
-0001f280: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0001f290: 2020 2073 656c 662e 666f 726d 6174 5f73     self.format_s
-0001f2a0: 7472 2873 656c 662e 6d69 6e29 2c0a 2020  tr(self.min),.  
-0001f2b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001f2c0: 6c66 2e66 6f72 6d61 745f 7374 7228 7365  lf.format_str(se
-0001f2d0: 6c66 2e6d 6178 292c 0a20 2020 2020 2020  lf.max),.       
-0001f2e0: 2020 2020 2020 2020 2073 656c 662e 6e75           self.nu
-0001f2f0: 6d5f 7365 7173 2c0a 2020 2020 2020 2020  m_seqs,.        
-0001f300: 2020 2020 2020 2020 6578 7472 615f 7374          extra_st
-0001f310: 722c 0a20 2020 2020 2020 2020 2020 2029  r,.            )
-0001f320: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001f330: 2253 7461 7473 286e 756d 5f73 6571 733d  "Stats(num_seqs=
-0001f340: 3029 220a 0a20 2020 2064 6566 2063 6f6c  0)"..    def col
-0001f350: 6c65 6374 2873 656c 662c 2064 6174 6129  lect(self, data)
-0001f360: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0001f370: 2020 2020 2020 3a70 6172 616d 206e 756d        :param num
-0001f380: 7079 2e6e 6461 7272 6179 7c6c 6973 745b  py.ndarray|list[
-0001f390: 696e 745d 7c6c 6973 745b 666c 6f61 745d  int]|list[float]
-0001f3a0: 2064 6174 613a 2073 6861 7065 2028 7469   data: shape (ti
-0001f3b0: 6d65 2c20 6469 6d29 206f 7220 2874 696d  me, dim) or (tim
-0001f3c0: 652c 290a 2020 2020 2020 2020 2222 220a  e,).        """.
-0001f3d0: 2020 2020 2020 2020 696d 706f 7274 206e          import n
-0001f3e0: 756d 7079 0a0a 2020 2020 2020 2020 6966  umpy..        if
-0001f3f0: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
-0001f400: 2c20 286c 6973 742c 2074 7570 6c65 2929  , (list, tuple))
-0001f410: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
-0001f420: 7461 203d 206e 756d 7079 2e61 7272 6179  ta = numpy.array
-0001f430: 2864 6174 6129 0a20 2020 2020 2020 2061  (data).        a
-0001f440: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-0001f450: 2864 6174 612c 206e 756d 7079 2e6e 6461  (data, numpy.nda
-0001f460: 7272 6179 290a 2020 2020 2020 2020 6173  rray).        as
-0001f470: 7365 7274 2064 6174 612e 6e64 696d 203e  sert data.ndim >
-0001f480: 3d20 310a 2020 2020 2020 2020 6966 2064  = 1.        if d
-0001f490: 6174 612e 7368 6170 655b 305d 203d 3d20  ata.shape[0] == 
-0001f4a0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-0001f4b0: 6574 7572 6e0a 2020 2020 2020 2020 7365  eturn.        se
-0001f4c0: 6c66 2e6e 756d 5f73 6571 7320 2b3d 2031  lf.num_seqs += 1
-0001f4d0: 0a20 2020 2020 2020 2064 6174 615f 6d69  .        data_mi
-0001f4e0: 6e20 3d20 6e75 6d70 792e 6d69 6e28 6461  n = numpy.min(da
-0001f4f0: 7461 2c20 6178 6973 3d30 290a 2020 2020  ta, axis=0).    
-0001f500: 2020 2020 6461 7461 5f6d 6178 203d 206e      data_max = n
-0001f510: 756d 7079 2e6d 6178 2864 6174 612c 2061  umpy.max(data, a
-0001f520: 7869 733d 3029 0a20 2020 2020 2020 2069  xis=0).        i
-0001f530: 6620 7365 6c66 2e6d 696e 2069 7320 4e6f  f self.min is No
-0001f540: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0001f550: 7365 6c66 2e6d 696e 203d 2064 6174 615f  self.min = data_
-0001f560: 6d69 6e0a 2020 2020 2020 2020 2020 2020  min.            
-0001f570: 7365 6c66 2e6d 6178 203d 2064 6174 615f  self.max = data_
-0001f580: 6d61 780a 2020 2020 2020 2020 656c 7365  max.        else
-0001f590: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001f5a0: 6c66 2e6d 696e 203d 206e 756d 7079 2e6d  lf.min = numpy.m
-0001f5b0: 696e 696d 756d 2873 656c 662e 6d69 6e2c  inimum(self.min,
-0001f5c0: 2064 6174 615f 6d69 6e29 0a20 2020 2020   data_min).     
-0001f5d0: 2020 2020 2020 2073 656c 662e 6d61 7820         self.max 
-0001f5e0: 3d20 6e75 6d70 792e 6d61 7869 6d75 6d28  = numpy.maximum(
-0001f5f0: 7365 6c66 2e6d 6178 2c20 6461 7461 5f6d  self.max, data_m
-0001f600: 6178 290a 2020 2020 2020 2020 6e65 775f  ax).        new_
-0001f610: 746f 7461 6c5f 6461 7461 5f6c 656e 203d  total_data_len =
-0001f620: 2073 656c 662e 746f 7461 6c5f 6461 7461   self.total_data
-0001f630: 5f6c 656e 202b 2064 6174 612e 7368 6170  _len + data.shap
-0001f640: 655b 305d 0a20 2020 2020 2020 206d 6561  e[0].        mea
-0001f650: 6e5f 6469 6666 203d 206e 756d 7079 2e6d  n_diff = numpy.m
-0001f660: 6561 6e28 6461 7461 2c20 6178 6973 3d30  ean(data, axis=0
-0001f670: 2920 2d20 7365 6c66 2e6d 6561 6e0a 2020  ) - self.mean.  
-0001f680: 2020 2020 2020 6d5f 6120 3d20 7365 6c66        m_a = self
-0001f690: 2e76 6172 202a 2073 656c 662e 746f 7461  .var * self.tota
-0001f6a0: 6c5f 6461 7461 5f6c 656e 0a20 2020 2020  l_data_len.     
-0001f6b0: 2020 206d 5f62 203d 206e 756d 7079 2e76     m_b = numpy.v
-0001f6c0: 6172 2864 6174 612c 2061 7869 733d 3029  ar(data, axis=0)
-0001f6d0: 202a 2064 6174 612e 7368 6170 655b 305d   * data.shape[0]
-0001f6e0: 0a20 2020 2020 2020 206d 3220 3d20 6d5f  .        m2 = m_
-0001f6f0: 6120 2b20 6d5f 6220 2b20 6d65 616e 5f64  a + m_b + mean_d
-0001f700: 6966 662a 2a32 202a 2073 656c 662e 746f  iff**2 * self.to
-0001f710: 7461 6c5f 6461 7461 5f6c 656e 202a 2064  tal_data_len * d
-0001f720: 6174 612e 7368 6170 655b 305d 202f 206e  ata.shape[0] / n
-0001f730: 6577 5f74 6f74 616c 5f64 6174 615f 6c65  ew_total_data_le
-0001f740: 6e0a 2020 2020 2020 2020 7365 6c66 2e76  n.        self.v
-0001f750: 6172 203d 206d 3220 2f20 6e65 775f 746f  ar = m2 / new_to
-0001f760: 7461 6c5f 6461 7461 5f6c 656e 0a20 2020  tal_data_len.   
-0001f770: 2020 2020 2064 6174 615f 7375 6d20 3d20       data_sum = 
-0001f780: 6e75 6d70 792e 7375 6d28 6461 7461 2c20  numpy.sum(data, 
-0001f790: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
-0001f7a0: 6465 6c74 6120 3d20 6461 7461 5f73 756d  delta = data_sum
-0001f7b0: 202d 2073 656c 662e 6d65 616e 202a 2064   - self.mean * d
-0001f7c0: 6174 612e 7368 6170 655b 305d 0a20 2020  ata.shape[0].   
-0001f7d0: 2020 2020 2073 656c 662e 6d65 616e 202b       self.mean +
-0001f7e0: 3d20 6465 6c74 6120 2f20 6e65 775f 746f  = delta / new_to
-0001f7f0: 7461 6c5f 6461 7461 5f6c 656e 0a20 2020  tal_data_len.   
-0001f800: 2020 2020 2064 656c 7461 5f73 7120 3d20       delta_sq = 
-0001f810: 6e75 6d70 792e 7375 6d28 6461 7461 202a  numpy.sum(data *
-0001f820: 2064 6174 612c 2061 7869 733d 3029 202d   data, axis=0) -
-0001f830: 2073 656c 662e 6d65 616e 5f73 7120 2a20   self.mean_sq * 
-0001f840: 6461 7461 2e73 6861 7065 5b30 5d0a 2020  data.shape[0].  
-0001f850: 2020 2020 2020 7365 6c66 2e6d 6561 6e5f        self.mean_
-0001f860: 7371 202b 3d20 6465 6c74 615f 7371 202f  sq += delta_sq /
-0001f870: 206e 6577 5f74 6f74 616c 5f64 6174 615f   new_total_data_
-0001f880: 6c65 6e0a 2020 2020 2020 2020 7365 6c66  len.        self
-0001f890: 2e74 6f74 616c 5f64 6174 615f 6c65 6e20  .total_data_len 
-0001f8a0: 3d20 6e65 775f 746f 7461 6c5f 6461 7461  = new_total_data
-0001f8b0: 5f6c 656e 0a0a 2020 2020 6465 6620 6765  _len..    def ge
-0001f8c0: 745f 6d65 616e 2873 656c 6629 3a0a 2020  t_mean(self):.  
-0001f8d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001f8e0: 2020 3a72 6574 7572 6e3a 206d 6561 6e2c    :return: mean,
-0001f8f0: 2073 6861 7065 2028 6469 6d2c 290a 2020   shape (dim,).  
-0001f900: 2020 2020 2020 3a72 7479 7065 3a20 6e75        :rtype: nu
-0001f910: 6d70 792e 6e64 6172 7261 790a 2020 2020  mpy.ndarray.    
-0001f920: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0001f930: 6173 7365 7274 2073 656c 662e 6e75 6d5f  assert self.num_
-0001f940: 7365 7173 203e 2030 0a20 2020 2020 2020  seqs > 0.       
-0001f950: 2072 6574 7572 6e20 7365 6c66 2e6d 6561   return self.mea
-0001f960: 6e0a 0a20 2020 2064 6566 2067 6574 5f73  n..    def get_s
-0001f970: 7464 5f64 6576 2873 656c 6629 3a0a 2020  td_dev(self):.  
-0001f980: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001f990: 2020 3a72 6574 7572 6e3a 2073 7464 2064    :return: std d
-0001f9a0: 6576 2c20 7368 6170 6520 2864 696d 2c29  ev, shape (dim,)
-0001f9b0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-0001f9c0: 206e 756d 7079 2e6e 6461 7272 6179 0a20   numpy.ndarray. 
-0001f9d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001f9e0: 2020 2069 6d70 6f72 7420 6e75 6d70 790a     import numpy.
-0001f9f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0001fa00: 7365 6c66 2e6e 756d 5f73 6571 7320 3e20  self.num_seqs > 
-0001fa10: 300a 2020 2020 2020 2020 7265 7475 726e  0.        return
-0001fa20: 206e 756d 7079 2e73 7172 7428 7365 6c66   numpy.sqrt(self
-0001fa30: 2e76 6172 290a 2020 2020 2020 2020 2320  .var).        # 
-0001fa40: 7265 7475 726e 206e 756d 7079 2e73 7172  return numpy.sqr
-0001fa50: 7428 7365 6c66 2e6d 6561 6e5f 7371 202d  t(self.mean_sq -
-0001fa60: 2073 656c 662e 6d65 616e 202a 2073 656c   self.mean * sel
-0001fa70: 662e 6d65 616e 290a 0a20 2020 2064 6566  f.mean)..    def
-0001fa80: 2064 756d 7028 7365 6c66 2c20 6f75 7470   dump(self, outp
-0001fa90: 7574 5f66 696c 655f 7072 6566 6978 3d4e  ut_file_prefix=N
-0001faa0: 6f6e 652c 2073 7472 6561 6d3d 4e6f 6e65  one, stream=None
-0001fab0: 2c20 7374 7265 616d 5f70 7265 6669 783d  , stream_prefix=
-0001fac0: 2222 293a 0a20 2020 2020 2020 2022 2222  ""):.        """
-0001fad0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0001fae0: 7374 727c 4e6f 6e65 206f 7574 7075 745f  str|None output_
-0001faf0: 6669 6c65 5f70 7265 6669 783a 2069 6620  file_prefix: if 
-0001fb00: 6769 7665 6e2c 2077 696c 6c20 6e75 6d70  given, will nump
-0001fb10: 792e 7361 7665 7478 7420 6d65 616e 7c73  y.savetxt mean|s
-0001fb20: 7464 5f64 6576 2074 6f20 6469 736b 0a20  td_dev to disk. 
-0001fb30: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-0001fb40: 7220 7374 7265 616d 5f70 7265 6669 783a  r stream_prefix:
-0001fb50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0001fb60: 696f 2e54 6578 7449 4f42 6173 6520 7374  io.TextIOBase st
-0001fb70: 7265 616d 3a20 7379 732e 7374 646f 7574  ream: sys.stdout
-0001fb80: 2062 7920 6465 6661 756c 740a 2020 2020   by default.    
-0001fb90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0001fba0: 6966 2073 7472 6561 6d20 6973 204e 6f6e  if stream is Non
-0001fbb0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0001fbc0: 7472 6561 6d20 3d20 7379 732e 7374 646f  tream = sys.stdo
-0001fbd0: 7574 0a20 2020 2020 2020 2069 6d70 6f72  ut.        impor
-0001fbe0: 7420 6e75 6d70 790a 0a20 2020 2020 2020  t numpy..       
-0001fbf0: 2070 7269 6e74 2822 2573 5374 6174 733a   print("%sStats:
-0001fc00: 2220 2520 7374 7265 616d 5f70 7265 6669  " % stream_prefi
-0001fc10: 782c 2066 696c 653d 7374 7265 616d 290a  x, file=stream).
-0001fc20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001fc30: 6e75 6d5f 7365 7173 2021 3d20 7365 6c66  num_seqs != self
-0001fc40: 2e74 6f74 616c 5f64 6174 615f 6c65 6e3a  .total_data_len:
-0001fc50: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0001fc60: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-0001fc70: 2020 2020 2220 2025 6920 7365 7173 2c20      "  %i seqs, 
-0001fc80: 2569 2074 6f74 616c 2066 7261 6d65 732c  %i total frames,
-0001fc90: 2025 6620 6176 6572 6167 6520 6672 616d   %f average fram
-0001fca0: 6573 220a 2020 2020 2020 2020 2020 2020  es".            
-0001fcb0: 2020 2020 2520 2873 656c 662e 6e75 6d5f      % (self.num_
-0001fcc0: 7365 7173 2c20 7365 6c66 2e74 6f74 616c  seqs, self.total
-0001fcd0: 5f64 6174 615f 6c65 6e2c 2073 656c 662e  _data_len, self.
-0001fce0: 746f 7461 6c5f 6461 7461 5f6c 656e 202f  total_data_len /
-0001fcf0: 2066 6c6f 6174 2873 656c 662e 6e75 6d5f   float(self.num_
-0001fd00: 7365 7173 2929 2c0a 2020 2020 2020 2020  seqs)),.        
-0001fd10: 2020 2020 2020 2020 6669 6c65 3d73 7472          file=str
-0001fd20: 6561 6d2c 0a20 2020 2020 2020 2020 2020  eam,.           
-0001fd30: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
-0001fd40: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0001fd50: 6e74 2822 2020 2569 2073 6571 7322 2025  nt("  %i seqs" %
-0001fd60: 2028 7365 6c66 2e6e 756d 5f73 6571 732c   (self.num_seqs,
-0001fd70: 292c 2066 696c 653d 7374 7265 616d 290a  ), file=stream).
-0001fd80: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
-0001fd90: 204d 6561 6e3a 2025 7322 2025 2028 7365   Mean: %s" % (se
-0001fda0: 6c66 2e66 6f72 6d61 745f 7374 7228 7365  lf.format_str(se
-0001fdb0: 6c66 2e67 6574 5f6d 6561 6e28 2929 2c29  lf.get_mean()),)
-0001fdc0: 2c20 6669 6c65 3d73 7472 6561 6d29 0a20  , file=stream). 
-0001fdd0: 2020 2020 2020 2070 7269 6e74 2822 2020         print("  
-0001fde0: 5374 6420 6465 763a 2025 7322 2025 2028  Std dev: %s" % (
-0001fdf0: 7365 6c66 2e66 6f72 6d61 745f 7374 7228  self.format_str(
-0001fe00: 7365 6c66 2e67 6574 5f73 7464 5f64 6576  self.get_std_dev
-0001fe10: 2829 292c 292c 2066 696c 653d 7374 7265  ()),), file=stre
-0001fe20: 616d 290a 2020 2020 2020 2020 7072 696e  am).        prin
-0001fe30: 7428 2220 204d 696e 2f6d 6178 3a20 2573  t("  Min/max: %s
-0001fe40: 202f 2025 7322 2025 2028 7365 6c66 2e66   / %s" % (self.f
-0001fe50: 6f72 6d61 745f 7374 7228 7365 6c66 2e6d  ormat_str(self.m
-0001fe60: 696e 292c 2073 656c 662e 666f 726d 6174  in), self.format
-0001fe70: 5f73 7472 2873 656c 662e 6d61 7829 292c  _str(self.max)),
-0001fe80: 2066 696c 653d 7374 7265 616d 290a 2020   file=stream).  
-0001fe90: 2020 2020 2020 2320 7072 696e 7428 2253        # print("S
-0001fea0: 7464 2064 6576 2028 6e61 6976 6529 3a20  td dev (naive): 
-0001feb0: 2573 2220 2520 6e75 6d70 792e 7371 7274  %s" % numpy.sqrt
-0001fec0: 2873 656c 662e 6d65 616e 5f73 7120 2d20  (self.mean_sq - 
-0001fed0: 7365 6c66 2e6d 6561 6e20 2a20 7365 6c66  self.mean * self
-0001fee0: 2e6d 6561 6e29 2c20 6669 6c65 3d73 7472  .mean), file=str
-0001fef0: 6561 6d29 0a20 2020 2020 2020 2069 6620  eam).        if 
-0001ff00: 6f75 7470 7574 5f66 696c 655f 7072 6566  output_file_pref
-0001ff10: 6978 3a0a 2020 2020 2020 2020 2020 2020  ix:.            
-0001ff20: 7072 696e 7428 2220 2057 7269 7465 206d  print("  Write m
-0001ff30: 6561 6e2f 7374 642d 6465 7620 746f 2025  ean/std-dev to %
-0001ff40: 732e 286d 6561 6e7c 7374 645f 6465 7629  s.(mean|std_dev)
-0001ff50: 2e74 7874 2e22 2025 2028 6f75 7470 7574  .txt." % (output
-0001ff60: 5f66 696c 655f 7072 6566 6978 2c29 2c20  _file_prefix,), 
-0001ff70: 6669 6c65 3d73 7472 6561 6d29 0a20 2020  file=stream).   
-0001ff80: 2020 2020 2020 2020 206e 756d 7079 2e73           numpy.s
-0001ff90: 6176 6574 7874 2822 2573 2e6d 6561 6e2e  avetxt("%s.mean.
-0001ffa0: 7478 7422 2025 206f 7574 7075 745f 6669  txt" % output_fi
-0001ffb0: 6c65 5f70 7265 6669 782c 2073 656c 662e  le_prefix, self.
-0001ffc0: 6765 745f 6d65 616e 2829 290a 2020 2020  get_mean()).    
-0001ffd0: 2020 2020 2020 2020 6e75 6d70 792e 7361          numpy.sa
-0001ffe0: 7665 7478 7428 2225 732e 7374 645f 6465  vetxt("%s.std_de
-0001fff0: 762e 7478 7422 2025 206f 7574 7075 745f  v.txt" % output_
-00020000: 6669 6c65 5f70 7265 6669 782c 2073 656c  file_prefix, sel
-00020010: 662e 6765 745f 7374 645f 6465 7628 2929  f.get_std_dev())
-00020020: 0a0a 0a64 6566 2069 735f 6e61 6d65 6474  ...def is_namedt
-00020030: 7570 6c65 2863 6c73 293a 0a20 2020 2022  uple(cls):.    "
-00020040: 2222 0a20 2020 203a 7061 7261 6d20 5420  "".    :param T 
-00020050: 636c 733a 2074 7570 6c65 2c20 6c69 7374  cls: tuple, list
-00020060: 206f 7220 6e61 6d65 6474 7570 6c65 2074   or namedtuple t
-00020070: 7970 650a 2020 2020 3a72 6574 7572 6e3a  ype.    :return:
-00020080: 2077 6865 7468 6572 2063 6c73 2069 7320   whether cls is 
-00020090: 6120 6e61 6d65 6474 7570 6c65 2074 7970  a namedtuple typ
-000200a0: 650a 2020 2020 3a72 7479 7065 3a20 626f  e.    :rtype: bo
-000200b0: 6f6c 0a20 2020 2022 2222 0a20 2020 2072  ol.    """.    r
-000200c0: 6574 7572 6e20 6973 7375 6263 6c61 7373  eturn issubclass
-000200d0: 2863 6c73 2c20 7475 706c 6529 2061 6e64  (cls, tuple) and
-000200e0: 2063 6c73 2069 7320 6e6f 7420 7475 706c   cls is not tupl
-000200f0: 650a 0a0a 6465 6620 6d61 6b65 5f73 6571  e...def make_seq
-00020100: 5f6f 665f 7479 7065 2863 6c73 2c20 7365  _of_type(cls, se
-00020110: 7129 3a0a 2020 2020 2222 220a 2020 2020  q):.    """.    
-00020120: 3a70 6172 616d 2074 7970 655b 545d 2063  :param type[T] c
-00020130: 6c73 3a20 652e 672e 2074 7570 6c65 2c20  ls: e.g. tuple, 
-00020140: 6c69 7374 206f 7220 6e61 6d65 6474 7570  list or namedtup
-00020150: 6c65 0a20 2020 203a 7061 7261 6d20 6c69  le.    :param li
-00020160: 7374 7c74 7570 6c65 7c54 2073 6571 3a0a  st|tuple|T seq:.
-00020170: 2020 2020 3a72 6574 7572 6e3a 2063 6c73      :return: cls
-00020180: 2873 6571 2920 6f72 2063 6c73 282a 7365  (seq) or cls(*se
-00020190: 7129 0a20 2020 203a 7274 7970 653a 2054  q).    :rtype: T
-000201a0: 7c6c 6973 747c 7475 706c 650a 2020 2020  |list|tuple.    
-000201b0: 2222 220a 2020 2020 6173 7365 7274 2069  """.    assert i
-000201c0: 7373 7562 636c 6173 7328 636c 732c 2028  ssubclass(cls, (
-000201d0: 6c69 7374 2c20 7475 706c 6529 290a 2020  list, tuple)).  
-000201e0: 2020 6966 2069 735f 6e61 6d65 6474 7570    if is_namedtup
-000201f0: 6c65 2863 6c73 293a 0a20 2020 2020 2020  le(cls):.       
-00020200: 2072 6574 7572 6e20 636c 7328 2a73 6571   return cls(*seq
-00020210: 2920 2023 206e 6f71 610a 2020 2020 7265  )  # noqa.    re
-00020220: 7475 726e 2063 6c73 2873 6571 2920 2023  turn cls(seq)  #
-00020230: 206e 6f71 610a 0a0a 6465 6620 656e 7375   noqa...def ensu
-00020240: 7265 5f6c 6973 745f 6f66 5f74 7970 6528  re_list_of_type(
-00020250: 6c73 2c20 7479 7065 5f29 3a0a 2020 2020  ls, type_):.    
-00020260: 2222 220a 2020 2020 3a70 6172 616d 206c  """.    :param l
-00020270: 6973 7420 6c73 3a0a 2020 2020 3a70 6172  ist ls:.    :par
-00020280: 616d 2028 2829 2d3e 5429 7c74 7970 655b  am (()->T)|type[
-00020290: 545d 2074 7970 655f 3a20 7479 7065 206f  T] type_: type o
-000202a0: 6620 696e 7374 616e 6365 7320 6f66 2060  f instances of `
-000202b0: 6c73 602e 0a20 2020 2020 204e 6f74 6520  ls`..      Note 
-000202c0: 7468 6520 7374 7261 6e67 6520 7479 7065  the strange type
-000202d0: 2068 6572 6520 696e 2074 6865 2064 6f63   here in the doc
-000202e0: 7374 7269 6e67 2069 7320 6475 6520 746f  string is due to
-000202f0: 2073 6f6d 6520 5079 4368 6172 6d20 7479   some PyCharm ty
-00020300: 7065 2069 6e66 6572 656e 6365 2070 726f  pe inference pro
-00020310: 626c 656d 730a 2020 2020 2020 2868 7474  blems.      (htt
-00020320: 7073 3a2f 2f79 6f75 7472 6163 6b2e 6a65  ps://youtrack.je
-00020330: 7462 7261 696e 732e 636f 6d2f 6973 7375  tbrains.com/issu
-00020340: 652f 5059 2d35 3038 3238 292e 0a20 2020  e/PY-50828)..   
-00020350: 203a 7274 7970 653a 206c 6973 745b 545d   :rtype: list[T]
-00020360: 0a20 2020 2022 2222 0a20 2020 2061 7373  .    """.    ass
-00020370: 6572 7420 616c 6c28 6973 696e 7374 616e  ert all(isinstan
-00020380: 6365 2865 6c65 6d2c 2074 7970 655f 2920  ce(elem, type_) 
-00020390: 666f 7220 656c 656d 2069 6e20 6c73 290a  for elem in ls).
-000203a0: 2020 2020 7265 7475 726e 206c 730a 0a0a      return ls...
-000203b0: 4063 6f6e 7465 7874 6c69 622e 636f 6e74  @contextlib.cont
-000203c0: 6578 746d 616e 6167 6572 0a64 6566 2064  extmanager.def d
-000203d0: 756d 6d79 5f6e 6f6f 705f 6374 7828 293a  ummy_noop_ctx():
-000203e0: 0a20 2020 2022 2222 0a20 2020 2050 726f  .    """.    Pro
-000203f0: 7669 6465 7320 6120 6e6f 2d6f 7020 636f  vides a no-op co
-00020400: 6e74 6578 7420 6d61 6e61 6765 722e 0a20  ntext manager.. 
-00020410: 2020 2022 2222 0a20 2020 2079 6965 6c64     """.    yield
-00020420: 204e 6f6e 650a 0a0a 6465 6620 5f67 6574   None...def _get
-00020430: 5f6e 6772 616d 7328 7365 676d 656e 742c  _ngrams(segment,
-00020440: 206d 6178 5f6f 7264 6572 293a 0a20 2020   max_order):.   
-00020450: 2022 2222 4578 7472 6163 7473 2061 6c6c   """Extracts all
-00020460: 206e 2d67 7261 6d73 2075 7074 6f20 6120   n-grams upto a 
-00020470: 6769 7665 6e20 6d61 7869 6d75 6d20 6f72  given maximum or
-00020480: 6465 7220 6672 6f6d 2061 6e20 696e 7075  der from an inpu
-00020490: 7420 7365 676d 656e 742e 0a20 2020 2043  t segment..    C
-000204a0: 6f64 6520 6164 6170 7465 6420 6672 6f6d  ode adapted from
-000204b0: 2047 6f6f 676c 6520 5465 6e73 6f72 3254   Google Tensor2T
-000204c0: 656e 736f 722e 0a0a 2020 2020 4172 6773  ensor...    Args
-000204d0: 3a0a 2020 2020 2020 7365 676d 656e 7420  :.      segment 
-000204e0: 286c 6973 745b 696e 745d 7c6c 6973 745b  (list[int]|list[
-000204f0: 7374 725d 293a 2074 6578 7420 7365 676d  str]): text segm
-00020500: 656e 7420 6672 6f6d 2077 6869 6368 206e  ent from which n
-00020510: 2d67 7261 6d73 2077 696c 6c20 6265 2065  -grams will be e
-00020520: 7874 7261 6374 6564 2e0a 2020 2020 2020  xtracted..      
-00020530: 6d61 785f 6f72 6465 7220 2869 6e74 293a  max_order (int):
-00020540: 206d 6178 696d 756d 206c 656e 6774 6820   maximum length 
-00020550: 696e 2074 6f6b 656e 7320 6f66 2074 6865  in tokens of the
-00020560: 206e 2d67 7261 6d73 2072 6574 7572 6e65   n-grams returne
-00020570: 6420 6279 2074 6869 730a 2020 2020 2020  d by this.      
-00020580: 2020 2020 6d65 7468 6f64 732e 0a0a 2020      methods...  
-00020590: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000205a0: 2054 6865 2043 6f75 6e74 6572 2063 6f6e   The Counter con
-000205b0: 7461 696e 696e 6720 616c 6c20 6e2d 6772  taining all n-gr
-000205c0: 616d 7320 7570 746f 206d 6178 5f6f 7264  ams upto max_ord
-000205d0: 6572 2069 6e20 7365 676d 656e 740a 2020  er in segment.  
-000205e0: 2020 2020 7769 7468 2061 2063 6f75 6e74      with a count
-000205f0: 206f 6620 686f 7720 6d61 6e79 2074 696d   of how many tim
-00020600: 6573 2065 6163 6820 6e2d 6772 616d 206f  es each n-gram o
-00020610: 6363 7572 7265 642e 0a20 2020 2022 2222  ccurred..    """
-00020620: 0a20 2020 2069 6d70 6f72 7420 636f 6c6c  .    import coll
-00020630: 6563 7469 6f6e 730a 0a20 2020 206e 6772  ections..    ngr
-00020640: 616d 5f63 6f75 6e74 7320 3d20 636f 6c6c  am_counts = coll
-00020650: 6563 7469 6f6e 732e 436f 756e 7465 7228  ections.Counter(
-00020660: 290a 2020 2020 666f 7220 6f72 6465 7220  ).    for order 
-00020670: 696e 2072 616e 6765 2831 2c20 6d61 785f  in range(1, max_
-00020680: 6f72 6465 7220 2b20 3129 3a0a 2020 2020  order + 1):.    
-00020690: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-000206a0: 6765 2830 2c20 6c65 6e28 7365 676d 656e  ge(0, len(segmen
-000206b0: 7429 202d 206f 7264 6572 202b 2031 293a  t) - order + 1):
-000206c0: 0a20 2020 2020 2020 2020 2020 206e 6772  .            ngr
-000206d0: 616d 203d 2074 7570 6c65 2873 6567 6d65  am = tuple(segme
-000206e0: 6e74 5b69 203a 2069 202b 206f 7264 6572  nt[i : i + order
-000206f0: 5d29 0a20 2020 2020 2020 2020 2020 206e  ]).            n
-00020700: 6772 616d 5f63 6f75 6e74 735b 6e67 7261  gram_counts[ngra
-00020710: 6d5d 202b 3d20 310a 2020 2020 7265 7475  m] += 1.    retu
-00020720: 726e 206e 6772 616d 5f63 6f75 6e74 730a  rn ngram_counts.
-00020730: 0a0a 6465 6620 636f 6d70 7574 655f 626c  ..def compute_bl
-00020740: 6575 2872 6566 6572 656e 6365 5f63 6f72  eu(reference_cor
-00020750: 7075 732c 2074 7261 6e73 6c61 7469 6f6e  pus, translation
-00020760: 5f63 6f72 7075 732c 206d 6178 5f6f 7264  _corpus, max_ord
-00020770: 6572 3d34 2c20 7573 655f 6270 3d54 7275  er=4, use_bp=Tru
-00020780: 6529 3a0a 2020 2020 2222 2243 6f6d 7075  e):.    """Compu
-00020790: 7465 7320 424c 4555 2073 636f 7265 206f  tes BLEU score o
-000207a0: 6620 7472 616e 736c 6174 6564 2073 6567  f translated seg
-000207b0: 6d65 6e74 7320 6167 6169 6e73 7420 6f6e  ments against on
-000207c0: 6520 6f72 206d 6f72 6520 7265 6665 7265  e or more refere
-000207d0: 6e63 6573 2e0a 2020 2020 436f 6465 2061  nces..    Code a
-000207e0: 6461 7074 6564 2066 726f 6d20 476f 6f67  dapted from Goog
-000207f0: 6c65 2054 656e 736f 7232 5465 6e73 6f72  le Tensor2Tensor
-00020800: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00020810: 2020 2072 6566 6572 656e 6365 5f63 6f72     reference_cor
-00020820: 7075 7320 286c 6973 745b 6c69 7374 5b69  pus (list[list[i
-00020830: 6e74 5d7c 6c69 7374 5b73 7472 5d5d 293a  nt]|list[str]]):
-00020840: 206c 6973 7420 6f66 2072 6566 6572 656e   list of referen
-00020850: 6365 7320 666f 7220 6561 6368 2074 7261  ces for each tra
-00020860: 6e73 6c61 7469 6f6e 2e20 4561 6368 0a20  nslation. Each. 
-00020870: 2020 2020 2020 2020 2072 6566 6572 656e           referen
-00020880: 6365 2073 686f 756c 6420 6265 2074 6f6b  ce should be tok
-00020890: 656e 697a 6564 2069 6e74 6f20 6120 6c69  enized into a li
-000208a0: 7374 206f 6620 746f 6b65 6e73 2e0a 2020  st of tokens..  
-000208b0: 2020 2020 7472 616e 736c 6174 696f 6e5f      translation_
-000208c0: 636f 7270 7573 2028 6c69 7374 5b6c 6973  corpus (list[lis
-000208d0: 745b 696e 745d 7c6c 6973 745b 7374 725d  t[int]|list[str]
-000208e0: 5d29 3a20 6c69 7374 206f 6620 7472 616e  ]): list of tran
-000208f0: 736c 6174 696f 6e73 2074 6f20 7363 6f72  slations to scor
-00020900: 652e 2045 6163 6820 7472 616e 736c 6174  e. Each translat
-00020910: 696f 6e0a 2020 2020 2020 2020 2020 7368  ion.          sh
-00020920: 6f75 6c64 2062 6520 746f 6b65 6e69 7a65  ould be tokenize
-00020930: 6420 696e 746f 2061 206c 6973 7420 6f66  d into a list of
-00020940: 2074 6f6b 656e 732e 0a20 2020 2020 206d   tokens..      m
-00020950: 6178 5f6f 7264 6572 2028 696e 7429 3a20  ax_order (int): 
-00020960: 4d61 7869 6d75 6d20 6e2d 6772 616d 206f  Maximum n-gram o
-00020970: 7264 6572 2074 6f20 7573 6520 7768 656e  rder to use when
-00020980: 2063 6f6d 7075 7469 6e67 2042 4c45 5520   computing BLEU 
-00020990: 7363 6f72 652e 0a20 2020 2020 2075 7365  score..      use
-000209a0: 5f62 7020 2862 6f6f 6c29 3a20 626f 6f6c  _bp (bool): bool
-000209b0: 6561 6e2c 2077 6865 7468 6572 2074 6f20  ean, whether to 
-000209c0: 6170 706c 7920 6272 6576 6974 7920 7065  apply brevity pe
-000209d0: 6e61 6c74 792e 0a0a 2020 2020 5265 7475  nalty...    Retu
-000209e0: 726e 733a 0a20 2020 2020 2042 4c45 5520  rns:.      BLEU 
-000209f0: 7363 6f72 652e 0a20 2020 2022 2222 0a20  score..    """. 
-00020a00: 2020 2069 6d70 6f72 7420 6d61 7468 0a0a     import math..
-00020a10: 2020 2020 7265 6665 7265 6e63 655f 6c65      reference_le
-00020a20: 6e67 7468 203d 2030 0a20 2020 2074 7261  ngth = 0.    tra
-00020a30: 6e73 6c61 7469 6f6e 5f6c 656e 6774 6820  nslation_length 
-00020a40: 3d20 300a 2020 2020 6270 203d 2031 2e30  = 0.    bp = 1.0
-00020a50: 0a20 2020 2067 656f 5f6d 6561 6e20 3d20  .    geo_mean = 
-00020a60: 300a 0a20 2020 206d 6174 6368 6573 5f62  0..    matches_b
-00020a70: 795f 6f72 6465 7220 3d20 5b30 5d20 2a20  y_order = [0] * 
-00020a80: 6d61 785f 6f72 6465 720a 2020 2020 706f  max_order.    po
-00020a90: 7373 6962 6c65 5f6d 6174 6368 6573 5f62  ssible_matches_b
-00020aa0: 795f 6f72 6465 7220 3d20 5b30 5d20 2a20  y_order = [0] * 
-00020ab0: 6d61 785f 6f72 6465 720a 0a20 2020 2066  max_order..    f
-00020ac0: 6f72 2028 7265 6665 7265 6e63 6573 2c20  or (references, 
-00020ad0: 7472 616e 736c 6174 696f 6e73 2920 696e  translations) in
-00020ae0: 207a 6970 2872 6566 6572 656e 6365 5f63   zip(reference_c
-00020af0: 6f72 7075 732c 2074 7261 6e73 6c61 7469  orpus, translati
-00020b00: 6f6e 5f63 6f72 7075 7329 3a0a 2020 2020  on_corpus):.    
-00020b10: 2020 2020 7265 6665 7265 6e63 655f 6c65      reference_le
-00020b20: 6e67 7468 202b 3d20 6c65 6e28 7265 6665  ngth += len(refe
-00020b30: 7265 6e63 6573 290a 2020 2020 2020 2020  rences).        
-00020b40: 7472 616e 736c 6174 696f 6e5f 6c65 6e67  translation_leng
-00020b50: 7468 202b 3d20 6c65 6e28 7472 616e 736c  th += len(transl
-00020b60: 6174 696f 6e73 290a 2020 2020 2020 2020  ations).        
-00020b70: 7265 665f 6e67 7261 6d5f 636f 756e 7473  ref_ngram_counts
-00020b80: 203d 205f 6765 745f 6e67 7261 6d73 2872   = _get_ngrams(r
-00020b90: 6566 6572 656e 6365 732c 206d 6178 5f6f  eferences, max_o
-00020ba0: 7264 6572 290a 2020 2020 2020 2020 7472  rder).        tr
-00020bb0: 616e 736c 6174 696f 6e5f 6e67 7261 6d5f  anslation_ngram_
-00020bc0: 636f 756e 7473 203d 205f 6765 745f 6e67  counts = _get_ng
-00020bd0: 7261 6d73 2874 7261 6e73 6c61 7469 6f6e  rams(translation
-00020be0: 732c 206d 6178 5f6f 7264 6572 290a 0a20  s, max_order).. 
-00020bf0: 2020 2020 2020 206f 7665 726c 6170 203d         overlap =
-00020c00: 207b 6e67 7261 6d3a 206d 696e 2863 6f75   {ngram: min(cou
-00020c10: 6e74 2c20 7472 616e 736c 6174 696f 6e5f  nt, translation_
-00020c20: 6e67 7261 6d5f 636f 756e 7473 5b6e 6772  ngram_counts[ngr
-00020c30: 616d 5d29 2066 6f72 206e 6772 616d 2c20  am]) for ngram, 
-00020c40: 636f 756e 7420 696e 2072 6566 5f6e 6772  count in ref_ngr
-00020c50: 616d 5f63 6f75 6e74 732e 6974 656d 7328  am_counts.items(
-00020c60: 297d 0a0a 2020 2020 2020 2020 666f 7220  )}..        for 
-00020c70: 6e67 7261 6d20 696e 206f 7665 726c 6170  ngram in overlap
-00020c80: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-00020c90: 7463 6865 735f 6279 5f6f 7264 6572 5b6c  tches_by_order[l
-00020ca0: 656e 286e 6772 616d 2920 2d20 315d 202b  en(ngram) - 1] +
-00020cb0: 3d20 6f76 6572 6c61 705b 6e67 7261 6d5d  = overlap[ngram]
-00020cc0: 0a20 2020 2020 2020 2066 6f72 206e 6772  .        for ngr
-00020cd0: 616d 2069 6e20 7472 616e 736c 6174 696f  am in translatio
-00020ce0: 6e5f 6e67 7261 6d5f 636f 756e 7473 3a0a  n_ngram_counts:.
-00020cf0: 2020 2020 2020 2020 2020 2020 706f 7373              poss
-00020d00: 6962 6c65 5f6d 6174 6368 6573 5f62 795f  ible_matches_by_
-00020d10: 6f72 6465 725b 6c65 6e28 6e67 7261 6d29  order[len(ngram)
-00020d20: 202d 2031 5d20 2b3d 2074 7261 6e73 6c61   - 1] += transla
-00020d30: 7469 6f6e 5f6e 6772 616d 5f63 6f75 6e74  tion_ngram_count
-00020d40: 735b 6e67 7261 6d5d 0a0a 2020 2020 7072  s[ngram]..    pr
-00020d50: 6563 6973 696f 6e73 203d 205b 302e 305d  ecisions = [0.0]
-00020d60: 202a 206d 6178 5f6f 7264 6572 0a20 2020   * max_order.   
-00020d70: 2073 6d6f 6f74 6820 3d20 312e 300a 2020   smooth = 1.0.  
-00020d80: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00020d90: 2830 2c20 6d61 785f 6f72 6465 7229 3a0a  (0, max_order):.
-00020da0: 2020 2020 2020 2020 6966 2070 6f73 7369          if possi
-00020db0: 626c 655f 6d61 7463 6865 735f 6279 5f6f  ble_matches_by_o
-00020dc0: 7264 6572 5b69 5d20 3e20 303a 0a20 2020  rder[i] > 0:.   
-00020dd0: 2020 2020 2020 2020 2070 7265 6369 7369           precisi
-00020de0: 6f6e 735b 695d 203d 206d 6174 6368 6573  ons[i] = matches
-00020df0: 5f62 795f 6f72 6465 725b 695d 202f 2070  _by_order[i] / p
-00020e00: 6f73 7369 626c 655f 6d61 7463 6865 735f  ossible_matches_
-00020e10: 6279 5f6f 7264 6572 5b69 5d0a 2020 2020  by_order[i].    
-00020e20: 2020 2020 2020 2020 6966 206d 6174 6368          if match
-00020e30: 6573 5f62 795f 6f72 6465 725b 695d 203e  es_by_order[i] >
-00020e40: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00020e50: 2020 2020 7072 6563 6973 696f 6e73 5b69      precisions[i
-00020e60: 5d20 3d20 6d61 7463 6865 735f 6279 5f6f  ] = matches_by_o
-00020e70: 7264 6572 5b69 5d20 2f20 706f 7373 6962  rder[i] / possib
-00020e80: 6c65 5f6d 6174 6368 6573 5f62 795f 6f72  le_matches_by_or
-00020e90: 6465 725b 695d 0a20 2020 2020 2020 2020  der[i].         
-00020ea0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00020eb0: 2020 2020 2020 2020 2073 6d6f 6f74 6820           smooth 
-00020ec0: 2a3d 2032 0a20 2020 2020 2020 2020 2020  *= 2.           
-00020ed0: 2020 2020 2070 7265 6369 7369 6f6e 735b       precisions[
-00020ee0: 695d 203d 2031 2e30 202f 2028 736d 6f6f  i] = 1.0 / (smoo
-00020ef0: 7468 202a 2070 6f73 7369 626c 655f 6d61  th * possible_ma
-00020f00: 7463 6865 735f 6279 5f6f 7264 6572 5b69  tches_by_order[i
-00020f10: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
-00020f20: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
-00020f30: 6369 7369 6f6e 735b 695d 203d 2030 2e30  cisions[i] = 0.0
-00020f40: 0a0a 2020 2020 6966 206d 6178 2870 7265  ..    if max(pre
-00020f50: 6369 7369 6f6e 7329 203e 2030 3a0a 2020  cisions) > 0:.  
-00020f60: 2020 2020 2020 705f 6c6f 675f 7375 6d20        p_log_sum 
-00020f70: 3d20 7375 6d28 6d61 7468 2e6c 6f67 2870  = sum(math.log(p
-00020f80: 2920 666f 7220 7020 696e 2070 7265 6369  ) for p in preci
-00020f90: 7369 6f6e 7320 6966 2070 290a 2020 2020  sions if p).    
-00020fa0: 2020 2020 6765 6f5f 6d65 616e 203d 206d      geo_mean = m
-00020fb0: 6174 682e 6578 7028 705f 6c6f 675f 7375  ath.exp(p_log_su
-00020fc0: 6d20 2f20 6d61 785f 6f72 6465 7229 0a0a  m / max_order)..
-00020fd0: 2020 2020 6966 2075 7365 5f62 703a 0a20      if use_bp:. 
-00020fe0: 2020 2020 2020 2072 6174 696f 203d 2074         ratio = t
-00020ff0: 7261 6e73 6c61 7469 6f6e 5f6c 656e 6774  ranslation_lengt
-00021000: 6820 2f20 7265 6665 7265 6e63 655f 6c65  h / reference_le
-00021010: 6e67 7468 0a20 2020 2020 2020 2069 6620  ngth.        if 
-00021020: 7261 7469 6f20 3c20 3165 2d33 303a 0a20  ratio < 1e-30:. 
-00021030: 2020 2020 2020 2020 2020 2062 7020 3d20             bp = 
-00021040: 302e 300a 2020 2020 2020 2020 656c 6966  0.0.        elif
-00021050: 2072 6174 696f 203c 2031 2e30 3a0a 2020   ratio < 1.0:.  
-00021060: 2020 2020 2020 2020 2020 6270 203d 206d            bp = m
-00021070: 6174 682e 6578 7028 3120 2d20 312e 3020  ath.exp(1 - 1.0 
-00021080: 2f20 7261 7469 6f29 0a20 2020 2020 2020  / ratio).       
-00021090: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000210a0: 2020 2062 7020 3d20 312e 300a 2020 2020     bp = 1.0.    
-000210b0: 626c 6575 203d 2067 656f 5f6d 6561 6e20  bleu = geo_mean 
-000210c0: 2a20 6270 0a20 2020 2072 6574 7572 6e20  * bp.    return 
-000210d0: 6e70 2e66 6c6f 6174 3332 2862 6c65 7529  np.float32(bleu)
-000210e0: 0a0a 0a23 206e 6f69 6e73 7065 6374 696f  ...# noinspectio
-000210f0: 6e20 5079 5061 636b 6167 6552 6571 7569  n PyPackageRequi
-00021100: 7265 6d65 6e74 730a 6465 6620 6d6f 6e6b  rements.def monk
-00021110: 6579 6669 785f 676c 6962 2829 3a0a 2020  eyfix_glib():.  
-00021120: 2020 2222 220a 2020 2020 4669 7865 7320    """.    Fixes 
-00021130: 736f 6d65 2073 7475 7069 6420 6275 6773  some stupid bugs
-00021140: 2073 7563 6820 7468 6174 2053 4947 494e   such that SIGIN
-00021150: 5420 6973 206e 6f74 2077 6f72 6b69 6e67  T is not working
-00021160: 2e0a 2020 2020 5468 6973 2069 7320 7573  ..    This is us
-00021170: 6564 2062 7920 6175 6469 6f72 6561 642c  ed by audioread,
-00021180: 2061 6e64 2069 6e64 6972 6563 746c 7920   and indirectly 
-00021190: 6279 206c 6962 726f 7361 2066 6f72 206c  by librosa for l
-000211a0: 6f61 6469 6e67 2061 7564 696f 2e0a 2020  oading audio..  
-000211b0: 2020 6874 7470 733a 2f2f 7374 6163 6b6f    https://stacko
-000211c0: 7665 7266 6c6f 772e 636f 6d2f 7175 6573  verflow.com/ques
-000211d0: 7469 6f6e 732f 3136 3431 3038 3532 2f0a  tions/16410852/.
-000211e0: 2020 2020 5365 6520 616c 736f 203a 6675      See also :fu
-000211f0: 6e63 3a60 6d6f 6e6b 6579 7061 7463 685f  nc:`monkeypatch_
-00021200: 6175 6469 6f72 6561 6460 2e0a 2020 2020  audioread`..    
-00021210: 2222 220a 2020 2020 7472 793a 0a20 2020  """.    try:.   
-00021220: 2020 2020 2069 6d70 6f72 7420 6769 0a20       import gi. 
-00021230: 2020 2065 7863 6570 7420 496d 706f 7274     except Import
-00021240: 4572 726f 723a 0a20 2020 2020 2020 2072  Error:.        r
-00021250: 6574 7572 6e0a 2020 2020 7472 793a 0a20  eturn.    try:. 
-00021260: 2020 2020 2020 2066 726f 6d20 6769 2e72         from gi.r
-00021270: 6570 6f73 6974 6f72 7920 696d 706f 7274  epository import
-00021280: 2047 4c69 620a 2020 2020 6578 6365 7074   GLib.    except
-00021290: 2049 6d70 6f72 7445 7272 6f72 3a0a 2020   ImportError:.  
-000212a0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-000212b0: 7469 6f6e 2050 7955 6e72 6573 6f6c 7665  tion PyUnresolve
-000212c0: 6452 6566 6572 656e 6365 730a 2020 2020  dReferences.    
-000212d0: 2020 2020 6672 6f6d 2067 692e 6f76 6572      from gi.over
-000212e0: 7269 6465 7320 696d 706f 7274 2047 4c69  rides import GLi
-000212f0: 620a 2020 2020 2320 446f 206e 6f74 6869  b.    # Do nothi
-00021300: 6e67 2e0a 2020 2020 2320 5468 6520 6f72  ng..    # The or
-00021310: 6967 696e 616c 2062 6568 6176 696f 7220  iginal behavior 
-00021320: 776f 756c 6420 696e 7374 616c 6c20 6120  would install a 
-00021330: 5349 4749 4e54 2068 616e 646c 6572 2077  SIGINT handler w
-00021340: 6869 6368 2063 616c 6c73 2047 4c69 622e  hich calls GLib.
-00021350: 4d61 696e 4c6f 6f70 2e71 7569 7428 292c  MainLoop.quit(),
-00021360: 0a20 2020 2023 2061 6e64 2074 6865 6e20  .    # and then 
-00021370: 7265 7261 6973 6520 6120 4b65 7962 6f61  reraise a Keyboa
-00021380: 7264 496e 7465 7272 7570 7420 696e 2074  rdInterrupt in t
-00021390: 6861 7420 7468 7265 6164 2e0a 2020 2020  hat thread..    
-000213a0: 2320 486f 7765 7665 722c 2077 6520 7761  # However, we wa
-000213b0: 6e74 2061 6e64 2065 7870 6563 7420 746f  nt and expect to
-000213c0: 2067 6574 2074 6865 204b 6579 626f 6172   get the Keyboar
-000213d0: 6449 6e74 6572 7275 7074 2069 6e20 7468  dInterrupt in th
-000213e0: 6520 6d61 696e 2074 6872 6561 642e 0a20  e main thread.. 
-000213f0: 2020 2047 4c69 622e 4d61 696e 4c6f 6f70     GLib.MainLoop
-00021400: 2e5f 5f69 6e69 745f 5f20 3d20 6c61 6d62  .__init__ = lamb
-00021410: 6461 202a 6172 6773 2c20 2a2a 6b77 6172  da *args, **kwar
-00021420: 6773 3a20 4e6f 6e65 0a0a 0a64 6566 206d  gs: None...def m
-00021430: 6f6e 6b65 7970 6174 6368 5f61 7564 696f  onkeypatch_audio
-00021440: 7265 6164 2829 3a0a 2020 2020 2222 220a  read():.    """.
-00021450: 2020 2020 6175 6469 6f72 6561 6420 646f      audioread do
-00021460: 6573 206e 6f74 2062 6568 6176 6520 6f70  es not behave op
-00021470: 7469 6d61 6c20 696e 2073 6f6d 6520 6361  timal in some ca
-00021480: 7365 732e 0a20 2020 2045 2e67 2e20 6561  ses..    E.g. ea
-00021490: 6368 2063 616c 6c20 746f 205f 6361 5f61  ch call to _ca_a
-000214a0: 7661 696c 6162 6c65 2829 2074 616b 6573  vailable() takes
-000214b0: 2071 7569 7465 206c 6f6e 6720 6265 6361   quite long beca
-000214c0: 7573 6520 6f66 2074 6865 2063 7479 7065  use of the ctype
-000214d0: 732e 7574 696c 2e66 696e 645f 6c69 6272  s.util.find_libr
-000214e0: 6172 7920 7573 6167 652e 0a20 2020 2057  ary usage..    W
-000214f0: 6520 7769 6c6c 2070 6174 6368 2074 6869  e will patch thi
-00021500: 732e 0a0a 2020 2020 486f 7765 7665 722c  s...    However,
-00021510: 2074 6865 2072 6563 6f6d 6d65 6e64 6174   the recommendat
-00021520: 696f 6e20 776f 756c 6420 6265 2074 6f20  ion would be to 
-00021530: 6e6f 7420 7573 6520 6175 6469 6f72 6561  not use audiorea
-00021540: 6420 286c 6962 726f 7361 2e6c 6f61 6429  d (librosa.load)
-00021550: 2e0a 2020 2020 6175 6469 6f72 6561 6420  ..    audioread 
-00021560: 7573 6573 2047 7374 7265 616d 6572 2061  uses Gstreamer a
-00021570: 7320 6120 6261 636b 656e 6420 6279 2064  s a backend by d
-00021580: 6566 6175 6c74 2063 7572 7265 6e74 6c79  efault currently
-00021590: 2028 6f6e 204c 696e 7578 292e 0a20 2020   (on Linux)..   
-000215a0: 2047 7374 7265 616d 6572 2068 6173 206d   Gstreamer has m
-000215b0: 756c 7469 706c 6520 6973 7375 6573 2e20  ultiple issues. 
-000215c0: 5365 6520 616c 736f 203a 6675 6e63 3a60  See also :func:`
-000215d0: 6d6f 6e6b 6579 6669 785f 676c 6962 602c  monkeyfix_glib`,
-000215e0: 2061 6e64 2068 6572 6520 666f 7220 6469   and here for di
-000215f0: 7363 7573 7369 6f6e 3a0a 2020 2020 6874  scussion:.    ht
-00021600: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00021610: 2f62 6565 7462 6f78 2f61 7564 696f 7265  /beetbox/audiore
-00021620: 6164 2f69 7373 7565 732f 3632 0a20 2020  ad/issues/62.   
-00021630: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00021640: 636f 6d2f 6265 6574 626f 782f 6175 6469  com/beetbox/audi
-00021650: 6f72 6561 642f 6973 7375 6573 2f36 330a  oread/issues/63.
-00021660: 0a20 2020 2049 6e73 7465 6164 2c20 7573  .    Instead, us
-00021670: 6520 5079 536f 756e 6446 696c 652c 2077  e PySoundFile, w
-00021680: 6869 6368 2069 7320 616c 736f 2066 6173  hich is also fas
-00021690: 7465 722e 2053 6565 2068 6572 6520 666f  ter. See here fo
-000216a0: 7220 6469 7363 7573 7369 6f6e 733a 0a20  r discussions:. 
-000216b0: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
-000216c0: 622e 636f 6d2f 6265 6574 626f 782f 6175  b.com/beetbox/au
-000216d0: 6469 6f72 6561 642f 6973 7375 6573 2f36  dioread/issues/6
-000216e0: 340a 2020 2020 6874 7470 733a 2f2f 6769  4.    https://gi
-000216f0: 7468 7562 2e63 6f6d 2f6c 6962 726f 7361  thub.com/librosa
-00021700: 2f6c 6962 726f 7361 2f69 7373 7565 732f  /librosa/issues/
-00021710: 3638 310a 2020 2020 2222 220a 2020 2020  681.    """.    
-00021720: 7472 793a 0a20 2020 2020 2020 2023 206e  try:.        # n
-00021730: 6f69 6e73 7065 6374 696f 6e20 5079 5061  oinspection PyPa
-00021740: 636b 6167 6552 6571 7569 7265 6d65 6e74  ckageRequirement
-00021750: 730a 2020 2020 2020 2020 696d 706f 7274  s.        import
-00021760: 2061 7564 696f 7265 6164 0a20 2020 2065   audioread.    e
-00021770: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
-00021780: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
-00021790: 6e0a 2020 2020 2320 6e6f 696e 7370 6563  n.    # noinspec
-000217a0: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-000217b0: 4d65 6d62 6572 0a20 2020 2072 6573 203d  Member.    res =
-000217c0: 2061 7564 696f 7265 6164 2e5f 6361 5f61   audioread._ca_a
-000217d0: 7661 696c 6162 6c65 2829 0a20 2020 2061  vailable().    a
-000217e0: 7564 696f 7265 6164 2e5f 6361 5f61 7661  udioread._ca_ava
-000217f0: 696c 6162 6c65 203d 206c 616d 6264 613a  ilable = lambda:
-00021800: 2072 6573 0a0a 0a5f 6366 5f63 6163 6865   res..._cf_cache
-00021810: 203d 207b 7d0a 5f63 665f 6d73 675f 7072   = {}._cf_msg_pr
-00021820: 696e 7465 6420 3d20 4661 6c73 650a 0a0a  inted = False...
-00021830: 6465 6620 6366 2866 696c 656e 616d 6529  def cf(filename)
-00021840: 3a0a 2020 2020 2222 220a 2020 2020 4361  :.    """.    Ca
-00021850: 6368 6520 6d61 6e61 6765 722e 2069 3620  che manager. i6 
-00021860: 7370 6563 6966 6963 2e0a 0a20 2020 203a  specific...    :
-00021870: 7265 7475 726e 3a20 6669 6c65 6e61 6d65  return: filename
-00021880: 0a20 2020 203a 7274 7970 653a 2073 7472  .    :rtype: str
-00021890: 0a20 2020 2022 2222 0a20 2020 2067 6c6f  .    """.    glo
-000218a0: 6261 6c20 5f63 665f 6d73 675f 7072 696e  bal _cf_msg_prin
-000218b0: 7465 640a 2020 2020 696d 706f 7274 206f  ted.    import o
-000218c0: 730a 2020 2020 6672 6f6d 2073 7562 7072  s.    from subpr
-000218d0: 6f63 6573 7320 696d 706f 7274 2063 6865  ocess import che
-000218e0: 636b 5f6f 7574 7075 740a 0a20 2020 2069  ck_output..    i
-000218f0: 6620 6669 6c65 6e61 6d65 2069 6e20 5f63  f filename in _c
-00021900: 665f 6361 6368 653a 0a20 2020 2020 2020  f_cache:.       
-00021910: 2072 6574 7572 6e20 5f63 665f 6361 6368   return _cf_cach
-00021920: 655b 6669 6c65 6e61 6d65 5d0a 2020 2020  e[filename].    
-00021930: 6465 6275 675f 6d6f 6465 203d 2069 6e74  debug_mode = int
-00021940: 286f 732e 656e 7669 726f 6e2e 6765 7428  (os.environ.get(
-00021950: 2244 4542 5547 222c 2030 2929 0a20 2020  "DEBUG", 0)).   
-00021960: 2069 6620 6465 6275 675f 6d6f 6465 206f   if debug_mode o
-00021970: 7220 6765 745f 686f 7374 6e61 6d65 2829  r get_hostname()
-00021980: 203d 3d20 2263 6c75 7374 6572 2d63 6e2d   == "cluster-cn-
-00021990: 3231 3122 206f 7220 6e6f 7420 6973 5f72  211" or not is_r
-000219a0: 756e 6e69 6e67 5f6f 6e5f 636c 7573 7465  unning_on_cluste
-000219b0: 7228 293a 0a20 2020 2020 2020 2069 6620  r():.        if 
-000219c0: 6e6f 7420 5f63 665f 6d73 675f 7072 696e  not _cf_msg_prin
-000219d0: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
-000219e0: 2070 7269 6e74 2822 4361 6368 6520 6d61   print("Cache ma
-000219f0: 6e61 6765 723a 206e 6f74 2075 7365 642c  nager: not used,
-00021a00: 2075 7365 206c 6f63 616c 2066 696c 653a   use local file:
-00021a10: 2025 7320 2864 6973 6361 7264 2066 7572   %s (discard fur
-00021a20: 7468 6572 206d 6573 7361 6765 7329 2220  ther messages)" 
-00021a30: 2520 6669 6c65 6e61 6d65 290a 2020 2020  % filename).    
-00021a40: 2020 2020 2020 2020 5f63 665f 6d73 675f          _cf_msg_
-00021a50: 7072 696e 7465 6420 3d20 5472 7565 0a20  printed = True. 
-00021a60: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
-00021a70: 6c65 6e61 6d65 2020 2320 666f 7220 6465  lename  # for de
-00021a80: 6275 6767 696e 670a 2020 2020 7472 793a  bugging.    try:
-00021a90: 0a20 2020 2020 2020 2063 6163 6865 645f  .        cached_
-00021aa0: 666e 203d 2063 6865 636b 5f6f 7574 7075  fn = check_outpu
-00021ab0: 7428 5b22 6366 222c 2066 696c 656e 616d  t(["cf", filenam
-00021ac0: 655d 292e 7374 7269 7028 292e 6465 636f  e]).strip().deco
-00021ad0: 6465 2822 7574 6638 2229 0a20 2020 2065  de("utf8").    e
-00021ae0: 7863 6570 7420 4361 6c6c 6564 5072 6f63  xcept CalledProc
-00021af0: 6573 7345 7272 6f72 3a0a 2020 2020 2020  essError:.      
-00021b00: 2020 6966 206e 6f74 205f 6366 5f6d 7367    if not _cf_msg
-00021b10: 5f70 7269 6e74 6564 3a0a 2020 2020 2020  _printed:.      
-00021b20: 2020 2020 2020 7072 696e 7428 2243 6163        print("Cac
-00021b30: 6865 206d 616e 6167 6572 3a20 4572 726f  he manager: Erro
-00021b40: 7220 6f63 6375 7272 6564 2c20 7573 696e  r occurred, usin
-00021b50: 6720 6c6f 6361 6c20 6669 6c65 2229 0a20  g local file"). 
-00021b60: 2020 2020 2020 2020 2020 205f 6366 5f6d             _cf_m
-00021b70: 7367 5f70 7269 6e74 6564 203d 2054 7275  sg_printed = Tru
-00021b80: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00021b90: 2066 696c 656e 616d 650a 2020 2020 6173   filename.    as
-00021ba0: 7365 7274 206f 732e 7061 7468 2e65 7869  sert os.path.exi
-00021bb0: 7374 7328 6361 6368 6564 5f66 6e29 0a20  sts(cached_fn). 
-00021bc0: 2020 205f 6366 5f63 6163 6865 5b66 696c     _cf_cache[fil
-00021bd0: 656e 616d 655d 203d 2063 6163 6865 645f  ename] = cached_
-00021be0: 666e 0a20 2020 2072 6574 7572 6e20 6361  fn.    return ca
-00021bf0: 6368 6564 5f66 6e0a 0a0a 6465 6620 6269  ched_fn...def bi
-00021c00: 6e61 7279 5f73 6561 7263 685f 616e 7928  nary_search_any(
-00021c10: 636d 702c 206c 6f77 2c20 6869 6768 293a  cmp, low, high):
-00021c20: 0a20 2020 2022 2222 0a20 2020 2042 696e  .    """.    Bin
-00021c30: 6172 7920 7365 6172 6368 2066 6f72 2061  ary search for a
-00021c40: 2063 7573 746f 6d20 636f 6d70 6172 6520   custom compare 
-00021c50: 6675 6e63 7469 6f6e 2e0a 0a20 2020 203a  function...    :
-00021c60: 7061 7261 6d20 2869 6e74 292d 3e69 6e74  param (int)->int
-00021c70: 2063 6d70 3a20 652e 672e 2063 6d70 2869   cmp: e.g. cmp(i
-00021c80: 6478 2920 3d3d 2063 6f6d 7061 7265 2861  dx) == compare(a
-00021c90: 7272 6179 5b69 6478 5d2c 206b 6579 290a  rray[idx], key).
-00021ca0: 2020 2020 3a70 6172 616d 2069 6e74 206c      :param int l
-00021cb0: 6f77 3a20 696e 636c 7573 6976 650a 2020  ow: inclusive.  
-00021cc0: 2020 3a70 6172 616d 2069 6e74 2068 6967    :param int hig
-00021cd0: 683a 2065 7863 6c75 7369 7665 0a20 2020  h: exclusive.   
-00021ce0: 203a 7274 7970 653a 2069 6e74 7c4e 6f6e   :rtype: int|Non
-00021cf0: 650a 2020 2020 2222 220a 2020 2020 7768  e.    """.    wh
-00021d00: 696c 6520 6c6f 7720 3c20 6869 6768 3a0a  ile low < high:.
-00021d10: 2020 2020 2020 2020 6d69 6420 3d20 286c          mid = (l
-00021d20: 6f77 202b 2068 6967 6829 202f 2f20 320a  ow + high) // 2.
-00021d30: 2020 2020 2020 2020 7220 3d20 636d 7028          r = cmp(
-00021d40: 6d69 6429 0a20 2020 2020 2020 2069 6620  mid).        if 
-00021d50: 7220 3c20 303a 0a20 2020 2020 2020 2020  r < 0:.         
-00021d60: 2020 206c 6f77 203d 206d 6964 202b 2031     low = mid + 1
-00021d70: 0a20 2020 2020 2020 2065 6c69 6620 7220  .        elif r 
-00021d80: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-00021d90: 2068 6967 6820 3d20 6d69 640a 2020 2020   high = mid.    
-00021da0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00021db0: 2020 2020 2020 7265 7475 726e 206d 6964        return mid
-00021dc0: 0a20 2020 2072 6574 7572 6e20 6c6f 770a  .    return low.
-00021dd0: 0a0a 6465 6620 6765 6e65 7269 635f 696d  ..def generic_im
-00021de0: 706f 7274 5f6d 6f64 756c 6528 6669 6c65  port_module(file
-00021df0: 6e61 6d65 293a 0a20 2020 2022 2222 0a20  name):.    """. 
-00021e00: 2020 203a 7061 7261 6d20 7374 7220 6669     :param str fi
-00021e10: 6c65 6e61 6d65 3a0a 2020 2020 2020 5765  lename:.      We
-00021e20: 2074 7279 2074 6f20 6265 2063 6c65 7665   try to be cleve
-00021e30: 7220 6162 6f75 7420 6669 6c65 6e61 6d65  r about filename
-00021e40: 2e0a 2020 2020 2020 4966 2069 7420 6c6f  ..      If it lo
-00021e50: 6f6b 7320 6c69 6b65 2061 206d 6f64 756c  oks like a modul
-00021e60: 6520 6e61 6d65 2c20 6a75 7374 2064 6f20  e name, just do 
-00021e70: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
-00021e80: 5f6d 6f64 756c 652e 0a20 2020 2020 2049  _module..      I
-00021e90: 6620 6974 206c 6f6f 6b73 206c 696b 6520  f it looks like 
-00021ea0: 6120 6669 6c65 6e61 6d65 2c20 7365 6172  a filename, sear
-00021eb0: 6368 2066 6f72 2061 2062 6173 6520 7061  ch for a base pa
-00021ec0: 7468 2028 7768 6963 6820 646f 6573 206e  th (which does n
-00021ed0: 6f74 2068 6176 6520 5f5f 696e 6974 5f5f  ot have __init__
-00021ee0: 2e70 7929 2c0a 2020 2020 2020 6164 6420  .py),.      add 
-00021ef0: 7468 6174 2070 6174 6820 746f 2073 7973  that path to sys
-00021f00: 2e70 6174 6820 6966 206e 6565 6465 642c  .path if needed,
-00021f10: 2061 6e64 2069 6d70 6f72 7420 7468 6520   and import the 
-00021f20: 7265 6d61 696e 696e 6720 7768 6572 6520  remaining where 
-00021f30: 222f 2220 6973 2072 6570 6c61 6365 6420  "/" is replaced 
-00021f40: 6279 2022 2e22 0a20 2020 2020 2061 6e64  by ".".      and
-00021f50: 2074 6865 2066 696c 6520 6578 7465 6e73   the file extens
-00021f60: 696f 6e20 6973 2072 656d 6f76 6564 2e0a  ion is removed..
-00021f70: 2020 2020 3a72 6574 7572 6e3a 2074 6865      :return: the
-00021f80: 206d 6f64 756c 650a 2020 2020 3a72 7479   module.    :rty
-00021f90: 7065 3a20 7479 7065 732e 4d6f 6475 6c65  pe: types.Module
-00021fa0: 5479 7065 0a20 2020 2022 2222 0a20 2020  Type.    """.   
-00021fb0: 2061 7373 6572 7420 6669 6c65 6e61 6d65   assert filename
-00021fc0: 0a20 2020 2069 6d70 6f72 7420 696d 706f  .    import impo
-00021fd0: 7274 6c69 620a 0a20 2020 2069 6620 222f  rtlib..    if "/
-00021fe0: 2220 6e6f 7420 696e 2066 696c 656e 616d  " not in filenam
-00021ff0: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-00022000: 6e20 696d 706f 7274 6c69 622e 696d 706f  n importlib.impo
-00022010: 7274 5f6d 6f64 756c 6528 6669 6c65 6e61  rt_module(filena
-00022020: 6d65 290a 2020 2020 7072 6566 6978 5f64  me).    prefix_d
-00022030: 6972 203d 2022 220a 2020 2020 6966 206e  ir = "".    if n
-00022040: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
-00022050: 7328 6669 6c65 6e61 6d65 293a 0a20 2020  s(filename):.   
-00022060: 2020 2020 2061 7373 6572 7420 6669 6c65       assert file
-00022070: 6e61 6d65 5b30 5d20 213d 2022 2f22 0a20  name[0] != "/". 
-00022080: 2020 2020 2020 2023 204d 6179 6265 2072         # Maybe r
-00022090: 656c 6174 6976 6520 746f 2052 6574 7572  elative to Retur
-000220a0: 6e6e 3f0a 2020 2020 2020 2020 7072 6566  nn?.        pref
-000220b0: 6978 5f64 6972 203d 2022 2573 2f22 2025  ix_dir = "%s/" %
-000220c0: 2072 6574 7572 6e6e 5f72 6f6f 745f 6469   returnn_root_di
-000220d0: 720a 2020 2020 6173 7365 7274 206f 732e  r.    assert os.
-000220e0: 7061 7468 2e65 7869 7374 7328 7072 6566  path.exists(pref
-000220f0: 6978 5f64 6972 202b 2066 696c 656e 616d  ix_dir + filenam
-00022100: 6529 0a20 2020 2061 7373 6572 7420 6669  e).    assert fi
-00022110: 6c65 6e61 6d65 2e65 6e64 7377 6974 6828  lename.endswith(
-00022120: 222e 7079 2229 206f 7220 6f73 2e70 6174  ".py") or os.pat
-00022130: 682e 6973 6469 7228 7072 6566 6978 5f64  h.isdir(prefix_d
-00022140: 6972 202b 2066 696c 656e 616d 6529 0a20  ir + filename). 
-00022150: 2020 2064 6972 7320 3d20 6669 6c65 6e61     dirs = filena
-00022160: 6d65 2e73 706c 6974 2822 2f22 290a 2020  me.split("/").  
-00022170: 2020 6469 7273 2c20 6261 7365 5f66 6e20    dirs, base_fn 
-00022180: 3d20 6469 7273 5b3a 2d31 5d2c 2064 6972  = dirs[:-1], dir
-00022190: 735b 2d31 5d0a 2020 2020 6173 7365 7274  s[-1].    assert
-000221a0: 206c 656e 2864 6972 7329 203e 3d20 310a   len(dirs) >= 1.
-000221b0: 2020 2020 666f 7220 6920 696e 2072 6576      for i in rev
-000221c0: 6572 7365 6428 7261 6e67 6528 6c65 6e28  ersed(range(len(
-000221d0: 6469 7273 2929 293a 0a20 2020 2020 2020  dirs))):.       
-000221e0: 2064 203d 2070 7265 6669 785f 6469 7220   d = prefix_dir 
-000221f0: 2b20 222f 222e 6a6f 696e 2864 6972 735b  + "/".join(dirs[
-00022200: 3a20 6920 2b20 315d 290a 2020 2020 2020  : i + 1]).      
-00022210: 2020 6173 7365 7274 206f 732e 7061 7468    assert os.path
-00022220: 2e69 7364 6972 2864 290a 2020 2020 2020  .isdir(d).      
-00022230: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
-00022240: 7374 7328 2225 732f 5f5f 696e 6974 5f5f  sts("%s/__init__
-00022250: 2e70 7922 2025 2064 293a 0a20 2020 2020  .py" % d):.     
-00022260: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00022270: 2020 2020 2020 2020 6966 2064 206e 6f74          if d not
-00022280: 2069 6e20 7379 732e 7061 7468 3a0a 2020   in sys.path:.  
-00022290: 2020 2020 2020 2020 2020 7379 732e 7061            sys.pa
-000222a0: 7468 2e61 7070 656e 6428 6429 0a20 2020  th.append(d).   
-000222b0: 2020 2020 206d 203d 2022 2e22 2e6a 6f69       m = ".".joi
-000222c0: 6e28 6469 7273 5b69 202b 2031 203a 5d20  n(dirs[i + 1 :] 
-000222d0: 2b20 5b62 6173 655f 666e 5d29 0a20 2020  + [base_fn]).   
-000222e0: 2020 2020 2069 6620 6261 7365 5f66 6e2e       if base_fn.
-000222f0: 656e 6473 7769 7468 2822 2e70 7922 293a  endswith(".py"):
-00022300: 0a20 2020 2020 2020 2020 2020 206d 203d  .            m =
-00022310: 206d 5b3a 2d33 5d0a 2020 2020 2020 2020   m[:-3].        
-00022320: 7265 7475 726e 2069 6d70 6f72 746c 6962  return importlib
-00022330: 2e69 6d70 6f72 745f 6d6f 6475 6c65 286d  .import_module(m
-00022340: 290a 2020 2020 7261 6973 6520 5661 6c75  ).    raise Valu
-00022350: 6545 7272 6f72 2822 6361 6e6e 6f74 2066  eError("cannot f
-00022360: 6967 7572 6520 6f75 7420 6261 7365 206d  igure out base m
-00022370: 6f64 756c 6520 7061 7468 2066 726f 6d20  odule path from 
-00022380: 2572 2220 2520 6669 6c65 6e61 6d65 290a  %r" % filename).
-00022390: 0a0a 6465 6620 736f 6674 6d61 7828 782c  ..def softmax(x,
-000223a0: 2061 7869 733d 4e6f 6e65 293a 0a20 2020   axis=None):.   
-000223b0: 2022 2222 0a20 2020 203a 7061 7261 6d20   """.    :param 
-000223c0: 6e75 6d70 792e 6e64 6172 7261 7920 783a  numpy.ndarray x:
-000223d0: 0a20 2020 203a 7061 7261 6d20 696e 747c  .    :param int|
-000223e0: 4e6f 6e65 2061 7869 733a 0a20 2020 203a  None axis:.    :
-000223f0: 7274 7970 653a 206e 756d 7079 2e6e 6461  rtype: numpy.nda
-00022400: 7272 6179 0a20 2020 2022 2222 0a20 2020  rray.    """.   
-00022410: 2069 6d70 6f72 7420 6e75 6d70 790a 0a20   import numpy.. 
-00022420: 2020 2065 5f78 203d 206e 756d 7079 2e65     e_x = numpy.e
-00022430: 7870 2878 202d 206e 756d 7079 2e6d 6178  xp(x - numpy.max
-00022440: 2878 2c20 6178 6973 3d61 7869 732c 206b  (x, axis=axis, k
-00022450: 6565 7064 696d 733d 5472 7565 2929 0a20  eepdims=True)). 
-00022460: 2020 2072 6574 7572 6e20 655f 7820 2f20     return e_x / 
-00022470: 6e75 6d70 792e 7375 6d28 655f 782c 2061  numpy.sum(e_x, a
-00022480: 7869 733d 6178 6973 2c20 6b65 6570 6469  xis=axis, keepdi
-00022490: 6d73 3d54 7275 6529 0a0a 0a64 6566 2063  ms=True)...def c
-000224a0: 6f6c 6c65 6374 5f70 726f 635f 6d61 7073  ollect_proc_maps
-000224b0: 5f65 7865 635f 6669 6c65 7328 293a 0a20  _exec_files():. 
-000224c0: 2020 2022 2222 0a20 2020 2043 7572 7265     """.    Curre
-000224d0: 6e74 6c79 206f 6e6c 7920 776f 726b 7320  ntly only works 
-000224e0: 6f6e 204c 696e 7578 2e2e 2e0a 0a20 2020  on Linux.....   
-000224f0: 203a 7265 7475 726e 3a20 6c69 7374 206f   :return: list o
-00022500: 6620 6d61 7070 6564 2065 7865 6375 7461  f mapped executa
-00022510: 626c 6573 2028 6c69 6273 290a 2020 2020  bles (libs).    
-00022520: 3a72 7479 7065 3a20 6c69 7374 5b73 7472  :rtype: list[str
-00022530: 5d0a 2020 2020 2222 220a 2020 2020 696d  ].    """.    im
-00022540: 706f 7274 2072 650a 0a20 2020 2070 6964  port re..    pid
-00022550: 203d 206f 732e 6765 7470 6964 2829 0a20   = os.getpid(). 
-00022560: 2020 2066 6e73 203d 205b 5d0a 2020 2020     fns = [].    
-00022570: 666f 7220 6c69 6e65 2069 6e20 6f70 656e  for line in open
-00022580: 2822 2f70 726f 632f 2569 2f6d 6170 7322  ("/proc/%i/maps"
-00022590: 2025 2070 6964 2c20 2272 2229 2e72 6561   % pid, "r").rea
-000225a0: 6428 292e 7370 6c69 746c 696e 6573 2829  d().splitlines()
-000225b0: 3a20 2023 2066 6f72 2065 6163 6820 6d61  :  # for each ma
-000225c0: 7070 6564 2072 6567 696f 6e0a 2020 2020  pped region.    
-000225d0: 2020 2020 2320 6874 7470 733a 2f2f 7374      # https://st
-000225e0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
-000225f0: 7175 6573 7469 6f6e 732f 3134 3031 3335  questions/140135
-00022600: 392f 756e 6465 7273 7461 6e64 696e 672d  9/understanding-
-00022610: 6c69 6e75 782d 7072 6f63 2d69 642d 6d61  linux-proc-id-ma
-00022620: 7073 0a20 2020 2020 2020 2023 2061 6464  ps.        # add
-00022630: 7265 7373 2020 2020 2020 2020 2020 2070  ress           p
-00022640: 6572 6d73 206f 6666 7365 7420 2064 6576  erms offset  dev
-00022650: 2020 2069 6e6f 6465 2020 2070 6174 686e     inode   pathn
-00022660: 616d 650a 2020 2020 2020 2020 2320 452e  ame.        # E.
-00022670: 672e 3a0a 2020 2020 2020 2020 2320 3766  g.:.        # 7f
-00022680: 6632 6465 3931 6330 3030 2d37 6666 3264  f2de91c000-7ff2d
-00022690: 6539 3165 3030 3020 7277 2d70 2030 3031  e91e000 rw-p 001
-000226a0: 3763 3030 3020 3038 3a30 3220 3739 3438  7c000 08:02 7948
-000226b0: 3434 2020 2020 2020 2020 2020 2020 2020  44              
-000226c0: 2020 2020 2020 202f 7573 722f 6c69 622f         /usr/lib/
-000226d0: 7838 365f 3634 2d6c 696e 7578 2d67 6e75  x86_64-linux-gnu
-000226e0: 2f6c 6962 7374 6463 2b2e 2e2e 0a20 2020  /libstdc+....   
-000226f0: 2020 2020 206d 203d 2072 652e 6d61 7463       m = re.matc
-00022700: 6828 0a20 2020 2020 2020 2020 2020 2072  h(.            r
-00022710: 225e 285b 302d 3941 2d46 612d 665d 2b29  "^([0-9A-Fa-f]+)
-00022720: 2d28 5b30 2d39 412d 4661 2d66 5d2b 295c  -([0-9A-Fa-f]+)\
-00022730: 732b 285b 7277 7870 735c 2d5d 2b29 5c73  s+([rwxps\-]+)\s
-00022740: 2b28 5b30 2d39 412d 4661 2d66 5d2b 295c  +([0-9A-Fa-f]+)\
-00022750: 732b 285b 302d 3941 2d46 612d 663a 5d2b  s+([0-9A-Fa-f:]+
-00022760: 295c 732b 285b 302d 395d 2b29 5c73 2a28  )\s+([0-9]+)\s*(
-00022770: 2e2a 2924 222c 206c 696e 650a 2020 2020  .*)$", line.    
-00022780: 2020 2020 290a 2020 2020 2020 2020 6173      ).        as
-00022790: 7365 7274 206d 2c20 226e 6f20 6d61 7463  sert m, "no matc
-000227a0: 6820 666f 7220 2572 2220 2520 6c69 6e65  h for %r" % line
-000227b0: 0a20 2020 2020 2020 2061 6464 7265 7373  .        address
-000227c0: 5f73 7461 7274 2c20 6164 6472 6573 735f  _start, address_
-000227d0: 656e 642c 2070 6572 6d73 2c20 6f66 6673  end, perms, offs
-000227e0: 6574 2c20 6465 762c 2069 5f6e 6f64 652c  et, dev, i_node,
-000227f0: 2070 6174 685f 6e61 6d65 203d 206d 2e67   path_name = m.g
-00022800: 726f 7570 7328 290a 2020 2020 2020 2020  roups().        
-00022810: 6966 2022 7822 206e 6f74 2069 6e20 7065  if "x" not in pe
-00022820: 726d 733a 0a20 2020 2020 2020 2020 2020  rms:.           
-00022830: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-00022840: 2020 6966 206e 6f74 2070 6174 685f 6e61    if not path_na
-00022850: 6d65 206f 7220 7061 7468 5f6e 616d 652e  me or path_name.
-00022860: 7374 6172 7473 7769 7468 2822 5b22 2920  startswith("[") 
-00022870: 6f72 2022 2864 656c 6574 6564 2922 2069  or "(deleted)" i
-00022880: 6e20 7061 7468 5f6e 616d 653a 0a20 2020  n path_name:.   
-00022890: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000228a0: 650a 2020 2020 2020 2020 6966 2070 6174  e.        if pat
-000228b0: 685f 6e61 6d65 206e 6f74 2069 6e20 666e  h_name not in fn
-000228c0: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-000228d0: 6e73 2e61 7070 656e 6428 7061 7468 5f6e  ns.append(path_n
-000228e0: 616d 6529 0a20 2020 2072 6574 7572 6e20  ame).    return 
-000228f0: 666e 730a 0a0a 6465 6620 6669 6e64 5f73  fns...def find_s
-00022900: 796d 5f69 6e5f 6578 6563 2866 6e2c 2073  ym_in_exec(fn, s
-00022910: 796d 293a 0a20 2020 2022 2222 0a20 2020  ym):.    """.   
-00022920: 2055 7365 7320 6060 6f62 6a64 756d 7060   Uses ``objdump`
-00022930: 6020 746f 206c 6973 7420 6176 6169 6c61  ` to list availa
-00022940: 626c 6520 7379 6d62 6f6c 732c 2061 6e64  ble symbols, and
-00022950: 2066 696c 7465 7273 2074 6865 6d20 6279   filters them by
-00022960: 2074 6865 2067 6976 656e 2060 6073 796d   the given ``sym
-00022970: 6060 2e0a 0a20 2020 203a 7061 7261 6d20  ``...    :param 
-00022980: 7374 7220 666e 3a20 7061 7468 0a20 2020  str fn: path.   
-00022990: 203a 7061 7261 6d20 7374 7220 7379 6d3a   :param str sym:
-000229a0: 0a20 2020 203a 7265 7475 726e 3a20 6d61  .    :return: ma
-000229b0: 7463 6865 6420 6f75 742c 206f 7220 4e6f  tched out, or No
-000229c0: 6e65 0a20 2020 203a 7274 7970 653a 2073  ne.    :rtype: s
-000229d0: 7472 7c4e 6f6e 650a 2020 2020 2222 220a  tr|None.    """.
-000229e0: 2020 2020 6672 6f6d 2073 7562 7072 6f63      from subproc
-000229f0: 6573 7320 696d 706f 7274 2043 616c 6c65  ess import Calle
-00022a00: 6450 726f 6365 7373 4572 726f 720a 0a20  dProcessError.. 
-00022a10: 2020 206f 626a 6475 6d70 203d 2022 6f62     objdump = "ob
-00022a20: 6a64 756d 7020 2d54 220a 2020 2020 6966  jdump -T".    if
-00022a30: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-00022a40: 2022 6461 7277 696e 223a 0a20 2020 2020   "darwin":.     
-00022a50: 2020 206f 626a 6475 6d70 203d 2022 6f74     objdump = "ot
-00022a60: 6f6f 6c20 2d49 4847 7622 0a20 2020 2073  ool -IHGv".    s
-00022a70: 6865 6c6c 5f63 6d64 203d 2022 2573 2025  hell_cmd = "%s %
-00022a80: 7320 7c20 6772 6570 2025 7322 2025 2028  s | grep %s" % (
-00022a90: 6f62 6a64 756d 702c 2066 6e2c 2073 796d  objdump, fn, sym
-00022aa0: 290a 2020 2020 7472 793a 0a20 2020 2020  ).    try:.     
-00022ab0: 2020 206f 7574 203d 2073 7973 5f65 7865     out = sys_exe
-00022ac0: 635f 6f75 7428 7368 656c 6c5f 636d 642c  c_out(shell_cmd,
-00022ad0: 2073 6865 6c6c 3d54 7275 6529 0a20 2020   shell=True).   
-00022ae0: 2065 7863 6570 7420 4361 6c6c 6564 5072   except CalledPr
-00022af0: 6f63 6573 7345 7272 6f72 3a20 2023 206e  ocessError:  # n
-00022b00: 6f6e 6520 666f 756e 640a 2020 2020 2020  one found.      
-00022b10: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00022b20: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00022b30: 6e63 6528 6f75 742c 2028 7374 722c 2075  nce(out, (str, u
-00022b40: 6e69 636f 6465 2929 0a20 2020 206f 7574  nicode)).    out
-00022b50: 5f6c 6e73 203d 206f 7574 2e73 706c 6974  _lns = out.split
-00022b60: 6c69 6e65 7328 290a 2020 2020 6f75 745f  lines().    out_
-00022b70: 6c6e 7320 3d20 5b6c 6e20 666f 7220 6c6e  lns = [ln for ln
-00022b80: 2069 6e20 6f75 745f 6c6e 7320 6966 2022   in out_lns if "
-00022b90: 2e74 6578 7422 2069 6e20 6c6e 5d20 2023  .text" in ln]  #
-00022ba0: 2073 6565 206f 626a 6475 6d70 0a20 2020   see objdump.   
-00022bb0: 206f 7574 5f6c 6e73 203d 205b 6c6e 2066   out_lns = [ln f
-00022bc0: 6f72 206c 6e20 696e 206f 7574 5f6c 6e73  or ln in out_lns
-00022bd0: 2069 6620 7379 6d20 696e 206c 6e2e 7370   if sym in ln.sp
-00022be0: 6c69 7428 295d 0a20 2020 2069 6620 6e6f  lit()].    if no
-00022bf0: 7420 6f75 745f 6c6e 733a 0a20 2020 2020  t out_lns:.     
-00022c00: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00022c10: 2020 2072 6574 7572 6e20 2246 6f75 6e64     return "Found
-00022c20: 2025 7220 696e 2025 723a 5c6e 2573 2220   %r in %r:\n%s" 
-00022c30: 2520 2873 796d 2c20 666e 2c20 225c 6e22  % (sym, fn, "\n"
-00022c40: 2e6a 6f69 6e28 6f75 745f 6c6e 7329 290a  .join(out_lns)).
-00022c50: 0a0a 6465 6620 6475 6d6d 795f 6e75 6d70  ..def dummy_nump
-00022c60: 795f 6765 6d6d 5f63 616c 6c28 293a 0a20  y_gemm_call():. 
-00022c70: 2020 2022 2222 0a20 2020 204a 7573 7420     """.    Just 
-00022c80: 7065 7266 6f72 6d73 2073 6f6d 6520 4745  performs some GE
-00022c90: 4d4d 2063 616c 6c20 7669 6120 4e75 6d70  MM call via Nump
-00022ca0: 792e 0a20 2020 2054 6869 7320 6d61 6b65  y..    This make
-00022cb0: 7320 7375 7265 2074 6861 7420 7468 6520  s sure that the 
-00022cc0: 424c 4153 206c 6962 7261 7279 2069 7320  BLAS library is 
-00022cd0: 6c6f 6164 6564 2e0a 2020 2020 2222 220a  loaded..    """.
-00022ce0: 2020 2020 696d 706f 7274 206e 756d 7079      import numpy
-00022cf0: 0a0a 2020 2020 6120 3d20 6e75 6d70 792e  ..    a = numpy.
-00022d00: 7261 6e64 6f6d 2e72 616e 646e 2835 2c20  random.randn(5, 
-00022d10: 3329 2e61 7374 7970 6528 6e75 6d70 792e  3).astype(numpy.
-00022d20: 666c 6f61 7433 3229 0a20 2020 2062 203d  float32).    b =
-00022d30: 206e 756d 7079 2e72 616e 646f 6d2e 7261   numpy.random.ra
-00022d40: 6e64 6e28 332c 2037 292e 6173 7479 7065  ndn(3, 7).astype
-00022d50: 286e 756d 7079 2e66 6c6f 6174 3332 290a  (numpy.float32).
-00022d60: 2020 2020 6320 3d20 6e75 6d70 792e 646f      c = numpy.do
-00022d70: 7428 612c 2062 290a 2020 2020 6173 7365  t(a, b).    asse
-00022d80: 7274 206e 756d 7079 2e69 7366 696e 6974  rt numpy.isfinit
-00022d90: 6528 6329 2e61 6c6c 2829 0a0a 0a5f 6669  e(c).all()..._fi
-00022da0: 6e64 5f73 6765 6d6d 5f6c 6962 5f66 726f  nd_sgemm_lib_fro
-00022db0: 6d5f 7275 6e74 696d 655f 6361 6368 6564  m_runtime_cached
-00022dc0: 203d 204e 6f6e 650a 0a0a 6465 6620 6669   = None...def fi
-00022dd0: 6e64 5f73 6765 6d6d 5f6c 6962 735f 6672  nd_sgemm_libs_fr
-00022de0: 6f6d 5f72 756e 7469 6d65 2829 3a0a 2020  om_runtime():.  
-00022df0: 2020 2222 220a 2020 2020 4c6f 6f6b 7320    """.    Looks 
-00022e00: 7468 726f 7567 6820 616c 6c20 6c69 6273  through all libs
-00022e10: 2076 6961 203a 6675 6e63 3a60 636f 6c6c   via :func:`coll
-00022e20: 6563 745f 7072 6f63 5f6d 6170 735f 6578  ect_proc_maps_ex
-00022e30: 6563 5f66 696c 6573 602c 0a20 2020 2061  ec_files`,.    a
-00022e40: 6e64 2073 6561 7263 6865 7320 666f 7220  nd searches for 
-00022e50: 616c 6c20 7768 6963 6820 6861 7665 2074  all which have t
-00022e60: 6865 2060 6073 6765 6d6d 6060 2073 796d  he ``sgemm`` sym
-00022e70: 626f 6c2e 0a20 2020 2043 7572 7265 6e74  bol..    Current
-00022e80: 6c79 206f 6e6c 7920 776f 726b 7320 6f6e  ly only works on
-00022e90: 204c 696e 7578 2028 6265 6361 7573 6520   Linux (because 
-00022ea0: 636f 6c6c 6563 745f 7072 6f63 5f6d 6170  collect_proc_map
-00022eb0: 735f 6578 6563 5f66 696c 6573 292e 0a0a  s_exec_files)...
-00022ec0: 2020 2020 3a72 6574 7572 6e3a 206c 6973      :return: lis
-00022ed0: 7420 6f66 206c 6962 7320 2874 6865 6972  t of libs (their
-00022ee0: 2070 6174 6829 0a20 2020 203a 7274 7970   path).    :rtyp
-00022ef0: 653a 206c 6973 745b 7374 725d 0a20 2020  e: list[str].   
-00022f00: 2022 2222 0a20 2020 2069 6620 6e6f 7420   """.    if not 
-00022f10: 6f73 2e70 6174 682e 6578 6973 7473 2822  os.path.exists("
-00022f20: 2f70 726f 6322 293a 0a20 2020 2020 2020  /proc"):.       
-00022f30: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
-00022f40: 2067 6c6f 6261 6c20 5f66 696e 645f 7367   global _find_sg
-00022f50: 656d 6d5f 6c69 625f 6672 6f6d 5f72 756e  emm_lib_from_run
-00022f60: 7469 6d65 5f63 6163 6865 640a 2020 2020  time_cached.    
-00022f70: 6966 205f 6669 6e64 5f73 6765 6d6d 5f6c  if _find_sgemm_l
-00022f80: 6962 5f66 726f 6d5f 7275 6e74 696d 655f  ib_from_runtime_
-00022f90: 6361 6368 6564 2069 7320 6e6f 7420 4e6f  cached is not No
-00022fa0: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
-00022fb0: 726e 205f 6669 6e64 5f73 6765 6d6d 5f6c  rn _find_sgemm_l
-00022fc0: 6962 5f66 726f 6d5f 7275 6e74 696d 655f  ib_from_runtime_
-00022fd0: 6361 6368 6564 0a20 2020 2064 756d 6d79  cached.    dummy
-00022fe0: 5f6e 756d 7079 5f67 656d 6d5f 6361 6c6c  _numpy_gemm_call
-00022ff0: 2829 2020 2320 6d61 6b65 2073 7572 6520  ()  # make sure 
-00023000: 7468 6174 204e 756d 7079 2069 7320 6c6f  that Numpy is lo
-00023010: 6164 6564 2061 6e64 204e 756d 7079 2073  aded and Numpy s
-00023020: 6765 6d6d 2069 7320 6176 6169 6c61 626c  gemm is availabl
-00023030: 650a 2020 2020 666e 7320 3d20 636f 6c6c  e.    fns = coll
-00023040: 6563 745f 7072 6f63 5f6d 6170 735f 6578  ect_proc_maps_ex
-00023050: 6563 5f66 696c 6573 2829 0a20 2020 2066  ec_files().    f
-00023060: 6e73 5f77 6974 685f 7367 656d 6d20 3d20  ns_with_sgemm = 
-00023070: 5b5d 0a20 2020 2066 6f72 2066 6e20 696e  [].    for fn in
-00023080: 2066 6e73 3a0a 2020 2020 2020 2020 6f75   fns:.        ou
-00023090: 7420 3d20 6669 6e64 5f73 796d 5f69 6e5f  t = find_sym_in_
-000230a0: 6578 6563 2866 6e2c 2022 7367 656d 6d5f  exec(fn, "sgemm_
-000230b0: 2229 0a20 2020 2020 2020 2069 6620 6f75  ").        if ou
-000230c0: 743a 0a20 2020 2020 2020 2020 2020 2066  t:.            f
-000230d0: 6e73 5f77 6974 685f 7367 656d 6d2e 6170  ns_with_sgemm.ap
-000230e0: 7065 6e64 2866 6e29 0a20 2020 205f 6669  pend(fn).    _fi
-000230f0: 6e64 5f73 6765 6d6d 5f6c 6962 5f66 726f  nd_sgemm_lib_fro
-00023100: 6d5f 7275 6e74 696d 655f 6361 6368 6564  m_runtime_cached
-00023110: 203d 2066 6e73 5f77 6974 685f 7367 656d   = fns_with_sgem
-00023120: 6d0a 2020 2020 7265 7475 726e 2066 6e73  m.    return fns
-00023130: 5f77 6974 685f 7367 656d 6d0a 0a0a 5f66  _with_sgemm..._f
-00023140: 696e 645f 6c69 6263 7564 6172 745f 6672  ind_libcudart_fr
-00023150: 6f6d 5f72 756e 7469 6d65 5f63 6163 6865  om_runtime_cache
-00023160: 6420 3d20 4e6f 6e65 0a0a 0a64 6566 2066  d = None...def f
-00023170: 696e 645f 6c69 6263 7564 6172 745f 6672  ind_libcudart_fr
-00023180: 6f6d 5f72 756e 7469 6d65 2829 3a0a 2020  om_runtime():.  
-00023190: 2020 2222 220a 2020 2020 4c6f 6f6b 7320    """.    Looks 
-000231a0: 7468 726f 7567 6820 616c 6c20 6c69 6273  through all libs
-000231b0: 2076 6961 203a 6675 6e63 3a60 636f 6c6c   via :func:`coll
-000231c0: 6563 745f 7072 6f63 5f6d 6170 735f 6578  ect_proc_maps_ex
-000231d0: 6563 5f66 696c 6573 602c 0a20 2020 2061  ec_files`,.    a
-000231e0: 6e64 2073 6561 7263 6865 7320 666f 7220  nd searches for 
-000231f0: 616c 6c20 7768 6963 6820 6861 7665 2074  all which have t
-00023200: 6865 2060 6073 6765 6d6d 6060 2073 796d  he ``sgemm`` sym
-00023210: 626f 6c2e 0a20 2020 2043 7572 7265 6e74  bol..    Current
-00023220: 6c79 206f 6e6c 7920 776f 726b 7320 6f6e  ly only works on
-00023230: 204c 696e 7578 2028 6265 6361 7573 6520   Linux (because 
-00023240: 636f 6c6c 6563 745f 7072 6f63 5f6d 6170  collect_proc_map
-00023250: 735f 6578 6563 5f66 696c 6573 292e 0a0a  s_exec_files)...
-00023260: 2020 2020 3a72 6574 7572 6e3a 206c 6973      :return: lis
-00023270: 7420 6f66 206c 6962 7320 2874 6865 6972  t of libs (their
-00023280: 2070 6174 6829 0a20 2020 203a 7274 7970   path).    :rtyp
-00023290: 653a 2073 7472 7c4e 6f6e 650a 2020 2020  e: str|None.    
-000232a0: 2222 220a 2020 2020 6966 206e 6f74 206f  """.    if not o
-000232b0: 732e 7061 7468 2e65 7869 7374 7328 222f  s.path.exists("/
-000232c0: 7072 6f63 2229 3a0a 2020 2020 2020 2020  proc"):.        
-000232d0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-000232e0: 676c 6f62 616c 205f 6669 6e64 5f6c 6962  global _find_lib
-000232f0: 6375 6461 7274 5f66 726f 6d5f 7275 6e74  cudart_from_runt
-00023300: 696d 655f 6361 6368 6564 0a20 2020 2069  ime_cached.    i
-00023310: 6620 5f66 696e 645f 6c69 6263 7564 6172  f _find_libcudar
-00023320: 745f 6672 6f6d 5f72 756e 7469 6d65 5f63  t_from_runtime_c
-00023330: 6163 6865 6420 6973 206e 6f74 204e 6f6e  ached is not Non
-00023340: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-00023350: 6e20 5f66 696e 645f 6c69 6263 7564 6172  n _find_libcudar
-00023360: 745f 6672 6f6d 5f72 756e 7469 6d65 5f63  t_from_runtime_c
-00023370: 6163 6865 645b 305d 0a20 2020 2066 6e73  ached[0].    fns
-00023380: 203d 2063 6f6c 6c65 6374 5f70 726f 635f   = collect_proc_
-00023390: 6d61 7073 5f65 7865 635f 6669 6c65 7328  maps_exec_files(
-000233a0: 290a 2020 2020 666f 7220 666e 2069 6e20  ).    for fn in 
-000233b0: 666e 733a 0a20 2020 2020 2020 2069 6620  fns:.        if 
-000233c0: 7265 2e6d 6174 6368 2822 2e2a 2f6c 6962  re.match(".*/lib
-000233d0: 6375 6461 7274 5c5c 2e73 6f28 5c5c 2e2e  cudart\\.so(\\..
-000233e0: 2a29 3f22 2c20 666e 293a 0a20 2020 2020  *)?", fn):.     
-000233f0: 2020 2020 2020 205f 6669 6e64 5f6c 6962         _find_lib
-00023400: 6375 6461 7274 5f66 726f 6d5f 7275 6e74  cudart_from_runt
-00023410: 696d 655f 6361 6368 6564 203d 205b 666e  ime_cached = [fn
-00023420: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
-00023430: 7475 726e 2066 6e0a 2020 2020 5f66 696e  turn fn.    _fin
-00023440: 645f 6c69 6263 7564 6172 745f 6672 6f6d  d_libcudart_from
-00023450: 5f72 756e 7469 6d65 5f63 6163 6865 6420  _runtime_cached 
-00023460: 3d20 5b4e 6f6e 655d 0a20 2020 2072 6574  = [None].    ret
-00023470: 7572 6e20 4e6f 6e65 0a                   urn None.
+0001ac50: 650a 0a0a 5f64 6566 6175 6c74 5f67 6c6f  e..._default_glo
+0001ac60: 6261 6c5f 696e 665f 7661 6c75 6520 3d20  bal_inf_value = 
+0001ac70: 666c 6f61 7428 2269 6e66 2229 0a0a 0a64  float("inf")...d
+0001ac80: 6566 2067 6574 5f67 6c6f 6261 6c5f 696e  ef get_global_in
+0001ac90: 665f 7661 6c75 6528 2920 2d3e 2066 6c6f  f_value() -> flo
+0001aca0: 6174 3a0a 2020 2020 2222 220a 2020 2020  at:.    """.    
+0001acb0: 3a72 6574 7572 6e3a 2066 6c6f 6174 2822  :return: float("
+0001acc0: 696e 6622 2920 6279 2064 6566 6175 6c74  inf") by default
+0001acd0: 2c20 6275 7420 7472 6965 7320 746f 2072  , but tries to r
+0001ace0: 6561 6420 6069 6e66 5f76 616c 7565 6020  ead `inf_value` 
+0001acf0: 6672 6f6d 2074 6865 2067 6c6f 6261 6c20  from the global 
+0001ad00: 636f 6e66 6967 0a20 2020 2022 2222 0a20  config.    """. 
+0001ad10: 2020 2066 726f 6d20 7265 7475 726e 6e2e     from returnn.
+0001ad20: 636f 6e66 6967 2069 6d70 6f72 7420 6765  config import ge
+0001ad30: 745f 676c 6f62 616c 5f63 6f6e 6669 670a  t_global_config.
+0001ad40: 0a20 2020 2063 6f6e 6669 6720 3d20 6765  .    config = ge
+0001ad50: 745f 676c 6f62 616c 5f63 6f6e 6669 6728  t_global_config(
+0001ad60: 7261 6973 655f 6578 6365 7074 696f 6e3d  raise_exception=
+0001ad70: 4661 6c73 6529 0a20 2020 2069 6620 6e6f  False).    if no
+0001ad80: 7420 636f 6e66 6967 3a0a 2020 2020 2020  t config:.      
+0001ad90: 2020 7265 7475 726e 205f 6465 6661 756c    return _defaul
+0001ada0: 745f 676c 6f62 616c 5f69 6e66 5f76 616c  t_global_inf_val
+0001adb0: 7565 0a20 2020 2072 6574 7572 6e20 636f  ue.    return co
+0001adc0: 6e66 6967 2e66 6c6f 6174 2822 696e 665f  nfig.float("inf_
+0001add0: 7661 6c75 6522 2c20 5f64 6566 6175 6c74  value", _default
+0001ade0: 5f67 6c6f 6261 6c5f 696e 665f 7661 6c75  _global_inf_valu
+0001adf0: 6529 0a0a 0a63 6c61 7373 204e 6174 6976  e)...class Nativ
+0001ae00: 6543 6f64 6543 6f6d 7069 6c65 7228 6f62  eCodeCompiler(ob
+0001ae10: 6a65 6374 293a 0a20 2020 2022 2222 0a20  ject):.    """. 
+0001ae20: 2020 2048 656c 7065 7220 636c 6173 7320     Helper class 
+0001ae30: 746f 2063 6f6d 7069 6c65 206e 6174 6976  to compile nativ
+0001ae40: 6520 432f 432b 2b20 636f 6465 206f 6e2d  e C/C++ code on-
+0001ae50: 7468 652d 666c 792e 0a20 2020 2022 2222  the-fly..    """
+0001ae60: 0a0a 2020 2020 4361 6368 6544 6972 4e61  ..    CacheDirNa
+0001ae70: 6d65 203d 2022 7265 7475 726e 6e5f 6e61  me = "returnn_na
+0001ae80: 7469 7665 220a 2020 2020 436f 6c6c 6563  tive".    Collec
+0001ae90: 7465 6443 6f6d 7069 6c65 7273 203d 204e  tedCompilers = N
+0001aea0: 6f6e 6520 2023 2074 7970 653a 2074 7970  one  # type: typ
+0001aeb0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0001aec0: 696e 672e 4c69 7374 5b4e 6174 6976 6543  ing.List[NativeC
+0001aed0: 6f64 6543 6f6d 7069 6c65 725d 5d0a 0a20  odeCompiler]].. 
+0001aee0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0001aef0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0001af00: 2020 2020 2020 2062 6173 655f 6e61 6d65         base_name
+0001af10: 2c0a 2020 2020 2020 2020 636f 6465 5f76  ,.        code_v
+0001af20: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
+0001af30: 636f 6465 2c0a 2020 2020 2020 2020 6973  code,.        is
+0001af40: 5f63 7070 3d54 7275 652c 0a20 2020 2020  _cpp=True,.     
+0001af50: 2020 2063 5f6d 6163 726f 5f64 6566 696e     c_macro_defin
+0001af60: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
+0001af70: 206c 645f 666c 6167 733d 4e6f 6e65 2c0a   ld_flags=None,.
+0001af80: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+0001af90: 7061 7468 733d 2829 2c0a 2020 2020 2020  paths=(),.      
+0001afa0: 2020 696e 636c 7564 655f 6465 7073 3d4e    include_deps=N
+0001afb0: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+0001afc0: 7469 635f 7665 7273 696f 6e5f 6e61 6d65  tic_version_name
+0001afd0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2073  =None,.        s
+0001afe0: 686f 756c 645f 636c 6561 6e75 705f 6f6c  hould_cleanup_ol
+0001aff0: 645f 616c 6c3d 5472 7565 2c0a 2020 2020  d_all=True,.    
+0001b000: 2020 2020 7368 6f75 6c64 5f63 6c65 616e      should_clean
+0001b010: 7570 5f6f 6c64 5f6d 7964 6972 3d46 616c  up_old_mydir=Fal
+0001b020: 7365 2c0a 2020 2020 2020 2020 7573 655f  se,.        use_
+0001b030: 6378 7831 315f 6162 693d 4661 6c73 652c  cxx11_abi=False,
+0001b040: 0a20 2020 2020 2020 206c 6f67 5f73 7472  .        log_str
+0001b050: 6561 6d3d 4e6f 6e65 2c0a 2020 2020 2020  eam=None,.      
+0001b060: 2020 7665 7262 6f73 653d 4661 6c73 652c    verbose=False,
+0001b070: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0001b080: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+0001b090: 616d 2073 7472 2062 6173 655f 6e61 6d65  am str base_name
+0001b0a0: 3a20 6261 7365 206e 616d 6520 666f 7220  : base name for 
+0001b0b0: 7468 6520 6d6f 6475 6c65 2c20 652e 672e  the module, e.g.
+0001b0c0: 2022 7a65 726f 5f6f 7574 220a 2020 2020   "zero_out".    
+0001b0d0: 2020 2020 3a70 6172 616d 2069 6e74 7c74      :param int|t
+0001b0e0: 7570 6c65 5b69 6e74 5d20 636f 6465 5f76  uple[int] code_v
+0001b0f0: 6572 7369 6f6e 3a20 6368 6563 6b20 666f  ersion: check fo
+0001b100: 7220 7468 6520 6361 6368 6520 7768 6574  r the cache whet
+0001b110: 6865 7220 746f 2072 6575 7365 0a20 2020  her to reuse.   
+0001b120: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
+0001b130: 636f 6465 3a20 7468 6520 736f 7572 6365  code: the source
+0001b140: 2063 6f64 6520 6974 7365 6c66 0a20 2020   code itself.   
+0001b150: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
+0001b160: 2069 735f 6370 703a 2069 6620 4661 6c73   is_cpp: if Fals
+0001b170: 652c 2043 2069 7320 6173 7375 6d65 640a  e, C is assumed.
+0001b180: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+0001b190: 6963 745b 7374 722c 7374 727c 696e 747c  ict[str,str|int|
+0001b1a0: 4e6f 6e65 5d7c 4e6f 6e65 2063 5f6d 6163  None]|None c_mac
+0001b1b0: 726f 5f64 6566 696e 6573 3a20 652e 672e  ro_defines: e.g.
+0001b1c0: 207b 2254 454e 534f 5246 4c4f 5722 3a20   {"TENSORFLOW": 
+0001b1d0: 317d 0a20 2020 2020 2020 203a 7061 7261  1}.        :para
+0001b1e0: 6d20 6c69 7374 5b73 7472 5d7c 4e6f 6e65  m list[str]|None
+0001b1f0: 206c 645f 666c 6167 733a 2065 2e67 2e20   ld_flags: e.g. 
+0001b200: 5b22 2d6c 626c 6173 225d 0a20 2020 2020  ["-lblas"].     
+0001b210: 2020 203a 7061 7261 6d20 6c69 7374 5b73     :param list[s
+0001b220: 7472 5d7c 7475 706c 655b 7374 725d 2069  tr]|tuple[str] i
+0001b230: 6e63 6c75 6465 5f70 6174 6873 3a0a 2020  nclude_paths:.  
+0001b240: 2020 2020 2020 3a70 6172 616d 206c 6973        :param lis
+0001b250: 745b 7374 725d 7c4e 6f6e 6520 696e 636c  t[str]|None incl
+0001b260: 7564 655f 6465 7073 3a20 6966 2070 726f  ude_deps: if pro
+0001b270: 7669 6465 6420 616e 6420 616e 2065 7869  vided and an exi
+0001b280: 7374 696e 6720 6c69 6220 6669 6c65 2c0a  sting lib file,.
+0001b290: 2020 2020 2020 2020 2020 2020 7765 2077              we w
+0001b2a0: 696c 6c20 6368 6563 6b20 6966 2061 6e79  ill check if any
+0001b2b0: 2064 6570 656e 6465 6e63 7920 6973 206e   dependency is n
+0001b2c0: 6577 6572 0a20 2020 2020 2020 2020 2020  ewer.           
+0001b2d0: 2061 6e64 2077 6520 6e65 6564 2074 6f20   and we need to 
+0001b2e0: 7265 636f 6d70 696c 652e 2077 6520 636f  recompile. we co
+0001b2f0: 756c 6420 616c 736f 2064 6f20 6974 2061  uld also do it a
+0001b300: 7574 6f6d 6174 6963 616c 6c79 2076 6961  utomatically via
+0001b310: 202d 4d44 2062 7574 2074 6861 7420 7365   -MD but that se
+0001b320: 656d 7320 6f76 6572 6b69 6c6c 2061 6e64  ems overkill and
+0001b330: 2074 6f6f 2073 6c6f 772e 0a20 2020 2020   too slow..     
+0001b340: 2020 203a 7061 7261 6d20 7374 727c 4e6f     :param str|No
+0001b350: 6e65 2073 7461 7469 635f 7665 7273 696f  ne static_versio
+0001b360: 6e5f 6e61 6d65 3a20 6e6f 726d 616c 6c79  n_name: normally
+0001b370: 2c20 7765 2075 7365 202e 2e2e 2f62 6173  , we use .../bas
+0001b380: 655f 6e61 6d65 2f68 6173 6820 6173 2074  e_name/hash as t
+0001b390: 6865 2064 6972 0a20 2020 2020 2020 2020  he dir.         
+0001b3a0: 2020 2062 7574 2074 6869 7320 776f 756c     but this woul
+0001b3b0: 6420 7573 6520 2e2e 2e2f 6261 7365 5f6e  d use .../base_n
+0001b3c0: 616d 652f 7374 6174 6963 5f76 6572 7369  ame/static_versi
+0001b3d0: 6f6e 5f6e 616d 652e 0a20 2020 2020 2020  on_name..       
+0001b3e0: 203a 7061 7261 6d20 626f 6f6c 2073 686f   :param bool sho
+0001b3f0: 756c 645f 636c 6561 6e75 705f 6f6c 645f  uld_cleanup_old_
+0001b400: 616c 6c3a 2077 6865 7468 6572 2077 6520  all: whether we 
+0001b410: 7368 6f75 6c64 206c 6f6f 6b20 696e 2074  should look in t
+0001b420: 6865 2063 6163 6865 2064 6972 0a20 2020  he cache dir.   
+0001b430: 2020 2020 2020 2020 2061 6e64 2063 6865           and che
+0001b440: 636b 2061 6c6c 206f 7073 2069 6620 7765  ck all ops if we
+0001b450: 2063 616e 2064 656c 6574 6520 736f 6d65   can delete some
+0001b460: 206f 6c64 206f 6e65 7320 7768 6963 6820   old ones which 
+0001b470: 6172 6520 6f6c 6465 7220 7468 616e 2073  are older than s
+0001b480: 6f6d 6520 6c69 6d69 740a 2020 2020 2020  ome limit.      
+0001b490: 2020 2020 2020 2873 656c 662e 5f63 6c65        (self._cle
+0001b4a0: 616e 7570 5f74 696d 655f 6c69 6d69 745f  anup_time_limit_
+0001b4b0: 6461 7973 290a 2020 2020 2020 2020 3a70  days).        :p
+0001b4c0: 6172 616d 2062 6f6f 6c20 7368 6f75 6c64  aram bool should
+0001b4d0: 5f63 6c65 616e 7570 5f6f 6c64 5f6d 7964  _cleanup_old_myd
+0001b4e0: 6972 3a20 7768 6574 6865 7220 7765 2073  ir: whether we s
+0001b4f0: 686f 756c 6420 6465 6c65 7465 206f 7572  hould delete our
+0001b500: 206f 7020 6469 7220 6265 666f 7265 2077   op dir before w
+0001b510: 6520 636f 6d70 696c 6520 7468 6572 652e  e compile there.
+0001b520: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0001b530: 7479 7069 6e67 2e54 6578 7449 4f7c 4e6f  typing.TextIO|No
+0001b540: 6e65 206c 6f67 5f73 7472 6561 6d3a 2066  ne log_stream: f
+0001b550: 696c 6520 7374 7265 616d 2066 6f72 2070  ile stream for p
+0001b560: 7269 6e74 2073 7461 7465 6d65 6e74 730a  rint statements.
+0001b570: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+0001b580: 6f6f 6c20 7665 7262 6f73 653a 2062 6520  ool verbose: be 
+0001b590: 736c 6967 6874 6c79 206d 6f72 6520 7665  slightly more ve
+0001b5a0: 7262 6f73 650a 2020 2020 2020 2020 2222  rbose.        ""
+0001b5b0: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+0001b5c0: 662e 436f 6c6c 6563 7465 6443 6f6d 7069  f.CollectedCompi
+0001b5d0: 6c65 7273 2069 7320 6e6f 7420 4e6f 6e65  lers is not None
+0001b5e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001b5f0: 6c66 2e43 6f6c 6c65 6374 6564 436f 6d70  lf.CollectedComp
+0001b600: 696c 6572 732e 6170 7065 6e64 2873 656c  ilers.append(sel
+0001b610: 6629 0a20 2020 2020 2020 2073 656c 662e  f).        self.
+0001b620: 7665 7262 6f73 6520 3d20 7665 7262 6f73  verbose = verbos
+0001b630: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
+0001b640: 6163 6865 5f64 6972 203d 2022 2573 2f25  ache_dir = "%s/%
+0001b650: 7322 2025 2028 6765 745f 6361 6368 655f  s" % (get_cache_
+0001b660: 6469 7228 292c 2073 656c 662e 4361 6368  dir(), self.Cach
+0001b670: 6544 6972 4e61 6d65 290a 2020 2020 2020  eDirName).      
+0001b680: 2020 7365 6c66 2e5f 696e 636c 7564 655f    self._include_
+0001b690: 7061 7468 7320 3d20 6c69 7374 2869 6e63  paths = list(inc
+0001b6a0: 6c75 6465 5f70 6174 6873 290a 2020 2020  lude_paths).    
+0001b6b0: 2020 2020 7365 6c66 2e62 6173 655f 6e61      self.base_na
+0001b6c0: 6d65 203d 2062 6173 655f 6e61 6d65 0a20  me = base_name. 
+0001b6d0: 2020 2020 2020 2073 656c 662e 636f 6465         self.code
+0001b6e0: 5f76 6572 7369 6f6e 203d 2063 6f64 655f  _version = code_
+0001b6f0: 7665 7273 696f 6e0a 2020 2020 2020 2020  version.        
+0001b700: 7365 6c66 2e63 6f64 6520 3d20 636f 6465  self.code = code
+0001b710: 0a20 2020 2020 2020 2073 656c 662e 6973  .        self.is
+0001b720: 5f63 7070 203d 2069 735f 6370 700a 2020  _cpp = is_cpp.  
+0001b730: 2020 2020 2020 7365 6c66 2e63 5f6d 6163        self.c_mac
+0001b740: 726f 5f64 6566 696e 6573 203d 207b 6b3a  ro_defines = {k:
+0001b750: 2076 2066 6f72 206b 2c20 7620 696e 2028   v for k, v in (
+0001b760: 635f 6d61 6372 6f5f 6465 6669 6e65 7320  c_macro_defines 
+0001b770: 6f72 207b 7d29 2e69 7465 6d73 2829 2069  or {}).items() i
+0001b780: 6620 7620 6973 206e 6f74 204e 6f6e 657d  f v is not None}
+0001b790: 0a20 2020 2020 2020 2073 656c 662e 6c64  .        self.ld
+0001b7a0: 5f66 6c61 6773 203d 206c 645f 666c 6167  _flags = ld_flag
+0001b7b0: 7320 6f72 205b 5d0a 2020 2020 2020 2020  s or [].        
+0001b7c0: 7365 6c66 2e69 6e63 6c75 6465 5f64 6570  self.include_dep
+0001b7d0: 7320 3d20 696e 636c 7564 655f 6465 7073  s = include_deps
+0001b7e0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0001b7f0: 6174 6963 5f76 6572 7369 6f6e 5f6e 616d  atic_version_nam
+0001b800: 6520 3d20 7374 6174 6963 5f76 6572 7369  e = static_versi
+0001b810: 6f6e 5f6e 616d 650a 2020 2020 2020 2020  on_name.        
+0001b820: 7365 6c66 2e5f 636f 6465 5f68 6173 6820  self._code_hash 
+0001b830: 3d20 7365 6c66 2e5f 6d61 6b65 5f63 6f64  = self._make_cod
+0001b840: 655f 6861 7368 2829 0a20 2020 2020 2020  e_hash().       
+0001b850: 2073 656c 662e 5f69 6e66 6f5f 6469 6374   self._info_dict
+0001b860: 203d 2073 656c 662e 5f6d 616b 655f 696e   = self._make_in
+0001b870: 666f 5f64 6963 7428 290a 2020 2020 2020  fo_dict().      
+0001b880: 2020 7365 6c66 2e5f 6861 7368 203d 2073    self._hash = s
+0001b890: 656c 662e 5f6d 616b 655f 6861 7368 2829  elf._make_hash()
+0001b8a0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+0001b8b0: 7479 7065 735f 6c69 6220 3d20 4e6f 6e65  types_lib = None
+0001b8c0: 0a20 2020 2020 2020 2069 6620 7368 6f75  .        if shou
+0001b8d0: 6c64 5f63 6c65 616e 7570 5f6f 6c64 5f61  ld_cleanup_old_a
+0001b8e0: 6c6c 3a0a 2020 2020 2020 2020 2020 2020  ll:.            
+0001b8f0: 7365 6c66 2e5f 636c 6561 6e75 705f 6f6c  self._cleanup_ol
+0001b900: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
+0001b910: 2e5f 7368 6f75 6c64 5f63 6c65 616e 7570  ._should_cleanup
+0001b920: 5f6f 6c64 5f6d 7964 6972 203d 2073 686f  _old_mydir = sho
+0001b930: 756c 645f 636c 6561 6e75 705f 6f6c 645f  uld_cleanup_old_
+0001b940: 6d79 6469 720a 2020 2020 2020 2020 7365  mydir.        se
+0001b950: 6c66 2e75 7365 5f63 7878 3131 5f61 6269  lf.use_cxx11_abi
+0001b960: 203d 2075 7365 5f63 7878 3131 5f61 6269   = use_cxx11_abi
+0001b970: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
+0001b980: 6f67 5f73 7472 6561 6d20 3d20 6c6f 675f  og_stream = log_
+0001b990: 7374 7265 616d 0a20 2020 2020 2020 2069  stream.        i
+0001b9a0: 6620 7365 6c66 2e76 6572 626f 7365 3a0a  f self.verbose:.
+0001b9b0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0001b9c0: 7428 2225 733a 2025 7222 2025 2028 7365  t("%s: %r" % (se
+0001b9d0: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
+0001b9e0: 616d 655f 5f2c 2073 656c 6629 2c20 6669  ame__, self), fi
+0001b9f0: 6c65 3d6c 6f67 5f73 7472 6561 6d29 0a0a  le=log_stream)..
+0001ba00: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+0001ba10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001ba20: 7265 7475 726e 2022 3c25 7320 2572 2069  return "<%s %r i
+0001ba30: 6e20 2572 3e22 2025 2028 7365 6c66 2e5f  n %r>" % (self._
+0001ba40: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
+0001ba50: 5f2c 2073 656c 662e 6261 7365 5f6e 616d  _, self.base_nam
+0001ba60: 652c 2073 656c 662e 5f6d 6f64 5f70 6174  e, self._mod_pat
+0001ba70: 6829 0a0a 2020 2020 4070 726f 7065 7274  h)..    @propert
+0001ba80: 790a 2020 2020 6465 6620 5f6d 6f64 5f70  y.    def _mod_p
+0001ba90: 6174 6828 7365 6c66 293a 0a20 2020 2020  ath(self):.     
+0001baa0: 2020 2072 6574 7572 6e20 2225 732f 2573     return "%s/%s
+0001bab0: 2f25 7322 2025 2028 7365 6c66 2e63 6163  /%s" % (self.cac
+0001bac0: 6865 5f64 6972 2c20 7365 6c66 2e62 6173  he_dir, self.bas
+0001bad0: 655f 6e61 6d65 2c20 7365 6c66 2e73 7461  e_name, self.sta
+0001bae0: 7469 635f 7665 7273 696f 6e5f 6e61 6d65  tic_version_name
+0001baf0: 206f 7220 7365 6c66 2e5f 6861 7368 5b3a   or self._hash[:
+0001bb00: 3130 5d29 0a0a 2020 2020 4070 726f 7065  10])..    @prope
+0001bb10: 7274 790a 2020 2020 6465 6620 5f69 6e66  rty.    def _inf
+0001bb20: 6f5f 6669 6c65 6e61 6d65 2873 656c 6629  o_filename(self)
+0001bb30: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001bb40: 2022 2573 2f69 6e66 6f2e 7079 2220 2520   "%s/info.py" % 
+0001bb50: 2873 656c 662e 5f6d 6f64 5f70 6174 682c  (self._mod_path,
+0001bb60: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0001bb70: 0a20 2020 2064 6566 205f 736f 5f66 696c  .    def _so_fil
+0001bb80: 656e 616d 6528 7365 6c66 293a 0a20 2020  ename(self):.   
+0001bb90: 2020 2020 2072 6574 7572 6e20 2225 732f       return "%s/
+0001bba0: 2573 2e73 6f22 2025 2028 7365 6c66 2e5f  %s.so" % (self._
+0001bbb0: 6d6f 645f 7061 7468 2c20 7365 6c66 2e62  mod_path, self.b
+0001bbc0: 6173 655f 6e61 6d65 290a 0a20 2020 2040  ase_name)..    @
+0001bbd0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0001bbe0: 205f 635f 6669 6c65 6e61 6d65 2873 656c   _c_filename(sel
+0001bbf0: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+0001bc00: 656c 662e 6973 5f63 7070 3a0a 2020 2020  elf.is_cpp:.    
+0001bc10: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+0001bc20: 2573 2f25 732e 6363 2220 2520 2873 656c  %s/%s.cc" % (sel
+0001bc30: 662e 5f6d 6f64 5f70 6174 682c 2073 656c  f._mod_path, sel
+0001bc40: 662e 6261 7365 5f6e 616d 6529 0a20 2020  f.base_name).   
+0001bc50: 2020 2020 2072 6574 7572 6e20 2225 732f       return "%s/
+0001bc60: 2573 2e63 2220 2520 2873 656c 662e 5f6d  %s.c" % (self._m
+0001bc70: 6f64 5f70 6174 682c 2073 656c 662e 6261  od_path, self.ba
+0001bc80: 7365 5f6e 616d 6529 0a0a 2020 2020 5f63  se_name)..    _c
+0001bc90: 6c65 616e 7570 5f74 696d 655f 6c69 6d69  leanup_time_limi
+0001bca0: 745f 6461 7973 203d 2036 300a 0a20 2020  t_days = 60..   
+0001bcb0: 2064 6566 205f 636c 6561 6e75 705f 6f6c   def _cleanup_ol
+0001bcc0: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
+0001bcd0: 206d 6f64 5f70 6174 6820 3d20 7365 6c66   mod_path = self
+0001bce0: 2e5f 6d6f 645f 7061 7468 2020 2320 2e2e  ._mod_path  # ..
+0001bcf0: 2e2f 6261 7365 5f6e 616d 652f 6861 7368  ./base_name/hash
+0001bd00: 0a20 2020 2020 2020 2062 6173 655f 6d6f  .        base_mo
+0001bd10: 645f 7061 7468 203d 206f 732e 7061 7468  d_path = os.path
+0001bd20: 2e64 6972 6e61 6d65 286d 6f64 5f70 6174  .dirname(mod_pat
+0001bd30: 6829 2020 2320 2e2e 2e2f 6261 7365 5f6e  h)  # .../base_n
+0001bd40: 616d 650a 2020 2020 2020 2020 6d79 5f6d  ame.        my_m
+0001bd50: 6f64 5f70 6174 685f 6e61 6d65 203d 206f  od_path_name = o
+0001bd60: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+0001bd70: 6d6f 645f 7061 7468 290a 2020 2020 2020  mod_path).      
+0001bd80: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
+0001bd90: 2e65 7869 7374 7328 6261 7365 5f6d 6f64  .exists(base_mod
+0001bda0: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
+0001bdb0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0001bdc0: 2020 2069 6d70 6f72 7420 7469 6d65 0a0a     import time..
+0001bdd0: 2020 2020 2020 2020 636c 6561 6e75 705f          cleanup_
+0001bde0: 7469 6d65 5f6c 696d 6974 5f73 6563 7320  time_limit_secs 
+0001bdf0: 3d20 7365 6c66 2e5f 636c 6561 6e75 705f  = self._cleanup_
+0001be00: 7469 6d65 5f6c 696d 6974 5f64 6179 7320  time_limit_days 
+0001be10: 2a20 3234 202a 2036 3020 2a20 3630 0a20  * 24 * 60 * 60. 
+0001be20: 2020 2020 2020 2066 6f72 2070 2069 6e20         for p in 
+0001be30: 6f73 2e6c 6973 7464 6972 2862 6173 655f  os.listdir(base_
+0001be40: 6d6f 645f 7061 7468 293a 0a20 2020 2020  mod_path):.     
+0001be50: 2020 2020 2020 2069 6620 7020 3d3d 206d         if p == m
+0001be60: 795f 6d6f 645f 7061 7468 5f6e 616d 653a  y_mod_path_name:
+0001be70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001be80: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+0001be90: 2020 2020 2020 6675 6c6c 5f64 6972 5f70        full_dir_p
+0001bea0: 6174 6820 3d20 2225 732f 2573 2220 2520  ath = "%s/%s" % 
+0001beb0: 2862 6173 655f 6d6f 645f 7061 7468 2c20  (base_mod_path, 
+0001bec0: 7029 0a20 2020 2020 2020 2020 2020 2069  p).            i
+0001bed0: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
+0001bee0: 6469 7228 6675 6c6c 5f64 6972 5f70 6174  dir(full_dir_pat
+0001bef0: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
+0001bf00: 2020 2020 636f 6e74 696e 7565 2020 2320      continue  # 
+0001bf10: 6967 6e6f 7265 2066 6f72 206e 6f77 0a20  ignore for now. 
+0001bf20: 2020 2020 2020 2020 2020 206c 6f63 6b20             lock 
+0001bf30: 3d20 4c6f 636b 4669 6c65 2866 756c 6c5f  = LockFile(full_
+0001bf40: 6469 725f 7061 7468 290a 2020 2020 2020  dir_path).      
+0001bf50: 2020 2020 2020 6966 206c 6f63 6b2e 6973        if lock.is
+0001bf60: 5f6c 6f63 6b65 6428 293a 0a20 2020 2020  _locked():.     
+0001bf70: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0001bf80: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+0001bf90: 6c6f 636b 2e6d 6179 6265 5f72 656d 6f76  lock.maybe_remov
+0001bfa0: 655f 6f6c 645f 6c6f 636b 6669 6c65 2829  e_old_lockfile()
+0001bfb0: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
+0001bfc0: 6f5f 7061 7468 203d 2022 2573 2f69 6e66  o_path = "%s/inf
+0001bfd0: 6f2e 7079 2220 2520 6675 6c6c 5f64 6972  o.py" % full_dir
+0001bfe0: 5f70 6174 680a 2020 2020 2020 2020 2020  _path.          
+0001bff0: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
+0001c000: 2e65 7869 7374 7328 696e 666f 5f70 6174  .exists(info_pat
+0001c010: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
+0001c020: 2020 2020 7365 6c66 2e5f 636c 6561 6e75      self._cleanu
+0001c030: 705f 6f6c 645f 7061 7468 2866 756c 6c5f  p_old_path(full_
+0001c040: 6469 725f 7061 7468 2c20 7265 6173 6f6e  dir_path, reason
+0001c050: 3d22 636f 7272 7570 7420 6469 722c 206d  ="corrupt dir, m
+0001c060: 6973 7369 6e67 2069 6e66 6f2e 7079 2229  issing info.py")
+0001c070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c080: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+0001c090: 2020 2020 2020 736f 5f70 6174 6820 3d20        so_path = 
+0001c0a0: 2225 732f 2573 2e73 6f22 2025 2028 6675  "%s/%s.so" % (fu
+0001c0b0: 6c6c 5f64 6972 5f70 6174 682c 2073 656c  ll_dir_path, sel
+0001c0c0: 662e 6261 7365 5f6e 616d 6529 0a20 2020  f.base_name).   
+0001c0d0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0001c0e0: 6f73 2e70 6174 682e 6578 6973 7473 2873  os.path.exists(s
+0001c0f0: 6f5f 7061 7468 293a 0a20 2020 2020 2020  o_path):.       
+0001c100: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+0001c110: 6c65 616e 7570 5f6f 6c64 5f70 6174 6828  leanup_old_path(
+0001c120: 6675 6c6c 5f64 6972 5f70 6174 682c 2072  full_dir_path, r
+0001c130: 6561 736f 6e3d 2263 6f72 7275 7074 2064  eason="corrupt d
+0001c140: 6972 2c20 6d69 7373 696e 6720 736f 2229  ir, missing so")
+0001c150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c160: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+0001c170: 2020 2020 2020 6474 203d 2074 696d 652e        dt = time.
+0001c180: 7469 6d65 2829 202d 206f 732e 7061 7468  time() - os.path
+0001c190: 2e67 6574 6d74 696d 6528 736f 5f70 6174  .getmtime(so_pat
+0001c1a0: 6829 0a20 2020 2020 2020 2020 2020 2069  h).            i
+0001c1b0: 6620 6474 203e 2063 6c65 616e 7570 5f74  f dt > cleanup_t
+0001c1c0: 696d 655f 6c69 6d69 745f 7365 6373 3a0a  ime_limit_secs:.
+0001c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1e0: 7365 6c66 2e5f 636c 6561 6e75 705f 6f6c  self._cleanup_ol
+0001c1f0: 645f 7061 7468 2866 756c 6c5f 6469 725f  d_path(full_dir_
+0001c200: 7061 7468 2c20 7265 6173 6f6e 3d22 2573  path, reason="%s
+0001c210: 206f 6c64 2220 2520 686d 7328 6474 2929   old" % hms(dt))
+0001c220: 0a0a 2020 2020 6465 6620 5f63 6c65 616e  ..    def _clean
+0001c230: 7570 5f6f 6c64 5f70 6174 6828 7365 6c66  up_old_path(self
+0001c240: 2c20 702c 2072 6561 736f 6e29 3a0a 2020  , p, reason):.  
+0001c250: 2020 2020 2020 7072 696e 7428 2225 7320        print("%s 
+0001c260: 6465 6c65 7465 206f 6c64 2c20 2573 3a20  delete old, %s: 
+0001c270: 2573 2220 2520 2873 656c 662e 5f5f 636c  %s" % (self.__cl
+0001c280: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20  ass__.__name__, 
+0001c290: 7265 6173 6f6e 2c20 7029 290a 2020 2020  reason, p)).    
+0001c2a0: 2020 2020 6173 7365 7274 206f 732e 7061      assert os.pa
+0001c2b0: 7468 2e65 7869 7374 7328 7029 0a20 2020  th.exists(p).   
+0001c2c0: 2020 2020 2069 6d70 6f72 7420 7368 7574       import shut
+0001c2d0: 696c 0a0a 2020 2020 2020 2020 7472 793a  il..        try:
+0001c2e0: 0a20 2020 2020 2020 2020 2020 2073 6875  .            shu
+0001c2f0: 7469 6c2e 726d 7472 6565 2870 290a 2020  til.rmtree(p).  
+0001c300: 2020 2020 2020 6578 6365 7074 204f 5345        except OSE
+0001c310: 7272 6f72 2061 7320 6578 633a 0a20 2020  rror as exc:.   
+0001c320: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+0001c330: 2573 2064 656c 6574 6520 6578 6365 7074  %s delete except
+0001c340: 696f 6e20 2825 7329 2e20 5769 6c6c 2069  ion (%s). Will i
+0001c350: 676e 6f72 6520 616e 6420 7472 7920 746f  gnore and try to
+0001c360: 2063 6f6e 7469 6e75 6520 616e 7977 6179   continue anyway
+0001c370: 2e22 2025 2028 7365 6c66 2e5f 5f63 6c61  ." % (self.__cla
+0001c380: 7373 5f5f 2e5f 5f6e 616d 655f 5f2c 2065  ss__.__name__, e
+0001c390: 7863 2929 0a0a 2020 2020 6465 6620 5f6c  xc))..    def _l
+0001c3a0: 6f61 645f 696e 666f 2873 656c 6629 3a0a  oad_info(self):.
+0001c3b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001c3c0: 2020 2020 3a72 7479 7065 3a20 6469 6374      :rtype: dict
+0001c3d0: 5b73 7472 5d7c 4e6f 6e65 0a20 2020 2020  [str]|None.     
+0001c3e0: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
+0001c3f0: 696c 656e 616d 6520 3d20 7365 6c66 2e5f  ilename = self._
+0001c400: 696e 666f 5f66 696c 656e 616d 650a 2020  info_filename.  
+0001c410: 2020 2020 2020 6966 206e 6f74 206f 732e        if not os.
+0001c420: 7061 7468 2e65 7869 7374 7328 6669 6c65  path.exists(file
+0001c430: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
+0001c440: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+0001c450: 2020 2020 2020 2073 203d 206f 7065 6e28         s = open(
+0001c460: 6669 6c65 6e61 6d65 292e 7265 6164 2829  filename).read()
+0001c470: 0a20 2020 2020 2020 2072 6573 203d 2065  .        res = e
+0001c480: 7661 6c28 7329 0a20 2020 2020 2020 2061  val(s).        a
+0001c490: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+0001c4a0: 2872 6573 2c20 6469 6374 290a 2020 2020  (res, dict).    
+0001c4b0: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
+0001c4c0: 2020 2020 5f72 656c 6576 616e 745f 696e      _relevant_in
+0001c4d0: 666f 5f6b 6579 7320 3d20 2822 636f 6465  fo_keys = ("code
+0001c4e0: 5f76 6572 7369 6f6e 222c 2022 636f 6465  _version", "code
+0001c4f0: 5f68 6173 6822 2c20 2263 5f6d 6163 726f  _hash", "c_macro
+0001c500: 5f64 6566 696e 6573 222c 2022 6c64 5f66  _defines", "ld_f
+0001c510: 6c61 6773 222c 2022 636f 6d70 696c 6572  lags", "compiler
+0001c520: 5f62 696e 2229 0a0a 2020 2020 6465 6620  _bin")..    def 
+0001c530: 5f6d 616b 655f 696e 666f 5f64 6963 7428  _make_info_dict(
+0001c540: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0001c550: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
+0001c560: 653a 2064 6963 745b 7374 725d 0a20 2020  e: dict[str].   
+0001c570: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001c580: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
+0001c590: 2020 2020 2020 2262 6173 655f 6e61 6d65        "base_name
+0001c5a0: 223a 2073 656c 662e 6261 7365 5f6e 616d  ": self.base_nam
+0001c5b0: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+0001c5c0: 696e 636c 7564 655f 7061 7468 7322 3a20  include_paths": 
+0001c5d0: 7365 6c66 2e5f 696e 636c 7564 655f 7061  self._include_pa
+0001c5e0: 7468 732c 0a20 2020 2020 2020 2020 2020  ths,.           
+0001c5f0: 2022 636f 6465 5f76 6572 7369 6f6e 223a   "code_version":
+0001c600: 2073 656c 662e 636f 6465 5f76 6572 7369   self.code_versi
+0001c610: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+0001c620: 2263 6f64 655f 6861 7368 223a 2073 656c  "code_hash": sel
+0001c630: 662e 5f63 6f64 655f 6861 7368 2c0a 2020  f._code_hash,.  
+0001c640: 2020 2020 2020 2020 2020 2263 5f6d 6163            "c_mac
+0001c650: 726f 5f64 6566 696e 6573 223a 2073 656c  ro_defines": sel
+0001c660: 662e 635f 6d61 6372 6f5f 6465 6669 6e65  f.c_macro_define
+0001c670: 732c 0a20 2020 2020 2020 2020 2020 2022  s,.            "
+0001c680: 6c64 5f66 6c61 6773 223a 2073 656c 662e  ld_flags": self.
+0001c690: 6c64 5f66 6c61 6773 2c0a 2020 2020 2020  ld_flags,.      
+0001c6a0: 2020 2020 2020 2263 6f6d 7069 6c65 725f        "compiler_
+0001c6b0: 6269 6e22 3a20 7365 6c66 2e5f 6765 745f  bin": self._get_
+0001c6c0: 636f 6d70 696c 6572 5f62 696e 2829 2c0a  compiler_bin(),.
+0001c6d0: 2020 2020 2020 2020 7d0a 0a20 2020 2064          }..    d
+0001c6e0: 6566 205f 6d61 6b65 5f63 6f64 655f 6861  ef _make_code_ha
+0001c6f0: 7368 2873 656c 6629 3a0a 2020 2020 2020  sh(self):.      
+0001c700: 2020 696d 706f 7274 2068 6173 686c 6962    import hashlib
+0001c710: 0a0a 2020 2020 2020 2020 6820 3d20 6861  ..        h = ha
+0001c720: 7368 6c69 622e 6d64 3528 290a 2020 2020  shlib.md5().    
+0001c730: 2020 2020 682e 7570 6461 7465 2873 656c      h.update(sel
+0001c740: 662e 636f 6465 2e65 6e63 6f64 6528 2275  f.code.encode("u
+0001c750: 7466 3822 2929 0a20 2020 2020 2020 2072  tf8")).        r
+0001c760: 6574 7572 6e20 682e 6865 7864 6967 6573  eturn h.hexdiges
+0001c770: 7428 290a 0a20 2020 2064 6566 205f 6d61  t()..    def _ma
+0001c780: 6b65 5f68 6173 6828 7365 6c66 293a 0a20  ke_hash(self):. 
+0001c790: 2020 2020 2020 2069 6d70 6f72 7420 6861         import ha
+0001c7a0: 7368 6c69 620a 0a20 2020 2020 2020 2068  shlib..        h
+0001c7b0: 203d 2068 6173 686c 6962 2e6d 6435 2829   = hashlib.md5()
+0001c7c0: 0a20 2020 2020 2020 2068 2e75 7064 6174  .        h.updat
+0001c7d0: 6528 227b 222e 656e 636f 6465 2822 7574  e("{".encode("ut
+0001c7e0: 6638 2229 290a 2020 2020 2020 2020 666f  f8")).        fo
+0001c7f0: 7220 6b65 7920 696e 2073 656c 662e 5f72  r key in self._r
+0001c800: 656c 6576 616e 745f 696e 666f 5f6b 6579  elevant_info_key
+0001c810: 733a 0a20 2020 2020 2020 2020 2020 2068  s:.            h
+0001c820: 2e75 7064 6174 6528 2822 2573 3a7b 2573  .update(("%s:{%s
+0001c830: 7d22 2025 2028 6b65 792c 2073 656c 662e  }" % (key, self.
+0001c840: 5f69 6e66 6f5f 6469 6374 5b6b 6579 5d29  _info_dict[key])
+0001c850: 292e 656e 636f 6465 2822 7574 6638 2229  ).encode("utf8")
+0001c860: 290a 2020 2020 2020 2020 682e 7570 6461  ).        h.upda
+0001c870: 7465 2822 7d22 2e65 6e63 6f64 6528 2275  te("}".encode("u
+0001c880: 7466 3822 2929 0a20 2020 2020 2020 2072  tf8")).        r
+0001c890: 6574 7572 6e20 682e 6865 7864 6967 6573  eturn h.hexdiges
+0001c8a0: 7428 290a 0a20 2020 2064 6566 205f 7361  t()..    def _sa
+0001c8b0: 7665 5f69 6e66 6f28 7365 6c66 293a 0a20  ve_info(self):. 
+0001c8c0: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
+0001c8d0: 3d20 7365 6c66 2e5f 696e 666f 5f66 696c  = self._info_fil
+0001c8e0: 656e 616d 650a 2020 2020 2020 2020 7769  ename.        wi
+0001c8f0: 7468 206f 7065 6e28 6669 6c65 6e61 6d65  th open(filename
+0001c900: 2c20 2277 2229 2061 7320 663a 0a20 2020  , "w") as f:.   
+0001c910: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+0001c920: 2822 2573 5c6e 2220 2520 6265 7474 6572  ("%s\n" % better
+0001c930: 5f72 6570 7228 7365 6c66 2e5f 696e 666f  _repr(self._info
+0001c940: 5f64 6963 7429 290a 0a20 2020 2064 6566  _dict))..    def
+0001c950: 205f 6e65 6564 5f72 6563 6f6d 7069 6c65   _need_recompile
+0001c960: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001c970: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
+0001c980: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
+0001c990: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+0001c9a0: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
+0001c9b0: 7473 2873 656c 662e 5f73 6f5f 6669 6c65  ts(self._so_file
+0001c9c0: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
+0001c9d0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+0001c9e0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+0001c9f0: 6e63 6c75 6465 5f64 6570 733a 0a20 2020  nclude_deps:.   
+0001ca00: 2020 2020 2020 2020 2073 6f5f 6d74 696d           so_mtim
+0001ca10: 6520 3d20 6f73 2e70 6174 682e 6765 746d  e = os.path.getm
+0001ca20: 7469 6d65 2873 656c 662e 5f73 6f5f 6669  time(self._so_fi
+0001ca30: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
+0001ca40: 2020 2020 666f 7220 666e 2069 6e20 7365      for fn in se
+0001ca50: 6c66 2e69 6e63 6c75 6465 5f64 6570 733a  lf.include_deps:
+0001ca60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ca70: 2069 6620 6f73 2e70 6174 682e 6765 746d   if os.path.getm
+0001ca80: 7469 6d65 2866 6e29 203e 2073 6f5f 6d74  time(fn) > so_mt
+0001ca90: 696d 653a 0a20 2020 2020 2020 2020 2020  ime:.           
+0001caa0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001cab0: 5472 7565 0a20 2020 2020 2020 206f 6c64  True.        old
+0001cac0: 5f69 6e66 6f20 3d20 7365 6c66 2e5f 6c6f  _info = self._lo
+0001cad0: 6164 5f69 6e66 6f28 290a 2020 2020 2020  ad_info().      
+0001cae0: 2020 6e65 775f 696e 666f 203d 2073 656c    new_info = sel
+0001caf0: 662e 5f6d 616b 655f 696e 666f 5f64 6963  f._make_info_dic
+0001cb00: 7428 290a 2020 2020 2020 2020 6966 206e  t().        if n
+0001cb10: 6f74 206f 6c64 5f69 6e66 6f3a 0a20 2020  ot old_info:.   
+0001cb20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001cb30: 5472 7565 0a20 2020 2020 2020 2023 2054  True.        # T
+0001cb40: 6865 2068 6173 6820 616c 7265 6164 7920  he hash already 
+0001cb50: 6d61 7463 6865 6420 6275 7420 7665 7279  matched but very
+0001cb60: 2075 6e6c 696b 656c 792c 2074 6869 7320   unlikely, this 
+0001cb70: 636f 756c 6420 6265 2061 2063 6f6c 6c69  could be a colli
+0001cb80: 7369 6f6e 2e0a 2020 2020 2020 2020 2320  sion..        # 
+0001cb90: 416e 7977 6179 2c20 6a75 7374 2064 6f20  Anyway, just do 
+0001cba0: 7468 6973 2076 6572 7920 6368 6561 7020  this very cheap 
+0001cbb0: 6368 6563 6b2e 0a20 2020 2020 2020 2066  check..        f
+0001cbc0: 6f72 206b 6579 2069 6e20 7365 6c66 2e5f  or key in self._
+0001cbd0: 7265 6c65 7661 6e74 5f69 6e66 6f5f 6b65  relevant_info_ke
+0001cbe0: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+0001cbf0: 6966 206b 6579 206e 6f74 2069 6e20 6f6c  if key not in ol
+0001cc00: 645f 696e 666f 3a0a 2020 2020 2020 2020  d_info:.        
+0001cc10: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0001cc20: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0001cc30: 6966 206f 6c64 5f69 6e66 6f5b 6b65 795d  if old_info[key]
+0001cc40: 2021 3d20 6e65 775f 696e 666f 5b6b 6579   != new_info[key
+0001cc50: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0001cc60: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+0001cc70: 2020 2020 2020 2023 2049 6620 6e6f 2063         # If no c
+0001cc80: 6f64 6520 7665 7273 696f 6e20 6973 2070  ode version is p
+0001cc90: 726f 7669 6465 642c 2077 6520 636f 756c  rovided, we coul
+0001cca0: 6420 616c 736f 2063 6865 636b 2074 6865  d also check the
+0001ccb0: 2063 6f64 6520 6974 7365 6c66 206e 6f77   code itself now
+0001ccc0: 2e0a 2020 2020 2020 2020 2320 4275 7420  ..        # But 
+0001ccd0: 4920 7468 696e 6b20 7468 6973 2069 7320  I think this is 
+0001cce0: 6f76 6572 6b69 6c6c 2e0a 2020 2020 2020  overkill..      
+0001ccf0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+0001cd00: 2020 2020 6465 6620 5f6d 6179 6265 5f63      def _maybe_c
+0001cd10: 6f6d 7069 6c65 2873 656c 6629 3a0a 2020  ompile(self):.  
+0001cd20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001cd30: 2020 4f6e 2073 7563 6365 7373 6675 6c20    On successful 
+0001cd40: 7265 7475 726e 2c20 7365 6c66 2e5f 736f  return, self._so
+0001cd50: 5f66 696c 656e 616d 6520 7368 6f75 6c64  _filename should
+0001cd60: 2065 7869 7374 2061 6e64 2062 6520 7570   exist and be up
+0001cd70: 2d74 6f2d 6461 7465 2e0a 2020 2020 2020  -to-date..      
+0001cd80: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0001cd90: 206e 6f74 2073 656c 662e 5f6e 6565 645f   not self._need_
+0001cda0: 7265 636f 6d70 696c 6528 293a 0a20 2020  recompile():.   
+0001cdb0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0001cdc0: 2e76 6572 626f 7365 3a0a 2020 2020 2020  .verbose:.      
+0001cdd0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0001cde0: 2225 733a 204e 6f20 6e65 6564 2074 6f20  "%s: No need to 
+0001cdf0: 7265 636f 6d70 696c 653a 2025 7322 2025  recompile: %s" %
+0001ce00: 2028 7365 6c66 2e5f 5f63 6c61 7373 5f5f   (self.__class__
+0001ce10: 2e5f 5f6e 616d 655f 5f2c 2073 656c 662e  .__name__, self.
+0001ce20: 5f73 6f5f 6669 6c65 6e61 6d65 2929 0a20  _so_filename)). 
+0001ce30: 2020 2020 2020 2020 2020 2023 2054 6f75             # Tou
+0001ce40: 6368 2069 7420 736f 2074 6861 7420 7765  ch it so that we
+0001ce50: 2063 616e 2073 6565 2074 6861 7420 7765   can see that we
+0001ce60: 2075 7365 6420 6974 2072 6563 656e 746c   used it recentl
+0001ce70: 792e 0a20 2020 2020 2020 2020 2020 206f  y..            o
+0001ce80: 732e 7574 696d 6528 7365 6c66 2e5f 696e  s.utime(self._in
+0001ce90: 666f 5f66 696c 656e 616d 652c 204e 6f6e  fo_filename, Non
+0001cea0: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+0001ceb0: 6574 7572 6e0a 2020 2020 2020 2020 6c6f  eturn.        lo
+0001cec0: 636b 203d 204c 6f63 6b46 696c 6528 7365  ck = LockFile(se
+0001ced0: 6c66 2e5f 6d6f 645f 7061 7468 290a 2020  lf._mod_path).  
+0001cee0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+0001cef0: 662e 5f6e 6565 645f 7265 636f 6d70 696c  f._need_recompil
+0001cf00: 6528 293a 2020 2320 6368 6563 6b20 6167  e():  # check ag
+0001cf10: 6169 6e0a 2020 2020 2020 2020 2020 2020  ain.            
+0001cf20: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
+0001cf30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cf40: 2070 7269 6e74 2822 2573 3a20 4e6f 206e   print("%s: No n
+0001cf50: 6565 6420 746f 2072 6563 6f6d 7069 6c65  eed to recompile
+0001cf60: 2061 6674 6572 2077 6520 7761 6974 6564   after we waited
+0001cf70: 3a20 2573 2220 2520 2873 656c 662e 5f5f  : %s" % (self.__
+0001cf80: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+0001cf90: 2c20 7365 6c66 2e5f 736f 5f66 696c 656e  , self._so_filen
+0001cfa0: 616d 6529 290a 2020 2020 2020 2020 2020  ame)).          
+0001cfb0: 2020 6f73 2e75 7469 6d65 2873 656c 662e    os.utime(self.
+0001cfc0: 5f69 6e66 6f5f 6669 6c65 6e61 6d65 2c20  _info_filename, 
+0001cfd0: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
+0001cfe0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0001cff0: 2069 6620 7365 6c66 2e5f 7368 6f75 6c64   if self._should
+0001d000: 5f63 6c65 616e 7570 5f6f 6c64 5f6d 7964  _cleanup_old_myd
+0001d010: 6972 2061 6e64 206e 6f74 206c 6f63 6b2e  ir and not lock.
+0001d020: 6973 5f6c 6f63 6b65 6428 293a 0a20 2020  is_locked():.   
+0001d030: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
+0001d040: 6174 682e 6578 6973 7473 2873 656c 662e  ath.exists(self.
+0001d050: 5f6d 6f64 5f70 6174 6829 3a0a 2020 2020  _mod_path):.    
+0001d060: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001d070: 2e5f 636c 6561 6e75 705f 6f6c 645f 7061  ._cleanup_old_pa
+0001d080: 7468 2873 656c 662e 5f6d 6f64 5f70 6174  th(self._mod_pat
+0001d090: 682c 2072 6561 736f 6e3d 226e 6565 6420  h, reason="need 
+0001d0a0: 7265 636f 6d70 696c 6522 290a 2020 2020  recompile").    
+0001d0b0: 2020 2020 7769 7468 206c 6f63 6b3a 0a20      with lock:. 
+0001d0c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001d0d0: 5f6d 6179 6265 5f63 6f6d 7069 6c65 5f69  _maybe_compile_i
+0001d0e0: 6e6e 6572 2829 0a0a 2020 2020 6465 6620  nner()..    def 
+0001d0f0: 5f67 6574 5f63 6f6d 7069 6c65 725f 6269  _get_compiler_bi
+0001d100: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+0001d110: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+0001d120: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+0001d130: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+0001d140: 7365 6c66 2e69 735f 6370 703a 0a20 2020  self.is_cpp:.   
+0001d150: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001d160: 2267 2b2b 220a 2020 2020 2020 2020 7265  "g++".        re
+0001d170: 7475 726e 2022 6763 6322 0a0a 2020 2020  turn "gcc"..    
+0001d180: 6465 6620 5f74 7261 6e73 666f 726d 5f63  def _transform_c
+0001d190: 6f6d 7069 6c65 725f 6f70 7473 2873 656c  ompiler_opts(sel
+0001d1a0: 662c 206f 7074 7329 3a0a 2020 2020 2020  f, opts):.      
+0001d1b0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+0001d1c0: 6172 616d 206c 6973 745b 7374 725d 206f  aram list[str] o
+0001d1d0: 7074 733a 0a20 2020 2020 2020 203a 7274  pts:.        :rt
+0001d1e0: 7970 653a 206c 6973 745b 7374 725d 0a20  ype: list[str]. 
+0001d1f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001d200: 2020 2072 6574 7572 6e20 6f70 7473 0a0a     return opts..
+0001d210: 2020 2020 6465 6620 5f65 7874 7261 5f63      def _extra_c
+0001d220: 6f6d 6d6f 6e5f 6f70 7473 2873 656c 6629  ommon_opts(self)
+0001d230: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0001d240: 2020 2020 2020 3a72 7479 7065 3a20 6c69        :rtype: li
+0001d250: 7374 5b73 7472 5d0a 2020 2020 2020 2020  st[str].        
+0001d260: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+0001d270: 656c 662e 6973 5f63 7070 3a0a 2020 2020  elf.is_cpp:.    
+0001d280: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+0001d290: 222d 7374 643d 632b 2b31 3122 5d0a 2020  "-std=c++11"].  
+0001d2a0: 2020 2020 2020 7265 7475 726e 205b 5d0a        return [].
+0001d2b0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+0001d2c0: 640a 2020 2020 6465 6620 5f74 7261 6e73  d.    def _trans
+0001d2d0: 666f 726d 5f6c 645f 666c 6167 2863 6c73  form_ld_flag(cls
+0001d2e0: 2c20 6f70 7429 3a0a 2020 2020 2020 2020  , opt):.        
+0001d2f0: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+0001d300: 616d 2073 7472 206f 7074 3a0a 2020 2020  am str opt:.    
+0001d310: 2020 2020 3a72 7479 7065 3a20 7374 720a      :rtype: str.
+0001d320: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001d330: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
+0001d340: 6f72 6d20 3d3d 2022 6461 7277 696e 223a  orm == "darwin":
+0001d350: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
+0001d360: 7420 7365 656d 7320 736f 6d65 2076 6572  t seems some ver
+0001d370: 7369 6f6e 7320 6f66 204d 6163 4f53 206c  sions of MacOS l
+0001d380: 6420 6361 6e6e 6f74 2068 616e 646c 6520  d cannot handle 
+0001d390: 7468 6520 602d 6c3a 6669 6c65 6e61 6d65  the `-l:filename
+0001d3a0: 6020 6172 6775 6d65 6e74 2063 6f72 7265  ` argument corre
+0001d3b0: 6374 6c79 2e0a 2020 2020 2020 2020 2020  ctly..          
+0001d3c0: 2020 2320 452e 672e 2054 656e 736f 7246    # E.g. TensorF
+0001d3d0: 6c6f 7720 312e 3134 2069 6e63 6f72 7265  low 1.14 incorre
+0001d3e0: 6374 6c79 2075 7365 7320 7468 6973 2e0a  ctly uses this..
+0001d3f0: 2020 2020 2020 2020 2020 2020 2320 6874              # ht
+0001d400: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0001d410: 2f74 656e 736f 7266 6c6f 772f 7465 6e73  /tensorflow/tens
+0001d420: 6f72 666c 6f77 2f69 7373 7565 732f 3330  orflow/issues/30
+0001d430: 3536 340a 2020 2020 2020 2020 2020 2020  564.            
+0001d440: 6966 206f 7074 2e73 7461 7274 7377 6974  if opt.startswit
+0001d450: 6828 222d 6c3a 6c69 6222 2920 616e 6420  h("-l:lib") and 
+0001d460: 6f70 742e 656e 6473 7769 7468 2822 2e64  opt.endswith(".d
+0001d470: 796c 6962 2229 3a0a 2020 2020 2020 2020  ylib"):.        
+0001d480: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+0001d490: 2d6c 2573 2220 2520 6f70 745b 6c65 6e28  -l%s" % opt[len(
+0001d4a0: 222d 6c3a 6c69 6222 2920 3a20 2d6c 656e  "-l:lib") : -len
+0001d4b0: 2822 2e64 796c 6962 2229 5d0a 2020 2020  (".dylib")].    
+0001d4c0: 2020 2020 7265 7475 726e 206f 7074 0a0a      return opt..
+0001d4d0: 2020 2020 6465 6620 5f6d 6179 6265 5f63      def _maybe_c
+0001d4e0: 6f6d 7069 6c65 5f69 6e6e 6572 2873 656c  ompile_inner(sel
+0001d4f0: 6629 3a0a 2020 2020 2020 2020 2320 4469  f):.        # Di
+0001d500: 7265 6374 6f72 7920 7368 6f75 6c64 2062  rectory should b
+0001d510: 6520 6372 6561 7465 6420 6279 2074 6865  e created by the
+0001d520: 206c 6f63 6b69 6e67 206d 6563 6861 6e69   locking mechani
+0001d530: 736d 2e0a 2020 2020 2020 2020 6173 7365  sm..        asse
+0001d540: 7274 206f 732e 7061 7468 2e65 7869 7374  rt os.path.exist
+0001d550: 7328 7365 6c66 2e5f 6d6f 645f 7061 7468  s(self._mod_path
+0001d560: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
+0001d570: 7065 6e28 7365 6c66 2e5f 635f 6669 6c65  pen(self._c_file
+0001d580: 6e61 6d65 2c20 2277 2229 2061 7320 663a  name, "w") as f:
+0001d590: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
+0001d5a0: 7269 7465 2873 656c 662e 636f 6465 290a  rite(self.code).
+0001d5b0: 2020 2020 2020 2020 636f 6d6d 6f6e 5f6f          common_o
+0001d5c0: 7074 7320 3d20 5b22 2d73 6861 7265 6422  pts = ["-shared"
+0001d5d0: 2c20 222d 4f32 225d 0a20 2020 2020 2020  , "-O2"].       
+0001d5e0: 2063 6f6d 6d6f 6e5f 6f70 7473 202b 3d20   common_opts += 
+0001d5f0: 7365 6c66 2e5f 6578 7472 615f 636f 6d6d  self._extra_comm
+0001d600: 6f6e 5f6f 7074 7328 290a 2020 2020 2020  on_opts().      
+0001d610: 2020 6966 2073 7973 2e70 6c61 7466 6f72    if sys.platfor
+0001d620: 6d20 3d3d 2022 6461 7277 696e 223a 0a20  m == "darwin":. 
+0001d630: 2020 2020 2020 2020 2020 2063 6f6d 6d6f             commo
+0001d640: 6e5f 6f70 7473 202b 3d20 5b22 2d75 6e64  n_opts += ["-und
+0001d650: 6566 696e 6564 222c 2022 6479 6e61 6d69  efined", "dynami
+0001d660: 635f 6c6f 6f6b 7570 225d 0a20 2020 2020  c_lookup"].     
+0001d670: 2020 2066 6f72 2069 6e63 6c75 6465 5f70     for include_p
+0001d680: 6174 6820 696e 2073 656c 662e 5f69 6e63  ath in self._inc
+0001d690: 6c75 6465 5f70 6174 6873 3a0a 2020 2020  lude_paths:.    
+0001d6a0: 2020 2020 2020 2020 636f 6d6d 6f6e 5f6f          common_o
+0001d6b0: 7074 7320 2b3d 205b 222d 4922 2c20 696e  pts += ["-I", in
+0001d6c0: 636c 7564 655f 7061 7468 5d0a 2020 2020  clude_path].    
+0001d6d0: 2020 2020 636f 6d70 696c 6572 5f6f 7074      compiler_opt
+0001d6e0: 7320 3d20 5b22 2d66 5049 4322 2c20 222d  s = ["-fPIC", "-
+0001d6f0: 7622 5d0a 2020 2020 2020 2020 636f 6d6d  v"].        comm
+0001d700: 6f6e 5f6f 7074 7320 2b3d 2073 656c 662e  on_opts += self.
+0001d710: 5f74 7261 6e73 666f 726d 5f63 6f6d 7069  _transform_compi
+0001d720: 6c65 725f 6f70 7473 2863 6f6d 7069 6c65  ler_opts(compile
+0001d730: 725f 6f70 7473 290a 2020 2020 2020 2020  r_opts).        
+0001d740: 636f 6d6d 6f6e 5f6f 7074 7320 2b3d 205b  common_opts += [
+0001d750: 222d 445f 474c 4942 4358 585f 5553 455f  "-D_GLIBCXX_USE_
+0001d760: 4358 5831 315f 4142 493d 2569 2220 2520  CXX11_ABI=%i" % 
+0001d770: 2831 2069 6620 7365 6c66 2e75 7365 5f63  (1 if self.use_c
+0001d780: 7878 3131 5f61 6269 2065 6c73 6520 3029  xx11_abi else 0)
+0001d790: 5d0a 2020 2020 2020 2020 636f 6d6d 6f6e  ].        common
+0001d7a0: 5f6f 7074 7320 2b3d 205b 222d 4425 733d  _opts += ["-D%s=
+0001d7b0: 2573 2220 2520 6974 656d 2066 6f72 2069  %s" % item for i
+0001d7c0: 7465 6d20 696e 2073 6f72 7465 6428 7365  tem in sorted(se
+0001d7d0: 6c66 2e63 5f6d 6163 726f 5f64 6566 696e  lf.c_macro_defin
+0001d7e0: 6573 2e69 7465 6d73 2829 295d 0a20 2020  es.items())].   
+0001d7f0: 2020 2020 2063 6f6d 6d6f 6e5f 6f70 7473       common_opts
+0001d800: 202b 3d20 5b22 2d67 225d 0a20 2020 2020   += ["-g"].     
+0001d810: 2020 206f 7074 7320 3d20 636f 6d6d 6f6e     opts = common
+0001d820: 5f6f 7074 7320 2b20 5b73 656c 662e 5f63  _opts + [self._c
+0001d830: 5f66 696c 656e 616d 652c 2022 2d6f 222c  _filename, "-o",
+0001d840: 2073 656c 662e 5f73 6f5f 6669 6c65 6e61   self._so_filena
+0001d850: 6d65 5d0a 2020 2020 2020 2020 6f70 7473  me].        opts
+0001d860: 202b 3d20 6c69 7374 286d 6170 2873 656c   += list(map(sel
+0001d870: 662e 5f74 7261 6e73 666f 726d 5f6c 645f  f._transform_ld_
+0001d880: 666c 6167 2c20 7365 6c66 2e6c 645f 666c  flag, self.ld_fl
+0001d890: 6167 7329 290a 2020 2020 2020 2020 636d  ags)).        cm
+0001d8a0: 645f 6269 6e20 3d20 7365 6c66 2e5f 6765  d_bin = self._ge
+0001d8b0: 745f 636f 6d70 696c 6572 5f62 696e 2829  t_compiler_bin()
+0001d8c0: 0a20 2020 2020 2020 2063 6d64 5f61 7267  .        cmd_arg
+0001d8d0: 7320 3d20 5b63 6d64 5f62 696e 5d20 2b20  s = [cmd_bin] + 
+0001d8e0: 6f70 7473 0a20 2020 2020 2020 2066 726f  opts.        fro
+0001d8f0: 6d20 7375 6270 726f 6365 7373 2069 6d70  m subprocess imp
+0001d900: 6f72 7420 506f 7065 6e2c 2050 4950 452c  ort Popen, PIPE,
+0001d910: 2053 5444 4f55 542c 2043 616c 6c65 6450   STDOUT, CalledP
+0001d920: 726f 6365 7373 4572 726f 720a 0a20 2020  rocessError..   
+0001d930: 2020 2020 2070 7269 6e74 2822 2573 2063       print("%s c
+0001d940: 616c 6c3a 2025 7322 2025 2028 7365 6c66  all: %s" % (self
+0001d950: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+0001d960: 655f 5f2c 2022 2022 2e6a 6f69 6e28 636d  e__, " ".join(cm
+0001d970: 645f 6172 6773 2929 2c20 6669 6c65 3d73  d_args)), file=s
+0001d980: 656c 662e 5f6c 6f67 5f73 7472 6561 6d29  elf._log_stream)
+0001d990: 0a20 2020 2020 2020 2070 726f 6320 3d20  .        proc = 
+0001d9a0: 506f 7065 6e28 636d 645f 6172 6773 2c20  Popen(cmd_args, 
+0001d9b0: 6377 643d 7365 6c66 2e5f 6d6f 645f 7061  cwd=self._mod_pa
+0001d9c0: 7468 2c20 7374 646f 7574 3d50 4950 452c  th, stdout=PIPE,
+0001d9d0: 2073 7464 6572 723d 5354 444f 5554 290a   stderr=STDOUT).
+0001d9e0: 2020 2020 2020 2020 7374 646f 7574 2c20          stdout, 
+0001d9f0: 7374 6465 7272 203d 2070 726f 632e 636f  stderr = proc.co
+0001da00: 6d6d 756e 6963 6174 6528 290a 2020 2020  mmunicate().    
+0001da10: 2020 2020 6173 7365 7274 2073 7464 6572      assert stder
+0001da20: 7220 6973 204e 6f6e 6520 2023 2073 686f  r is None  # sho
+0001da30: 756c 6420 6f6e 6c79 2068 6176 6520 7374  uld only have st
+0001da40: 646f 7574 0a20 2020 2020 2020 2069 6620  dout.        if 
+0001da50: 7072 6f63 2e72 6574 7572 6e63 6f64 6520  proc.returncode 
+0001da60: 213d 2030 3a0a 2020 2020 2020 2020 2020  != 0:.          
+0001da70: 2020 7072 696e 7428 2225 733a 2025 7320    print("%s: %s 
+0001da80: 6661 696c 6564 2e22 2025 2028 7365 6c66  failed." % (self
+0001da90: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+0001daa0: 655f 5f2c 2063 6d64 5f62 696e 2929 0a20  e__, cmd_bin)). 
+0001dab0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0001dac0: 2822 4f72 6967 696e 616c 2073 7464 6f75  ("Original stdou
+0001dad0: 742f 7374 6465 7272 3a22 290a 2020 2020  t/stderr:").    
+0001dae0: 2020 2020 2020 2020 7072 696e 7428 7374          print(st
+0001daf0: 646f 7574 2e64 6563 6f64 6528 2275 7466  dout.decode("utf
+0001db00: 3822 2929 0a20 2020 2020 2020 2020 2020  8")).           
+0001db10: 2070 7269 6e74 2829 0a20 2020 2020 2020   print().       
+0001db20: 2020 2020 2069 6620 636d 645f 6269 6e2e       if cmd_bin.
+0001db30: 656e 6473 7769 7468 2822 2f6e 7663 6322  endswith("/nvcc"
+0001db40: 2920 616e 6420 6222 6572 726f 723a 2063  ) and b"error: c
+0001db50: 6f6e 7374 6578 7072 2066 756e 6374 696f  onstexpr functio
+0001db60: 6e20 7265 7475 726e 2069 7320 6e6f 6e2d  n return is non-
+0001db70: 636f 6e73 7461 6e74 2220 696e 2073 7464  constant" in std
+0001db80: 6f75 743a 0a20 2020 2020 2020 2020 2020  out:.           
+0001db90: 2020 2020 2070 7269 6e74 2822 5468 6973       print("This
+0001dba0: 206d 6967 6874 2062 6520 7468 6520 6572   might be the er
+0001dbb0: 726f 723a 2068 7474 7073 3a2f 2f67 6974  ror: https://git
+0001dbc0: 6875 622e 636f 6d2f 7465 6e73 6f72 666c  hub.com/tensorfl
+0001dbd0: 6f77 2f74 656e 736f 7266 6c6f 772f 6973  ow/tensorflow/is
+0001dbe0: 7375 6573 2f32 3237 3636 2229 0a20 2020  sues/22766").   
+0001dbf0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0001dc00: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
+0001dc10: 2069 6620 636d 645f 6269 6e2e 656e 6473   if cmd_bin.ends
+0001dc20: 7769 7468 2822 2f6e 7663 6322 2920 616e  with("/nvcc") an
+0001dc30: 6420 6222 6763 6320 7665 7273 696f 6e73  d b"gcc versions
+0001dc40: 206c 6174 6572 2074 6861 6e22 2069 6e20   later than" in 
+0001dc50: 7374 646f 7574 3a0a 2020 2020 2020 2020  stdout:.        
+0001dc60: 2020 2020 2020 2020 7072 696e 7428 2259          print("Y
+0001dc70: 6f75 7220 4743 4320 7665 7273 696f 6e20  our GCC version 
+0001dc80: 6d69 6768 7420 6265 2074 6f6f 206e 6577  might be too new
+0001dc90: 2e20 5468 6973 2069 7320 6120 7072 6f62  . This is a prob
+0001dca0: 6c65 6d20 7769 7468 2073 6f6d 6520 6e76  lem with some nv
+0001dcb0: 6363 2076 6572 7369 6f6e 732e 2229 0a20  cc versions."). 
+0001dcc0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001dcd0: 7269 6e74 2829 0a20 2020 2020 2020 2020  rint().         
+0001dce0: 2020 2072 6169 7365 2043 616c 6c65 6450     raise CalledP
+0001dcf0: 726f 6365 7373 4572 726f 7228 7265 7475  rocessError(retu
+0001dd00: 726e 636f 6465 3d70 726f 632e 7265 7475  rncode=proc.retu
+0001dd10: 726e 636f 6465 2c20 636d 643d 636d 645f  rncode, cmd=cmd_
+0001dd20: 6172 6773 290a 2020 2020 2020 2020 6173  args).        as
+0001dd30: 7365 7274 206f 732e 7061 7468 2e65 7869  sert os.path.exi
+0001dd40: 7374 7328 7365 6c66 2e5f 736f 5f66 696c  sts(self._so_fil
+0001dd50: 656e 616d 6529 0a20 2020 2020 2020 2077  ename).        w
+0001dd60: 6974 6820 6f70 656e 2822 2573 2f63 6f6d  ith open("%s/com
+0001dd70: 7069 6c65 2e6c 6f67 2220 2520 7365 6c66  pile.log" % self
+0001dd80: 2e5f 6d6f 645f 7061 7468 2c20 2277 6222  ._mod_path, "wb"
+0001dd90: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+0001dda0: 2020 2020 6966 2073 656c 662e 7665 7262      if self.verb
+0001ddb0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+0001ddc0: 2020 2020 2070 7269 6e74 2822 2573 3a20       print("%s: 
+0001ddd0: 7772 6974 6520 636f 6d70 696c 6520 6c6f  write compile lo
+0001dde0: 6720 746f 3a20 2573 2220 2520 2873 656c  g to: %s" % (sel
+0001ddf0: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
+0001de00: 6d65 5f5f 2c20 662e 6e61 6d65 2929 0a20  me__, f.name)). 
+0001de10: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+0001de20: 7465 2828 222b 2025 735c 6e22 2025 2022  te(("+ %s\n" % "
+0001de30: 2022 2e6a 6f69 6e28 636d 645f 6172 6773   ".join(cmd_args
+0001de40: 2929 2e65 6e63 6f64 6528 2275 7466 3822  )).encode("utf8"
+0001de50: 2929 0a20 2020 2020 2020 2020 2020 2066  )).            f
+0001de60: 2e77 7269 7465 2873 7464 6f75 7429 0a20  .write(stdout). 
+0001de70: 2020 2020 2020 2073 656c 662e 5f73 6176         self._sav
+0001de80: 655f 696e 666f 2829 0a20 2020 2020 2020  e_info().       
+0001de90: 2061 7373 6572 7420 6e6f 7420 7365 6c66   assert not self
+0001dea0: 2e5f 6e65 6564 5f72 6563 6f6d 7069 6c65  ._need_recompile
+0001deb0: 2829 0a0a 2020 2020 6465 6620 6c6f 6164  ()..    def load
+0001dec0: 5f6c 6962 5f63 7479 7065 7328 7365 6c66  _lib_ctypes(self
+0001ded0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0001dee0: 2020 2020 2020 203a 7274 7970 653a 2063         :rtype: c
+0001def0: 7479 7065 732e 4344 4c4c 0a20 2020 2020  types.CDLL.     
+0001df00: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0001df10: 6620 7365 6c66 2e5f 6374 7970 6573 5f6c  f self._ctypes_l
+0001df20: 6962 3a0a 2020 2020 2020 2020 2020 2020  ib:.            
+0001df30: 7265 7475 726e 2073 656c 662e 5f63 7479  return self._cty
+0001df40: 7065 735f 6c69 620a 2020 2020 2020 2020  pes_lib.        
+0001df50: 7365 6c66 2e5f 6d61 7962 655f 636f 6d70  self._maybe_comp
+0001df60: 696c 6528 290a 2020 2020 2020 2020 696d  ile().        im
+0001df70: 706f 7274 2063 7479 7065 730a 0a20 2020  port ctypes..   
+0001df80: 2020 2020 2073 656c 662e 5f63 7479 7065       self._ctype
+0001df90: 735f 6c69 6220 3d20 6374 7970 6573 2e63  s_lib = ctypes.c
+0001dfa0: 646c 6c2e 4c6f 6164 4c69 6272 6172 7928  dll.LoadLibrary(
+0001dfb0: 7365 6c66 2e5f 736f 5f66 696c 656e 616d  self._so_filenam
+0001dfc0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+0001dfd0: 6e20 7365 6c66 2e5f 6374 7970 6573 5f6c  n self._ctypes_l
+0001dfe0: 6962 0a0a 2020 2020 6465 6620 6765 745f  ib..    def get_
+0001dff0: 6c69 625f 6669 6c65 6e61 6d65 2873 656c  lib_filename(sel
+0001e000: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+0001e010: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+0001e020: 7374 720a 2020 2020 2020 2020 2222 220a  str.        """.
+0001e030: 2020 2020 2020 2020 7365 6c66 2e5f 6d61          self._ma
+0001e040: 7962 655f 636f 6d70 696c 6528 290a 2020  ybe_compile().  
+0001e050: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001e060: 662e 5f73 6f5f 6669 6c65 6e61 6d65 0a0a  f._so_filename..
+0001e070: 0a23 2053 6565 203a 6675 6e63 3a60 6d61  .# See :func:`ma
+0001e080: 7962 655f 7265 7374 6172 745f 7265 7475  ybe_restart_retu
+0001e090: 726e 6e5f 7769 7468 5f61 7466 6f72 6b5f  rnn_with_atfork_
+0001e0a0: 7061 7463 6860 2062 656c 6f77 2066 6f72  patch` below for
+0001e0b0: 2077 6879 2079 6f75 206d 6967 6874 2077   why you might w
+0001e0c0: 616e 7420 746f 2075 7365 2074 6869 732e  ant to use this.
+0001e0d0: 0a5f 635f 636f 6465 5f70 6174 6368 5f61  ._c_code_patch_a
+0001e0e0: 7466 6f72 6b20 3d20 2222 220a 2364 6566  tfork = """.#def
+0001e0f0: 696e 6520 5f47 4e55 5f53 4f55 5243 450a  ine _GNU_SOURCE.
+0001e100: 2369 6e63 6c75 6465 203c 7363 6865 642e  #include <sched.
+0001e110: 683e 0a23 696e 636c 7564 6520 3c73 6967  h>.#include <sig
+0001e120: 6e61 6c2e 683e 0a23 696e 636c 7564 6520  nal.h>.#include 
+0001e130: 3c73 7973 2f73 7973 6361 6c6c 2e68 3e0a  <sys/syscall.h>.
+0001e140: 2369 6e63 6c75 6465 203c 7374 6469 6f2e  #include <stdio.
+0001e150: 683e 0a23 696e 636c 7564 6520 3c73 7464  h>.#include <std
+0001e160: 6c69 622e 683e 0a23 696e 636c 7564 6520  lib.h>.#include 
+0001e170: 3c75 6e69 7374 642e 683e 0a0a 2f2f 2068  <unistd.h>..// h
+0001e180: 7474 7073 3a2f 2f73 7461 636b 6f76 6572  ttps://stackover
+0001e190: 666c 6f77 2e63 6f6d 2f71 7565 7374 696f  flow.com/questio
+0001e1a0: 6e73 2f34 3638 3435 3439 362f 6c64 2d70  ns/46845496/ld-p
+0001e1b0: 7265 6c6f 6164 2d61 6e64 2d6c 696e 6b61  reload-and-linka
+0001e1c0: 6765 0a2f 2f20 6874 7470 733a 2f2f 7374  ge.// https://st
+0001e1d0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
+0001e1e0: 7175 6573 7469 6f6e 732f 3436 3831 3035  questions/468105
+0001e1f0: 3937 2f66 6f72 6b65 7865 632d 7769 7468  97/forkexec-with
+0001e200: 6f75 742d 6174 666f 726b 2d68 616e 646c  out-atfork-handl
+0001e210: 6572 730a 0a69 6e74 2070 7468 7265 6164  ers..int pthread
+0001e220: 5f61 7466 6f72 6b28 766f 6964 2028 2a70  _atfork(void (*p
+0001e230: 7265 7061 7265 2928 766f 6964 292c 2076  repare)(void), v
+0001e240: 6f69 6420 282a 7061 7265 6e74 2928 766f  oid (*parent)(vo
+0001e250: 6964 292c 2076 6f69 6420 282a 6368 696c  id), void (*chil
+0001e260: 6429 2876 6f69 6429 2920 7b0a 2020 7072  d)(void)) {.  pr
+0001e270: 696e 7466 2822 4967 6e6f 7269 6e67 2070  intf("Ignoring p
+0001e280: 7468 7265 6164 5f61 7466 6f72 6b20 6361  thread_atfork ca
+0001e290: 6c6c 215c 5c6e 2229 3b0a 2020 6666 6c75  ll!\\n");.  fflu
+0001e2a0: 7368 2873 7464 6f75 7429 3b0a 2020 7265  sh(stdout);.  re
+0001e2b0: 7475 726e 2030 3b0a 7d0a 0a69 6e74 205f  turn 0;.}..int _
+0001e2c0: 5f72 6567 6973 7465 725f 6174 666f 726b  _register_atfork
+0001e2d0: 2876 6f69 6420 282a 7072 6570 6172 6529  (void (*prepare)
+0001e2e0: 2876 6f69 6429 2c20 766f 6964 2028 2a70  (void), void (*p
+0001e2f0: 6172 656e 7429 2876 6f69 6429 2c20 766f  arent)(void), vo
+0001e300: 6964 2028 2a63 6869 6c64 2928 766f 6964  id (*child)(void
+0001e310: 2929 207b 0a20 2070 7269 6e74 6628 2249  )) {.  printf("I
+0001e320: 676e 6f72 696e 6720 5f5f 7265 6769 7374  gnoring __regist
+0001e330: 6572 5f61 7466 6f72 6b20 6361 6c6c 215c  er_atfork call!\
+0001e340: 5c6e 2229 3b0a 2020 6666 6c75 7368 2873  \n");.  fflush(s
+0001e350: 7464 6f75 7429 3b0a 2020 7265 7475 726e  tdout);.  return
+0001e360: 2030 3b0a 7d0a 0a2f 2f20 416e 6f74 6865   0;.}..// Anothe
+0001e370: 7220 7761 7920 746f 2069 676e 6f72 6520  r way to ignore 
+0001e380: 6174 666f 726b 2068 616e 646c 6572 733a  atfork handlers:
+0001e390: 204f 7665 7272 6964 6520 666f 726b 2e0a   Override fork..
+0001e3a0: 2369 6664 6566 205f 5f6c 696e 7578 5f5f  #ifdef __linux__
+0001e3b0: 202f 2f20 6f6e 6c79 2077 6f72 6b73 206f   // only works o
+0001e3c0: 6e20 4c69 6e75 7820 6375 7272 656e 746c  n Linux currentl
+0001e3d0: 790a 7069 645f 7420 666f 726b 2876 6f69  y.pid_t fork(voi
+0001e3e0: 6429 207b 0a20 2072 6574 7572 6e20 7379  d) {.  return sy
+0001e3f0: 7363 616c 6c28 5359 535f 636c 6f6e 652c  scall(SYS_clone,
+0001e400: 2053 4947 4348 4c44 2c20 3029 3b0a 7d0a   SIGCHLD, 0);.}.
+0001e410: 2365 6e64 6966 0a0a 5f5f 6174 7472 6962  #endif..__attrib
+0001e420: 7574 655f 5f28 2863 6f6e 7374 7275 6374  ute__((construct
+0001e430: 6f72 2929 0a76 6f69 6420 7061 7463 685f  or)).void patch_
+0001e440: 6174 666f 726b 5f69 6e69 7428 2920 7b0a  atfork_init() {.
+0001e450: 2020 7365 7465 6e76 2822 5f5f 5245 5455    setenv("__RETU
+0001e460: 524e 4e5f 4154 464f 524b 5f50 4154 4348  RNN_ATFORK_PATCH
+0001e470: 4544 222c 2022 3122 2c20 3129 3b0a 7d0a  ED", "1", 1);.}.
+0001e480: 2222 220a 0a0a 6465 6620 6765 745f 7061  """...def get_pa
+0001e490: 7463 685f 6174 666f 726b 5f6c 6962 2829  tch_atfork_lib()
+0001e4a0: 3a0a 2020 2020 2222 220a 2020 2020 3a72  :.    """.    :r
+0001e4b0: 6574 7572 6e3a 2070 6174 6820 746f 206f  eturn: path to o
+0001e4c0: 7572 2070 6174 6368 5f61 7466 6f72 6b20  ur patch_atfork 
+0001e4d0: 6c69 622e 2073 6565 203a 6675 6e63 3a60  lib. see :func:`
+0001e4e0: 6d61 7962 655f 7265 7374 6172 745f 7265  maybe_restart_re
+0001e4f0: 7475 726e 6e5f 7769 7468 5f61 7466 6f72  turnn_with_atfor
+0001e500: 6b5f 7061 7463 6860 0a20 2020 203a 7274  k_patch`.    :rt
+0001e510: 7970 653a 2073 7472 0a20 2020 2022 2222  ype: str.    """
+0001e520: 0a20 2020 206e 6174 6976 6520 3d20 4e61  .    native = Na
+0001e530: 7469 7665 436f 6465 436f 6d70 696c 6572  tiveCodeCompiler
+0001e540: 2862 6173 655f 6e61 6d65 3d22 7061 7463  (base_name="patc
+0001e550: 685f 6174 666f 726b 222c 2063 6f64 655f  h_atfork", code_
+0001e560: 7665 7273 696f 6e3d 322c 2063 6f64 653d  version=2, code=
+0001e570: 5f63 5f63 6f64 655f 7061 7463 685f 6174  _c_code_patch_at
+0001e580: 666f 726b 2c20 6973 5f63 7070 3d46 616c  fork, is_cpp=Fal
+0001e590: 7365 290a 2020 2020 666e 203d 206e 6174  se).    fn = nat
+0001e5a0: 6976 652e 6765 745f 6c69 625f 6669 6c65  ive.get_lib_file
+0001e5b0: 6e61 6d65 2829 0a20 2020 2072 6574 7572  name().    retur
+0001e5c0: 6e20 666e 0a0a 0a64 6566 2072 6573 7461  n fn...def resta
+0001e5d0: 7274 5f72 6574 7572 6e6e 2829 3a0a 2020  rt_returnn():.  
+0001e5e0: 2020 2222 220a 2020 2020 5265 7374 6172    """.    Restar
+0001e5f0: 7473 2052 4554 5552 4e4e 2e0a 2020 2020  ts RETURNN..    
+0001e600: 2222 220a 2020 2020 6c6f 672e 666c 7573  """.    log.flus
+0001e610: 6828 290a 2020 2020 7379 732e 7374 646f  h().    sys.stdo
+0001e620: 7574 2e66 6c75 7368 2829 0a20 2020 2073  ut.flush().    s
+0001e630: 7973 2e73 7464 6572 722e 666c 7573 6828  ys.stderr.flush(
+0001e640: 290a 2020 2020 2320 6874 7470 733a 2f2f  ).    # https://
+0001e650: 7374 6163 6b6f 7665 7266 6c6f 772e 636f  stackoverflow.co
+0001e660: 6d2f 7175 6573 7469 6f6e 732f 3732 3333  m/questions/7233
+0001e670: 3539 3034 2f73 696d 706c 652d 7761 792d  5904/simple-way-
+0001e680: 746f 2d72 6573 7461 7274 2d61 7070 6c69  to-restart-appli
+0001e690: 6361 7469 6f6e 0a20 2020 2063 6c6f 7365  cation.    close
+0001e6a0: 5f61 6c6c 5f66 6473 5f65 7863 6570 7428  _all_fds_except(
+0001e6b0: 7b30 2c20 312c 2032 7d29 0a20 2020 206f  {0, 1, 2}).    o
+0001e6c0: 732e 6578 6563 7628 7379 732e 6578 6563  s.execv(sys.exec
+0001e6d0: 7574 6162 6c65 2c20 5b73 7973 2e65 7865  utable, [sys.exe
+0001e6e0: 6375 7461 626c 655d 202b 2073 7973 2e61  cutable] + sys.a
+0001e6f0: 7267 7629 0a20 2020 2072 6169 7365 2045  rgv).    raise E
+0001e700: 7863 6570 7469 6f6e 2822 7265 7374 6172  xception("restar
+0001e710: 745f 7265 7475 726e 6e3a 2065 7865 6376  t_returnn: execv
+0001e720: 2066 6169 6c65 6422 290a 0a0a 6465 6620   failed")...def 
+0001e730: 6d61 7962 655f 7265 7374 6172 745f 7265  maybe_restart_re
+0001e740: 7475 726e 6e5f 7769 7468 5f61 7466 6f72  turnn_with_atfor
+0001e750: 6b5f 7061 7463 6828 293a 0a20 2020 2022  k_patch():.    "
+0001e760: 2222 0a20 2020 2057 6861 7420 7765 2077  "".    What we w
+0001e770: 616e 743a 2073 7562 7072 6f63 6573 732e  ant: subprocess.
+0001e780: 506f 7065 6e20 746f 2061 6c77 6179 7320  Popen to always 
+0001e790: 776f 726b 2e0a 2020 2020 5072 6f62 6c65  work..    Proble
+0001e7a0: 6d3a 2049 7420 7573 6573 2066 6f72 6b2b  m: It uses fork+
+0001e7b0: 6578 6563 2069 6e74 6572 6e61 6c6c 7920  exec internally 
+0001e7c0: 696e 2073 7562 7072 6f63 6573 735f 666f  in subprocess_fo
+0001e7d0: 726b 5f65 7865 632c 2076 6961 205f 706f  rk_exec, via _po
+0001e7e0: 7369 7873 7562 7072 6f63 6573 732e 666f  sixsubprocess.fo
+0001e7f0: 726b 5f65 7865 632e 0a20 2020 2054 6861  rk_exec..    Tha
+0001e800: 7420 6973 2061 2070 726f 626c 656d 2062  t is a problem b
+0001e810: 6563 6175 7365 2066 6f72 6b20 6361 6e20  ecause fork can 
+0001e820: 7472 6967 6765 7220 616e 7920 6174 666f  trigger any atfo
+0001e830: 726b 2068 616e 646c 6572 7320 7265 6769  rk handlers regi
+0001e840: 7374 6572 6564 2076 6961 2070 7468 7265  stered via pthre
+0001e850: 6164 5f61 7466 6f72 6b2c 0a20 2020 2061  ad_atfork,.    a
+0001e860: 6e64 2074 686f 7365 2063 616e 2063 7261  nd those can cra
+0001e870: 7368 2f64 6561 646c 6f63 6b20 696e 2073  sh/deadlock in s
+0001e880: 6f6d 6520 6361 7365 732e 0a0a 2020 2020  ome cases...    
+0001e890: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0001e8a0: 6f6d 2f74 656e 736f 7266 6c6f 772f 7465  om/tensorflow/te
+0001e8b0: 6e73 6f72 666c 6f77 2f69 7373 7565 732f  nsorflow/issues/
+0001e8c0: 3133 3830 320a 2020 2020 6874 7470 733a  13802.    https:
+0001e8d0: 2f2f 6769 7468 7562 2e63 6f6d 2f78 6961  //github.com/xia
+0001e8e0: 6e79 692f 4f70 656e 424c 4153 2f69 7373  nyi/OpenBLAS/iss
+0001e8f0: 7565 732f 3234 300a 2020 2020 6874 7470  ues/240.    http
+0001e900: 733a 2f2f 7472 6163 2e73 6167 656d 6174  s://trac.sagemat
+0001e910: 682e 6f72 672f 7469 636b 6574 2f32 3230  h.org/ticket/220
+0001e920: 3231 0a20 2020 2068 7474 7073 3a2f 2f62  21.    https://b
+0001e930: 7567 732e 7079 7468 6f6e 2e6f 7267 2f69  ugs.python.org/i
+0001e940: 7373 7565 3331 3831 340a 2020 2020 6874  ssue31814.    ht
+0001e950: 7470 733a 2f2f 7374 6163 6b6f 7665 7266  tps://stackoverf
+0001e960: 6c6f 772e 636f 6d2f 7175 6573 7469 6f6e  low.com/question
+0001e970: 732f 3436 3834 3534 3936 2f6c 642d 7072  s/46845496/ld-pr
+0001e980: 656c 6f61 642d 616e 642d 6c69 6e6b 6167  eload-and-linkag
+0001e990: 650a 2020 2020 6874 7470 733a 2f2f 7374  e.    https://st
+0001e9a0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
+0001e9b0: 7175 6573 7469 6f6e 732f 3436 3831 3035  questions/468105
+0001e9c0: 3937 2f66 6f72 6b65 7865 632d 7769 7468  97/forkexec-with
+0001e9d0: 6f75 742d 6174 666f 726b 2d68 616e 646c  out-atfork-handl
+0001e9e0: 6572 730a 0a20 2020 2054 6865 2073 6f6c  ers..    The sol
+0001e9f0: 7574 696f 6e20 6865 7265 3a20 4a75 7374  ution here: Just
+0001ea00: 206f 7665 7272 6964 6520 7074 6872 6561   override pthrea
+0001ea10: 645f 6174 666f 726b 2c20 7669 6120 4c44  d_atfork, via LD
+0001ea20: 5f50 5245 4c4f 4144 2e0a 2020 2020 4e6f  _PRELOAD..    No
+0001ea30: 7465 2074 6861 7420 696e 2073 6f6d 6520  te that in some 
+0001ea40: 6361 7365 732c 2074 6869 7320 6973 206e  cases, this is n
+0001ea50: 6f74 2065 6e6f 7567 6820 2873 6565 2074  ot enough (see t
+0001ea60: 6865 2053 4f20 6469 7363 7573 7369 6f6e  he SO discussion
+0001ea70: 292c 0a20 2020 2073 6f20 7765 2061 6c73  ),.    so we als
+0001ea80: 6f20 6f76 6572 7772 6974 6520 666f 726b  o overwrite fork
+0001ea90: 2069 7473 656c 662e 0a20 2020 2053 6565   itself..    See
+0001eaa0: 2061 6c73 6f20 7465 7374 732f 7465 7374   also tests/test
+0001eab0: 5f66 6f72 6b5f 6578 6563 2e70 7920 666f  _fork_exec.py fo
+0001eac0: 7220 6120 6465 6d6f 2e0a 2020 2020 2222  r a demo..    ""
+0001ead0: 220a 2020 2020 6966 206f 732e 656e 7669  ".    if os.envi
+0001eae0: 726f 6e2e 6765 7428 225f 5f52 4554 5552  ron.get("__RETUR
+0001eaf0: 4e4e 5f41 5446 4f52 4b5f 5041 5443 4845  NN_ATFORK_PATCHE
+0001eb00: 4422 2920 3d3d 2022 3122 3a0a 2020 2020  D") == "1":.    
+0001eb10: 2020 2020 7072 696e 7428 2252 756e 6e69      print("Runni
+0001eb20: 6e67 2077 6974 6820 7061 7463 6865 6420  ng with patched 
+0001eb30: 6174 666f 726b 2e22 290a 2020 2020 2020  atfork.").      
+0001eb40: 2020 7265 7475 726e 0a20 2020 2069 6620    return.    if 
+0001eb50: 6f73 2e65 6e76 6972 6f6e 2e67 6574 2822  os.environ.get("
+0001eb60: 5f5f 5245 5455 524e 4e5f 5452 595f 4154  __RETURNN_TRY_AT
+0001eb70: 464f 524b 5f50 4154 4348 4544 2229 203d  FORK_PATCHED") =
+0001eb80: 3d20 2231 223a 0a20 2020 2020 2020 2070  = "1":.        p
+0001eb90: 7269 6e74 2822 5061 7463 6869 6e67 2061  rint("Patching a
+0001eba0: 7466 6f72 6b20 6469 6420 6e6f 7420 776f  tfork did not wo
+0001ebb0: 726b 2120 5769 6c6c 2063 6f6e 7469 6e75  rk! Will continu
+0001ebc0: 6520 616e 7977 6179 2e22 290a 2020 2020  e anyway.").    
+0001ebd0: 2020 2020 7265 7475 726e 0a20 2020 206c      return.    l
+0001ebe0: 6962 203d 2067 6574 5f70 6174 6368 5f61  ib = get_patch_a
+0001ebf0: 7466 6f72 6b5f 6c69 6228 290a 2020 2020  tfork_lib().    
+0001ec00: 656e 7620 3d20 6f73 2e65 6e76 6972 6f6e  env = os.environ
+0001ec10: 2e63 6f70 7928 290a 2020 2020 656e 765b  .copy().    env[
+0001ec20: 2244 594c 445f 494e 5345 5254 5f4c 4942  "DYLD_INSERT_LIB
+0001ec30: 5241 5249 4553 2220 6966 2073 7973 2e70  RARIES" if sys.p
+0001ec40: 6c61 7466 6f72 6d20 3d3d 2022 6461 7277  latform == "darw
+0001ec50: 696e 2220 656c 7365 2022 4c44 5f50 5245  in" else "LD_PRE
+0001ec60: 4c4f 4144 225d 203d 206c 6962 0a20 2020  LOAD"] = lib.   
+0001ec70: 2065 6e76 5b22 5f5f 5245 5455 524e 4e5f   env["__RETURNN_
+0001ec80: 5452 595f 4154 464f 524b 5f50 4154 4348  TRY_ATFORK_PATCH
+0001ec90: 4544 225d 203d 2022 3122 0a20 2020 2070  ED"] = "1".    p
+0001eca0: 7269 6e74 2822 5265 7374 6172 7469 6e67  rint("Restarting
+0001ecb0: 2052 6574 7572 6e6e 2077 6974 6820 6174   Returnn with at
+0001ecc0: 666f 726b 2070 6174 6368 2e2e 2e22 2c20  fork patch...", 
+0001ecd0: 7379 732e 6578 6563 7574 6162 6c65 2c20  sys.executable, 
+0001ece0: 7379 732e 6172 6776 290a 2020 2020 7379  sys.argv).    sy
+0001ecf0: 732e 7374 646f 7574 2e66 6c75 7368 2829  s.stdout.flush()
+0001ed00: 0a20 2020 206f 732e 6578 6563 7670 6528  .    os.execvpe(
+0001ed10: 7379 732e 6578 6563 7574 6162 6c65 2c20  sys.executable, 
+0001ed20: 5b73 7973 2e65 7865 6375 7461 626c 655d  [sys.executable]
+0001ed30: 202b 2073 7973 2e61 7267 762c 2065 6e76   + sys.argv, env
+0001ed40: 290a 2020 2020 7072 696e 7428 2265 7865  ).    print("exe
+0001ed50: 6376 7065 2064 6964 206e 6f74 2077 6f72  cvpe did not wor
+0001ed60: 6b3f 2229 0a0a 0a64 6566 2063 6c6f 7365  k?")...def close
+0001ed70: 5f61 6c6c 5f66 6473 5f65 7863 6570 7428  _all_fds_except(
+0001ed80: 6578 6365 7074 5f66 6473 293a 0a20 2020  except_fds):.   
+0001ed90: 2022 2222 0a20 2020 2043 616c 6c73 206f   """.    Calls o
+0001eda0: 732e 636c 6f73 6572 616e 6765 2065 7863  s.closerange exc
+0001edb0: 6570 7420 666f 7220 7468 6520 6769 7665  ept for the give
+0001edc0: 6e20 6664 732e 0a20 2020 2043 6f64 6520  n fds..    Code 
+0001edd0: 6164 6f70 7465 6420 616e 6420 6578 7465  adopted and exte
+0001ede0: 6e64 6564 2066 726f 6d20 6d75 6c74 6970  nded from multip
+0001edf0: 726f 6365 7373 696e 672e 7574 696c 2e63  rocessing.util.c
+0001ee00: 6c6f 7365 5f61 6c6c 5f66 6473 5f65 7863  lose_all_fds_exc
+0001ee10: 6570 742e 0a0a 2020 2020 3a70 6172 616d  ept...    :param
+0001ee20: 2074 7970 696e 672e 436f 6c6c 6563 7469   typing.Collecti
+0001ee30: 6f6e 5b69 6e74 5d20 6578 6365 7074 5f66  on[int] except_f
+0001ee40: 6473 3a20 7573 7561 6c6c 7920 6174 206c  ds: usually at l
+0001ee50: 6561 7374 207b 302c 312c 327d 0a20 2020  east {0,1,2}.   
+0001ee60: 2022 2222 0a20 2020 2023 206e 6f69 6e73   """.    # noins
+0001ee70: 7065 6374 696f 6e20 5079 4272 6f61 6445  pection PyBroadE
+0001ee80: 7863 6570 7469 6f6e 0a20 2020 2074 7279  xception.    try
+0001ee90: 3a0a 2020 2020 2020 2020 6d61 785f 6664  :.        max_fd
+0001eea0: 203d 206f 732e 7379 7363 6f6e 6628 2253   = os.sysconf("S
+0001eeb0: 435f 4f50 454e 5f4d 4158 2229 0a20 2020  C_OPEN_MAX").   
+0001eec0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0001eed0: 6e3a 0a20 2020 2020 2020 206d 6178 5f66  n:.        max_f
+0001eee0: 6420 3d20 3235 360a 0a20 2020 2065 7863  d = 256..    exc
+0001eef0: 6570 745f 6664 7320 3d20 736f 7274 6564  ept_fds = sorted
+0001ef00: 286c 6973 7428 6578 6365 7074 5f66 6473  (list(except_fds
+0001ef10: 2920 2b20 5b2d 312c 206d 6178 5f66 645d  ) + [-1, max_fd]
+0001ef20: 290a 2020 2020 6173 7365 7274 2065 7863  ).    assert exc
+0001ef30: 6570 745f 6664 735b 305d 203d 3d20 2d31  ept_fds[0] == -1
+0001ef40: 2061 6e64 2065 7863 6570 745f 6664 735b   and except_fds[
+0001ef50: 2d31 5d20 3d3d 206d 6178 5f66 642c 2022  -1] == max_fd, "
+0001ef60: 6664 2069 6e76 616c 6964 220a 0a20 2020  fd invalid"..   
+0001ef70: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0001ef80: 6c65 6e28 6578 6365 7074 5f66 6473 2920  len(except_fds) 
+0001ef90: 2d20 3129 3a0a 2020 2020 2020 2020 6966  - 1):.        if
+0001efa0: 2065 7863 6570 745f 6664 735b 695d 202b   except_fds[i] +
+0001efb0: 2031 203c 2065 7863 6570 745f 6664 735b   1 < except_fds[
+0001efc0: 6920 2b20 315d 3a0a 2020 2020 2020 2020  i + 1]:.        
+0001efd0: 2020 2020 6f73 2e63 6c6f 7365 7261 6e67      os.closerang
+0001efe0: 6528 6578 6365 7074 5f66 6473 5b69 5d20  e(except_fds[i] 
+0001eff0: 2b20 312c 2065 7863 6570 745f 6664 735b  + 1, except_fds[
+0001f000: 6920 2b20 315d 290a 0a0a 636c 6173 7320  i + 1])...class 
+0001f010: 5374 6174 733a 0a20 2020 2022 2222 0a20  Stats:.    """. 
+0001f020: 2020 2043 6f6c 6c65 6374 7320 6d65 616e     Collects mean
+0001f030: 2061 6e64 2076 6172 6961 6e63 652c 2072   and variance, r
+0001f040: 756e 6e69 6e67 2061 7665 7261 6765 2e0a  unning average..
+0001f050: 0a20 2020 2068 7474 7073 3a2f 2f65 6e2e  .    https://en.
+0001f060: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
+0001f070: 6b69 2f41 6c67 6f72 6974 686d 735f 666f  ki/Algorithms_fo
+0001f080: 725f 6361 6c63 756c 6174 696e 675f 7661  r_calculating_va
+0001f090: 7269 616e 6365 0a20 2020 2022 2222 0a0a  riance.    """..
+0001f0a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0001f0b0: 2873 656c 662c 2066 6f72 6d61 745f 7374  (self, format_st
+0001f0c0: 723d 4e6f 6e65 293a 0a20 2020 2020 2020  r=None):.       
+0001f0d0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+0001f0e0: 7261 6d20 4e6f 6e65 7c28 2866 6c6f 6174  ram None|((float
+0001f0f0: 7c6e 756d 7079 2e6e 6461 7272 6179 292d  |numpy.ndarray)-
+0001f100: 3e73 7472 2920 666f 726d 6174 5f73 7472  >str) format_str
+0001f110: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0001f120: 2020 2020 2020 7365 6c66 2e66 6f72 6d61        self.forma
+0001f130: 745f 7374 7220 3d20 666f 726d 6174 5f73  t_str = format_s
+0001f140: 7472 206f 7220 7374 720a 2020 2020 2020  tr or str.      
+0001f150: 2020 7365 6c66 2e6d 6561 6e20 3d20 302e    self.mean = 0.
+0001f160: 300a 2020 2020 2020 2020 7365 6c66 2e6d  0.        self.m
+0001f170: 6561 6e5f 7371 203d 2030 2e30 0a20 2020  ean_sq = 0.0.   
+0001f180: 2020 2020 2073 656c 662e 7661 7220 3d20       self.var = 
+0001f190: 302e 300a 2020 2020 2020 2020 7365 6c66  0.0.        self
+0001f1a0: 2e6d 696e 203d 204e 6f6e 650a 2020 2020  .min = None.    
+0001f1b0: 2020 2020 7365 6c66 2e6d 6178 203d 204e      self.max = N
+0001f1c0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0001f1d0: 2e74 6f74 616c 5f64 6174 615f 6c65 6e20  .total_data_len 
+0001f1e0: 3d20 300a 2020 2020 2020 2020 7365 6c66  = 0.        self
+0001f1f0: 2e6e 756d 5f73 6571 7320 3d20 300a 0a20  .num_seqs = 0.. 
+0001f200: 2020 2064 6566 205f 5f73 7472 5f5f 2873     def __str__(s
+0001f210: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+0001f220: 2073 656c 662e 6e75 6d5f 7365 7173 203e   self.num_seqs >
+0001f230: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0001f240: 6966 2073 656c 662e 6e75 6d5f 7365 7173  if self.num_seqs
+0001f250: 203d 3d20 7365 6c66 2e74 6f74 616c 5f64   == self.total_d
+0001f260: 6174 615f 6c65 6e3a 0a20 2020 2020 2020  ata_len:.       
+0001f270: 2020 2020 2020 2020 2065 7874 7261 5f73           extra_s
+0001f280: 7472 203d 2022 6176 675f 6461 7461 5f6c  tr = "avg_data_l
+0001f290: 656e 3d31 220a 2020 2020 2020 2020 2020  en=1".          
+0001f2a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001f2b0: 2020 2020 2020 2020 6578 7472 615f 7374          extra_st
+0001f2c0: 7220 3d20 2274 6f74 616c 5f64 6174 615f  r = "total_data_
+0001f2d0: 6c65 6e3d 2569 2c20 6176 675f 6461 7461  len=%i, avg_data
+0001f2e0: 5f6c 656e 3d25 6622 2025 2028 0a20 2020  _len=%f" % (.   
+0001f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f300: 2073 656c 662e 746f 7461 6c5f 6461 7461   self.total_data
+0001f310: 5f6c 656e 2c0a 2020 2020 2020 2020 2020  _len,.          
+0001f320: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+0001f330: 7365 6c66 2e74 6f74 616c 5f64 6174 615f  self.total_data_
+0001f340: 6c65 6e29 202f 2073 656c 662e 6e75 6d5f  len) / self.num_
+0001f350: 7365 7173 2c0a 2020 2020 2020 2020 2020  seqs,.          
+0001f360: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001f370: 2020 2020 7265 7475 726e 2022 5374 6174      return "Stat
+0001f380: 7328 6d65 616e 3d25 732c 2073 7464 5f64  s(mean=%s, std_d
+0001f390: 6576 3d25 732c 206d 696e 3d25 732c 206d  ev=%s, min=%s, m
+0001f3a0: 6178 3d25 732c 206e 756d 5f73 6571 733d  ax=%s, num_seqs=
+0001f3b0: 2569 2c20 2573 2922 2025 2028 0a20 2020  %i, %s)" % (.   
+0001f3c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001f3d0: 662e 666f 726d 6174 5f73 7472 2873 656c  f.format_str(sel
+0001f3e0: 662e 6765 745f 6d65 616e 2829 292c 0a20  f.get_mean()),. 
+0001f3f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001f400: 656c 662e 666f 726d 6174 5f73 7472 2873  elf.format_str(s
+0001f410: 656c 662e 6765 745f 7374 645f 6465 7628  elf.get_std_dev(
+0001f420: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+0001f430: 2020 2020 7365 6c66 2e66 6f72 6d61 745f      self.format_
+0001f440: 7374 7228 7365 6c66 2e6d 696e 292c 0a20  str(self.min),. 
+0001f450: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001f460: 656c 662e 666f 726d 6174 5f73 7472 2873  elf.format_str(s
+0001f470: 656c 662e 6d61 7829 2c0a 2020 2020 2020  elf.max),.      
+0001f480: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001f490: 756d 5f73 6571 732c 0a20 2020 2020 2020  um_seqs,.       
+0001f4a0: 2020 2020 2020 2020 2065 7874 7261 5f73           extra_s
+0001f4b0: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+0001f4c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001f4d0: 2022 5374 6174 7328 6e75 6d5f 7365 7173   "Stats(num_seqs
+0001f4e0: 3d30 2922 0a0a 2020 2020 6465 6620 636f  =0)"..    def co
+0001f4f0: 6c6c 6563 7428 7365 6c66 2c20 6461 7461  llect(self, data
+0001f500: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0001f510: 2020 2020 2020 203a 7061 7261 6d20 6e75         :param nu
+0001f520: 6d70 792e 6e64 6172 7261 797c 6c69 7374  mpy.ndarray|list
+0001f530: 5b69 6e74 5d7c 6c69 7374 5b66 6c6f 6174  [int]|list[float
+0001f540: 5d20 6461 7461 3a20 7368 6170 6520 2874  ] data: shape (t
+0001f550: 696d 652c 2064 696d 2920 6f72 2028 7469  ime, dim) or (ti
+0001f560: 6d65 2c29 0a20 2020 2020 2020 2022 2222  me,).        """
+0001f570: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+0001f580: 6e75 6d70 790a 0a20 2020 2020 2020 2069  numpy..        i
+0001f590: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+0001f5a0: 612c 2028 6c69 7374 2c20 7475 706c 6529  a, (list, tuple)
+0001f5b0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
+0001f5c0: 6174 6120 3d20 6e75 6d70 792e 6172 7261  ata = numpy.arra
+0001f5d0: 7928 6461 7461 290a 2020 2020 2020 2020  y(data).        
+0001f5e0: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+0001f5f0: 6528 6461 7461 2c20 6e75 6d70 792e 6e64  e(data, numpy.nd
+0001f600: 6172 7261 7929 0a20 2020 2020 2020 2061  array).        a
+0001f610: 7373 6572 7420 6461 7461 2e6e 6469 6d20  ssert data.ndim 
+0001f620: 3e3d 2031 0a20 2020 2020 2020 2069 6620  >= 1.        if 
+0001f630: 6461 7461 2e73 6861 7065 5b30 5d20 3d3d  data.shape[0] ==
+0001f640: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0001f650: 7265 7475 726e 0a20 2020 2020 2020 2073  return.        s
+0001f660: 656c 662e 6e75 6d5f 7365 7173 202b 3d20  elf.num_seqs += 
+0001f670: 310a 2020 2020 2020 2020 6461 7461 5f6d  1.        data_m
+0001f680: 696e 203d 206e 756d 7079 2e6d 696e 2864  in = numpy.min(d
+0001f690: 6174 612c 2061 7869 733d 3029 0a20 2020  ata, axis=0).   
+0001f6a0: 2020 2020 2064 6174 615f 6d61 7820 3d20       data_max = 
+0001f6b0: 6e75 6d70 792e 6d61 7828 6461 7461 2c20  numpy.max(data, 
+0001f6c0: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+0001f6d0: 6966 2073 656c 662e 6d69 6e20 6973 204e  if self.min is N
+0001f6e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0001f6f0: 2073 656c 662e 6d69 6e20 3d20 6461 7461   self.min = data
+0001f700: 5f6d 696e 0a20 2020 2020 2020 2020 2020  _min.           
+0001f710: 2073 656c 662e 6d61 7820 3d20 6461 7461   self.max = data
+0001f720: 5f6d 6178 0a20 2020 2020 2020 2065 6c73  _max.        els
+0001f730: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001f740: 656c 662e 6d69 6e20 3d20 6e75 6d70 792e  elf.min = numpy.
+0001f750: 6d69 6e69 6d75 6d28 7365 6c66 2e6d 696e  minimum(self.min
+0001f760: 2c20 6461 7461 5f6d 696e 290a 2020 2020  , data_min).    
+0001f770: 2020 2020 2020 2020 7365 6c66 2e6d 6178          self.max
+0001f780: 203d 206e 756d 7079 2e6d 6178 696d 756d   = numpy.maximum
+0001f790: 2873 656c 662e 6d61 782c 2064 6174 615f  (self.max, data_
+0001f7a0: 6d61 7829 0a20 2020 2020 2020 206e 6577  max).        new
+0001f7b0: 5f74 6f74 616c 5f64 6174 615f 6c65 6e20  _total_data_len 
+0001f7c0: 3d20 7365 6c66 2e74 6f74 616c 5f64 6174  = self.total_dat
+0001f7d0: 615f 6c65 6e20 2b20 6461 7461 2e73 6861  a_len + data.sha
+0001f7e0: 7065 5b30 5d0a 2020 2020 2020 2020 6d65  pe[0].        me
+0001f7f0: 616e 5f64 6966 6620 3d20 6e75 6d70 792e  an_diff = numpy.
+0001f800: 6d65 616e 2864 6174 612c 2061 7869 733d  mean(data, axis=
+0001f810: 3029 202d 2073 656c 662e 6d65 616e 0a20  0) - self.mean. 
+0001f820: 2020 2020 2020 206d 5f61 203d 2073 656c         m_a = sel
+0001f830: 662e 7661 7220 2a20 7365 6c66 2e74 6f74  f.var * self.tot
+0001f840: 616c 5f64 6174 615f 6c65 6e0a 2020 2020  al_data_len.    
+0001f850: 2020 2020 6d5f 6220 3d20 6e75 6d70 792e      m_b = numpy.
+0001f860: 7661 7228 6461 7461 2c20 6178 6973 3d30  var(data, axis=0
+0001f870: 2920 2a20 6461 7461 2e73 6861 7065 5b30  ) * data.shape[0
+0001f880: 5d0a 2020 2020 2020 2020 6d32 203d 206d  ].        m2 = m
+0001f890: 5f61 202b 206d 5f62 202b 206d 6561 6e5f  _a + m_b + mean_
+0001f8a0: 6469 6666 2a2a 3220 2a20 7365 6c66 2e74  diff**2 * self.t
+0001f8b0: 6f74 616c 5f64 6174 615f 6c65 6e20 2a20  otal_data_len * 
+0001f8c0: 6461 7461 2e73 6861 7065 5b30 5d20 2f20  data.shape[0] / 
+0001f8d0: 6e65 775f 746f 7461 6c5f 6461 7461 5f6c  new_total_data_l
+0001f8e0: 656e 0a20 2020 2020 2020 2073 656c 662e  en.        self.
+0001f8f0: 7661 7220 3d20 6d32 202f 206e 6577 5f74  var = m2 / new_t
+0001f900: 6f74 616c 5f64 6174 615f 6c65 6e0a 2020  otal_data_len.  
+0001f910: 2020 2020 2020 6461 7461 5f73 756d 203d        data_sum =
+0001f920: 206e 756d 7079 2e73 756d 2864 6174 612c   numpy.sum(data,
+0001f930: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+0001f940: 2064 656c 7461 203d 2064 6174 615f 7375   delta = data_su
+0001f950: 6d20 2d20 7365 6c66 2e6d 6561 6e20 2a20  m - self.mean * 
+0001f960: 6461 7461 2e73 6861 7065 5b30 5d0a 2020  data.shape[0].  
+0001f970: 2020 2020 2020 7365 6c66 2e6d 6561 6e20        self.mean 
+0001f980: 2b3d 2064 656c 7461 202f 206e 6577 5f74  += delta / new_t
+0001f990: 6f74 616c 5f64 6174 615f 6c65 6e0a 2020  otal_data_len.  
+0001f9a0: 2020 2020 2020 6465 6c74 615f 7371 203d        delta_sq =
+0001f9b0: 206e 756d 7079 2e73 756d 2864 6174 6120   numpy.sum(data 
+0001f9c0: 2a20 6461 7461 2c20 6178 6973 3d30 2920  * data, axis=0) 
+0001f9d0: 2d20 7365 6c66 2e6d 6561 6e5f 7371 202a  - self.mean_sq *
+0001f9e0: 2064 6174 612e 7368 6170 655b 305d 0a20   data.shape[0]. 
+0001f9f0: 2020 2020 2020 2073 656c 662e 6d65 616e         self.mean
+0001fa00: 5f73 7120 2b3d 2064 656c 7461 5f73 7120  _sq += delta_sq 
+0001fa10: 2f20 6e65 775f 746f 7461 6c5f 6461 7461  / new_total_data
+0001fa20: 5f6c 656e 0a20 2020 2020 2020 2073 656c  _len.        sel
+0001fa30: 662e 746f 7461 6c5f 6461 7461 5f6c 656e  f.total_data_len
+0001fa40: 203d 206e 6577 5f74 6f74 616c 5f64 6174   = new_total_dat
+0001fa50: 615f 6c65 6e0a 0a20 2020 2064 6566 2067  a_len..    def g
+0001fa60: 6574 5f6d 6561 6e28 7365 6c66 293a 0a20  et_mean(self):. 
+0001fa70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001fa80: 2020 203a 7265 7475 726e 3a20 6d65 616e     :return: mean
+0001fa90: 2c20 7368 6170 6520 2864 696d 2c29 0a20  , shape (dim,). 
+0001faa0: 2020 2020 2020 203a 7274 7970 653a 206e         :rtype: n
+0001fab0: 756d 7079 2e6e 6461 7272 6179 0a20 2020  umpy.ndarray.   
+0001fac0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001fad0: 2061 7373 6572 7420 7365 6c66 2e6e 756d   assert self.num
+0001fae0: 5f73 6571 7320 3e20 300a 2020 2020 2020  _seqs > 0.      
+0001faf0: 2020 7265 7475 726e 2073 656c 662e 6d65    return self.me
+0001fb00: 616e 0a0a 2020 2020 6465 6620 6765 745f  an..    def get_
+0001fb10: 7374 645f 6465 7628 7365 6c66 293a 0a20  std_dev(self):. 
+0001fb20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001fb30: 2020 203a 7265 7475 726e 3a20 7374 6420     :return: std 
+0001fb40: 6465 762c 2073 6861 7065 2028 6469 6d2c  dev, shape (dim,
+0001fb50: 290a 2020 2020 2020 2020 3a72 7479 7065  ).        :rtype
+0001fb60: 3a20 6e75 6d70 792e 6e64 6172 7261 790a  : numpy.ndarray.
+0001fb70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001fb80: 2020 2020 696d 706f 7274 206e 756d 7079      import numpy
+0001fb90: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+0001fba0: 2073 656c 662e 6e75 6d5f 7365 7173 203e   self.num_seqs >
+0001fbb0: 2030 0a20 2020 2020 2020 2072 6574 7572   0.        retur
+0001fbc0: 6e20 6e75 6d70 792e 7371 7274 2873 656c  n numpy.sqrt(sel
+0001fbd0: 662e 7661 7229 0a20 2020 2020 2020 2023  f.var).        #
+0001fbe0: 2072 6574 7572 6e20 6e75 6d70 792e 7371   return numpy.sq
+0001fbf0: 7274 2873 656c 662e 6d65 616e 5f73 7120  rt(self.mean_sq 
+0001fc00: 2d20 7365 6c66 2e6d 6561 6e20 2a20 7365  - self.mean * se
+0001fc10: 6c66 2e6d 6561 6e29 0a0a 2020 2020 6465  lf.mean)..    de
+0001fc20: 6620 6475 6d70 2873 656c 662c 206f 7574  f dump(self, out
+0001fc30: 7075 745f 6669 6c65 5f70 7265 6669 783d  put_file_prefix=
+0001fc40: 4e6f 6e65 2c20 7374 7265 616d 3d4e 6f6e  None, stream=Non
+0001fc50: 652c 2073 7472 6561 6d5f 7072 6566 6978  e, stream_prefix
+0001fc60: 3d22 2229 3a0a 2020 2020 2020 2020 2222  =""):.        ""
+0001fc70: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+0001fc80: 2073 7472 7c4e 6f6e 6520 6f75 7470 7574   str|None output
+0001fc90: 5f66 696c 655f 7072 6566 6978 3a20 6966  _file_prefix: if
+0001fca0: 2067 6976 656e 2c20 7769 6c6c 206e 756d   given, will num
+0001fcb0: 7079 2e73 6176 6574 7874 206d 6561 6e7c  py.savetxt mean|
+0001fcc0: 7374 645f 6465 7620 746f 2064 6973 6b0a  std_dev to disk.
+0001fcd0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+0001fce0: 7472 2073 7472 6561 6d5f 7072 6566 6978  tr stream_prefix
+0001fcf0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+0001fd00: 2069 6f2e 5465 7874 494f 4261 7365 2073   io.TextIOBase s
+0001fd10: 7472 6561 6d3a 2073 7973 2e73 7464 6f75  tream: sys.stdou
+0001fd20: 7420 6279 2064 6566 6175 6c74 0a20 2020  t by default.   
+0001fd30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001fd40: 2069 6620 7374 7265 616d 2069 7320 4e6f   if stream is No
+0001fd50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001fd60: 7374 7265 616d 203d 2073 7973 2e73 7464  stream = sys.std
+0001fd70: 6f75 740a 2020 2020 2020 2020 696d 706f  out.        impo
+0001fd80: 7274 206e 756d 7079 0a0a 2020 2020 2020  rt numpy..      
+0001fd90: 2020 7072 696e 7428 2225 7353 7461 7473    print("%sStats
+0001fda0: 3a22 2025 2073 7472 6561 6d5f 7072 6566  :" % stream_pref
+0001fdb0: 6978 2c20 6669 6c65 3d73 7472 6561 6d29  ix, file=stream)
+0001fdc0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0001fdd0: 2e6e 756d 5f73 6571 7320 213d 2073 656c  .num_seqs != sel
+0001fde0: 662e 746f 7461 6c5f 6461 7461 5f6c 656e  f.total_data_len
+0001fdf0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+0001fe00: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+0001fe10: 2020 2020 2022 2020 2569 2073 6571 732c       "  %i seqs,
+0001fe20: 2025 6920 746f 7461 6c20 6672 616d 6573   %i total frames
+0001fe30: 2c20 2566 2061 7665 7261 6765 2066 7261  , %f average fra
+0001fe40: 6d65 7322 0a20 2020 2020 2020 2020 2020  mes".           
+0001fe50: 2020 2020 2025 2028 7365 6c66 2e6e 756d       % (self.num
+0001fe60: 5f73 6571 732c 2073 656c 662e 746f 7461  _seqs, self.tota
+0001fe70: 6c5f 6461 7461 5f6c 656e 2c20 7365 6c66  l_data_len, self
+0001fe80: 2e74 6f74 616c 5f64 6174 615f 6c65 6e20  .total_data_len 
+0001fe90: 2f20 666c 6f61 7428 7365 6c66 2e6e 756d  / float(self.num
+0001fea0: 5f73 6571 7329 292c 0a20 2020 2020 2020  _seqs)),.       
+0001feb0: 2020 2020 2020 2020 2066 696c 653d 7374           file=st
+0001fec0: 7265 616d 2c0a 2020 2020 2020 2020 2020  ream,.          
+0001fed0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+0001fee0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+0001fef0: 696e 7428 2220 2025 6920 7365 7173 2220  int("  %i seqs" 
+0001ff00: 2520 2873 656c 662e 6e75 6d5f 7365 7173  % (self.num_seqs
+0001ff10: 2c29 2c20 6669 6c65 3d73 7472 6561 6d29  ,), file=stream)
+0001ff20: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0001ff30: 2020 4d65 616e 3a20 2573 2220 2520 2873    Mean: %s" % (s
+0001ff40: 656c 662e 666f 726d 6174 5f73 7472 2873  elf.format_str(s
+0001ff50: 656c 662e 6765 745f 6d65 616e 2829 292c  elf.get_mean()),
+0001ff60: 292c 2066 696c 653d 7374 7265 616d 290a  ), file=stream).
+0001ff70: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+0001ff80: 2053 7464 2064 6576 3a20 2573 2220 2520   Std dev: %s" % 
+0001ff90: 2873 656c 662e 666f 726d 6174 5f73 7472  (self.format_str
+0001ffa0: 2873 656c 662e 6765 745f 7374 645f 6465  (self.get_std_de
+0001ffb0: 7628 2929 2c29 2c20 6669 6c65 3d73 7472  v()),), file=str
+0001ffc0: 6561 6d29 0a20 2020 2020 2020 2070 7269  eam).        pri
+0001ffd0: 6e74 2822 2020 4d69 6e2f 6d61 783a 2025  nt("  Min/max: %
+0001ffe0: 7320 2f20 2573 2220 2520 2873 656c 662e  s / %s" % (self.
+0001fff0: 666f 726d 6174 5f73 7472 2873 656c 662e  format_str(self.
+00020000: 6d69 6e29 2c20 7365 6c66 2e66 6f72 6d61  min), self.forma
+00020010: 745f 7374 7228 7365 6c66 2e6d 6178 2929  t_str(self.max))
+00020020: 2c20 6669 6c65 3d73 7472 6561 6d29 0a20  , file=stream). 
+00020030: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
+00020040: 5374 6420 6465 7620 286e 6169 7665 293a  Std dev (naive):
+00020050: 2025 7322 2025 206e 756d 7079 2e73 7172   %s" % numpy.sqr
+00020060: 7428 7365 6c66 2e6d 6561 6e5f 7371 202d  t(self.mean_sq -
+00020070: 2073 656c 662e 6d65 616e 202a 2073 656c   self.mean * sel
+00020080: 662e 6d65 616e 292c 2066 696c 653d 7374  f.mean), file=st
+00020090: 7265 616d 290a 2020 2020 2020 2020 6966  ream).        if
+000200a0: 206f 7574 7075 745f 6669 6c65 5f70 7265   output_file_pre
+000200b0: 6669 783a 0a20 2020 2020 2020 2020 2020  fix:.           
+000200c0: 2070 7269 6e74 2822 2020 5772 6974 6520   print("  Write 
+000200d0: 6d65 616e 2f73 7464 2d64 6576 2074 6f20  mean/std-dev to 
+000200e0: 2573 2e28 6d65 616e 7c73 7464 5f64 6576  %s.(mean|std_dev
+000200f0: 292e 7478 742e 2220 2520 286f 7574 7075  ).txt." % (outpu
+00020100: 745f 6669 6c65 5f70 7265 6669 782c 292c  t_file_prefix,),
+00020110: 2066 696c 653d 7374 7265 616d 290a 2020   file=stream).  
+00020120: 2020 2020 2020 2020 2020 6e75 6d70 792e            numpy.
+00020130: 7361 7665 7478 7428 2225 732e 6d65 616e  savetxt("%s.mean
+00020140: 2e74 7874 2220 2520 6f75 7470 7574 5f66  .txt" % output_f
+00020150: 696c 655f 7072 6566 6978 2c20 7365 6c66  ile_prefix, self
+00020160: 2e67 6574 5f6d 6561 6e28 2929 0a20 2020  .get_mean()).   
+00020170: 2020 2020 2020 2020 206e 756d 7079 2e73           numpy.s
+00020180: 6176 6574 7874 2822 2573 2e73 7464 5f64  avetxt("%s.std_d
+00020190: 6576 2e74 7874 2220 2520 6f75 7470 7574  ev.txt" % output
+000201a0: 5f66 696c 655f 7072 6566 6978 2c20 7365  _file_prefix, se
+000201b0: 6c66 2e67 6574 5f73 7464 5f64 6576 2829  lf.get_std_dev()
+000201c0: 290a 0a0a 6465 6620 6973 5f6e 616d 6564  )...def is_named
+000201d0: 7475 706c 6528 636c 7329 3a0a 2020 2020  tuple(cls):.    
+000201e0: 2222 220a 2020 2020 3a70 6172 616d 2054  """.    :param T
+000201f0: 2063 6c73 3a20 7475 706c 652c 206c 6973   cls: tuple, lis
+00020200: 7420 6f72 206e 616d 6564 7475 706c 6520  t or namedtuple 
+00020210: 7479 7065 0a20 2020 203a 7265 7475 726e  type.    :return
+00020220: 3a20 7768 6574 6865 7220 636c 7320 6973  : whether cls is
+00020230: 2061 206e 616d 6564 7475 706c 6520 7479   a namedtuple ty
+00020240: 7065 0a20 2020 203a 7274 7970 653a 2062  pe.    :rtype: b
+00020250: 6f6f 6c0a 2020 2020 2222 220a 2020 2020  ool.    """.    
+00020260: 7265 7475 726e 2069 7373 7562 636c 6173  return issubclas
+00020270: 7328 636c 732c 2074 7570 6c65 2920 616e  s(cls, tuple) an
+00020280: 6420 636c 7320 6973 206e 6f74 2074 7570  d cls is not tup
+00020290: 6c65 0a0a 0a64 6566 206d 616b 655f 7365  le...def make_se
+000202a0: 715f 6f66 5f74 7970 6528 636c 732c 2073  q_of_type(cls, s
+000202b0: 6571 293a 0a20 2020 2022 2222 0a20 2020  eq):.    """.   
+000202c0: 203a 7061 7261 6d20 7479 7065 5b54 5d20   :param type[T] 
+000202d0: 636c 733a 2065 2e67 2e20 7475 706c 652c  cls: e.g. tuple,
+000202e0: 206c 6973 7420 6f72 206e 616d 6564 7475   list or namedtu
+000202f0: 706c 650a 2020 2020 3a70 6172 616d 206c  ple.    :param l
+00020300: 6973 747c 7475 706c 657c 5420 7365 713a  ist|tuple|T seq:
+00020310: 0a20 2020 203a 7265 7475 726e 3a20 636c  .    :return: cl
+00020320: 7328 7365 7129 206f 7220 636c 7328 2a73  s(seq) or cls(*s
+00020330: 6571 290a 2020 2020 3a72 7479 7065 3a20  eq).    :rtype: 
+00020340: 547c 6c69 7374 7c74 7570 6c65 0a20 2020  T|list|tuple.   
+00020350: 2022 2222 0a20 2020 2061 7373 6572 7420   """.    assert 
+00020360: 6973 7375 6263 6c61 7373 2863 6c73 2c20  issubclass(cls, 
+00020370: 286c 6973 742c 2074 7570 6c65 2929 0a20  (list, tuple)). 
+00020380: 2020 2069 6620 6973 5f6e 616d 6564 7475     if is_namedtu
+00020390: 706c 6528 636c 7329 3a0a 2020 2020 2020  ple(cls):.      
+000203a0: 2020 7265 7475 726e 2063 6c73 282a 7365    return cls(*se
+000203b0: 7129 2020 2320 6e6f 7161 0a20 2020 2072  q)  # noqa.    r
+000203c0: 6574 7572 6e20 636c 7328 7365 7129 2020  eturn cls(seq)  
+000203d0: 2320 6e6f 7161 0a0a 0a64 6566 2065 6e73  # noqa...def ens
+000203e0: 7572 655f 6c69 7374 5f6f 665f 7479 7065  ure_list_of_type
+000203f0: 286c 732c 2074 7970 655f 293a 0a20 2020  (ls, type_):.   
+00020400: 2022 2222 0a20 2020 203a 7061 7261 6d20   """.    :param 
+00020410: 6c69 7374 206c 733a 0a20 2020 203a 7061  list ls:.    :pa
+00020420: 7261 6d20 2828 292d 3e54 297c 7479 7065  ram (()->T)|type
+00020430: 5b54 5d20 7479 7065 5f3a 2074 7970 6520  [T] type_: type 
+00020440: 6f66 2069 6e73 7461 6e63 6573 206f 6620  of instances of 
+00020450: 606c 7360 2e0a 2020 2020 2020 4e6f 7465  `ls`..      Note
+00020460: 2074 6865 2073 7472 616e 6765 2074 7970   the strange typ
+00020470: 6520 6865 7265 2069 6e20 7468 6520 646f  e here in the do
+00020480: 6373 7472 696e 6720 6973 2064 7565 2074  cstring is due t
+00020490: 6f20 736f 6d65 2050 7943 6861 726d 2074  o some PyCharm t
+000204a0: 7970 6520 696e 6665 7265 6e63 6520 7072  ype inference pr
+000204b0: 6f62 6c65 6d73 0a20 2020 2020 2028 6874  oblems.      (ht
+000204c0: 7470 733a 2f2f 796f 7574 7261 636b 2e6a  tps://youtrack.j
+000204d0: 6574 6272 6169 6e73 2e63 6f6d 2f69 7373  etbrains.com/iss
+000204e0: 7565 2f50 592d 3530 3832 3829 2e0a 2020  ue/PY-50828)..  
+000204f0: 2020 3a72 7479 7065 3a20 6c69 7374 5b54    :rtype: list[T
+00020500: 5d0a 2020 2020 2222 220a 2020 2020 6173  ].    """.    as
+00020510: 7365 7274 2061 6c6c 2869 7369 6e73 7461  sert all(isinsta
+00020520: 6e63 6528 656c 656d 2c20 7479 7065 5f29  nce(elem, type_)
+00020530: 2066 6f72 2065 6c65 6d20 696e 206c 7329   for elem in ls)
+00020540: 0a20 2020 2072 6574 7572 6e20 6c73 0a0a  .    return ls..
+00020550: 0a40 636f 6e74 6578 746c 6962 2e63 6f6e  .@contextlib.con
+00020560: 7465 7874 6d61 6e61 6765 720a 6465 6620  textmanager.def 
+00020570: 6475 6d6d 795f 6e6f 6f70 5f63 7478 2829  dummy_noop_ctx()
+00020580: 3a0a 2020 2020 2222 220a 2020 2020 5072  :.    """.    Pr
+00020590: 6f76 6964 6573 2061 206e 6f2d 6f70 2063  ovides a no-op c
+000205a0: 6f6e 7465 7874 206d 616e 6167 6572 2e0a  ontext manager..
+000205b0: 2020 2020 2222 220a 2020 2020 7969 656c      """.    yiel
+000205c0: 6420 4e6f 6e65 0a0a 0a64 6566 205f 6765  d None...def _ge
+000205d0: 745f 6e67 7261 6d73 2873 6567 6d65 6e74  t_ngrams(segment
+000205e0: 2c20 6d61 785f 6f72 6465 7229 3a0a 2020  , max_order):.  
+000205f0: 2020 2222 2245 7874 7261 6374 7320 616c    """Extracts al
+00020600: 6c20 6e2d 6772 616d 7320 7570 746f 2061  l n-grams upto a
+00020610: 2067 6976 656e 206d 6178 696d 756d 206f   given maximum o
+00020620: 7264 6572 2066 726f 6d20 616e 2069 6e70  rder from an inp
+00020630: 7574 2073 6567 6d65 6e74 2e0a 2020 2020  ut segment..    
+00020640: 436f 6465 2061 6461 7074 6564 2066 726f  Code adapted fro
+00020650: 6d20 476f 6f67 6c65 2054 656e 736f 7232  m Google Tensor2
+00020660: 5465 6e73 6f72 2e0a 0a20 2020 2041 7267  Tensor...    Arg
+00020670: 733a 0a20 2020 2020 2073 6567 6d65 6e74  s:.      segment
+00020680: 2028 6c69 7374 5b69 6e74 5d7c 6c69 7374   (list[int]|list
+00020690: 5b73 7472 5d29 3a20 7465 7874 2073 6567  [str]): text seg
+000206a0: 6d65 6e74 2066 726f 6d20 7768 6963 6820  ment from which 
+000206b0: 6e2d 6772 616d 7320 7769 6c6c 2062 6520  n-grams will be 
+000206c0: 6578 7472 6163 7465 642e 0a20 2020 2020  extracted..     
+000206d0: 206d 6178 5f6f 7264 6572 2028 696e 7429   max_order (int)
+000206e0: 3a20 6d61 7869 6d75 6d20 6c65 6e67 7468  : maximum length
+000206f0: 2069 6e20 746f 6b65 6e73 206f 6620 7468   in tokens of th
+00020700: 6520 6e2d 6772 616d 7320 7265 7475 726e  e n-grams return
+00020710: 6564 2062 7920 7468 6973 0a20 2020 2020  ed by this.     
+00020720: 2020 2020 206d 6574 686f 6473 2e0a 0a20       methods... 
+00020730: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00020740: 2020 5468 6520 436f 756e 7465 7220 636f    The Counter co
+00020750: 6e74 6169 6e69 6e67 2061 6c6c 206e 2d67  ntaining all n-g
+00020760: 7261 6d73 2075 7074 6f20 6d61 785f 6f72  rams upto max_or
+00020770: 6465 7220 696e 2073 6567 6d65 6e74 0a20  der in segment. 
+00020780: 2020 2020 2077 6974 6820 6120 636f 756e       with a coun
+00020790: 7420 6f66 2068 6f77 206d 616e 7920 7469  t of how many ti
+000207a0: 6d65 7320 6561 6368 206e 2d67 7261 6d20  mes each n-gram 
+000207b0: 6f63 6375 7272 6564 2e0a 2020 2020 2222  occurred..    ""
+000207c0: 220a 2020 2020 696d 706f 7274 2063 6f6c  ".    import col
+000207d0: 6c65 6374 696f 6e73 0a0a 2020 2020 6e67  lections..    ng
+000207e0: 7261 6d5f 636f 756e 7473 203d 2063 6f6c  ram_counts = col
+000207f0: 6c65 6374 696f 6e73 2e43 6f75 6e74 6572  lections.Counter
+00020800: 2829 0a20 2020 2066 6f72 206f 7264 6572  ().    for order
+00020810: 2069 6e20 7261 6e67 6528 312c 206d 6178   in range(1, max
+00020820: 5f6f 7264 6572 202b 2031 293a 0a20 2020  _order + 1):.   
+00020830: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00020840: 6e67 6528 302c 206c 656e 2873 6567 6d65  nge(0, len(segme
+00020850: 6e74 2920 2d20 6f72 6465 7220 2b20 3129  nt) - order + 1)
+00020860: 3a0a 2020 2020 2020 2020 2020 2020 6e67  :.            ng
+00020870: 7261 6d20 3d20 7475 706c 6528 7365 676d  ram = tuple(segm
+00020880: 656e 745b 6920 3a20 6920 2b20 6f72 6465  ent[i : i + orde
+00020890: 725d 290a 2020 2020 2020 2020 2020 2020  r]).            
+000208a0: 6e67 7261 6d5f 636f 756e 7473 5b6e 6772  ngram_counts[ngr
+000208b0: 616d 5d20 2b3d 2031 0a20 2020 2072 6574  am] += 1.    ret
+000208c0: 7572 6e20 6e67 7261 6d5f 636f 756e 7473  urn ngram_counts
+000208d0: 0a0a 0a64 6566 2063 6f6d 7075 7465 5f62  ...def compute_b
+000208e0: 6c65 7528 7265 6665 7265 6e63 655f 636f  leu(reference_co
+000208f0: 7270 7573 2c20 7472 616e 736c 6174 696f  rpus, translatio
+00020900: 6e5f 636f 7270 7573 2c20 6d61 785f 6f72  n_corpus, max_or
+00020910: 6465 723d 342c 2075 7365 5f62 703d 5472  der=4, use_bp=Tr
+00020920: 7565 293a 0a20 2020 2022 2222 436f 6d70  ue):.    """Comp
+00020930: 7574 6573 2042 4c45 5520 7363 6f72 6520  utes BLEU score 
+00020940: 6f66 2074 7261 6e73 6c61 7465 6420 7365  of translated se
+00020950: 676d 656e 7473 2061 6761 696e 7374 206f  gments against o
+00020960: 6e65 206f 7220 6d6f 7265 2072 6566 6572  ne or more refer
+00020970: 656e 6365 732e 0a20 2020 2043 6f64 6520  ences..    Code 
+00020980: 6164 6170 7465 6420 6672 6f6d 2047 6f6f  adapted from Goo
+00020990: 676c 6520 5465 6e73 6f72 3254 656e 736f  gle Tensor2Tenso
+000209a0: 722e 0a0a 2020 2020 4172 6773 3a0a 2020  r...    Args:.  
+000209b0: 2020 2020 7265 6665 7265 6e63 655f 636f      reference_co
+000209c0: 7270 7573 2028 6c69 7374 5b6c 6973 745b  rpus (list[list[
+000209d0: 696e 745d 7c6c 6973 745b 7374 725d 5d29  int]|list[str]])
+000209e0: 3a20 6c69 7374 206f 6620 7265 6665 7265  : list of refere
+000209f0: 6e63 6573 2066 6f72 2065 6163 6820 7472  nces for each tr
+00020a00: 616e 736c 6174 696f 6e2e 2045 6163 680a  anslation. Each.
+00020a10: 2020 2020 2020 2020 2020 7265 6665 7265            refere
+00020a20: 6e63 6520 7368 6f75 6c64 2062 6520 746f  nce should be to
+00020a30: 6b65 6e69 7a65 6420 696e 746f 2061 206c  kenized into a l
+00020a40: 6973 7420 6f66 2074 6f6b 656e 732e 0a20  ist of tokens.. 
+00020a50: 2020 2020 2074 7261 6e73 6c61 7469 6f6e       translation
+00020a60: 5f63 6f72 7075 7320 286c 6973 745b 6c69  _corpus (list[li
+00020a70: 7374 5b69 6e74 5d7c 6c69 7374 5b73 7472  st[int]|list[str
+00020a80: 5d5d 293a 206c 6973 7420 6f66 2074 7261  ]]): list of tra
+00020a90: 6e73 6c61 7469 6f6e 7320 746f 2073 636f  nslations to sco
+00020aa0: 7265 2e20 4561 6368 2074 7261 6e73 6c61  re. Each transla
+00020ab0: 7469 6f6e 0a20 2020 2020 2020 2020 2073  tion.          s
+00020ac0: 686f 756c 6420 6265 2074 6f6b 656e 697a  hould be tokeniz
+00020ad0: 6564 2069 6e74 6f20 6120 6c69 7374 206f  ed into a list o
+00020ae0: 6620 746f 6b65 6e73 2e0a 2020 2020 2020  f tokens..      
+00020af0: 6d61 785f 6f72 6465 7220 2869 6e74 293a  max_order (int):
+00020b00: 204d 6178 696d 756d 206e 2d67 7261 6d20   Maximum n-gram 
+00020b10: 6f72 6465 7220 746f 2075 7365 2077 6865  order to use whe
+00020b20: 6e20 636f 6d70 7574 696e 6720 424c 4555  n computing BLEU
+00020b30: 2073 636f 7265 2e0a 2020 2020 2020 7573   score..      us
+00020b40: 655f 6270 2028 626f 6f6c 293a 2062 6f6f  e_bp (bool): boo
+00020b50: 6c65 616e 2c20 7768 6574 6865 7220 746f  lean, whether to
+00020b60: 2061 7070 6c79 2062 7265 7669 7479 2070   apply brevity p
+00020b70: 656e 616c 7479 2e0a 0a20 2020 2052 6574  enalty...    Ret
+00020b80: 7572 6e73 3a0a 2020 2020 2020 424c 4555  urns:.      BLEU
+00020b90: 2073 636f 7265 2e0a 2020 2020 2222 220a   score..    """.
+00020ba0: 2020 2020 696d 706f 7274 206d 6174 680a      import math.
+00020bb0: 0a20 2020 2072 6566 6572 656e 6365 5f6c  .    reference_l
+00020bc0: 656e 6774 6820 3d20 300a 2020 2020 7472  ength = 0.    tr
+00020bd0: 616e 736c 6174 696f 6e5f 6c65 6e67 7468  anslation_length
+00020be0: 203d 2030 0a20 2020 2062 7020 3d20 312e   = 0.    bp = 1.
+00020bf0: 300a 2020 2020 6765 6f5f 6d65 616e 203d  0.    geo_mean =
+00020c00: 2030 0a0a 2020 2020 6d61 7463 6865 735f   0..    matches_
+00020c10: 6279 5f6f 7264 6572 203d 205b 305d 202a  by_order = [0] *
+00020c20: 206d 6178 5f6f 7264 6572 0a20 2020 2070   max_order.    p
+00020c30: 6f73 7369 626c 655f 6d61 7463 6865 735f  ossible_matches_
+00020c40: 6279 5f6f 7264 6572 203d 205b 305d 202a  by_order = [0] *
+00020c50: 206d 6178 5f6f 7264 6572 0a0a 2020 2020   max_order..    
+00020c60: 666f 7220 2872 6566 6572 656e 6365 732c  for (references,
+00020c70: 2074 7261 6e73 6c61 7469 6f6e 7329 2069   translations) i
+00020c80: 6e20 7a69 7028 7265 6665 7265 6e63 655f  n zip(reference_
+00020c90: 636f 7270 7573 2c20 7472 616e 736c 6174  corpus, translat
+00020ca0: 696f 6e5f 636f 7270 7573 293a 0a20 2020  ion_corpus):.   
+00020cb0: 2020 2020 2072 6566 6572 656e 6365 5f6c       reference_l
+00020cc0: 656e 6774 6820 2b3d 206c 656e 2872 6566  ength += len(ref
+00020cd0: 6572 656e 6365 7329 0a20 2020 2020 2020  erences).       
+00020ce0: 2074 7261 6e73 6c61 7469 6f6e 5f6c 656e   translation_len
+00020cf0: 6774 6820 2b3d 206c 656e 2874 7261 6e73  gth += len(trans
+00020d00: 6c61 7469 6f6e 7329 0a20 2020 2020 2020  lations).       
+00020d10: 2072 6566 5f6e 6772 616d 5f63 6f75 6e74   ref_ngram_count
+00020d20: 7320 3d20 5f67 6574 5f6e 6772 616d 7328  s = _get_ngrams(
+00020d30: 7265 6665 7265 6e63 6573 2c20 6d61 785f  references, max_
+00020d40: 6f72 6465 7229 0a20 2020 2020 2020 2074  order).        t
+00020d50: 7261 6e73 6c61 7469 6f6e 5f6e 6772 616d  ranslation_ngram
+00020d60: 5f63 6f75 6e74 7320 3d20 5f67 6574 5f6e  _counts = _get_n
+00020d70: 6772 616d 7328 7472 616e 736c 6174 696f  grams(translatio
+00020d80: 6e73 2c20 6d61 785f 6f72 6465 7229 0a0a  ns, max_order)..
+00020d90: 2020 2020 2020 2020 6f76 6572 6c61 7020          overlap 
+00020da0: 3d20 7b6e 6772 616d 3a20 6d69 6e28 636f  = {ngram: min(co
+00020db0: 756e 742c 2074 7261 6e73 6c61 7469 6f6e  unt, translation
+00020dc0: 5f6e 6772 616d 5f63 6f75 6e74 735b 6e67  _ngram_counts[ng
+00020dd0: 7261 6d5d 2920 666f 7220 6e67 7261 6d2c  ram]) for ngram,
+00020de0: 2063 6f75 6e74 2069 6e20 7265 665f 6e67   count in ref_ng
+00020df0: 7261 6d5f 636f 756e 7473 2e69 7465 6d73  ram_counts.items
+00020e00: 2829 7d0a 0a20 2020 2020 2020 2066 6f72  ()}..        for
+00020e10: 206e 6772 616d 2069 6e20 6f76 6572 6c61   ngram in overla
+00020e20: 703a 0a20 2020 2020 2020 2020 2020 206d  p:.            m
+00020e30: 6174 6368 6573 5f62 795f 6f72 6465 725b  atches_by_order[
+00020e40: 6c65 6e28 6e67 7261 6d29 202d 2031 5d20  len(ngram) - 1] 
+00020e50: 2b3d 206f 7665 726c 6170 5b6e 6772 616d  += overlap[ngram
+00020e60: 5d0a 2020 2020 2020 2020 666f 7220 6e67  ].        for ng
+00020e70: 7261 6d20 696e 2074 7261 6e73 6c61 7469  ram in translati
+00020e80: 6f6e 5f6e 6772 616d 5f63 6f75 6e74 733a  on_ngram_counts:
+00020e90: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
+00020ea0: 7369 626c 655f 6d61 7463 6865 735f 6279  sible_matches_by
+00020eb0: 5f6f 7264 6572 5b6c 656e 286e 6772 616d  _order[len(ngram
+00020ec0: 2920 2d20 315d 202b 3d20 7472 616e 736c  ) - 1] += transl
+00020ed0: 6174 696f 6e5f 6e67 7261 6d5f 636f 756e  ation_ngram_coun
+00020ee0: 7473 5b6e 6772 616d 5d0a 0a20 2020 2070  ts[ngram]..    p
+00020ef0: 7265 6369 7369 6f6e 7320 3d20 5b30 2e30  recisions = [0.0
+00020f00: 5d20 2a20 6d61 785f 6f72 6465 720a 2020  ] * max_order.  
+00020f10: 2020 736d 6f6f 7468 203d 2031 2e30 0a20    smooth = 1.0. 
+00020f20: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00020f30: 6528 302c 206d 6178 5f6f 7264 6572 293a  e(0, max_order):
+00020f40: 0a20 2020 2020 2020 2069 6620 706f 7373  .        if poss
+00020f50: 6962 6c65 5f6d 6174 6368 6573 5f62 795f  ible_matches_by_
+00020f60: 6f72 6465 725b 695d 203e 2030 3a0a 2020  order[i] > 0:.  
+00020f70: 2020 2020 2020 2020 2020 7072 6563 6973            precis
+00020f80: 696f 6e73 5b69 5d20 3d20 6d61 7463 6865  ions[i] = matche
+00020f90: 735f 6279 5f6f 7264 6572 5b69 5d20 2f20  s_by_order[i] / 
+00020fa0: 706f 7373 6962 6c65 5f6d 6174 6368 6573  possible_matches
+00020fb0: 5f62 795f 6f72 6465 725b 695d 0a20 2020  _by_order[i].   
+00020fc0: 2020 2020 2020 2020 2069 6620 6d61 7463           if matc
+00020fd0: 6865 735f 6279 5f6f 7264 6572 5b69 5d20  hes_by_order[i] 
+00020fe0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00020ff0: 2020 2020 2070 7265 6369 7369 6f6e 735b       precisions[
+00021000: 695d 203d 206d 6174 6368 6573 5f62 795f  i] = matches_by_
+00021010: 6f72 6465 725b 695d 202f 2070 6f73 7369  order[i] / possi
+00021020: 626c 655f 6d61 7463 6865 735f 6279 5f6f  ble_matches_by_o
+00021030: 7264 6572 5b69 5d0a 2020 2020 2020 2020  rder[i].        
+00021040: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00021050: 2020 2020 2020 2020 2020 736d 6f6f 7468            smooth
+00021060: 202a 3d20 320a 2020 2020 2020 2020 2020   *= 2.          
+00021070: 2020 2020 2020 7072 6563 6973 696f 6e73        precisions
+00021080: 5b69 5d20 3d20 312e 3020 2f20 2873 6d6f  [i] = 1.0 / (smo
+00021090: 6f74 6820 2a20 706f 7373 6962 6c65 5f6d  oth * possible_m
+000210a0: 6174 6368 6573 5f62 795f 6f72 6465 725b  atches_by_order[
+000210b0: 695d 290a 2020 2020 2020 2020 656c 7365  i]).        else
+000210c0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000210d0: 6563 6973 696f 6e73 5b69 5d20 3d20 302e  ecisions[i] = 0.
+000210e0: 300a 0a20 2020 2069 6620 6d61 7828 7072  0..    if max(pr
+000210f0: 6563 6973 696f 6e73 2920 3e20 303a 0a20  ecisions) > 0:. 
+00021100: 2020 2020 2020 2070 5f6c 6f67 5f73 756d         p_log_sum
+00021110: 203d 2073 756d 286d 6174 682e 6c6f 6728   = sum(math.log(
+00021120: 7029 2066 6f72 2070 2069 6e20 7072 6563  p) for p in prec
+00021130: 6973 696f 6e73 2069 6620 7029 0a20 2020  isions if p).   
+00021140: 2020 2020 2067 656f 5f6d 6561 6e20 3d20       geo_mean = 
+00021150: 6d61 7468 2e65 7870 2870 5f6c 6f67 5f73  math.exp(p_log_s
+00021160: 756d 202f 206d 6178 5f6f 7264 6572 290a  um / max_order).
+00021170: 0a20 2020 2069 6620 7573 655f 6270 3a0a  .    if use_bp:.
+00021180: 2020 2020 2020 2020 7261 7469 6f20 3d20          ratio = 
+00021190: 7472 616e 736c 6174 696f 6e5f 6c65 6e67  translation_leng
+000211a0: 7468 202f 2072 6566 6572 656e 6365 5f6c  th / reference_l
+000211b0: 656e 6774 680a 2020 2020 2020 2020 6966  ength.        if
+000211c0: 2072 6174 696f 203c 2031 652d 3330 3a0a   ratio < 1e-30:.
+000211d0: 2020 2020 2020 2020 2020 2020 6270 203d              bp =
+000211e0: 2030 2e30 0a20 2020 2020 2020 2065 6c69   0.0.        eli
+000211f0: 6620 7261 7469 6f20 3c20 312e 303a 0a20  f ratio < 1.0:. 
+00021200: 2020 2020 2020 2020 2020 2062 7020 3d20             bp = 
+00021210: 6d61 7468 2e65 7870 2831 202d 2031 2e30  math.exp(1 - 1.0
+00021220: 202f 2072 6174 696f 290a 2020 2020 2020   / ratio).      
+00021230: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00021240: 2020 2020 6270 203d 2031 2e30 0a20 2020      bp = 1.0.   
+00021250: 2062 6c65 7520 3d20 6765 6f5f 6d65 616e   bleu = geo_mean
+00021260: 202a 2062 700a 2020 2020 7265 7475 726e   * bp.    return
+00021270: 206e 702e 666c 6f61 7433 3228 626c 6575   np.float32(bleu
+00021280: 290a 0a0a 2320 6e6f 696e 7370 6563 7469  )...# noinspecti
+00021290: 6f6e 2050 7950 6163 6b61 6765 5265 7175  on PyPackageRequ
+000212a0: 6972 656d 656e 7473 0a64 6566 206d 6f6e  irements.def mon
+000212b0: 6b65 7966 6978 5f67 6c69 6228 293a 0a20  keyfix_glib():. 
+000212c0: 2020 2022 2222 0a20 2020 2046 6978 6573     """.    Fixes
+000212d0: 2073 6f6d 6520 7374 7570 6964 2062 7567   some stupid bug
+000212e0: 7320 7375 6368 2074 6861 7420 5349 4749  s such that SIGI
+000212f0: 4e54 2069 7320 6e6f 7420 776f 726b 696e  NT is not workin
+00021300: 672e 0a20 2020 2054 6869 7320 6973 2075  g..    This is u
+00021310: 7365 6420 6279 2061 7564 696f 7265 6164  sed by audioread
+00021320: 2c20 616e 6420 696e 6469 7265 6374 6c79  , and indirectly
+00021330: 2062 7920 6c69 6272 6f73 6120 666f 7220   by librosa for 
+00021340: 6c6f 6164 696e 6720 6175 6469 6f2e 0a20  loading audio.. 
+00021350: 2020 2068 7474 7073 3a2f 2f73 7461 636b     https://stack
+00021360: 6f76 6572 666c 6f77 2e63 6f6d 2f71 7565  overflow.com/que
+00021370: 7374 696f 6e73 2f31 3634 3130 3835 322f  stions/16410852/
+00021380: 0a20 2020 2053 6565 2061 6c73 6f20 3a66  .    See also :f
+00021390: 756e 633a 606d 6f6e 6b65 7970 6174 6368  unc:`monkeypatch
+000213a0: 5f61 7564 696f 7265 6164 602e 0a20 2020  _audioread`..   
+000213b0: 2022 2222 0a20 2020 2074 7279 3a0a 2020   """.    try:.  
+000213c0: 2020 2020 2020 696d 706f 7274 2067 690a        import gi.
+000213d0: 2020 2020 6578 6365 7074 2049 6d70 6f72      except Impor
+000213e0: 7445 7272 6f72 3a0a 2020 2020 2020 2020  tError:.        
+000213f0: 7265 7475 726e 0a20 2020 2074 7279 3a0a  return.    try:.
+00021400: 2020 2020 2020 2020 6672 6f6d 2067 692e          from gi.
+00021410: 7265 706f 7369 746f 7279 2069 6d70 6f72  repository impor
+00021420: 7420 474c 6962 0a20 2020 2065 7863 6570  t GLib.    excep
+00021430: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
+00021440: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
+00021450: 6374 696f 6e20 5079 556e 7265 736f 6c76  ction PyUnresolv
+00021460: 6564 5265 6665 7265 6e63 6573 0a20 2020  edReferences.   
+00021470: 2020 2020 2066 726f 6d20 6769 2e6f 7665       from gi.ove
+00021480: 7272 6964 6573 2069 6d70 6f72 7420 474c  rrides import GL
+00021490: 6962 0a20 2020 2023 2044 6f20 6e6f 7468  ib.    # Do noth
+000214a0: 696e 672e 0a20 2020 2023 2054 6865 206f  ing..    # The o
+000214b0: 7269 6769 6e61 6c20 6265 6861 7669 6f72  riginal behavior
+000214c0: 2077 6f75 6c64 2069 6e73 7461 6c6c 2061   would install a
+000214d0: 2053 4947 494e 5420 6861 6e64 6c65 7220   SIGINT handler 
+000214e0: 7768 6963 6820 6361 6c6c 7320 474c 6962  which calls GLib
+000214f0: 2e4d 6169 6e4c 6f6f 702e 7175 6974 2829  .MainLoop.quit()
+00021500: 2c0a 2020 2020 2320 616e 6420 7468 656e  ,.    # and then
+00021510: 2072 6572 6169 7365 2061 204b 6579 626f   reraise a Keybo
+00021520: 6172 6449 6e74 6572 7275 7074 2069 6e20  ardInterrupt in 
+00021530: 7468 6174 2074 6872 6561 642e 0a20 2020  that thread..   
+00021540: 2023 2048 6f77 6576 6572 2c20 7765 2077   # However, we w
+00021550: 616e 7420 616e 6420 6578 7065 6374 2074  ant and expect t
+00021560: 6f20 6765 7420 7468 6520 4b65 7962 6f61  o get the Keyboa
+00021570: 7264 496e 7465 7272 7570 7420 696e 2074  rdInterrupt in t
+00021580: 6865 206d 6169 6e20 7468 7265 6164 2e0a  he main thread..
+00021590: 2020 2020 474c 6962 2e4d 6169 6e4c 6f6f      GLib.MainLoo
+000215a0: 702e 5f5f 696e 6974 5f5f 203d 206c 616d  p.__init__ = lam
+000215b0: 6264 6120 2a61 7267 732c 202a 2a6b 7761  bda *args, **kwa
+000215c0: 7267 733a 204e 6f6e 650a 0a0a 6465 6620  rgs: None...def 
+000215d0: 6d6f 6e6b 6579 7061 7463 685f 6175 6469  monkeypatch_audi
+000215e0: 6f72 6561 6428 293a 0a20 2020 2022 2222  oread():.    """
+000215f0: 0a20 2020 2061 7564 696f 7265 6164 2064  .    audioread d
+00021600: 6f65 7320 6e6f 7420 6265 6861 7665 206f  oes not behave o
+00021610: 7074 696d 616c 2069 6e20 736f 6d65 2063  ptimal in some c
+00021620: 6173 6573 2e0a 2020 2020 452e 672e 2065  ases..    E.g. e
+00021630: 6163 6820 6361 6c6c 2074 6f20 5f63 615f  ach call to _ca_
+00021640: 6176 6169 6c61 626c 6528 2920 7461 6b65  available() take
+00021650: 7320 7175 6974 6520 6c6f 6e67 2062 6563  s quite long bec
+00021660: 6175 7365 206f 6620 7468 6520 6374 7970  ause of the ctyp
+00021670: 6573 2e75 7469 6c2e 6669 6e64 5f6c 6962  es.util.find_lib
+00021680: 7261 7279 2075 7361 6765 2e0a 2020 2020  rary usage..    
+00021690: 5765 2077 696c 6c20 7061 7463 6820 7468  We will patch th
+000216a0: 6973 2e0a 0a20 2020 2048 6f77 6576 6572  is...    However
+000216b0: 2c20 7468 6520 7265 636f 6d6d 656e 6461  , the recommenda
+000216c0: 7469 6f6e 2077 6f75 6c64 2062 6520 746f  tion would be to
+000216d0: 206e 6f74 2075 7365 2061 7564 696f 7265   not use audiore
+000216e0: 6164 2028 6c69 6272 6f73 612e 6c6f 6164  ad (librosa.load
+000216f0: 292e 0a20 2020 2061 7564 696f 7265 6164  )..    audioread
+00021700: 2075 7365 7320 4773 7472 6561 6d65 7220   uses Gstreamer 
+00021710: 6173 2061 2062 6163 6b65 6e64 2062 7920  as a backend by 
+00021720: 6465 6661 756c 7420 6375 7272 656e 746c  default currentl
+00021730: 7920 286f 6e20 4c69 6e75 7829 2e0a 2020  y (on Linux)..  
+00021740: 2020 4773 7472 6561 6d65 7220 6861 7320    Gstreamer has 
+00021750: 6d75 6c74 6970 6c65 2069 7373 7565 732e  multiple issues.
+00021760: 2053 6565 2061 6c73 6f20 3a66 756e 633a   See also :func:
+00021770: 606d 6f6e 6b65 7966 6978 5f67 6c69 6260  `monkeyfix_glib`
+00021780: 2c20 616e 6420 6865 7265 2066 6f72 2064  , and here for d
+00021790: 6973 6375 7373 696f 6e3a 0a20 2020 2068  iscussion:.    h
+000217a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000217b0: 6d2f 6265 6574 626f 782f 6175 6469 6f72  m/beetbox/audior
+000217c0: 6561 642f 6973 7375 6573 2f36 320a 2020  ead/issues/62.  
+000217d0: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
+000217e0: 2e63 6f6d 2f62 6565 7462 6f78 2f61 7564  .com/beetbox/aud
+000217f0: 696f 7265 6164 2f69 7373 7565 732f 3633  ioread/issues/63
+00021800: 0a0a 2020 2020 496e 7374 6561 642c 2075  ..    Instead, u
+00021810: 7365 2050 7953 6f75 6e64 4669 6c65 2c20  se PySoundFile, 
+00021820: 7768 6963 6820 6973 2061 6c73 6f20 6661  which is also fa
+00021830: 7374 6572 2e20 5365 6520 6865 7265 2066  ster. See here f
+00021840: 6f72 2064 6973 6375 7373 696f 6e73 3a0a  or discussions:.
+00021850: 2020 2020 6874 7470 733a 2f2f 6769 7468      https://gith
+00021860: 7562 2e63 6f6d 2f62 6565 7462 6f78 2f61  ub.com/beetbox/a
+00021870: 7564 696f 7265 6164 2f69 7373 7565 732f  udioread/issues/
+00021880: 3634 0a20 2020 2068 7474 7073 3a2f 2f67  64.    https://g
+00021890: 6974 6875 622e 636f 6d2f 6c69 6272 6f73  ithub.com/libros
+000218a0: 612f 6c69 6272 6f73 612f 6973 7375 6573  a/librosa/issues
+000218b0: 2f36 3831 0a20 2020 2022 2222 0a20 2020  /681.    """.   
+000218c0: 2074 7279 3a0a 2020 2020 2020 2020 2320   try:.        # 
+000218d0: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+000218e0: 6163 6b61 6765 5265 7175 6972 656d 656e  ackageRequiremen
+000218f0: 7473 0a20 2020 2020 2020 2069 6d70 6f72  ts.        impor
+00021900: 7420 6175 6469 6f72 6561 640a 2020 2020  t audioread.    
+00021910: 6578 6365 7074 2049 6d70 6f72 7445 7272  except ImportErr
+00021920: 6f72 3a0a 2020 2020 2020 2020 7265 7475  or:.        retu
+00021930: 726e 0a20 2020 2023 206e 6f69 6e73 7065  rn.    # noinspe
+00021940: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
+00021950: 644d 656d 6265 720a 2020 2020 7265 7320  dMember.    res 
+00021960: 3d20 6175 6469 6f72 6561 642e 5f63 615f  = audioread._ca_
+00021970: 6176 6169 6c61 626c 6528 290a 2020 2020  available().    
+00021980: 6175 6469 6f72 6561 642e 5f63 615f 6176  audioread._ca_av
+00021990: 6169 6c61 626c 6520 3d20 6c61 6d62 6461  ailable = lambda
+000219a0: 3a20 7265 730a 0a0a 5f63 665f 6361 6368  : res..._cf_cach
+000219b0: 6520 3d20 7b7d 0a5f 6366 5f6d 7367 5f70  e = {}._cf_msg_p
+000219c0: 7269 6e74 6564 203d 2046 616c 7365 0a0a  rinted = False..
+000219d0: 0a64 6566 2063 6628 6669 6c65 6e61 6d65  .def cf(filename
+000219e0: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
+000219f0: 6163 6865 206d 616e 6167 6572 2e20 6936  ache manager. i6
+00021a00: 2073 7065 6369 6669 632e 0a0a 2020 2020   specific...    
+00021a10: 3a72 6574 7572 6e3a 2066 696c 656e 616d  :return: filenam
+00021a20: 650a 2020 2020 3a72 7479 7065 3a20 7374  e.    :rtype: st
+00021a30: 720a 2020 2020 2222 220a 2020 2020 676c  r.    """.    gl
+00021a40: 6f62 616c 205f 6366 5f6d 7367 5f70 7269  obal _cf_msg_pri
+00021a50: 6e74 6564 0a20 2020 2069 6d70 6f72 7420  nted.    import 
+00021a60: 6f73 0a20 2020 2066 726f 6d20 7375 6270  os.    from subp
+00021a70: 726f 6365 7373 2069 6d70 6f72 7420 6368  rocess import ch
+00021a80: 6563 6b5f 6f75 7470 7574 0a0a 2020 2020  eck_output..    
+00021a90: 6966 2066 696c 656e 616d 6520 696e 205f  if filename in _
+00021aa0: 6366 5f63 6163 6865 3a0a 2020 2020 2020  cf_cache:.      
+00021ab0: 2020 7265 7475 726e 205f 6366 5f63 6163    return _cf_cac
+00021ac0: 6865 5b66 696c 656e 616d 655d 0a20 2020  he[filename].   
+00021ad0: 2064 6562 7567 5f6d 6f64 6520 3d20 696e   debug_mode = in
+00021ae0: 7428 6f73 2e65 6e76 6972 6f6e 2e67 6574  t(os.environ.get
+00021af0: 2822 4445 4255 4722 2c20 3029 290a 2020  ("DEBUG", 0)).  
+00021b00: 2020 6966 2064 6562 7567 5f6d 6f64 6520    if debug_mode 
+00021b10: 6f72 2067 6574 5f68 6f73 746e 616d 6528  or get_hostname(
+00021b20: 2920 3d3d 2022 636c 7573 7465 722d 636e  ) == "cluster-cn
+00021b30: 2d32 3131 2220 6f72 206e 6f74 2069 735f  -211" or not is_
+00021b40: 7275 6e6e 696e 675f 6f6e 5f63 6c75 7374  running_on_clust
+00021b50: 6572 2829 3a0a 2020 2020 2020 2020 6966  er():.        if
+00021b60: 206e 6f74 205f 6366 5f6d 7367 5f70 7269   not _cf_msg_pri
+00021b70: 6e74 6564 3a0a 2020 2020 2020 2020 2020  nted:.          
+00021b80: 2020 7072 696e 7428 2243 6163 6865 206d    print("Cache m
+00021b90: 616e 6167 6572 3a20 6e6f 7420 7573 6564  anager: not used
+00021ba0: 2c20 7573 6520 6c6f 6361 6c20 6669 6c65  , use local file
+00021bb0: 3a20 2573 2028 6469 7363 6172 6420 6675  : %s (discard fu
+00021bc0: 7274 6865 7220 6d65 7373 6167 6573 2922  rther messages)"
+00021bd0: 2025 2066 696c 656e 616d 6529 0a20 2020   % filename).   
+00021be0: 2020 2020 2020 2020 205f 6366 5f6d 7367           _cf_msg
+00021bf0: 5f70 7269 6e74 6564 203d 2054 7275 650a  _printed = True.
+00021c00: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00021c10: 696c 656e 616d 6520 2023 2066 6f72 2064  ilename  # for d
+00021c20: 6562 7567 6769 6e67 0a20 2020 2074 7279  ebugging.    try
+00021c30: 3a0a 2020 2020 2020 2020 6361 6368 6564  :.        cached
+00021c40: 5f66 6e20 3d20 6368 6563 6b5f 6f75 7470  _fn = check_outp
+00021c50: 7574 285b 2263 6622 2c20 6669 6c65 6e61  ut(["cf", filena
+00021c60: 6d65 5d29 2e73 7472 6970 2829 2e64 6563  me]).strip().dec
+00021c70: 6f64 6528 2275 7466 3822 290a 2020 2020  ode("utf8").    
+00021c80: 6578 6365 7074 2043 616c 6c65 6450 726f  except CalledPro
+00021c90: 6365 7373 4572 726f 723a 0a20 2020 2020  cessError:.     
+00021ca0: 2020 2069 6620 6e6f 7420 5f63 665f 6d73     if not _cf_ms
+00021cb0: 675f 7072 696e 7465 643a 0a20 2020 2020  g_printed:.     
+00021cc0: 2020 2020 2020 2070 7269 6e74 2822 4361         print("Ca
+00021cd0: 6368 6520 6d61 6e61 6765 723a 2045 7272  che manager: Err
+00021ce0: 6f72 206f 6363 7572 7265 642c 2075 7369  or occurred, usi
+00021cf0: 6e67 206c 6f63 616c 2066 696c 6522 290a  ng local file").
+00021d00: 2020 2020 2020 2020 2020 2020 5f63 665f              _cf_
+00021d10: 6d73 675f 7072 696e 7465 6420 3d20 5472  msg_printed = Tr
+00021d20: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00021d30: 6e20 6669 6c65 6e61 6d65 0a20 2020 2061  n filename.    a
+00021d40: 7373 6572 7420 6f73 2e70 6174 682e 6578  ssert os.path.ex
+00021d50: 6973 7473 2863 6163 6865 645f 666e 290a  ists(cached_fn).
+00021d60: 2020 2020 5f63 665f 6361 6368 655b 6669      _cf_cache[fi
+00021d70: 6c65 6e61 6d65 5d20 3d20 6361 6368 6564  lename] = cached
+00021d80: 5f66 6e0a 2020 2020 7265 7475 726e 2063  _fn.    return c
+00021d90: 6163 6865 645f 666e 0a0a 0a64 6566 2062  ached_fn...def b
+00021da0: 696e 6172 795f 7365 6172 6368 5f61 6e79  inary_search_any
+00021db0: 2863 6d70 2c20 6c6f 772c 2068 6967 6829  (cmp, low, high)
+00021dc0: 3a0a 2020 2020 2222 220a 2020 2020 4269  :.    """.    Bi
+00021dd0: 6e61 7279 2073 6561 7263 6820 666f 7220  nary search for 
+00021de0: 6120 6375 7374 6f6d 2063 6f6d 7061 7265  a custom compare
+00021df0: 2066 756e 6374 696f 6e2e 0a0a 2020 2020   function...    
+00021e00: 3a70 6172 616d 2028 696e 7429 2d3e 696e  :param (int)->in
+00021e10: 7420 636d 703a 2065 2e67 2e20 636d 7028  t cmp: e.g. cmp(
+00021e20: 6964 7829 203d 3d20 636f 6d70 6172 6528  idx) == compare(
+00021e30: 6172 7261 795b 6964 785d 2c20 6b65 7929  array[idx], key)
+00021e40: 0a20 2020 203a 7061 7261 6d20 696e 7420  .    :param int 
+00021e50: 6c6f 773a 2069 6e63 6c75 7369 7665 0a20  low: inclusive. 
+00021e60: 2020 203a 7061 7261 6d20 696e 7420 6869     :param int hi
+00021e70: 6768 3a20 6578 636c 7573 6976 650a 2020  gh: exclusive.  
+00021e80: 2020 3a72 7479 7065 3a20 696e 747c 4e6f    :rtype: int|No
+00021e90: 6e65 0a20 2020 2022 2222 0a20 2020 2077  ne.    """.    w
+00021ea0: 6869 6c65 206c 6f77 203c 2068 6967 683a  hile low < high:
+00021eb0: 0a20 2020 2020 2020 206d 6964 203d 2028  .        mid = (
+00021ec0: 6c6f 7720 2b20 6869 6768 2920 2f2f 2032  low + high) // 2
+00021ed0: 0a20 2020 2020 2020 2072 203d 2063 6d70  .        r = cmp
+00021ee0: 286d 6964 290a 2020 2020 2020 2020 6966  (mid).        if
+00021ef0: 2072 203c 2030 3a0a 2020 2020 2020 2020   r < 0:.        
+00021f00: 2020 2020 6c6f 7720 3d20 6d69 6420 2b20      low = mid + 
+00021f10: 310a 2020 2020 2020 2020 656c 6966 2072  1.        elif r
+00021f20: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00021f30: 2020 6869 6768 203d 206d 6964 0a20 2020    high = mid.   
+00021f40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00021f50: 2020 2020 2020 2072 6574 7572 6e20 6d69         return mi
+00021f60: 640a 2020 2020 7265 7475 726e 206c 6f77  d.    return low
+00021f70: 0a0a 0a64 6566 2067 656e 6572 6963 5f69  ...def generic_i
+00021f80: 6d70 6f72 745f 6d6f 6475 6c65 2866 696c  mport_module(fil
+00021f90: 656e 616d 6529 3a0a 2020 2020 2222 220a  ename):.    """.
+00021fa0: 2020 2020 3a70 6172 616d 2073 7472 2066      :param str f
+00021fb0: 696c 656e 616d 653a 0a20 2020 2020 2057  ilename:.      W
+00021fc0: 6520 7472 7920 746f 2062 6520 636c 6576  e try to be clev
+00021fd0: 6572 2061 626f 7574 2066 696c 656e 616d  er about filenam
+00021fe0: 652e 0a20 2020 2020 2049 6620 6974 206c  e..      If it l
+00021ff0: 6f6f 6b73 206c 696b 6520 6120 6d6f 6475  ooks like a modu
+00022000: 6c65 206e 616d 652c 206a 7573 7420 646f  le name, just do
+00022010: 2069 6d70 6f72 746c 6962 2e69 6d70 6f72   importlib.impor
+00022020: 745f 6d6f 6475 6c65 2e0a 2020 2020 2020  t_module..      
+00022030: 4966 2069 7420 6c6f 6f6b 7320 6c69 6b65  If it looks like
+00022040: 2061 2066 696c 656e 616d 652c 2073 6561   a filename, sea
+00022050: 7263 6820 666f 7220 6120 6261 7365 2070  rch for a base p
+00022060: 6174 6820 2877 6869 6368 2064 6f65 7320  ath (which does 
+00022070: 6e6f 7420 6861 7665 205f 5f69 6e69 745f  not have __init_
+00022080: 5f2e 7079 292c 0a20 2020 2020 2061 6464  _.py),.      add
+00022090: 2074 6861 7420 7061 7468 2074 6f20 7379   that path to sy
+000220a0: 732e 7061 7468 2069 6620 6e65 6564 6564  s.path if needed
+000220b0: 2c20 616e 6420 696d 706f 7274 2074 6865  , and import the
+000220c0: 2072 656d 6169 6e69 6e67 2077 6865 7265   remaining where
+000220d0: 2022 2f22 2069 7320 7265 706c 6163 6564   "/" is replaced
+000220e0: 2062 7920 222e 220a 2020 2020 2020 616e   by ".".      an
+000220f0: 6420 7468 6520 6669 6c65 2065 7874 656e  d the file exten
+00022100: 7369 6f6e 2069 7320 7265 6d6f 7665 642e  sion is removed.
+00022110: 0a20 2020 203a 7265 7475 726e 3a20 7468  .    :return: th
+00022120: 6520 6d6f 6475 6c65 0a20 2020 203a 7274  e module.    :rt
+00022130: 7970 653a 2074 7970 6573 2e4d 6f64 756c  ype: types.Modul
+00022140: 6554 7970 650a 2020 2020 2222 220a 2020  eType.    """.  
+00022150: 2020 6173 7365 7274 2066 696c 656e 616d    assert filenam
+00022160: 650a 2020 2020 696d 706f 7274 2069 6d70  e.    import imp
+00022170: 6f72 746c 6962 0a0a 2020 2020 6966 2022  ortlib..    if "
+00022180: 2f22 206e 6f74 2069 6e20 6669 6c65 6e61  /" not in filena
+00022190: 6d65 3a0a 2020 2020 2020 2020 7265 7475  me:.        retu
+000221a0: 726e 2069 6d70 6f72 746c 6962 2e69 6d70  rn importlib.imp
+000221b0: 6f72 745f 6d6f 6475 6c65 2866 696c 656e  ort_module(filen
+000221c0: 616d 6529 0a20 2020 2070 7265 6669 785f  ame).    prefix_
+000221d0: 6469 7220 3d20 2222 0a20 2020 2069 6620  dir = "".    if 
+000221e0: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
+000221f0: 7473 2866 696c 656e 616d 6529 3a0a 2020  ts(filename):.  
+00022200: 2020 2020 2020 6173 7365 7274 2066 696c        assert fil
+00022210: 656e 616d 655b 305d 2021 3d20 222f 220a  ename[0] != "/".
+00022220: 2020 2020 2020 2020 2320 4d61 7962 6520          # Maybe 
+00022230: 7265 6c61 7469 7665 2074 6f20 5265 7475  relative to Retu
+00022240: 726e 6e3f 0a20 2020 2020 2020 2070 7265  rnn?.        pre
+00022250: 6669 785f 6469 7220 3d20 2225 732f 2220  fix_dir = "%s/" 
+00022260: 2520 7265 7475 726e 6e5f 726f 6f74 5f64  % returnn_root_d
+00022270: 6972 0a20 2020 2061 7373 6572 7420 6f73  ir.    assert os
+00022280: 2e70 6174 682e 6578 6973 7473 2870 7265  .path.exists(pre
+00022290: 6669 785f 6469 7220 2b20 6669 6c65 6e61  fix_dir + filena
+000222a0: 6d65 290a 2020 2020 6173 7365 7274 2066  me).    assert f
+000222b0: 696c 656e 616d 652e 656e 6473 7769 7468  ilename.endswith
+000222c0: 2822 2e70 7922 2920 6f72 206f 732e 7061  (".py") or os.pa
+000222d0: 7468 2e69 7364 6972 2870 7265 6669 785f  th.isdir(prefix_
+000222e0: 6469 7220 2b20 6669 6c65 6e61 6d65 290a  dir + filename).
+000222f0: 2020 2020 6469 7273 203d 2066 696c 656e      dirs = filen
+00022300: 616d 652e 7370 6c69 7428 222f 2229 0a20  ame.split("/"). 
+00022310: 2020 2064 6972 732c 2062 6173 655f 666e     dirs, base_fn
+00022320: 203d 2064 6972 735b 3a2d 315d 2c20 6469   = dirs[:-1], di
+00022330: 7273 5b2d 315d 0a20 2020 2061 7373 6572  rs[-1].    asser
+00022340: 7420 6c65 6e28 6469 7273 2920 3e3d 2031  t len(dirs) >= 1
+00022350: 0a20 2020 2066 6f72 2069 2069 6e20 7265  .    for i in re
+00022360: 7665 7273 6564 2872 616e 6765 286c 656e  versed(range(len
+00022370: 2864 6972 7329 2929 3a0a 2020 2020 2020  (dirs))):.      
+00022380: 2020 6420 3d20 7072 6566 6978 5f64 6972    d = prefix_dir
+00022390: 202b 2022 2f22 2e6a 6f69 6e28 6469 7273   + "/".join(dirs
+000223a0: 5b3a 2069 202b 2031 5d29 0a20 2020 2020  [: i + 1]).     
+000223b0: 2020 2061 7373 6572 7420 6f73 2e70 6174     assert os.pat
+000223c0: 682e 6973 6469 7228 6429 0a20 2020 2020  h.isdir(d).     
+000223d0: 2020 2069 6620 6f73 2e70 6174 682e 6578     if os.path.ex
+000223e0: 6973 7473 2822 2573 2f5f 5f69 6e69 745f  ists("%s/__init_
+000223f0: 5f2e 7079 2220 2520 6429 3a0a 2020 2020  _.py" % d):.    
+00022400: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00022410: 0a20 2020 2020 2020 2069 6620 6420 6e6f  .        if d no
+00022420: 7420 696e 2073 7973 2e70 6174 683a 0a20  t in sys.path:. 
+00022430: 2020 2020 2020 2020 2020 2073 7973 2e70             sys.p
+00022440: 6174 682e 6170 7065 6e64 2864 290a 2020  ath.append(d).  
+00022450: 2020 2020 2020 6d20 3d20 222e 222e 6a6f        m = ".".jo
+00022460: 696e 2864 6972 735b 6920 2b20 3120 3a5d  in(dirs[i + 1 :]
+00022470: 202b 205b 6261 7365 5f66 6e5d 290a 2020   + [base_fn]).  
+00022480: 2020 2020 2020 6966 2062 6173 655f 666e        if base_fn
+00022490: 2e65 6e64 7377 6974 6828 222e 7079 2229  .endswith(".py")
+000224a0: 3a0a 2020 2020 2020 2020 2020 2020 6d20  :.            m 
+000224b0: 3d20 6d5b 3a2d 335d 0a20 2020 2020 2020  = m[:-3].       
+000224c0: 2072 6574 7572 6e20 696d 706f 7274 6c69   return importli
+000224d0: 622e 696d 706f 7274 5f6d 6f64 756c 6528  b.import_module(
+000224e0: 6d29 0a20 2020 2072 6169 7365 2056 616c  m).    raise Val
+000224f0: 7565 4572 726f 7228 2263 616e 6e6f 7420  ueError("cannot 
+00022500: 6669 6775 7265 206f 7574 2062 6173 6520  figure out base 
+00022510: 6d6f 6475 6c65 2070 6174 6820 6672 6f6d  module path from
+00022520: 2025 7222 2025 2066 696c 656e 616d 6529   %r" % filename)
+00022530: 0a0a 0a64 6566 2073 6f66 746d 6178 2878  ...def softmax(x
+00022540: 2c20 6178 6973 3d4e 6f6e 6529 3a0a 2020  , axis=None):.  
+00022550: 2020 2222 220a 2020 2020 3a70 6172 616d    """.    :param
+00022560: 206e 756d 7079 2e6e 6461 7272 6179 2078   numpy.ndarray x
+00022570: 3a0a 2020 2020 3a70 6172 616d 2069 6e74  :.    :param int
+00022580: 7c4e 6f6e 6520 6178 6973 3a0a 2020 2020  |None axis:.    
+00022590: 3a72 7479 7065 3a20 6e75 6d70 792e 6e64  :rtype: numpy.nd
+000225a0: 6172 7261 790a 2020 2020 2222 220a 2020  array.    """.  
+000225b0: 2020 696d 706f 7274 206e 756d 7079 0a0a    import numpy..
+000225c0: 2020 2020 655f 7820 3d20 6e75 6d70 792e      e_x = numpy.
+000225d0: 6578 7028 7820 2d20 6e75 6d70 792e 6d61  exp(x - numpy.ma
+000225e0: 7828 782c 2061 7869 733d 6178 6973 2c20  x(x, axis=axis, 
+000225f0: 6b65 6570 6469 6d73 3d54 7275 6529 290a  keepdims=True)).
+00022600: 2020 2020 7265 7475 726e 2065 5f78 202f      return e_x /
+00022610: 206e 756d 7079 2e73 756d 2865 5f78 2c20   numpy.sum(e_x, 
+00022620: 6178 6973 3d61 7869 732c 206b 6565 7064  axis=axis, keepd
+00022630: 696d 733d 5472 7565 290a 0a0a 6465 6620  ims=True)...def 
+00022640: 636f 6c6c 6563 745f 7072 6f63 5f6d 6170  collect_proc_map
+00022650: 735f 6578 6563 5f66 696c 6573 2829 3a0a  s_exec_files():.
+00022660: 2020 2020 2222 220a 2020 2020 4375 7272      """.    Curr
+00022670: 656e 746c 7920 6f6e 6c79 2077 6f72 6b73  ently only works
+00022680: 206f 6e20 4c69 6e75 782e 2e2e 0a0a 2020   on Linux.....  
+00022690: 2020 3a72 6574 7572 6e3a 206c 6973 7420    :return: list 
+000226a0: 6f66 206d 6170 7065 6420 6578 6563 7574  of mapped execut
+000226b0: 6162 6c65 7320 286c 6962 7329 0a20 2020  ables (libs).   
+000226c0: 203a 7274 7970 653a 206c 6973 745b 7374   :rtype: list[st
+000226d0: 725d 0a20 2020 2022 2222 0a20 2020 2069  r].    """.    i
+000226e0: 6d70 6f72 7420 7265 0a0a 2020 2020 7069  mport re..    pi
+000226f0: 6420 3d20 6f73 2e67 6574 7069 6428 290a  d = os.getpid().
+00022700: 2020 2020 666e 7320 3d20 5b5d 0a20 2020      fns = [].   
+00022710: 2066 6f72 206c 696e 6520 696e 206f 7065   for line in ope
+00022720: 6e28 222f 7072 6f63 2f25 692f 6d61 7073  n("/proc/%i/maps
+00022730: 2220 2520 7069 642c 2022 7222 292e 7265  " % pid, "r").re
+00022740: 6164 2829 2e73 706c 6974 6c69 6e65 7328  ad().splitlines(
+00022750: 293a 2020 2320 666f 7220 6561 6368 206d  ):  # for each m
+00022760: 6170 7065 6420 7265 6769 6f6e 0a20 2020  apped region.   
+00022770: 2020 2020 2023 2068 7474 7073 3a2f 2f73       # https://s
+00022780: 7461 636b 6f76 6572 666c 6f77 2e63 6f6d  tackoverflow.com
+00022790: 2f71 7565 7374 696f 6e73 2f31 3430 3133  /questions/14013
+000227a0: 3539 2f75 6e64 6572 7374 616e 6469 6e67  59/understanding
+000227b0: 2d6c 696e 7578 2d70 726f 632d 6964 2d6d  -linux-proc-id-m
+000227c0: 6170 730a 2020 2020 2020 2020 2320 6164  aps.        # ad
+000227d0: 6472 6573 7320 2020 2020 2020 2020 2020  dress           
+000227e0: 7065 726d 7320 6f66 6673 6574 2020 6465  perms offset  de
+000227f0: 7620 2020 696e 6f64 6520 2020 7061 7468  v   inode   path
+00022800: 6e61 6d65 0a20 2020 2020 2020 2023 2045  name.        # E
+00022810: 2e67 2e3a 0a20 2020 2020 2020 2023 2037  .g.:.        # 7
+00022820: 6666 3264 6539 3163 3030 302d 3766 6632  ff2de91c000-7ff2
+00022830: 6465 3931 6530 3030 2072 772d 7020 3030  de91e000 rw-p 00
+00022840: 3137 6330 3030 2030 383a 3032 2037 3934  17c000 08:02 794
+00022850: 3834 3420 2020 2020 2020 2020 2020 2020  844             
+00022860: 2020 2020 2020 2020 2f75 7372 2f6c 6962          /usr/lib
+00022870: 2f78 3836 5f36 342d 6c69 6e75 782d 676e  /x86_64-linux-gn
+00022880: 752f 6c69 6273 7464 632b 2e2e 2e0a 2020  u/libstdc+....  
+00022890: 2020 2020 2020 6d20 3d20 7265 2e6d 6174        m = re.mat
+000228a0: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
+000228b0: 7222 5e28 5b30 2d39 412d 4661 2d66 5d2b  r"^([0-9A-Fa-f]+
+000228c0: 292d 285b 302d 3941 2d46 612d 665d 2b29  )-([0-9A-Fa-f]+)
+000228d0: 5c73 2b28 5b72 7778 7073 5c2d 5d2b 295c  \s+([rwxps\-]+)\
+000228e0: 732b 285b 302d 3941 2d46 612d 665d 2b29  s+([0-9A-Fa-f]+)
+000228f0: 5c73 2b28 5b30 2d39 412d 4661 2d66 3a5d  \s+([0-9A-Fa-f:]
+00022900: 2b29 5c73 2b28 5b30 2d39 5d2b 295c 732a  +)\s+([0-9]+)\s*
+00022910: 282e 2a29 2422 2c20 6c69 6e65 0a20 2020  (.*)$", line.   
+00022920: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
+00022930: 7373 6572 7420 6d2c 2022 6e6f 206d 6174  ssert m, "no mat
+00022940: 6368 2066 6f72 2025 7222 2025 206c 696e  ch for %r" % lin
+00022950: 650a 2020 2020 2020 2020 6164 6472 6573  e.        addres
+00022960: 735f 7374 6172 742c 2061 6464 7265 7373  s_start, address
+00022970: 5f65 6e64 2c20 7065 726d 732c 206f 6666  _end, perms, off
+00022980: 7365 742c 2064 6576 2c20 695f 6e6f 6465  set, dev, i_node
+00022990: 2c20 7061 7468 5f6e 616d 6520 3d20 6d2e  , path_name = m.
+000229a0: 6772 6f75 7073 2829 0a20 2020 2020 2020  groups().       
+000229b0: 2069 6620 2278 2220 6e6f 7420 696e 2070   if "x" not in p
+000229c0: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
+000229d0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+000229e0: 2020 2069 6620 6e6f 7420 7061 7468 5f6e     if not path_n
+000229f0: 616d 6520 6f72 2070 6174 685f 6e61 6d65  ame or path_name
+00022a00: 2e73 7461 7274 7377 6974 6828 225b 2229  .startswith("[")
+00022a10: 206f 7220 2228 6465 6c65 7465 6429 2220   or "(deleted)" 
+00022a20: 696e 2070 6174 685f 6e61 6d65 3a0a 2020  in path_name:.  
+00022a30: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00022a40: 7565 0a20 2020 2020 2020 2069 6620 7061  ue.        if pa
+00022a50: 7468 5f6e 616d 6520 6e6f 7420 696e 2066  th_name not in f
+00022a60: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00022a70: 666e 732e 6170 7065 6e64 2870 6174 685f  fns.append(path_
+00022a80: 6e61 6d65 290a 2020 2020 7265 7475 726e  name).    return
+00022a90: 2066 6e73 0a0a 0a64 6566 2066 696e 645f   fns...def find_
+00022aa0: 7379 6d5f 696e 5f65 7865 6328 666e 2c20  sym_in_exec(fn, 
+00022ab0: 7379 6d29 3a0a 2020 2020 2222 220a 2020  sym):.    """.  
+00022ac0: 2020 5573 6573 2060 606f 626a 6475 6d70    Uses ``objdump
+00022ad0: 6060 2074 6f20 6c69 7374 2061 7661 696c  `` to list avail
+00022ae0: 6162 6c65 2073 796d 626f 6c73 2c20 616e  able symbols, an
+00022af0: 6420 6669 6c74 6572 7320 7468 656d 2062  d filters them b
+00022b00: 7920 7468 6520 6769 7665 6e20 6060 7379  y the given ``sy
+00022b10: 6d60 602e 0a0a 2020 2020 3a70 6172 616d  m``...    :param
+00022b20: 2073 7472 2066 6e3a 2070 6174 680a 2020   str fn: path.  
+00022b30: 2020 3a70 6172 616d 2073 7472 2073 796d    :param str sym
+00022b40: 3a0a 2020 2020 3a72 6574 7572 6e3a 206d  :.    :return: m
+00022b50: 6174 6368 6564 206f 7574 2c20 6f72 204e  atched out, or N
+00022b60: 6f6e 650a 2020 2020 3a72 7479 7065 3a20  one.    :rtype: 
+00022b70: 7374 727c 4e6f 6e65 0a20 2020 2022 2222  str|None.    """
+00022b80: 0a20 2020 2066 726f 6d20 7375 6270 726f  .    from subpro
+00022b90: 6365 7373 2069 6d70 6f72 7420 4361 6c6c  cess import Call
+00022ba0: 6564 5072 6f63 6573 7345 7272 6f72 0a0a  edProcessError..
+00022bb0: 2020 2020 6f62 6a64 756d 7020 3d20 226f      objdump = "o
+00022bc0: 626a 6475 6d70 202d 5422 0a20 2020 2069  bjdump -T".    i
+00022bd0: 6620 7379 732e 706c 6174 666f 726d 203d  f sys.platform =
+00022be0: 3d20 2264 6172 7769 6e22 3a0a 2020 2020  = "darwin":.    
+00022bf0: 2020 2020 6f62 6a64 756d 7020 3d20 226f      objdump = "o
+00022c00: 746f 6f6c 202d 4948 4776 220a 2020 2020  tool -IHGv".    
+00022c10: 7368 656c 6c5f 636d 6420 3d20 2225 7320  shell_cmd = "%s 
+00022c20: 2573 207c 2067 7265 7020 2573 2220 2520  %s | grep %s" % 
+00022c30: 286f 626a 6475 6d70 2c20 666e 2c20 7379  (objdump, fn, sy
+00022c40: 6d29 0a20 2020 2074 7279 3a0a 2020 2020  m).    try:.    
+00022c50: 2020 2020 6f75 7420 3d20 7379 735f 6578      out = sys_ex
+00022c60: 6563 5f6f 7574 2873 6865 6c6c 5f63 6d64  ec_out(shell_cmd
+00022c70: 2c20 7368 656c 6c3d 5472 7565 290a 2020  , shell=True).  
+00022c80: 2020 6578 6365 7074 2043 616c 6c65 6450    except CalledP
+00022c90: 726f 6365 7373 4572 726f 723a 2020 2320  rocessError:  # 
+00022ca0: 6e6f 6e65 2066 6f75 6e64 0a20 2020 2020  none found.     
+00022cb0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00022cc0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+00022cd0: 616e 6365 286f 7574 2c20 2873 7472 2c20  ance(out, (str, 
+00022ce0: 756e 6963 6f64 6529 290a 2020 2020 6f75  unicode)).    ou
+00022cf0: 745f 6c6e 7320 3d20 6f75 742e 7370 6c69  t_lns = out.spli
+00022d00: 746c 696e 6573 2829 0a20 2020 206f 7574  tlines().    out
+00022d10: 5f6c 6e73 203d 205b 6c6e 2066 6f72 206c  _lns = [ln for l
+00022d20: 6e20 696e 206f 7574 5f6c 6e73 2069 6620  n in out_lns if 
+00022d30: 222e 7465 7874 2220 696e 206c 6e5d 2020  ".text" in ln]  
+00022d40: 2320 7365 6520 6f62 6a64 756d 700a 2020  # see objdump.  
+00022d50: 2020 6f75 745f 6c6e 7320 3d20 5b6c 6e20    out_lns = [ln 
+00022d60: 666f 7220 6c6e 2069 6e20 6f75 745f 6c6e  for ln in out_ln
+00022d70: 7320 6966 2073 796d 2069 6e20 6c6e 2e73  s if sym in ln.s
+00022d80: 706c 6974 2829 5d0a 2020 2020 6966 206e  plit()].    if n
+00022d90: 6f74 206f 7574 5f6c 6e73 3a0a 2020 2020  ot out_lns:.    
+00022da0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00022db0: 2020 2020 7265 7475 726e 2022 466f 756e      return "Foun
+00022dc0: 6420 2572 2069 6e20 2572 3a5c 6e25 7322  d %r in %r:\n%s"
+00022dd0: 2025 2028 7379 6d2c 2066 6e2c 2022 5c6e   % (sym, fn, "\n
+00022de0: 222e 6a6f 696e 286f 7574 5f6c 6e73 2929  ".join(out_lns))
+00022df0: 0a0a 0a64 6566 2064 756d 6d79 5f6e 756d  ...def dummy_num
+00022e00: 7079 5f67 656d 6d5f 6361 6c6c 2829 3a0a  py_gemm_call():.
+00022e10: 2020 2020 2222 220a 2020 2020 4a75 7374      """.    Just
+00022e20: 2070 6572 666f 726d 7320 736f 6d65 2047   performs some G
+00022e30: 454d 4d20 6361 6c6c 2076 6961 204e 756d  EMM call via Num
+00022e40: 7079 2e0a 2020 2020 5468 6973 206d 616b  py..    This mak
+00022e50: 6573 2073 7572 6520 7468 6174 2074 6865  es sure that the
+00022e60: 2042 4c41 5320 6c69 6272 6172 7920 6973   BLAS library is
+00022e70: 206c 6f61 6465 642e 0a20 2020 2022 2222   loaded..    """
+00022e80: 0a20 2020 2069 6d70 6f72 7420 6e75 6d70  .    import nump
+00022e90: 790a 0a20 2020 2061 203d 206e 756d 7079  y..    a = numpy
+00022ea0: 2e72 616e 646f 6d2e 7261 6e64 6e28 352c  .random.randn(5,
+00022eb0: 2033 292e 6173 7479 7065 286e 756d 7079   3).astype(numpy
+00022ec0: 2e66 6c6f 6174 3332 290a 2020 2020 6220  .float32).    b 
+00022ed0: 3d20 6e75 6d70 792e 7261 6e64 6f6d 2e72  = numpy.random.r
+00022ee0: 616e 646e 2833 2c20 3729 2e61 7374 7970  andn(3, 7).astyp
+00022ef0: 6528 6e75 6d70 792e 666c 6f61 7433 3229  e(numpy.float32)
+00022f00: 0a20 2020 2063 203d 206e 756d 7079 2e64  .    c = numpy.d
+00022f10: 6f74 2861 2c20 6229 0a20 2020 2061 7373  ot(a, b).    ass
+00022f20: 6572 7420 6e75 6d70 792e 6973 6669 6e69  ert numpy.isfini
+00022f30: 7465 2863 292e 616c 6c28 290a 0a0a 5f66  te(c).all()..._f
+00022f40: 696e 645f 7367 656d 6d5f 6c69 625f 6672  ind_sgemm_lib_fr
+00022f50: 6f6d 5f72 756e 7469 6d65 5f63 6163 6865  om_runtime_cache
+00022f60: 6420 3d20 4e6f 6e65 0a0a 0a64 6566 2066  d = None...def f
+00022f70: 696e 645f 7367 656d 6d5f 6c69 6273 5f66  ind_sgemm_libs_f
+00022f80: 726f 6d5f 7275 6e74 696d 6528 293a 0a20  rom_runtime():. 
+00022f90: 2020 2022 2222 0a20 2020 204c 6f6f 6b73     """.    Looks
+00022fa0: 2074 6872 6f75 6768 2061 6c6c 206c 6962   through all lib
+00022fb0: 7320 7669 6120 3a66 756e 633a 6063 6f6c  s via :func:`col
+00022fc0: 6c65 6374 5f70 726f 635f 6d61 7073 5f65  lect_proc_maps_e
+00022fd0: 7865 635f 6669 6c65 7360 2c0a 2020 2020  xec_files`,.    
+00022fe0: 616e 6420 7365 6172 6368 6573 2066 6f72  and searches for
+00022ff0: 2061 6c6c 2077 6869 6368 2068 6176 6520   all which have 
+00023000: 7468 6520 6060 7367 656d 6d60 6020 7379  the ``sgemm`` sy
+00023010: 6d62 6f6c 2e0a 2020 2020 4375 7272 656e  mbol..    Curren
+00023020: 746c 7920 6f6e 6c79 2077 6f72 6b73 206f  tly only works o
+00023030: 6e20 4c69 6e75 7820 2862 6563 6175 7365  n Linux (because
+00023040: 2063 6f6c 6c65 6374 5f70 726f 635f 6d61   collect_proc_ma
+00023050: 7073 5f65 7865 635f 6669 6c65 7329 2e0a  ps_exec_files)..
+00023060: 0a20 2020 203a 7265 7475 726e 3a20 6c69  .    :return: li
+00023070: 7374 206f 6620 6c69 6273 2028 7468 6569  st of libs (thei
+00023080: 7220 7061 7468 290a 2020 2020 3a72 7479  r path).    :rty
+00023090: 7065 3a20 6c69 7374 5b73 7472 5d0a 2020  pe: list[str].  
+000230a0: 2020 2222 220a 2020 2020 6966 206e 6f74    """.    if not
+000230b0: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+000230c0: 222f 7072 6f63 2229 3a0a 2020 2020 2020  "/proc"):.      
+000230d0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+000230e0: 2020 676c 6f62 616c 205f 6669 6e64 5f73    global _find_s
+000230f0: 6765 6d6d 5f6c 6962 5f66 726f 6d5f 7275  gemm_lib_from_ru
+00023100: 6e74 696d 655f 6361 6368 6564 0a20 2020  ntime_cached.   
+00023110: 2069 6620 5f66 696e 645f 7367 656d 6d5f   if _find_sgemm_
+00023120: 6c69 625f 6672 6f6d 5f72 756e 7469 6d65  lib_from_runtime
+00023130: 5f63 6163 6865 6420 6973 206e 6f74 204e  _cached is not N
+00023140: 6f6e 653a 0a20 2020 2020 2020 2072 6574  one:.        ret
+00023150: 7572 6e20 5f66 696e 645f 7367 656d 6d5f  urn _find_sgemm_
+00023160: 6c69 625f 6672 6f6d 5f72 756e 7469 6d65  lib_from_runtime
+00023170: 5f63 6163 6865 640a 2020 2020 6475 6d6d  _cached.    dumm
+00023180: 795f 6e75 6d70 795f 6765 6d6d 5f63 616c  y_numpy_gemm_cal
+00023190: 6c28 2920 2023 206d 616b 6520 7375 7265  l()  # make sure
+000231a0: 2074 6861 7420 4e75 6d70 7920 6973 206c   that Numpy is l
+000231b0: 6f61 6465 6420 616e 6420 4e75 6d70 7920  oaded and Numpy 
+000231c0: 7367 656d 6d20 6973 2061 7661 696c 6162  sgemm is availab
+000231d0: 6c65 0a20 2020 2066 6e73 203d 2063 6f6c  le.    fns = col
+000231e0: 6c65 6374 5f70 726f 635f 6d61 7073 5f65  lect_proc_maps_e
+000231f0: 7865 635f 6669 6c65 7328 290a 2020 2020  xec_files().    
+00023200: 666e 735f 7769 7468 5f73 6765 6d6d 203d  fns_with_sgemm =
+00023210: 205b 5d0a 2020 2020 666f 7220 666e 2069   [].    for fn i
+00023220: 6e20 666e 733a 0a20 2020 2020 2020 206f  n fns:.        o
+00023230: 7574 203d 2066 696e 645f 7379 6d5f 696e  ut = find_sym_in
+00023240: 5f65 7865 6328 666e 2c20 2273 6765 6d6d  _exec(fn, "sgemm
+00023250: 5f22 290a 2020 2020 2020 2020 6966 206f  _").        if o
+00023260: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
+00023270: 666e 735f 7769 7468 5f73 6765 6d6d 2e61  fns_with_sgemm.a
+00023280: 7070 656e 6428 666e 290a 2020 2020 5f66  ppend(fn).    _f
+00023290: 696e 645f 7367 656d 6d5f 6c69 625f 6672  ind_sgemm_lib_fr
+000232a0: 6f6d 5f72 756e 7469 6d65 5f63 6163 6865  om_runtime_cache
+000232b0: 6420 3d20 666e 735f 7769 7468 5f73 6765  d = fns_with_sge
+000232c0: 6d6d 0a20 2020 2072 6574 7572 6e20 666e  mm.    return fn
+000232d0: 735f 7769 7468 5f73 6765 6d6d 0a0a 0a5f  s_with_sgemm..._
+000232e0: 6669 6e64 5f6c 6962 6375 6461 7274 5f66  find_libcudart_f
+000232f0: 726f 6d5f 7275 6e74 696d 655f 6361 6368  rom_runtime_cach
+00023300: 6564 203d 204e 6f6e 650a 0a0a 6465 6620  ed = None...def 
+00023310: 6669 6e64 5f6c 6962 6375 6461 7274 5f66  find_libcudart_f
+00023320: 726f 6d5f 7275 6e74 696d 6528 293a 0a20  rom_runtime():. 
+00023330: 2020 2022 2222 0a20 2020 204c 6f6f 6b73     """.    Looks
+00023340: 2074 6872 6f75 6768 2061 6c6c 206c 6962   through all lib
+00023350: 7320 7669 6120 3a66 756e 633a 6063 6f6c  s via :func:`col
+00023360: 6c65 6374 5f70 726f 635f 6d61 7073 5f65  lect_proc_maps_e
+00023370: 7865 635f 6669 6c65 7360 2c0a 2020 2020  xec_files`,.    
+00023380: 616e 6420 7365 6172 6368 6573 2066 6f72  and searches for
+00023390: 2061 6c6c 2077 6869 6368 2068 6176 6520   all which have 
+000233a0: 7468 6520 6060 7367 656d 6d60 6020 7379  the ``sgemm`` sy
+000233b0: 6d62 6f6c 2e0a 2020 2020 4375 7272 656e  mbol..    Curren
+000233c0: 746c 7920 6f6e 6c79 2077 6f72 6b73 206f  tly only works o
+000233d0: 6e20 4c69 6e75 7820 2862 6563 6175 7365  n Linux (because
+000233e0: 2063 6f6c 6c65 6374 5f70 726f 635f 6d61   collect_proc_ma
+000233f0: 7073 5f65 7865 635f 6669 6c65 7329 2e0a  ps_exec_files)..
+00023400: 0a20 2020 203a 7265 7475 726e 3a20 6c69  .    :return: li
+00023410: 7374 206f 6620 6c69 6273 2028 7468 6569  st of libs (thei
+00023420: 7220 7061 7468 290a 2020 2020 3a72 7479  r path).    :rty
+00023430: 7065 3a20 7374 727c 4e6f 6e65 0a20 2020  pe: str|None.   
+00023440: 2022 2222 0a20 2020 2069 6620 6e6f 7420   """.    if not 
+00023450: 6f73 2e70 6174 682e 6578 6973 7473 2822  os.path.exists("
+00023460: 2f70 726f 6322 293a 0a20 2020 2020 2020  /proc"):.       
+00023470: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+00023480: 2067 6c6f 6261 6c20 5f66 696e 645f 6c69   global _find_li
+00023490: 6263 7564 6172 745f 6672 6f6d 5f72 756e  bcudart_from_run
+000234a0: 7469 6d65 5f63 6163 6865 640a 2020 2020  time_cached.    
+000234b0: 6966 205f 6669 6e64 5f6c 6962 6375 6461  if _find_libcuda
+000234c0: 7274 5f66 726f 6d5f 7275 6e74 696d 655f  rt_from_runtime_
+000234d0: 6361 6368 6564 2069 7320 6e6f 7420 4e6f  cached is not No
+000234e0: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
+000234f0: 726e 205f 6669 6e64 5f6c 6962 6375 6461  rn _find_libcuda
+00023500: 7274 5f66 726f 6d5f 7275 6e74 696d 655f  rt_from_runtime_
+00023510: 6361 6368 6564 5b30 5d0a 2020 2020 666e  cached[0].    fn
+00023520: 7320 3d20 636f 6c6c 6563 745f 7072 6f63  s = collect_proc
+00023530: 5f6d 6170 735f 6578 6563 5f66 696c 6573  _maps_exec_files
+00023540: 2829 0a20 2020 2066 6f72 2066 6e20 696e  ().    for fn in
+00023550: 2066 6e73 3a0a 2020 2020 2020 2020 6966   fns:.        if
+00023560: 2072 652e 6d61 7463 6828 222e 2a2f 6c69   re.match(".*/li
+00023570: 6263 7564 6172 745c 5c2e 736f 285c 5c2e  bcudart\\.so(\\.
+00023580: 2e2a 293f 222c 2066 6e29 3a0a 2020 2020  .*)?", fn):.    
+00023590: 2020 2020 2020 2020 5f66 696e 645f 6c69          _find_li
+000235a0: 6263 7564 6172 745f 6672 6f6d 5f72 756e  bcudart_from_run
+000235b0: 7469 6d65 5f63 6163 6865 6420 3d20 5b66  time_cached = [f
+000235c0: 6e5d 0a20 2020 2020 2020 2020 2020 2072  n].            r
+000235d0: 6574 7572 6e20 666e 0a20 2020 205f 6669  eturn fn.    _fi
+000235e0: 6e64 5f6c 6962 6375 6461 7274 5f66 726f  nd_libcudart_fro
+000235f0: 6d5f 7275 6e74 696d 655f 6361 6368 6564  m_runtime_cached
+00023600: 203d 205b 4e6f 6e65 5d0a 2020 2020 7265   = [None].    re
+00023610: 7475 726e 204e 6f6e 650a                 turn None.
```

### Comparing `returnn-1.20230413.93323/returnn/util/better_exchook.py` & `returnn-1.20230414.110554/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/bpe.py` & `returnn-1.20230414.110554/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/debug.py` & `returnn-1.20230414.110554/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/debug_helpers.py` & `returnn-1.20230414.110554/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/fsa.py` & `returnn-1.20230414.110554/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230414.110554/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/pprint.py` & `returnn-1.20230414.110554/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/py-to-pickle.cpp` & `returnn-1.20230414.110554/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/sig_proc.py` & `returnn-1.20230414.110554/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn/util/task_system.py` & `returnn-1.20230414.110554/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/returnn.egg-info/PKG-INFO` & `returnn-1.20230414.110554/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230413.93323
+Version: 1.20230414.110554
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230413.93323/returnn.egg-info/SOURCES.txt` & `returnn-1.20230414.110554/returnn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -151,25 +151,29 @@
 returnn/extern/graph_editor/transform.py
 returnn/extern/graph_editor/util.py
 returnn/frontend/__init__.py
 returnn/frontend/_backend.py
 returnn/frontend/_numpy_backend.py
 returnn/frontend/_utils.py
 returnn/frontend/array_.py
+returnn/frontend/attention.py
 returnn/frontend/cond.py
 returnn/frontend/const.py
+returnn/frontend/container.py
 returnn/frontend/dims.py
 returnn/frontend/dropout.py
 returnn/frontend/dtype.py
+returnn/frontend/gradient.py
 returnn/frontend/init.py
 returnn/frontend/linear.py
 returnn/frontend/loss.py
 returnn/frontend/math_.py
 returnn/frontend/matmul.py
 returnn/frontend/module.py
+returnn/frontend/normalization.py
 returnn/frontend/parameter.py
 returnn/frontend/rand.py
 returnn/frontend/reduce.py
 returnn/frontend/run_ctx.py
 returnn/frontend/state.py
 returnn/frontend/types.py
 returnn/import_/__init__.py
@@ -294,15 +298,18 @@
 tests/test_TaskSystem.py
 tests/test_TaskSystem_SharedMem.py
 tests/test_TranslationDataset.py
 tests/test_Util.py
 tests/test_demos.py
 tests/test_fork_exec.py
 tests/test_hdf_dump.py
+tests/test_rf_array.py
+tests/test_rf_attention.py
 tests/test_rf_base.py
+tests/test_rf_container.py
 tests/test_tensor.py
 tests/test_tools.py
 tests/test_torch_frontend.py
 tests/test_torch_internal_frontend.py
 tests/PyCharm.idea/.gitignore
 tests/PyCharm.idea/.name
 tests/PyCharm.idea/codeStyleSettings.xml
```

### Comparing `returnn-1.20230413.93323/setup.py` & `returnn-1.20230414.110554/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/DummySprintExec.py` & `returnn-1.20230414.110554/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230414.110554/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230414.110554/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230414.110554/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/_set_num_threads1.py` & `returnn-1.20230414.110554/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/_setup_test_env.py` & `returnn-1.20230414.110554/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/bpe-unicode-demo.codes` & `returnn-1.20230414.110554/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/bpe-unicode-demo.vocab` & `returnn-1.20230414.110554/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/lexicon_opt.isyms` & `returnn-1.20230414.110554/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/lexicon_opt.jpg` & `returnn-1.20230414.110554/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/lint_common.py` & `returnn-1.20230414.110554/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/pycharm-inspect.py` & `returnn-1.20230414.110554/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/pylint.py` & `returnn-1.20230414.110554/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/returnn-as-framework.py` & `returnn-1.20230414.110554/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/rf_utils.py` & `returnn-1.20230414.110554/tests/rf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     for k, v_pt in out_pt.data.items():
         v_tf = out_tf[k]
         # We cannot really check the dims directly for equality,
         # because the model code often creates new dims, which are different in each call.
         # However, via mark_as_output, the order of dims is well-defined.
         # So we can check the values.
         assert len(v_pt.dims) == len(v_tf.dims)
+        assert v_pt.feature_dim_axis == v_tf.feature_dim_axis
         for d_pt, d_tf in zip(v_pt.dims, v_tf.dims):
             assert isinstance(d_pt, Dim) and isinstance(d_tf, Dim)
             assert _dim_is_scalar_size(d_pt) == _dim_is_scalar_size(d_tf)
             if _dim_is_scalar_size(d_pt):
                 assert _dim_scalar_size(d_pt) == _dim_scalar_size(d_tf)
             else:
                 assert d_pt.dyn_size_ext and d_tf.dyn_size_ext
```

### Comparing `returnn-1.20230413.93323/tests/spelling.dic` & `returnn-1.20230414.110554/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_Config.py` & `returnn-1.20230414.110554/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_Dataset.py` & `returnn-1.20230414.110554/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_Fsa.py` & `returnn-1.20230414.110554/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_GeneratingDataset.py` & `returnn-1.20230414.110554/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_HDFDataset.py` & `returnn-1.20230414.110554/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_LearningRateControl.py` & `returnn-1.20230414.110554/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_Log.py` & `returnn-1.20230414.110554/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_MultiProcDataset.py` & `returnn-1.20230414.110554/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_PTDataset.py` & `returnn-1.20230414.110554/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_Pretrain.py` & `returnn-1.20230414.110554/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_ResNet.py` & `returnn-1.20230414.110554/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_SprintDataset.py` & `returnn-1.20230414.110554/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_SprintInterface.py` & `returnn-1.20230414.110554/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TFEngine.py` & `returnn-1.20230414.110554/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TFNativeOp.py` & `returnn-1.20230414.110554/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TFNetworkLayer.py` & `returnn-1.20230414.110554/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230414.110554/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230414.110554/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TFUpdater.py` & `returnn-1.20230414.110554/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TFUtil.py` & `returnn-1.20230414.110554/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TF_determinism.py` & `returnn-1.20230414.110554/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TaskSystem.py` & `returnn-1.20230414.110554/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230414.110554/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_TranslationDataset.py` & `returnn-1.20230414.110554/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_Util.py` & `returnn-1.20230414.110554/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_demos.py` & `returnn-1.20230414.110554/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_fork_exec.py` & `returnn-1.20230414.110554/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_hdf_dump.py` & `returnn-1.20230414.110554/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_rf_base.py` & `returnn-1.20230414.110554/tests/test_rf_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,36 +139,14 @@
         targets = extern_data["classes"]
         loss = rf.cross_entropy(estimated=logits, estimated_type="logits", target=targets, axis=out_dim)
         loss.mark_as_default_output()
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
 
 
-def test_pack():
-    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
-    in_dim = Dim(7, name="in")
-    extern_data = TensorDict(
-        {
-            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
-        }
-    )
-
-    class _Net(rf.Module):
-        def __call__(self, x: Tensor) -> Tuple[Tensor, Dim]:
-            pack, pack_dim = rf.pack(x, dims=[batch_dim, time_dim], enforce_sorted=False)
-            return pack, pack_dim
-
-    # noinspection PyShadowingNames
-    def _forward_step(*, model: _Net, extern_data: TensorDict):
-        out, pack_dim = model(extern_data["data"])
-        out.mark_as_default_output(shape=(pack_dim, in_dim))
-
-    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
-
-
 def test_dropout():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
     in_dim = Dim(7, name="in")
     extern_data = TensorDict(
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
```

### Comparing `returnn-1.20230413.93323/tests/test_tensor.py` & `returnn-1.20230414.110554/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_tools.py` & `returnn-1.20230414.110554/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_torch_frontend.py` & `returnn-1.20230414.110554/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tests/test_torch_internal_frontend.py` & `returnn-1.20230414.110554/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/analyze-dataset-batches.py` & `returnn-1.20230414.110554/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/bliss-collect-seq-lens.py` & `returnn-1.20230414.110554/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/bliss-dump-text.py` & `returnn-1.20230414.110554/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/bliss-get-segment-names.py` & `returnn-1.20230414.110554/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/bliss-to-ogg-zip.py` & `returnn-1.20230414.110554/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/bpe-create-lexicon.py` & `returnn-1.20230414.110554/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/calculate-word-error-rate.py` & `returnn-1.20230414.110554/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/cleanup-old-models.py` & `returnn-1.20230414.110554/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/collect-orth-symbols.py` & `returnn-1.20230414.110554/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/collect-words.py` & `returnn-1.20230414.110554/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/compile_native_op.py` & `returnn-1.20230414.110554/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/compile_tf_graph.py` & `returnn-1.20230414.110554/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/debug-dump-search-scores.py` & `returnn-1.20230414.110554/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/debug-plot-search-scores.py` & `returnn-1.20230414.110554/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/dump-dataset-raw-strings.py` & `returnn-1.20230414.110554/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/dump-dataset.py` & `returnn-1.20230414.110554/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/dump-forward-stats.py` & `returnn-1.20230414.110554/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/dump-forward.py` & `returnn-1.20230414.110554/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/dump-network-json.py` & `returnn-1.20230414.110554/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/dump-pickle.py` & `returnn-1.20230414.110554/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230414.110554/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/get-attention-weights.py` & `returnn-1.20230414.110554/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/get-best-model-epoch.py` & `returnn-1.20230414.110554/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/hdf_dump.py` & `returnn-1.20230414.110554/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230414.110554/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/import-blocks-mt-model.py` & `returnn-1.20230414.110554/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/import-t2t-mt-model.py` & `returnn-1.20230414.110554/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/Makefile` & `returnn-1.20230414.110554/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/README.md` & `returnn-1.20230414.110554/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/example/README.md` & `returnn-1.20230414.110554/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230414.110554/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230414.110554/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230414.110554/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/file.h` & `returnn-1.20230414.110554/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230414.110554/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230414.110554/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/main.cc` & `returnn-1.20230414.110554/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230414.110554/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230414.110554/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230414.110554/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/tf_avg_checkpoints.py` & `returnn-1.20230414.110554/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/tf_inspect_checkpoint.py` & `returnn-1.20230414.110554/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.93323/tools/tf_inspect_summary_log.py` & `returnn-1.20230414.110554/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

