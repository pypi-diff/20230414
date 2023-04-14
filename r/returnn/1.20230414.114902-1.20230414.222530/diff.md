# Comparing `tmp/returnn-1.20230414.114902.tar.gz` & `tmp/returnn-1.20230414.222530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230414.114902.tar", last modified: Fri Apr 14 10:10:41 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230414.222530.tar", last modified: Fri Apr 14 20:41:49 2023, max compression
```

## Comparing `returnn-1.20230414.114902.tar` & `returnn-1.20230414.222530.tar`

### file list

```diff
@@ -1,421 +1,421 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 10:10:20.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-14 10:10:24.000000 returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29694 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95121 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   154892 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151442 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22367 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   585898 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33286 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 10:10:40.000000 returnn-1.20230414.114902/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:10:41.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-14 10:10:19.000000 returnn-1.20230414.114902/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 20:41:29.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-14 20:41:33.000000 returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97348 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155428 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151442 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586512 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33286 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:41:49.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-14 20:41:28.000000 returnn-1.20230414.222530/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230414.114902/.gitignore` & `returnn-1.20230414.222530/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/.gitmodules` & `returnn-1.20230414.222530/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/CHANGELOG.md` & `returnn-1.20230414.222530/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/CODEOWNERS` & `returnn-1.20230414.222530/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/CONTRIBUTING.md` & `returnn-1.20230414.222530/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/LICENSE` & `returnn-1.20230414.222530/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/MANIFEST.in` & `returnn-1.20230414.222530/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/PKG-INFO` & `returnn-1.20230414.222530/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230414.114902
+Version: 1.20230414.222530
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230414.114902/README.rst` & `returnn-1.20230414.222530/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/__init__.py` & `returnn-1.20230414.222530/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/12AX.cluster_map` & `returnn-1.20230414.222530/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-fwd.config` & `returnn-1.20230414.222530/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-horovod-mpi.py` & `returnn-1.20230414.222530/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230414.222530/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-hyper-param-tuning.config` & `returnn-1.20230414.222530/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-iter-dataset.py` & `returnn-1.20230414.222530/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-list-devices.py` & `returnn-1.20230414.222530/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-lua-torch-layer.config` & `returnn-1.20230414.222530/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230414.222530/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-returnn-as-framework.py` & `returnn-1.20230414.222530/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-rf.config` & `returnn-1.20230414.222530/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-rhn-enwik8.config` & `returnn-1.20230414.222530/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-sprint-interface.py` & `returnn-1.20230414.222530/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-att-copy.config` & `returnn-1.20230414.222530/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-attention.config` & `returnn-1.20230414.222530/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230414.222530/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230414.222530/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-enc-dec.config` & `returnn-1.20230414.222530/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230414.222530/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230414.222530/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230414.222530/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230414.222530/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230414.222530/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230414.222530/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230414.222530/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230414.222530/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230414.222530/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230414.222530/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-rec-self-att.config` & `returnn-1.20230414.222530/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230414.222530/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230414.222530/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230414.222530/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-torch.config` & `returnn-1.20230414.222530/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230414.222530/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/demo.sh` & `returnn-1.20230414.222530/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230414.222530/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230414.222530/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230414.222530/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/README.txt` & `returnn-1.20230414.222530/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/config_demo` & `returnn-1.20230414.222530/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230414.222530/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/config_real` & `returnn-1.20230414.222530/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230414.222530/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/decode.py` & `returnn-1.20230414.222530/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230414.222530/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230414.222530/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230414.222530/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230414.222530/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230414.222530/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230414.222530/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230414.222530/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230414.222530/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230414.222530/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230414.222530/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/__init__.py` & `returnn-1.20230414.222530/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/__main__.py` & `returnn-1.20230414.222530/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/__old_mod_loader__.py` & `returnn-1.20230414.222530/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/__setup__.py` & `returnn-1.20230414.222530/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/config.py` & `returnn-1.20230414.222530/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/audio.py` & `returnn-1.20230414.222530/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/basic.py` & `returnn-1.20230414.222530/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/bundle_file.py` & `returnn-1.20230414.222530/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/cached.py` & `returnn-1.20230414.222530/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/cached2.py` & `returnn-1.20230414.222530/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/generating.py` & `returnn-1.20230414.222530/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/hdf.py` & `returnn-1.20230414.222530/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/lm.py` & `returnn-1.20230414.222530/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/map.py` & `returnn-1.20230414.222530/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/meta.py` & `returnn-1.20230414.222530/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/multi_proc.py` & `returnn-1.20230414.222530/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/normalization_data.py` & `returnn-1.20230414.222530/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/numpy_dump.py` & `returnn-1.20230414.222530/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/raw_wav.py` & `returnn-1.20230414.222530/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/sprint.py` & `returnn-1.20230414.222530/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/stereo.py` & `returnn-1.20230414.222530/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230414.222530/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/datasets/util/vocabulary.py` & `returnn-1.20230414.222530/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/engine/base.py` & `returnn-1.20230414.222530/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/engine/batch.py` & `returnn-1.20230414.222530/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230414.222530/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230414.222530/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230414.222530/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230414.222530/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/graph_editor/edit.py` & `returnn-1.20230414.222530/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230414.222530/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/graph_editor/select.py` & `returnn-1.20230414.222530/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230414.222530/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/graph_editor/transform.py` & `returnn-1.20230414.222530/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/extern/graph_editor/util.py` & `returnn-1.20230414.222530/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/__init__.py` & `returnn-1.20230414.222530/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/_backend.py` & `returnn-1.20230414.222530/returnn/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,29 @@
         :param raw_tensor: raw tensor
         :param perm: permutation
         :return: transposed raw tensor
         """
         raise NotImplementedError
 
     @staticmethod
+    def transpose(tensor: Tensor, perm: Sequence[Union[Dim, int]], *, allow_int: bool = False) -> Tensor:
+        """
+        :param tensor: tensor
+        :param perm: permutation
+        :param allow_int: allow int as axis in perm
+        :return: transposed tensor
+        """
+        # Default implementation using transpose_raw.
+        out = tensor.copy_template_transpose(perm, allow_int=allow_int)
+        backend = get_backend_by_tensor(tensor)
+        perm_ = [tensor.get_axis_from_description(a, allow_int=allow_int) for a in perm]
+        out.raw_tensor = backend.transpose_raw(tensor.raw_tensor, perm_)
+        return out
+
+    @staticmethod
     def expand_dims_raw(raw_tensor: T, axis: int) -> T:
         """
         :param raw_tensor:
         :param axis:
         :return: raw tensor with new axis
         """
         raise NotImplementedError
```

### Comparing `returnn-1.20230414.114902/returnn/frontend/_numpy_backend.py` & `returnn-1.20230414.222530/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/_utils.py` & `returnn-1.20230414.222530/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/array_.py` & `returnn-1.20230414.222530/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/attention.py` & `returnn-1.20230414.222530/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/cond.py` & `returnn-1.20230414.222530/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/const.py` & `returnn-1.20230414.222530/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/container.py` & `returnn-1.20230414.222530/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/dims.py` & `returnn-1.20230414.222530/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/dropout.py` & `returnn-1.20230414.222530/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/dtype.py` & `returnn-1.20230414.222530/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/init.py` & `returnn-1.20230414.222530/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/linear.py` & `returnn-1.20230414.222530/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/loss.py` & `returnn-1.20230414.222530/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/math_.py` & `returnn-1.20230414.222530/returnn/frontend/math_.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "greater",
     "greater_equal",
     "add",
     "sub",
     "mul",
     "true_divide",
     "floor_divide",
+    "ceil_divide",
     "neg",
     "mod",
     "pow",
     "squared_difference",
     "logical_and",
     "logical_or",
     "logical_not",
@@ -233,14 +234,19 @@
 
 
 def floor_divide(a: Tensor, b: Tensor) -> Tensor:
     """floordiv"""
     return combine(a, "floordiv", b)
 
 
+def ceil_divide(a: Tensor, b: Tensor) -> Tensor:
+    """ceildiv"""
+    return -(-a // b)
+
+
 def neg(a: Tensor) -> Tensor:
     """neg"""
     # noinspection PyProtectedMember
     return a._raw_backend.activation(a, "neg")
 
 
 def mod(a: Tensor, b: Tensor) -> Tensor:
```

### Comparing `returnn-1.20230414.114902/returnn/frontend/matmul.py` & `returnn-1.20230414.222530/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/module.py` & `returnn-1.20230414.222530/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/normalization.py` & `returnn-1.20230414.222530/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/parameter.py` & `returnn-1.20230414.222530/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/rand.py` & `returnn-1.20230414.222530/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/reduce.py` & `returnn-1.20230414.222530/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/run_ctx.py` & `returnn-1.20230414.222530/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/state.py` & `returnn-1.20230414.222530/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/frontend/types.py` & `returnn-1.20230414.222530/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/import_/common.py` & `returnn-1.20230414.222530/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/import_/git.py` & `returnn-1.20230414.222530/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/import_/import_.py` & `returnn-1.20230414.222530/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/learning_rate_control.py` & `returnn-1.20230414.222530/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/log.py` & `returnn-1.20230414.222530/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/native_op.cpp` & `returnn-1.20230414.222530/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/native_op.py` & `returnn-1.20230414.222530/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/pretrain.py` & `returnn-1.20230414.222530/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/sprint/cache.py` & `returnn-1.20230414.222530/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/sprint/control.py` & `returnn-1.20230414.222530/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/sprint/error_signals.py` & `returnn-1.20230414.222530/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/sprint/extern_interface.py` & `returnn-1.20230414.222530/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/sprint/interface.py` & `returnn-1.20230414.222530/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tensor/_dim_extra.py` & `returnn-1.20230414.222530/returnn/tensor/_dim_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -906,51 +906,74 @@
         """
         return getattr(x, "_is_size_of_dim_tag", None)
 
     def complete_dyn_size(self, template_only=False):
         """
         In case we can calculate the dyn size, do that now.
 
-        Warning: This is TensorFlow only currently.
-
         :param bool template_only:
         """
         if not self.is_dynamic():
             return
         self._validate_in_current_graph()
         if self.dyn_size_ext and (self.dyn_size_ext.placeholder is not None or template_only):
             return
         same_base = self.get_same_base()
         op = self.derived_from_op or same_base.derived_from_op
         if not op:
             return
 
-        import tensorflow as tf
-        from returnn.tf.util import basic as tf_util
+        for x in op.inputs:
+            if self.batch:
+                x = x.get_for_batch_ctx(self.batch, self.control_flow_ctx)
+            x.complete_dyn_size(template_only=template_only)
+
+        backend = None
+        for x in op.inputs:
+            if self.batch:
+                x = x.get_for_batch_ctx(self.batch, self.control_flow_ctx)
+            if x.dyn_size_ext and x.dyn_size_ext.raw_tensor is not None:
+                # noinspection PyProtectedMember
+                backend = x.dyn_size_ext._raw_backend
+                break
+
         import numpy
-        from tensorflow.python.framework import tensor_util
+        import returnn.frontend as rf
+        from returnn.tensor import Tensor
+
+        tf = tf_util = tensor_util = None
+        if backend and backend.is_tensorflow:
+            import tensorflow as tf
+
+            if backend.RawTensorType == tf.Tensor:
+                from returnn.tf.util import basic as tf_util
+                from tensorflow.python.framework import tensor_util
+            else:
+                tf = None
 
         kind = op.kind
         if kind.endswith("_right"):
             kind = kind[: -len("_right")]  # order does not matter here
         if kind.endswith("_left"):
             kind = kind[: -len("_left")]
 
         def _is_negative(x__):
             if isinstance(x__, numpy.ndarray):
                 return (x__ < 0).any()
             if isinstance(x__, (int, float, numpy.number)):
                 return x__ < 0
+            if not tf:
+                return False
             assert isinstance(x__, tf.Tensor)
             x__ = tensor_util.constant_value(x__)
             if x__ is not None:
                 return _is_negative(x__)
             return False
 
-        def _bin_op(a, b):
+        def _bin_op_tf(a, b):
             if template_only:
                 return None
             if a is None or b is None:
                 return None
             assert isinstance(a, tf.Tensor) and isinstance(b, (int, tf.Tensor))
             with tf_util.same_control_flow_ctx([a, b]):
                 if kind == "add":
@@ -965,32 +988,62 @@
                 elif kind in ("floordiv", "truediv"):  # truediv assumes there is no remainder
                     return a // b
                 elif kind == "ceildiv":
                     return -(-a // b)
                 else:
                     raise ValueError("unknown op kind %r" % op.kind)
 
+        def _bin_op(a, b):
+            if template_only or not backend:
+                if isinstance(a, _t.Tensor) and isinstance(b, _t.Tensor):
+                    return _t.Tensor.get_common_data([a, b], allow_broadcast_all_sources=True)
+                if isinstance(a, _t.Tensor):
+                    return a
+                if isinstance(b, _t.Tensor):
+                    return b
+            if kind == "add":
+                return a + b
+            elif kind == "sub":
+                return a - b
+            elif kind == "mul":
+                return a * b
+            elif kind in ("floordiv", "truediv"):  # truediv assumes there is no remainder
+                return a // b
+            elif kind == "ceildiv":
+                if isinstance(a, Tensor):
+                    return rf.ceil_divide(a, b)
+                return -(-a // b)
+            else:
+                raise ValueError("unknown op kind %r" % op.kind)
+
         y_name = self.description + ":seq-length"
         y: Optional[_t.Tensor] = None  # resulting dyn size
         inputs = list(op.inputs)
         assert inputs
         while inputs:
             x = inputs.pop(0)
             if not x.is_dynamic():  # static
                 assert x.dimension is not None
                 if y is None:
-                    with tf.control_dependencies(None):  # this will reset the context
+                    if not template_only and backend and not tf:
+                        y = backend.convert_to_tensor(x.dimension, dims=[], dtype=_t.Tensor.size_dtype, name=y_name)
+                    else:
                         y = _t.Tensor(
                             name=y_name,
                             dim_tags=[],
-                            dtype="int32",
-                            placeholder=None if template_only else tf.constant(x.dimension),
+                            dtype=_t.Tensor.size_dtype,
                         )
+                        if not template_only and tf:
+                            with tf.control_dependencies(None):  # this will reset the context
+                                y.raw_tensor = tf.constant(x.dimension)
                     continue
-                y.placeholder = _bin_op(y.placeholder, x.dimension)
+                if tf:
+                    y.placeholder = _bin_op_tf(y.placeholder, x.dimension)
+                else:
+                    y = _bin_op(y, x.dimension)
                 continue
             if self.batch:
                 x = x.get_for_batch_ctx(self.batch, self.control_flow_ctx)
             x.complete_dyn_size(template_only=template_only)
             if not x.dyn_size_ext:
                 return
             x = x.dyn_size_ext
@@ -1000,25 +1053,28 @@
             if x.dim_tags != y.dim_tags:
                 common = _t.Tensor.get_common_data([x, y], allow_broadcast_all_sources=True)
                 x_ = x.copy_compatible_to(common) if x.dim_tags else x
                 y_ = y.copy_compatible_to(common) if y.dim_tags else y
                 y = common
             else:
                 x_, y_ = x, y
-            y.placeholder = _bin_op(y_.placeholder, x_.placeholder)
-        assert y
+            if tf:
+                y.placeholder = _bin_op_tf(y_.placeholder, x_.placeholder)
+            else:
+                y = _bin_op(y_, x_)
+        assert y, f"op {op}?"
         if self.dyn_size_ext:
             assert self.dyn_size_ext.dim_tags == y.dim_tags
         if y.batch:
             if self.batch:
                 assert self.batch == y.batch
             else:
                 self.batch = y.batch
         self.dyn_size_ext = y
-        if y.placeholder is not None:
+        if tf and y.placeholder is not None:
             self.set_tag_on_size_tensor(y.placeholder)
 
     def is_equal(
         self,
         other,
         ignore_feature_dim=False,
         allow_same_feature_dim=False,
```

### Comparing `returnn-1.20230414.114902/returnn/tensor/_tensor_extra.py` & `returnn-1.20230414.222530/returnn/tensor/_tensor_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -647,15 +647,25 @@
         """
         :param int time_dim_axis:
         :return: copy of myself with specific time_dim_axis
         """
         assert self.time_dim_axis is not None
         return self.copy_move_axis(self.time_dim_axis, time_dim_axis)
 
-    def copy_transpose(self, perm: Sequence[Union[int, Dim]], *, allow_int: bool = True) -> _t.Tensor:
+    def copy_transpose(self: Tensor, perm: Sequence[Union[int, Dim]], *, allow_int: bool = True) -> _t.Tensor:
+        """
+        :param perm: permutation of the axes. Maps the new axes to the old axes
+        :param allow_int: allow int as axis, otherwise only :class:`Dim`
+        :return: copy of myself with permuted axes
+        """
+        if self.raw_tensor is not None:
+            return self._raw_backend.transpose(self, perm, allow_int=allow_int)
+        return self.copy_template_transpose(perm, allow_int=allow_int)
+
+    def copy_template_transpose(self: Tensor, perm: Sequence[Union[int, Dim]], *, allow_int: bool = True) -> _t.Tensor:
         """
         :param perm: permutation of the axes. Maps the new axes to the old axes
         :param allow_int: allow int as axis, otherwise only :class:`Dim`
         :return: copy of myself with permuted axes
         """
         assert len(perm) == self.batch_ndim, f"{self}: invalid perm {perm!r} length"
         perm_ = perm
@@ -665,20 +675,20 @@
             return self.copy()
 
         data_opts = self.get_kwargs(include_special_axes=False)
         if self._raw_tensor is not None:
             data_opts["raw_tensor"] = self._raw_backend.transpose_raw(self._raw_tensor, perm)
         data_opts["dims"] = tuple(self.dim_tags[perm[i]] for i in range(self.batch_ndim))
         data = _t.Tensor(**data_opts)
+        inv_perm = {j: i for (i, j) in enumerate(perm)}
         if self.version == 1:
-            inv_perm = {j: i for (i, j) in enumerate(perm)}
             if inv_perm.get(self.time_dim_axis, None) != data.time_dim_axis:
                 data.time_dim_axis = inv_perm.get(self.time_dim_axis, None)
-            if inv_perm.get(self.feature_dim_axis, None) != data.feature_dim_axis:
-                data.feature_dim_axis = inv_perm.get(self.feature_dim_axis, None)
+        if inv_perm.get(self.feature_dim_axis, None) != data.feature_dim_axis:
+            data.feature_dim_axis = inv_perm.get(self.feature_dim_axis, None)
         return data
 
     def copy_move_axis(self, old_axis, new_axis) -> _t.Tensor:
         """
         :param int old_axis: counted with batch-dim
         :param int new_axis: counted with batch-dim
         :return: copy of myself with moved axis (see :func:`move_axis`)
```

### Comparing `returnn-1.20230414.114902/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230414.222530/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230414.222530/returnn/tensor/_tensor_op_overloads.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,29 @@
 from ._tensor_mixin_base import _TensorMixinBase
 
 
 class _TensorOpOverloadsMixin(_TensorMixinBase):
 
     # --- comparisons
 
-    def __eq__(self: Tensor, other: Union[_rf_types.RawTensorTypes, Tensor]) -> Tensor:
-        return _rf().compare(self, "==", other)
+    def __eq__(self: Tensor, other: Union[_rf_types.RawTensorTypes, Tensor]) -> Union[Tensor, bool]:
+        # When comparing to some other invalid type, return False, not a Tensor.
+        # This is to allow easy equality checks with other random objects.
+        # See for example here: https://github.com/rwth-i6/returnn/pull/1284
+        if self.raw_tensor is None:
+            # The other op overloads would actually raise some exception in this case.
+            # However, here just return False.
+            return False
+
+        import returnn.frontend as rf
+
+        valid_types = (rf.Tensor, self._raw_backend.RawTensorType) + tuple(rf.RawTensorTypes.__args__)
+        if isinstance(other, valid_types):
+            return _rf().compare(self, "==", other)
+        return False
 
     def __ne__(self: Tensor, other: Union[_rf_types.RawTensorTypes, Tensor]) -> Tensor:
         return _rf().compare(self, "!=", other)
 
     def __lt__(self: Tensor, other: Union[_rf_types.RawTensorTypes, Tensor]) -> Tensor:
         return _rf().compare(self, "<", other)
 
@@ -74,33 +87,29 @@
 
     def __pow__(self: Tensor, other: Union[_rf_types.RawTensorTypes, Tensor]) -> Tensor:
         return _rf().combine(self, "**", other)
 
     def __rpow__(self: Tensor, other: Union[_rf_types.RawTensorTypes, Tensor]) -> Tensor:
         return _rf().combine(other, "**", self)
 
-    def __neg__(self):  # -x
-        if True:  # avoid warning: abstract base class...
-            raise NotImplementedError  # TODO
+    def __neg__(self: Tensor):  # -x
+        return _rf().neg(self)
 
     def __invert__(self):  # ~x
-        if True:
+        if True:  # avoid warning: abstract base class...
             raise NotImplementedError  # TODO
 
-    def __abs__(self):
-        if True:
-            raise NotImplementedError  # TODO
+    def __abs__(self: Tensor):
+        return _rf().abs(self)
 
-    def __ceil__(self):
-        if True:
-            raise NotImplementedError  # TODO
+    def __ceil__(self: Tensor):
+        return _rf().ceil(self)
 
-    def __floor__(self):
-        if True:
-            raise NotImplementedError  # TODO
+    def __floor__(self: Tensor):
+        return _rf().floor(self)
 
     def __and__(self: Tensor, other: Union[_rf_types.RawTensorTypes, Tensor]) -> Tensor:
         return _rf().combine(self, "logical_and", other)
 
     def __rand__(self: Tensor, other: Union[_rf_types.RawTensorTypes, Tensor]) -> Tensor:
         return _rf().combine(other, "logical_and", self)
```

### Comparing `returnn-1.20230414.114902/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230414.222530/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tensor/dim.py` & `returnn-1.20230414.222530/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tensor/marked_dim.py` & `returnn-1.20230414.222530/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tensor/tensor.py` & `returnn-1.20230414.222530/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tensor/tensor_dict.py` & `returnn-1.20230414.222530/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/compat.py` & `returnn-1.20230414.222530/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/data_pipeline.py` & `returnn-1.20230414.222530/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/distributed.py` & `returnn-1.20230414.222530/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/engine.py` & `returnn-1.20230414.222530/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230414.222530/returnn/tf/frontend_layers/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,17 +114,18 @@
 
     @staticmethod
     def reshape_raw(raw_tensor: Layer, shape: Union[Sequence[Union[int, Layer]], Layer]) -> Layer:
         """reshape_raw"""
         raise Exception("reshape_raw not supported in layers backend because dim tags would be unknown")
 
     @staticmethod
-    def transpose_raw(raw_tensor: Layer, perm: Sequence[int]) -> Layer:
-        """transpose_raw is a no-op in this backend"""
-        return raw_tensor
+    def transpose(tensor: Tensor, perm: Sequence[Union[Dim, int]], *, allow_int: bool = False) -> Tensor:
+        """transpose"""
+        assert not allow_int  # not supported
+        return rfl.make_layer({"class": "transpose", "from": tensor, "perm": perm}, name="transpose")
 
     @staticmethod
     def cast(tensor: Tensor, dtype: str) -> Tensor:
         """cast"""
         return rfl.make_layer({"class": "cast", "from": tensor, "dtype": dtype}, name="cast")
 
     @staticmethod
```

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230414.222530/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230414.222530/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230414.222530/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230414.222530/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230414.222530/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230414.222530/returnn/tf/frontend_layers/make_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,16 @@
         control_flow_ctx=rfl.Layer.inner_control_flow(),
     )
     net.extern_data.set_batch_info(_init_global_batch())
 
     ref_to_layer_name = {}  # type: Dict[rfl.Layer, str]
 
     def _get_unique_name(name) -> str:
+        name = name.replace("/", "_")
+        name = LayerBase.cls_get_tf_scope_name(name)
         reserved_names = set(net.layers.keys()) | {"data"}
         if name not in reserved_names:
             return name
         i = 0
         while True:
             name_ = f"{name}_{i}"
             if name_ not in reserved_names:
```

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230414.222530/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230414.222530/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/horovod.py` & `returnn-1.20230414.222530/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230414.222530/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/layers/base.py` & `returnn-1.20230414.222530/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/layers/basic.py` & `returnn-1.20230414.222530/returnn/tf/layers/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Many canonical basic layers.
 """
 
 from __future__ import annotations
 
-from typing import Optional, Union, Sequence, List
+from typing import Optional, Union, Sequence, List, Dict
 import typing
 import tensorflow as tf
 import contextlib
 import returnn.tf.compat as tf_compat
 import returnn.tf.util.basic as tf_util
 from returnn.util.basic import unicode, NotSpecified
 from returnn.tf.util.data import Data, SearchBeam, Dim, FeatureDim, SpatialDim
@@ -5466,78 +5466,88 @@
             opts["feature_dim_axis"] = cls._translate_axis(out.feature_dim_axis, axis1, axis2)
         return Data(**opts)
 
 
 class TransposeLayer(_ConcatInputLayer):
     """
     Basically a wrapper around :func:`tf.transpose`.
-    Note that usually, this should not be needed, and it is recommended not to be used,
+
+    Note that usually, this should not be needed,
+    and it is recommended not to be used,
     as this will be unnecessarily inefficient.
     Normally, all RETURNN layers will automatically transpose the input data into whatever format they need.
 
     All axes always have a special meaning (e.g. feature dim or time dim)
     or dimension tag (e.g. for time axes, including dyn seq lengths).
     If you need to change the meaning (and not actually transpose / swap axes),
     you need to use :class:`ReinterpretDataLayer`.
 
     See also :class:`ReinterpretDataLayer`, which does not transpose axes,
     but allows to reinterpret their meaning / dim tags.
+
+    One valid use case is to use this for the final output layer,
+    to make sure the output is in the correct format.
     """
 
     layer_class = "transpose"
 
-    def __init__(self, perm, **kwargs):
+    def __init__(self, perm: Union[Dict[Union[Dim, str, int], Union[Dim, str]], Sequence[Dim]], **kwargs):
         """
-        :param dict[str,str] perm: target axis -> source axis
+        :param perm: target axis -> source axis
         """
         super(TransposeLayer, self).__init__(**kwargs)
         self.perm = perm
         perm_ = self.get_perm_int(input_data=self.input_data, perm=perm)
-        self.output.placeholder = tf.transpose(
-            self.input_data.placeholder, [perm_[i] for i in range(self.input_data.batch_ndim)]
-        )
+        self.output.placeholder = tf.transpose(self.input_data.placeholder, perm_)
 
     @classmethod
-    def transpose(cls, input_data, perm, name=None):
+    def transpose(
+        cls,
+        input_data: Data,
+        perm: Union[Dict[Union[Dim, str, int], Union[Dim, str]], Sequence[Dim]],
+        name: Optional[str] = None,
+    ) -> Data:
         """
-        :param Data input_data:
-        :param dict[str,str] perm:
-        :param str|str name:
+        :param input_data:
+        :param perm:
+        :param name:
         :return: transposed data
-        :rtype: Data
         """
         perm_ = cls.get_perm_int(input_data=input_data, perm=perm)
-        perm__ = [perm_[i] for i in range(input_data.batch_ndim)]
-        return input_data.copy_transpose(perm__).copy(name=name)
+        return input_data.copy_transpose(perm_).copy(name=name)
 
     @classmethod
-    def get_perm_int(cls, input_data, perm):
+    def get_perm_int(
+        cls, input_data: Data, perm: Union[Dict[Union[Dim, str, int], Union[Dim, str]], Sequence[Dim]]
+    ) -> List[int]:
         """
-        :param Data input_data:
-        :param dict[str,str] perm:
-        :rtype: dict[int,int]
+        :param input_data:
+        :param perm:
         """
 
-        def _axis(a):
-            """
-            :param str a:
-            :rtype: int
-            """
-            return input_data.get_axis_from_description(a, allow_int=False)
+        def _axis(a: Union[Dim, str, int], *, allow_int: bool = False) -> int:
+            return input_data.get_axis_from_description(a, allow_int=allow_int)
 
-        perm_ = {_axis(i): _axis(j) for (i, j) in perm.items()}
+        if isinstance(perm, (list, tuple)):
+            assert len(perm) == input_data.batch_ndim
+            perm_ = {_axis(i, allow_int=True): _axis(j) for (i, j) in enumerate(perm)}
+        elif isinstance(perm, dict):
+            perm_ = {_axis(i, allow_int=True): _axis(j) for (i, j) in perm.items()}
+        else:
+            raise TypeError(f"unexpected perm {perm!r} of type {type(perm)}")
         assert len(perm) == len(perm_) == len(set(perm_.values())), "data %s, perm %r invalid" % (input_data, perm)
         target_axes = set(perm_)
         source_axes = set(perm_.values())
         rem_target_axes = [i for i in range(input_data.batch_ndim) if i not in target_axes]
         rem_source_axes = [i for i in range(input_data.batch_ndim) if i not in source_axes]
         assert len(rem_target_axes) == len(rem_source_axes)
         perm_.update({i: j for (i, j) in zip(rem_target_axes, rem_source_axes)})
-        assert len(perm_) == len(set(perm_.values())) == input_data.batch_ndim
-        return perm_
+        assert set(perm_.keys()) == set(perm_.values()) == set(range(input_data.batch_ndim))
+        perm__ = [perm_[i] for i in range(input_data.batch_ndim)]
+        return perm__
 
     @classmethod
     def get_out_data_from_opts(cls, name, sources, perm, **kwargs):
         """
         :param str name:
         :param list[LayerBase] sources:
         :param dict[str,str] perm: target axis -> source axis
@@ -5852,15 +5862,15 @@
         """
         from returnn.util import BehaviorVersion
 
         padding = padding.upper()
         assert padding in ["SAME", "VALID"], "no other padding supported at the moment"
         assert "out_type" not in kwargs, "don't set out_type explicitly for this layer"
         assert len(filter_size) in (1, 2, 3), "only 1D conv, 2D conv or 3D conv supported"
-        super(ConvLayer, self).__init__(**kwargs)
+        super(ConvLayer, self).__init__(in_dim=in_dim, out_dim=out_dim, **kwargs)
         if isinstance(strides, int):
             strides = [strides] * len(filter_size)
         else:
             strides = list(strides)
         assert len(strides) == len(filter_size)
         if isinstance(dilation_rate, int):
             dilation_rate = [dilation_rate] * len(filter_size)
```

### Comparing `returnn-1.20230414.114902/returnn/tf/layers/rec.py` & `returnn-1.20230414.222530/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/layers/segmental_model.py` & `returnn-1.20230414.222530/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/layers/signal_processing.py` & `returnn-1.20230414.222530/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/native_op.py` & `returnn-1.20230414.222530/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/network.py` & `returnn-1.20230414.222530/returnn/tf/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1702,14 +1702,15 @@
             if any(d.dimension is None for d in rem_dims):  # any other dynamic?
                 return False
             deps = _layer_deps(layer_)
             if not deps:
                 return False
             layer_kwargs = layer_.kwargs.copy()
             layer_kwargs.pop("out_shape", None)
+            layer_kwargs.pop("output", None)
             layer_kwargs_flat_values = nest.flatten(layer_kwargs)
             if any(dim in layer_kwargs_flat_values for dim in dims):  # e.g. to operate on the axis
                 return False
             valid_deps = all(
                 set(dep_.output.dim_tags).issuperset(dims) or set(dep_.output.dim_tags).isdisjoint(dims)
                 for dep_ in deps
             )
```

### Comparing `returnn-1.20230414.114902/returnn/tf/sprint.py` & `returnn-1.20230414.222530/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/updater.py` & `returnn-1.20230414.222530/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/util/basic.py` & `returnn-1.20230414.222530/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/util/data.py` & `returnn-1.20230414.222530/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/util/ken_lm.py` & `returnn-1.20230414.222530/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/tf/util/open_fst.py` & `returnn-1.20230414.222530/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/torch/data/pipeline.py` & `returnn-1.20230414.222530/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230414.222530/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/torch/data/tensor_utils.py` & `returnn-1.20230414.222530/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/torch/engine.py` & `returnn-1.20230414.222530/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/torch/frontend/_backend.py` & `returnn-1.20230414.222530/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/torch/frontend/_rand.py` & `returnn-1.20230414.222530/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/torch/frontend/bridge.py` & `returnn-1.20230414.222530/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/torch/updater.py` & `returnn-1.20230414.222530/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/basic.py` & `returnn-1.20230414.222530/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/better_exchook.py` & `returnn-1.20230414.222530/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/bpe.py` & `returnn-1.20230414.222530/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/debug.py` & `returnn-1.20230414.222530/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/debug_helpers.py` & `returnn-1.20230414.222530/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/fsa.py` & `returnn-1.20230414.222530/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230414.222530/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/pprint.py` & `returnn-1.20230414.222530/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/py-to-pickle.cpp` & `returnn-1.20230414.222530/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/sig_proc.py` & `returnn-1.20230414.222530/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn/util/task_system.py` & `returnn-1.20230414.222530/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/returnn.egg-info/PKG-INFO` & `returnn-1.20230414.222530/returnn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230414.114902
+Version: 1.20230414.222530
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230414.114902/returnn.egg-info/SOURCES.txt` & `returnn-1.20230414.222530/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/setup.py` & `returnn-1.20230414.222530/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/DummySprintExec.py` & `returnn-1.20230414.222530/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230414.222530/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230414.222530/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230414.222530/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/_set_num_threads1.py` & `returnn-1.20230414.222530/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/_setup_test_env.py` & `returnn-1.20230414.222530/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/bpe-unicode-demo.codes` & `returnn-1.20230414.222530/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/bpe-unicode-demo.vocab` & `returnn-1.20230414.222530/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/lexicon_opt.isyms` & `returnn-1.20230414.222530/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/lexicon_opt.jpg` & `returnn-1.20230414.222530/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/lint_common.py` & `returnn-1.20230414.222530/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/pycharm-inspect.py` & `returnn-1.20230414.222530/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/pylint.py` & `returnn-1.20230414.222530/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/returnn-as-framework.py` & `returnn-1.20230414.222530/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/rf_utils.py` & `returnn-1.20230414.222530/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/spelling.dic` & `returnn-1.20230414.222530/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_Config.py` & `returnn-1.20230414.222530/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_Dataset.py` & `returnn-1.20230414.222530/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_Fsa.py` & `returnn-1.20230414.222530/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_GeneratingDataset.py` & `returnn-1.20230414.222530/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_HDFDataset.py` & `returnn-1.20230414.222530/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_LearningRateControl.py` & `returnn-1.20230414.222530/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_Log.py` & `returnn-1.20230414.222530/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_MultiProcDataset.py` & `returnn-1.20230414.222530/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_PTDataset.py` & `returnn-1.20230414.222530/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_Pretrain.py` & `returnn-1.20230414.222530/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_ResNet.py` & `returnn-1.20230414.222530/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_SprintDataset.py` & `returnn-1.20230414.222530/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_SprintInterface.py` & `returnn-1.20230414.222530/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TFEngine.py` & `returnn-1.20230414.222530/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TFNativeOp.py` & `returnn-1.20230414.222530/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TFNetworkLayer.py` & `returnn-1.20230414.222530/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230414.222530/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230414.222530/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TFUpdater.py` & `returnn-1.20230414.222530/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TFUtil.py` & `returnn-1.20230414.222530/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TF_determinism.py` & `returnn-1.20230414.222530/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TaskSystem.py` & `returnn-1.20230414.222530/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230414.222530/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_TranslationDataset.py` & `returnn-1.20230414.222530/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_Util.py` & `returnn-1.20230414.222530/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_demos.py` & `returnn-1.20230414.222530/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_fork_exec.py` & `returnn-1.20230414.222530/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_hdf_dump.py` & `returnn-1.20230414.222530/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_rf_array.py` & `returnn-1.20230414.222530/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_rf_attention.py` & `returnn-1.20230414.222530/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_rf_base.py` & `returnn-1.20230414.222530/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_rf_container.py` & `returnn-1.20230414.222530/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_rf_normalization.py` & `returnn-1.20230414.222530/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_tensor.py` & `returnn-1.20230414.222530/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_tools.py` & `returnn-1.20230414.222530/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_torch_frontend.py` & `returnn-1.20230414.222530/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tests/test_torch_internal_frontend.py` & `returnn-1.20230414.222530/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/analyze-dataset-batches.py` & `returnn-1.20230414.222530/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/bliss-collect-seq-lens.py` & `returnn-1.20230414.222530/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/bliss-dump-text.py` & `returnn-1.20230414.222530/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/bliss-get-segment-names.py` & `returnn-1.20230414.222530/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/bliss-to-ogg-zip.py` & `returnn-1.20230414.222530/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/bpe-create-lexicon.py` & `returnn-1.20230414.222530/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/calculate-word-error-rate.py` & `returnn-1.20230414.222530/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/cleanup-old-models.py` & `returnn-1.20230414.222530/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/collect-orth-symbols.py` & `returnn-1.20230414.222530/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/collect-words.py` & `returnn-1.20230414.222530/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/compile_native_op.py` & `returnn-1.20230414.222530/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/compile_tf_graph.py` & `returnn-1.20230414.222530/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/debug-dump-search-scores.py` & `returnn-1.20230414.222530/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/debug-plot-search-scores.py` & `returnn-1.20230414.222530/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/dump-dataset-raw-strings.py` & `returnn-1.20230414.222530/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/dump-dataset.py` & `returnn-1.20230414.222530/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/dump-forward-stats.py` & `returnn-1.20230414.222530/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/dump-forward.py` & `returnn-1.20230414.222530/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/dump-network-json.py` & `returnn-1.20230414.222530/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/dump-pickle.py` & `returnn-1.20230414.222530/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230414.222530/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/get-attention-weights.py` & `returnn-1.20230414.222530/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/get-best-model-epoch.py` & `returnn-1.20230414.222530/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/hdf_dump.py` & `returnn-1.20230414.222530/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230414.222530/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/import-blocks-mt-model.py` & `returnn-1.20230414.222530/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/import-t2t-mt-model.py` & `returnn-1.20230414.222530/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/Makefile` & `returnn-1.20230414.222530/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/README.md` & `returnn-1.20230414.222530/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/example/README.md` & `returnn-1.20230414.222530/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230414.222530/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230414.222530/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230414.222530/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/file.h` & `returnn-1.20230414.222530/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230414.222530/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230414.222530/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/main.cc` & `returnn-1.20230414.222530/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230414.222530/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230414.222530/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230414.222530/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/tf_avg_checkpoints.py` & `returnn-1.20230414.222530/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/tf_inspect_checkpoint.py` & `returnn-1.20230414.222530/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.114902/tools/tf_inspect_summary_log.py` & `returnn-1.20230414.222530/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

