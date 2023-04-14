# Comparing `tmp/tw-3.8.1.tar.gz` & `tmp/tw-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tw-3.8.1.tar", last modified: Wed Feb  2 06:42:25 2022, max compression
+gzip compressed data, was "dist/tw-3.9.0.tar", last modified: Thu May 26 04:23:51 2022, max compression
```

## Comparing `tw-3.8.1.tar` & `tw-3.9.0.tar`

### file list

```diff
@@ -1,237 +1,248 @@
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2744 2021-06-02 02:57:54.000000 tw-3.8.1/README.md
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)       38 2022-02-02 06:42:25.000000 tw-3.8.1/setup.cfg
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw.egg-info/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        3 2022-02-02 06:42:25.000000 tw-3.8.1/tw.egg-info/top_level.txt
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)       81 2022-02-02 06:42:25.000000 tw-3.8.1/tw.egg-info/requires.txt
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4122 2022-02-02 06:42:25.000000 tw-3.8.1/tw.egg-info/PKG-INFO
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        1 2022-02-02 06:42:25.000000 tw-3.8.1/tw.egg-info/dependency_links.txt
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5977 2022-02-02 06:42:25.000000 tw-3.8.1/tw.egg-info/SOURCES.txt
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4122 2022-02-02 06:42:25.000000 tw-3.8.1/PKG-INFO
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/nn/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1847 2021-11-27 08:05:27.000000 tw-3.8.1/tw/nn/filter.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    22408 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/pooling.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      734 2021-06-15 12:30:17.000000 tw-3.8.1/tw/nn/functional.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3905 2021-06-29 07:02:33.000000 tw-3.8.1/tw/nn/nms.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5308 2021-11-27 08:05:27.000000 tw-3.8.1/tw/nn/convert.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5424 2022-01-28 06:57:43.000000 tw-3.8.1/tw/nn/initialize.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    15312 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/rnn.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7615 2022-01-28 06:57:43.000000 tw-3.8.1/tw/nn/normalize.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7390 2022-01-28 06:57:43.000000 tw-3.8.1/tw/nn/drop.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3743 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/sample.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1539 2021-07-25 15:30:25.000000 tw-3.8.1/tw/nn/search.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12655 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/attention.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5016 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/keypoints.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11753 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/head.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7658 2022-01-06 15:41:18.000000 tw-3.8.1/tw/nn/fft.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4304 2022-01-28 06:57:43.000000 tw-3.8.1/tw/nn/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    48495 2021-11-27 08:05:30.000000 tw-3.8.1/tw/nn/losses.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4626 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/embedding.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    37482 2021-11-27 08:05:29.000000 tw-3.8.1/tw/nn/conv.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6453 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/bbox.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      753 2021-06-02 02:57:54.000000 tw-3.8.1/tw/nn/transformer.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    18328 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/anchor.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11526 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/fpn.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1833 2021-12-31 12:42:53.000000 tw-3.8.1/tw/nn/interpolate.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1812 2021-11-27 08:05:28.000000 tw-3.8.1/tw/nn/activation.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/media/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4307 2021-12-31 12:29:51.000000 tw-3.8.1/tw/media/raw.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-12-29 12:14:03.000000 tw-3.8.1/tw/media/yuv.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8502 2021-12-29 12:52:12.000000 tw-3.8.1/tw/media/media.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      952 2021-12-31 12:42:53.000000 tw-3.8.1/tw/media/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10247 2021-12-29 12:13:27.000000 tw-3.8.1/tw/media/ply.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_alignment/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_alignment/__init__.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_landmark/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      720 2021-11-27 08:04:08.000000 tw-3.8.1/tw/contrib/face_landmark/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    18546 2021-11-27 08:04:09.000000 tw-3.8.1/tw/contrib/face_landmark/mobileface.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      771 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/__init__.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_detection/
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_detection/s3fd/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5670 2021-11-27 07:42:48.000000 tw-3.8.1/tw/contrib/face_detection/s3fd/nets.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/s3fd/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7122 2021-11-27 07:43:44.000000 tw-3.8.1/tw/contrib/face_detection/s3fd/box_utils.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2549 2021-11-27 07:43:35.000000 tw-3.8.1/tw/contrib/face_detection/s3fd/s3fd.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_detection/retinaface/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10477 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/retinaface/nets.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/retinaface/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    14132 2021-11-27 08:04:09.000000 tw-3.8.1/tw/contrib/face_detection/retinaface/box_utils.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3542 2021-11-27 08:04:08.000000 tw-3.8.1/tw/contrib/face_detection/retinaface/retinaface.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3115 2021-11-27 07:20:30.000000 tw-3.8.1/tw/contrib/face_detection/retinaface/data_utils.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1025 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/__init__.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_detection/pyramidbox/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     9370 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/pyramidbox/nets.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/pyramidbox/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6770 2021-11-27 08:04:09.000000 tw-3.8.1/tw/contrib/face_detection/pyramidbox/box_utils.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2587 2021-11-27 06:49:31.000000 tw-3.8.1/tw/contrib/face_detection/pyramidbox/pyramidbox.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_detection/dsfd/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10006 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/dsfd/nets.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2558 2021-11-27 06:49:31.000000 tw-3.8.1/tw/contrib/face_detection/dsfd/dsfd.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/dsfd/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7194 2021-11-27 07:44:41.000000 tw-3.8.1/tw/contrib/face_detection/dsfd/box_utils.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_detection/tinyface/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2365 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/tinyface/nets.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/tinyface/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3624 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/tinyface/box_utils.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4390 2021-11-27 06:49:31.000000 tw-3.8.1/tw/contrib/face_detection/tinyface/tinyface.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_detection/mtcnn/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3679 2021-11-27 08:04:09.000000 tw-3.8.1/tw/contrib/face_detection/mtcnn/first_stage.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4115 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/mtcnn/nets.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/mtcnn/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7169 2021-11-27 08:04:09.000000 tw-3.8.1/tw/contrib/face_detection/mtcnn/box_utils.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4593 2021-11-27 08:04:09.000000 tw-3.8.1/tw/contrib/face_detection/mtcnn/mtcnn.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/contrib/face_detection/faceboxes/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4866 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/faceboxes/nets.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2944 2021-11-27 08:04:09.000000 tw-3.8.1/tw/contrib/face_detection/faceboxes/faceboxes.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/contrib/face_detection/faceboxes/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3930 2021-11-27 08:04:09.000000 tw-3.8.1/tw/contrib/face_detection/faceboxes/box_utils.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/optim/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2294 2021-06-02 02:57:54.000000 tw-3.8.1/tw/optim/warmup_multistep_lr.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      939 2021-11-27 08:05:29.000000 tw-3.8.1/tw/optim/poly_lr.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      737 2021-11-27 08:05:29.000000 tw-3.8.1/tw/optim/__init__.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/datasets/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4401 2021-11-27 08:05:29.000000 tw-3.8.1/tw/datasets/widerface.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4761 2021-08-29 14:57:48.000000 tw-3.8.1/tw/datasets/coco.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1927 2021-06-02 02:57:54.000000 tw-3.8.1/tw/datasets/cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3852 2022-01-28 06:57:43.000000 tw-3.8.1/tw/datasets/pil.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8792 2022-01-06 12:35:42.000000 tw-3.8.1/tw/datasets/general.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    18173 2021-12-29 12:13:31.000000 tw-3.8.1/tw/datasets/point_cloud.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1356 2021-06-02 02:57:54.000000 tw-3.8.1/tw/datasets/imagenet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1723 2022-01-06 12:30:38.000000 tw-3.8.1/tw/datasets/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3558 2021-06-02 02:57:54.000000 tw-3.8.1/tw/datasets/base.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      919 2021-12-31 12:42:55.000000 tw-3.8.1/tw/datasets/super_resolution.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1328 2021-06-02 02:57:54.000000 tw-3.8.1/tw/datasets/mnist.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    27814 2021-11-27 08:05:30.000000 tw-3.8.1/tw/datasets/quality_assess.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3462 2021-06-24 04:02:33.000000 tw-3.8.1/tw/datasets/avec2014.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4432 2022-01-08 07:42:29.000000 tw-3.8.1/tw/datasets/denoise.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/utils/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4077 2021-10-31 03:43:01.000000 tw-3.8.1/tw/utils/checkpoint.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2809 2021-11-27 08:05:29.000000 tw-3.8.1/tw/utils/stat.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5824 2021-06-09 03:04:42.000000 tw-3.8.1/tw/utils/runner.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3053 2021-10-15 02:35:54.000000 tw-3.8.1/tw/utils/export.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    14972 2021-11-27 08:05:30.000000 tw-3.8.1/tw/utils/flops.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3418 2021-11-15 11:38:12.000000 tw-3.8.1/tw/utils/parser.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      685 2021-11-27 08:05:30.000000 tw-3.8.1/tw/utils/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5906 2022-01-08 07:43:18.000000 tw-3.8.1/tw/utils/drawer.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1023 2021-06-02 02:57:54.000000 tw-3.8.1/tw/utils/tensorboard.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3898 2021-08-06 04:02:16.000000 tw-3.8.1/tw/utils/logger.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1953 2021-06-02 02:57:54.000000 tw-3.8.1/tw/utils/timer.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3837 2021-06-02 02:57:54.000000 tw-3.8.1/tw/utils/filesystem.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/evaluator/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     9203 2021-11-27 08:05:30.000000 tw-3.8.1/tw/evaluator/widerface.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7062 2021-08-29 14:57:15.000000 tw-3.8.1/tw/evaluator/detection.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3681 2021-11-27 08:05:30.000000 tw-3.8.1/tw/evaluator/image.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    14169 2021-11-27 08:05:31.000000 tw-3.8.1/tw/evaluator/segmentation.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4634 2022-01-28 06:57:43.000000 tw-3.8.1/tw/evaluator/classification.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2554 2021-06-02 02:57:54.000000 tw-3.8.1/tw/evaluator/verification.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1666 2021-11-27 08:05:30.000000 tw-3.8.1/tw/evaluator/regression.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1395 2021-08-07 17:17:18.000000 tw-3.8.1/tw/evaluator/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1694 2021-06-02 02:57:54.000000 tw-3.8.1/tw/evaluator/base.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2665 2021-07-17 07:17:13.000000 tw-3.8.1/tw/evaluator/quality_assess.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6811 2021-11-27 08:05:30.000000 tw-3.8.1/tw/evaluator/avec2014.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1518 2021-12-29 12:18:46.000000 tw-3.8.1/tw/__init__.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/tools/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      995 2021-06-16 02:22:43.000000 tw-3.8.1/tw/tools/checkpoint.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1686 2021-06-16 02:21:59.000000 tw-3.8.1/tw/tools/busy.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1572 2021-11-27 08:05:30.000000 tw-3.8.1/tw/tools/media.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1033 2021-06-16 02:13:16.000000 tw-3.8.1/tw/tools/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6583 2021-11-27 08:05:30.000000 tw-3.8.1/tw/tools/monitor.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6742 2021-11-27 08:05:30.000000 tw-3.8.1/tw/tools/event.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/transform/
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/transform/primitive/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8408 2021-06-02 02:57:54.000000 tw-3.8.1/tw/transform/primitive/filter.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    20615 2021-11-27 08:05:31.000000 tw-3.8.1/tw/transform/primitive/crop.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10273 2021-12-30 13:14:26.000000 tw-3.8.1/tw/transform/primitive/normalize.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     9712 2021-11-27 08:05:31.000000 tw-3.8.1/tw/transform/primitive/affine.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12688 2021-11-27 08:05:31.000000 tw-3.8.1/tw/transform/primitive/pad.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-06-02 02:57:54.000000 tw-3.8.1/tw/transform/primitive/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12583 2021-11-27 08:05:31.000000 tw-3.8.1/tw/transform/primitive/colorspace.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5819 2021-11-27 08:05:31.000000 tw-3.8.1/tw/transform/primitive/bbox.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8481 2021-11-13 07:14:52.000000 tw-3.8.1/tw/transform/primitive/resize.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3366 2021-06-02 02:57:54.000000 tw-3.8.1/tw/transform/primitive/morphology.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4727 2021-11-27 08:05:31.000000 tw-3.8.1/tw/transform/pil.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    18016 2022-01-06 12:34:51.000000 tw-3.8.1/tw/transform/meta.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3656 2021-11-27 08:05:30.000000 tw-3.8.1/tw/transform/__init__.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/models/
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/models/transformer2d/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/transformer2d/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    31891 2022-01-28 06:57:43.000000 tw-3.8.1/tw/models/transformer2d/vit.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8239 2021-11-27 08:05:31.000000 tw-3.8.1/tw/models/res2net_v1b.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7860 2021-11-27 08:05:31.000000 tw-3.8.1/tw/models/ghostnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10531 2021-06-02 02:57:54.000000 tw-3.8.1/tw/models/mnasnet.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/models/backbone3d/
--rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)    13476 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone3d/r2plus1d.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2984 2021-11-27 08:05:31.000000 tw-3.8.1/tw/models/backbone3d/c3d.py
--rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)     9854 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone3d/p3d.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     9438 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone3d/i3d.py
--rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)     9067 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone3d/p3d_without_bn.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone3d/__init__.py
--rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)    10081 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone3d/r3d.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5560 2021-11-27 08:05:31.000000 tw-3.8.1/tw/models/resnets_deeplab.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11534 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/mixnet.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/models/backbone2d/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2462 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/alexnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2112 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/vgg_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    17150 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone2d/mobilenet_v3.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5930 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/resnet_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4736 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/mobilenet_v2.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6613 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone2d/resnet_tf.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3446 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone2d/shufflenet_v1_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5611 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone2d/squeezenet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    15646 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/senet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5219 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/efficientnet_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5882 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone2d/shufflenet_v2_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7275 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/vgg.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3782 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone2d/mobilenet_v2_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5134 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/senet_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6144 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/mobilenet_v2_deeplab.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10154 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone2d/googlenet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7537 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/shufflenet_v2.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8103 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/xception.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    47009 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/resnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6413 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/vgg_extractor.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7791 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/densenet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1551 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/backbone2d/bcnn.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12022 2021-11-27 08:05:33.000000 tw-3.8.1/tw/models/backbone2d/inceptionresnetv2.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3849 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/backbone2d/densenet_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)   127717 2021-11-27 08:05:37.000000 tw-3.8.1/tw/models/backbone2d/efficientnet.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/models/segment3d/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment3d/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2556 2022-01-28 06:57:43.000000 tw-3.8.1/tw/models/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3020 2021-06-26 14:23:47.000000 tw-3.8.1/tw/models/mobilenet_v1.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    15416 2021-06-02 02:57:54.000000 tw-3.8.1/tw/models/inception.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8989 2021-11-27 08:05:32.000000 tw-3.8.1/tw/models/res2net.py
-drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-02-02 06:42:25.000000 tw-3.8.1/tw/models/segment2d/
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8526 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/fastscnn.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7631 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/enet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8323 2021-11-27 08:05:33.000000 tw-3.8.1/tw/models/segment2d/frvsr.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11102 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/espnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    16115 2021-11-27 08:05:33.000000 tw-3.8.1/tw/models/segment2d/fenet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10654 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/ocnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6506 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/bisenet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4270 2021-11-27 08:05:33.000000 tw-3.8.1/tw/models/segment2d/deeplabv3p.py
--rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)     1498 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/lenet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6797 2021-11-27 08:05:33.000000 tw-3.8.1/tw/models/segment2d/erfnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    37948 2021-11-27 08:05:34.000000 tw-3.8.1/tw/models/segment2d/poolnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6078 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/lednet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12386 2021-11-27 08:05:33.000000 tw-3.8.1/tw/models/segment2d/drn.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4941 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/icnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3620 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/psanet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3334 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/pspnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4041 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/dunet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2764 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/ccnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/__init__.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5431 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/danet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4335 2021-11-27 08:05:33.000000 tw-3.8.1/tw/models/segment2d/fcn.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5864 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/encnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3642 2021-11-27 08:05:33.000000 tw-3.8.1/tw/models/segment2d/asffnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4155 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/utils.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3909 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/unet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    26039 2021-11-27 08:05:34.000000 tw-3.8.1/tw/models/segment2d/bgmv2.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5974 2021-07-17 07:17:13.000000 tw-3.8.1/tw/models/segment2d/cgnet.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6508 2021-11-27 08:05:31.000000 tw-3.8.1/tw/models/moco.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5285 2021-06-02 02:57:54.000000 tw-3.8.1/tw/models/resnext_cifar.py
--rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4100 2022-02-02 06:41:35.000000 tw-3.8.1/setup.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2744 2022-03-16 02:59:09.000000 tw-3.9.0/README.md
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4057 2022-05-26 04:22:35.000000 tw-3.9.0/setup.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)       38 2022-05-26 04:23:51.000000 tw-3.9.0/setup.cfg
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/optim/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      737 2022-03-16 02:59:09.000000 tw-3.9.0/tw/optim/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2294 2022-03-16 02:59:09.000000 tw-3.9.0/tw/optim/warmup_multistep_lr.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      939 2022-03-16 02:59:09.000000 tw-3.9.0/tw/optim/poly_lr.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/datasets/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7989 2022-05-21 04:34:50.000000 tw-3.9.0/tw/datasets/optical_flow.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    18173 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/point_cloud.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1927 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3852 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/pil.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2016 2022-05-21 12:00:41.000000 tw-3.9.0/tw/datasets/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1328 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/mnist.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4469 2022-05-21 04:34:50.000000 tw-3.9.0/tw/datasets/super_resolution.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4393 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/denoise.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4761 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/coco.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3462 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/avec2014.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4401 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/widerface.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1356 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/imagenet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    27814 2022-03-16 02:59:09.000000 tw-3.9.0/tw/datasets/quality_assess.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     9867 2022-03-24 12:21:19.000000 tw-3.9.0/tw/datasets/general.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    14088 2022-05-21 04:34:50.000000 tw-3.9.0/tw/datasets/face.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11188 2022-05-25 07:44:42.000000 tw-3.9.0/tw/datasets/facemesh.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3273 2022-05-21 04:34:50.000000 tw-3.9.0/tw/datasets/base.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1545 2022-05-24 07:47:33.000000 tw-3.9.0/tw/__init__.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/media/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    23209 2022-05-24 08:46:14.000000 tw-3.9.0/tw/media/mesh.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      952 2022-03-16 02:59:09.000000 tw-3.9.0/tw/media/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4307 2022-03-16 02:59:09.000000 tw-3.9.0/tw/media/raw.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10704 2022-05-21 04:34:50.000000 tw-3.9.0/tw/media/media.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10247 2022-03-16 02:59:09.000000 tw-3.9.0/tw/media/ply.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11194 2022-05-21 04:34:50.000000 tw-3.9.0/tw/media/flow.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_alignment/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_alignment/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      771 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/__init__.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_detection/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1025 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/__init__.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_detection/retinaface/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3542 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/retinaface/retinaface.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3115 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/retinaface/data_utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/retinaface/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    14132 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/retinaface/box_utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10477 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/retinaface/nets.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_detection/dsfd/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/dsfd/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7194 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/dsfd/box_utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2558 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/dsfd/dsfd.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10006 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/dsfd/nets.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_detection/s3fd/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/s3fd/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7122 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/s3fd/box_utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2549 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/s3fd/s3fd.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5670 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/s3fd/nets.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_detection/pyramidbox/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2587 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/pyramidbox/pyramidbox.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/pyramidbox/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6770 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/pyramidbox/box_utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     9370 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/pyramidbox/nets.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_detection/tinyface/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/tinyface/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3624 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/tinyface/box_utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4390 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/tinyface/tinyface.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2365 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/tinyface/nets.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_detection/faceboxes/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/faceboxes/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3930 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/faceboxes/box_utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4866 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/faceboxes/nets.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2944 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/faceboxes/faceboxes.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_detection/mtcnn/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/mtcnn/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7169 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/mtcnn/box_utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4593 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/mtcnn/mtcnn.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4115 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/mtcnn/nets.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3679 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_detection/mtcnn/first_stage.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/contrib/face_landmark/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    18546 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_landmark/mobileface.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      720 2022-03-16 02:59:09.000000 tw-3.9.0/tw/contrib/face_landmark/__init__.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/tools/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      995 2022-03-16 02:59:09.000000 tw-3.9.0/tw/tools/checkpoint.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1686 2022-03-16 02:59:09.000000 tw-3.9.0/tw/tools/busy.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1033 2022-03-16 02:59:09.000000 tw-3.9.0/tw/tools/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6898 2022-05-21 04:34:50.000000 tw-3.9.0/tw/tools/event.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1572 2022-03-16 02:59:09.000000 tw-3.9.0/tw/tools/media.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6583 2022-03-16 02:59:09.000000 tw-3.9.0/tw/tools/monitor.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/models/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8239 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/res2net_v1b.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/models/segment3d/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment3d/__init__.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/models/segment2d/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12386 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/drn.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3642 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/asffnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3334 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/pspnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11102 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/espnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8323 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/frvsr.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    26039 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/bgmv2.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5974 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/cgnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4270 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/deeplabv3p.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    37948 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/poolnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6797 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/erfnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8526 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/fastscnn.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4041 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/dunet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2764 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/ccnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3620 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/psanet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4941 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/icnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    16115 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/fenet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7631 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/enet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5864 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/encnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4155 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/utils.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6078 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/lednet.py
+-rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)     1498 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/lenet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4335 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/fcn.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10654 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/ocnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6506 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/bisenet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3909 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/unet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5431 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/segment2d/danet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7860 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/ghostnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3020 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/mobilenet_v1.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10531 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/mnasnet.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/models/optical_flow/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-24 12:21:19.000000 tw-3.9.0/tw/models/optical_flow/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7233 2022-03-24 12:21:19.000000 tw-3.9.0/tw/models/optical_flow/spynet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2556 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6508 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/moco.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5560 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/resnets_deeplab.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5285 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/resnext_cifar.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/models/backbone3d/
+-rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)    10081 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone3d/r3d.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     9438 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone3d/i3d.py
+-rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)     9067 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone3d/p3d_without_bn.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone3d/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2984 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone3d/c3d.py
+-rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)     9854 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone3d/p3d.py
+-rwxrwxr-x   0 jinkai   (20403) jinkai   (20403)    13476 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone3d/r2plus1d.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/models/backbone2d/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3446 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/shufflenet_v1_cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5930 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/resnet_cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4786 2022-05-25 09:09:09.000000 tw-3.9.0/tw/models/backbone2d/mobilenet_v2.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12022 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/inceptionresnetv2.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5882 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/shufflenet_v2_cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7537 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/shufflenet_v2.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7791 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/densenet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)   127717 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/efficientnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    15646 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/senet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    47009 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/resnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7275 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/vgg.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10154 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/googlenet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2112 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/vgg_cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6413 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/vgg_extractor.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5219 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/efficientnet_cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1551 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/bcnn.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5134 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/senet_cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2462 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/alexnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5611 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/squeezenet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3782 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/mobilenet_v2_cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3849 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/densenet_cifar.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6613 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/resnet_tf.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6144 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/mobilenet_v2_deeplab.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8103 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/xception.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    17150 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/backbone2d/mobilenet_v3.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/models/transformer2d/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    31891 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/transformer2d/vit.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/transformer2d/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11534 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/mixnet.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    15416 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/inception.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8989 2022-03-16 02:59:09.000000 tw-3.9.0/tw/models/res2net.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/transform/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    17790 2022-05-21 04:34:50.000000 tw-3.9.0/tw/transform/meta.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/transform/primitive/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10257 2022-05-21 04:34:50.000000 tw-3.9.0/tw/transform/primitive/filter.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     8481 2022-03-16 02:59:09.000000 tw-3.9.0/tw/transform/primitive/resize.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    20615 2022-03-16 02:59:09.000000 tw-3.9.0/tw/transform/primitive/crop.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    10357 2022-05-24 09:13:38.000000 tw-3.9.0/tw/transform/primitive/normalize.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12688 2022-03-16 02:59:09.000000 tw-3.9.0/tw/transform/primitive/pad.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5819 2022-03-16 02:59:09.000000 tw-3.9.0/tw/transform/primitive/bbox.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        0 2022-03-16 02:59:09.000000 tw-3.9.0/tw/transform/primitive/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12698 2022-05-21 04:34:50.000000 tw-3.9.0/tw/transform/primitive/colorspace.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    18191 2022-05-21 04:34:50.000000 tw-3.9.0/tw/transform/primitive/affine.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3366 2022-03-16 02:59:09.000000 tw-3.9.0/tw/transform/primitive/morphology.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4727 2022-03-16 02:59:09.000000 tw-3.9.0/tw/transform/pil.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3793 2022-05-21 04:34:50.000000 tw-3.9.0/tw/transform/__init__.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/evaluator/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5534 2022-05-21 04:34:50.000000 tw-3.9.0/tw/evaluator/optical_flow.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4634 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/classification.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2554 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/verification.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1536 2022-05-21 04:34:50.000000 tw-3.9.0/tw/evaluator/regression.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1487 2022-05-21 04:34:50.000000 tw-3.9.0/tw/evaluator/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2703 2022-05-21 04:34:50.000000 tw-3.9.0/tw/evaluator/landmark.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7062 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/detection.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6811 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/avec2014.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    14169 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/segmentation.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     9203 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/widerface.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2665 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/quality_assess.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3681 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/image.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1694 2022-03-16 02:59:09.000000 tw-3.9.0/tw/evaluator/base.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/utils/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4837 2022-05-24 10:02:30.000000 tw-3.9.0/tw/utils/checkpoint.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     2809 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/stat.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3898 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/logger.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6023 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/runner.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      685 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3053 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/export.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1023 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/tensorboard.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    14972 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/flops.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3418 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/parser.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1953 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/timer.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6702 2022-05-22 09:11:27.000000 tw-3.9.0/tw/utils/drawer.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3837 2022-03-16 02:59:09.000000 tw-3.9.0/tw/utils/filesystem.py
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw/nn/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1847 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/filter.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1833 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/interpolate.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5899 2022-05-24 09:37:35.000000 tw-3.9.0/tw/nn/render.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7615 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/normalize.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5308 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/convert.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5424 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/initialize.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1812 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/activation.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    12655 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/attention.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6453 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/bbox.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     1539 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/search.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4631 2022-05-21 04:34:50.000000 tw-3.9.0/tw/nn/__init__.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     4626 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/embedding.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    37482 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/conv.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      734 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/functional.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7390 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/drop.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     7658 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/fft.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3905 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/nms.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    15312 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/rnn.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5210 2022-05-21 04:34:50.000000 tw-3.9.0/tw/nn/correlation.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     5016 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/keypoints.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)      753 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/transformer.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    18328 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/anchor.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11526 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/fpn.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3743 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/sample.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    11753 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/head.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    68813 2022-05-21 04:34:50.000000 tw-3.9.0/tw/nn/losses.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)    22408 2022-03-16 02:59:09.000000 tw-3.9.0/tw/nn/pooling.py
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3463 2022-05-26 04:23:51.000000 tw-3.9.0/PKG-INFO
+drwxrwxr-x   0 jinkai   (20403) jinkai   (20403)        0 2022-05-26 04:23:51.000000 tw-3.9.0/tw.egg-info/
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        1 2022-05-26 04:23:51.000000 tw-3.9.0/tw.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     6226 2022-05-26 04:23:51.000000 tw-3.9.0/tw.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)     3463 2022-05-26 04:23:51.000000 tw-3.9.0/tw.egg-info/PKG-INFO
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)        3 2022-05-26 04:23:51.000000 tw-3.9.0/tw.egg-info/top_level.txt
+-rw-rw-r--   0 jinkai   (20403) jinkai   (20403)       47 2022-05-26 04:23:51.000000 tw-3.9.0/tw.egg-info/requires.txt
```

### Comparing `tw-3.8.1/README.md` & `tw-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw.egg-info/PKG-INFO` & `tw-3.9.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,100 +1,102 @@
 Metadata-Version: 2.1
 Name: tw
-Version: 3.8.1
+Version: 3.9.0
 Summary: TorchWrapper is a deep learning helper.
 Home-page: https://github.com/atranitell/TensorWrapper
 Author: Kai Jin
 Author-email: atranitell@gmail.com
 License: Apache 2.0 Licence
-Description: 
-        # TensorWrapper
-        TensorWrapper is a extension library for PyTorch framework. It aims to supplement a few of common components: newest optimizer, opeartors, utils, drawer, common structure and etc.
-        
-        ## Installation
-        ```bash
-        # install 3rd pip depedency.
-        pip install cython matplotlib opencv-python numpy tensorboard future memory_profiler profilehooks tqdm scipy scikit-image
-        HOROVOD_GPU_OPERATIONS=NCCL pip install horovod
-        ```
-        
-        ## Distributed Train/Val
-        
-        **Install openmpi**
-        ```bash
-        # install openmpi 4.0 version
-        curl -O -L https://download.open-mpi.org/release/open-mpi/v4.0/openmpi-4.0.1.tar.gz
-        tar xvzf openmpi-4.0.1.tar.gz
-        ./configure --prefix=/usr/local
-        make all && sudo make install
-        export PATH=/usr/local/bin:$PATH
-        
-        # or via conda
-        conda install openmpi
-        ```
-        
-        **Install NCCL**
-        ```bash
-        # download nccl library: https://developer.nvidia.com/nccl/nccl-legacy-downloads
-        # O/S agnostic local installer
-        # e.g. nccl_2.6.4-1+cuda10.0_x86_64.txz
-        
-        # or using deb fashion
-        # https://developer.nvidia.com/compute/machine-learning/nccl/secure/v2.6/prod/nccl-repo-ubuntu1604-2.6.4-ga-cuda10.0_1-1_amd64.deb
-        sudo apt install libnccl2=2.6.4-1+cuda10.0 libnccl-dev=2.6.4-1+cuda10.0
-        sudo apt install libnccl2=2.6.4-1+cuda10.1 libnccl-dev=2.6.4-1+cuda10.1
-        export LD_LIBRARY_PATH=`pwd`/nccl_2.6.4-1+cuda10.0_x86_64/lib:$LD_LIBRARY_PATH
-        ```
-        
-        **Install Horovod**
-        ```bash
-        HOROVOD_GPU_OPERATIONS=NCCL pip install horovod --no-cache-dir
-        
-        git config --global user.email "atranitell@gmail.com" && git config --global user.name "jk"
-        ```
-        
-        **Install CMake**
-        ```bash
-        # install cmake
-        # https://cmake.org/files/v3.14/
-        ```
-        
-        **Train**
-        ```bash
-        # demo for verificaiton distributed traning
-        cd research/Classifier
-        
-        # execute single node for mnist, note that batch size is set to 128
-        python Classifier.py --config configs/Classifier_Mnist_LeNet.py
-        
-        # execute 4 node with 4 gpu, note that batch size should be set to 32
-        python -m tw.api.launch --np 4 --device cuda python Classifier.py --config configs/Classifier_Mnist_LeNet.py
-        
-        # monitor the validation result, the test error should be similiar.
-        ```
-        
-        ## Usage
-        
-        ```bash
-        # dist train
-        python -m tw.api.launch --np 2 --dev cuda python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task train
-        
-        # dist eval
-        python -m tw.api.launch --np 2 --dev cuda python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task test
-        
-        # single train
-        python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task train
-        
-        # single eval
-        python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task test
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+
+
+# TensorWrapper
+TensorWrapper is a extension library for PyTorch framework. It aims to supplement a few of common components: newest optimizer, opeartors, utils, drawer, common structure and etc.
+
+## Installation
+```bash
+# install 3rd pip depedency.
+pip install cython matplotlib opencv-python numpy tensorboard future memory_profiler profilehooks tqdm scipy scikit-image
+HOROVOD_GPU_OPERATIONS=NCCL pip install horovod
+```
+
+## Distributed Train/Val
+
+**Install openmpi**
+```bash
+# install openmpi 4.0 version
+curl -O -L https://download.open-mpi.org/release/open-mpi/v4.0/openmpi-4.0.1.tar.gz
+tar xvzf openmpi-4.0.1.tar.gz
+./configure --prefix=/usr/local
+make all && sudo make install
+export PATH=/usr/local/bin:$PATH
+
+# or via conda
+conda install openmpi
+```
+
+**Install NCCL**
+```bash
+# download nccl library: https://developer.nvidia.com/nccl/nccl-legacy-downloads
+# O/S agnostic local installer
+# e.g. nccl_2.6.4-1+cuda10.0_x86_64.txz
+
+# or using deb fashion
+# https://developer.nvidia.com/compute/machine-learning/nccl/secure/v2.6/prod/nccl-repo-ubuntu1604-2.6.4-ga-cuda10.0_1-1_amd64.deb
+sudo apt install libnccl2=2.6.4-1+cuda10.0 libnccl-dev=2.6.4-1+cuda10.0
+sudo apt install libnccl2=2.6.4-1+cuda10.1 libnccl-dev=2.6.4-1+cuda10.1
+export LD_LIBRARY_PATH=`pwd`/nccl_2.6.4-1+cuda10.0_x86_64/lib:$LD_LIBRARY_PATH
+```
+
+**Install Horovod**
+```bash
+HOROVOD_GPU_OPERATIONS=NCCL pip install horovod --no-cache-dir
+
+git config --global user.email "atranitell@gmail.com" && git config --global user.name "jk"
+```
+
+**Install CMake**
+```bash
+# install cmake
+# https://cmake.org/files/v3.14/
+```
+
+**Train**
+```bash
+# demo for verificaiton distributed traning
+cd research/Classifier
+
+# execute single node for mnist, note that batch size is set to 128
+python Classifier.py --config configs/Classifier_Mnist_LeNet.py
+
+# execute 4 node with 4 gpu, note that batch size should be set to 32
+python -m tw.api.launch --np 4 --device cuda python Classifier.py --config configs/Classifier_Mnist_LeNet.py
+
+# monitor the validation result, the test error should be similiar.
+```
+
+## Usage
+
+```bash
+# dist train
+python -m tw.api.launch --np 2 --dev cuda python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task train
+
+# dist eval
+python -m tw.api.launch --np 2 --dev cuda python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task test
+
+# single train
+python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task train
+
+# single eval
+python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task test
+```
+
+
```

### Comparing `tw-3.8.1/tw.egg-info/SOURCES.txt` & `tw-3.9.0/tw.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,38 +43,44 @@
 tw/contrib/face_landmark/mobileface.py
 tw/datasets/__init__.py
 tw/datasets/avec2014.py
 tw/datasets/base.py
 tw/datasets/cifar.py
 tw/datasets/coco.py
 tw/datasets/denoise.py
+tw/datasets/face.py
+tw/datasets/facemesh.py
 tw/datasets/general.py
 tw/datasets/imagenet.py
 tw/datasets/mnist.py
+tw/datasets/optical_flow.py
 tw/datasets/pil.py
 tw/datasets/point_cloud.py
 tw/datasets/quality_assess.py
 tw/datasets/super_resolution.py
 tw/datasets/widerface.py
 tw/evaluator/__init__.py
 tw/evaluator/avec2014.py
 tw/evaluator/base.py
 tw/evaluator/classification.py
 tw/evaluator/detection.py
 tw/evaluator/image.py
+tw/evaluator/landmark.py
+tw/evaluator/optical_flow.py
 tw/evaluator/quality_assess.py
 tw/evaluator/regression.py
 tw/evaluator/segmentation.py
 tw/evaluator/verification.py
 tw/evaluator/widerface.py
 tw/media/__init__.py
+tw/media/flow.py
 tw/media/media.py
+tw/media/mesh.py
 tw/media/ply.py
 tw/media/raw.py
-tw/media/yuv.py
 tw/models/__init__.py
 tw/models/ghostnet.py
 tw/models/inception.py
 tw/models/mixnet.py
 tw/models/mnasnet.py
 tw/models/mobilenet_v1.py
 tw/models/moco.py
@@ -111,14 +117,16 @@
 tw/models/backbone3d/__init__.py
 tw/models/backbone3d/c3d.py
 tw/models/backbone3d/i3d.py
 tw/models/backbone3d/p3d.py
 tw/models/backbone3d/p3d_without_bn.py
 tw/models/backbone3d/r2plus1d.py
 tw/models/backbone3d/r3d.py
+tw/models/optical_flow/__init__.py
+tw/models/optical_flow/spynet.py
 tw/models/segment2d/__init__.py
 tw/models/segment2d/asffnet.py
 tw/models/segment2d/bgmv2.py
 tw/models/segment2d/bisenet.py
 tw/models/segment2d/ccnet.py
 tw/models/segment2d/cgnet.py
 tw/models/segment2d/danet.py
@@ -148,28 +156,30 @@
 tw/nn/__init__.py
 tw/nn/activation.py
 tw/nn/anchor.py
 tw/nn/attention.py
 tw/nn/bbox.py
 tw/nn/conv.py
 tw/nn/convert.py
+tw/nn/correlation.py
 tw/nn/drop.py
 tw/nn/embedding.py
 tw/nn/fft.py
 tw/nn/filter.py
 tw/nn/fpn.py
 tw/nn/functional.py
 tw/nn/head.py
 tw/nn/initialize.py
 tw/nn/interpolate.py
 tw/nn/keypoints.py
 tw/nn/losses.py
 tw/nn/nms.py
 tw/nn/normalize.py
 tw/nn/pooling.py
+tw/nn/render.py
 tw/nn/rnn.py
 tw/nn/sample.py
 tw/nn/search.py
 tw/nn/transformer.py
 tw/optim/__init__.py
 tw/optim/poly_lr.py
 tw/optim/warmup_multistep_lr.py
```

### Comparing `tw-3.8.1/PKG-INFO` & `tw-3.9.0/tw.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,100 +1,102 @@
 Metadata-Version: 2.1
 Name: tw
-Version: 3.8.1
+Version: 3.9.0
 Summary: TorchWrapper is a deep learning helper.
 Home-page: https://github.com/atranitell/TensorWrapper
 Author: Kai Jin
 Author-email: atranitell@gmail.com
 License: Apache 2.0 Licence
-Description: 
-        # TensorWrapper
-        TensorWrapper is a extension library for PyTorch framework. It aims to supplement a few of common components: newest optimizer, opeartors, utils, drawer, common structure and etc.
-        
-        ## Installation
-        ```bash
-        # install 3rd pip depedency.
-        pip install cython matplotlib opencv-python numpy tensorboard future memory_profiler profilehooks tqdm scipy scikit-image
-        HOROVOD_GPU_OPERATIONS=NCCL pip install horovod
-        ```
-        
-        ## Distributed Train/Val
-        
-        **Install openmpi**
-        ```bash
-        # install openmpi 4.0 version
-        curl -O -L https://download.open-mpi.org/release/open-mpi/v4.0/openmpi-4.0.1.tar.gz
-        tar xvzf openmpi-4.0.1.tar.gz
-        ./configure --prefix=/usr/local
-        make all && sudo make install
-        export PATH=/usr/local/bin:$PATH
-        
-        # or via conda
-        conda install openmpi
-        ```
-        
-        **Install NCCL**
-        ```bash
-        # download nccl library: https://developer.nvidia.com/nccl/nccl-legacy-downloads
-        # O/S agnostic local installer
-        # e.g. nccl_2.6.4-1+cuda10.0_x86_64.txz
-        
-        # or using deb fashion
-        # https://developer.nvidia.com/compute/machine-learning/nccl/secure/v2.6/prod/nccl-repo-ubuntu1604-2.6.4-ga-cuda10.0_1-1_amd64.deb
-        sudo apt install libnccl2=2.6.4-1+cuda10.0 libnccl-dev=2.6.4-1+cuda10.0
-        sudo apt install libnccl2=2.6.4-1+cuda10.1 libnccl-dev=2.6.4-1+cuda10.1
-        export LD_LIBRARY_PATH=`pwd`/nccl_2.6.4-1+cuda10.0_x86_64/lib:$LD_LIBRARY_PATH
-        ```
-        
-        **Install Horovod**
-        ```bash
-        HOROVOD_GPU_OPERATIONS=NCCL pip install horovod --no-cache-dir
-        
-        git config --global user.email "atranitell@gmail.com" && git config --global user.name "jk"
-        ```
-        
-        **Install CMake**
-        ```bash
-        # install cmake
-        # https://cmake.org/files/v3.14/
-        ```
-        
-        **Train**
-        ```bash
-        # demo for verificaiton distributed traning
-        cd research/Classifier
-        
-        # execute single node for mnist, note that batch size is set to 128
-        python Classifier.py --config configs/Classifier_Mnist_LeNet.py
-        
-        # execute 4 node with 4 gpu, note that batch size should be set to 32
-        python -m tw.api.launch --np 4 --device cuda python Classifier.py --config configs/Classifier_Mnist_LeNet.py
-        
-        # monitor the validation result, the test error should be similiar.
-        ```
-        
-        ## Usage
-        
-        ```bash
-        # dist train
-        python -m tw.api.launch --np 2 --dev cuda python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task train
-        
-        # dist eval
-        python -m tw.api.launch --np 2 --dev cuda python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task test
-        
-        # single train
-        python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task train
-        
-        # single eval
-        python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task test
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+
+
+# TensorWrapper
+TensorWrapper is a extension library for PyTorch framework. It aims to supplement a few of common components: newest optimizer, opeartors, utils, drawer, common structure and etc.
+
+## Installation
+```bash
+# install 3rd pip depedency.
+pip install cython matplotlib opencv-python numpy tensorboard future memory_profiler profilehooks tqdm scipy scikit-image
+HOROVOD_GPU_OPERATIONS=NCCL pip install horovod
+```
+
+## Distributed Train/Val
+
+**Install openmpi**
+```bash
+# install openmpi 4.0 version
+curl -O -L https://download.open-mpi.org/release/open-mpi/v4.0/openmpi-4.0.1.tar.gz
+tar xvzf openmpi-4.0.1.tar.gz
+./configure --prefix=/usr/local
+make all && sudo make install
+export PATH=/usr/local/bin:$PATH
+
+# or via conda
+conda install openmpi
+```
+
+**Install NCCL**
+```bash
+# download nccl library: https://developer.nvidia.com/nccl/nccl-legacy-downloads
+# O/S agnostic local installer
+# e.g. nccl_2.6.4-1+cuda10.0_x86_64.txz
+
+# or using deb fashion
+# https://developer.nvidia.com/compute/machine-learning/nccl/secure/v2.6/prod/nccl-repo-ubuntu1604-2.6.4-ga-cuda10.0_1-1_amd64.deb
+sudo apt install libnccl2=2.6.4-1+cuda10.0 libnccl-dev=2.6.4-1+cuda10.0
+sudo apt install libnccl2=2.6.4-1+cuda10.1 libnccl-dev=2.6.4-1+cuda10.1
+export LD_LIBRARY_PATH=`pwd`/nccl_2.6.4-1+cuda10.0_x86_64/lib:$LD_LIBRARY_PATH
+```
+
+**Install Horovod**
+```bash
+HOROVOD_GPU_OPERATIONS=NCCL pip install horovod --no-cache-dir
+
+git config --global user.email "atranitell@gmail.com" && git config --global user.name "jk"
+```
+
+**Install CMake**
+```bash
+# install cmake
+# https://cmake.org/files/v3.14/
+```
+
+**Train**
+```bash
+# demo for verificaiton distributed traning
+cd research/Classifier
+
+# execute single node for mnist, note that batch size is set to 128
+python Classifier.py --config configs/Classifier_Mnist_LeNet.py
+
+# execute 4 node with 4 gpu, note that batch size should be set to 32
+python -m tw.api.launch --np 4 --device cuda python Classifier.py --config configs/Classifier_Mnist_LeNet.py
+
+# monitor the validation result, the test error should be similiar.
+```
+
+## Usage
+
+```bash
+# dist train
+python -m tw.api.launch --np 2 --dev cuda python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task train
+
+# dist eval
+python -m tw.api.launch --np 2 --dev cuda python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task test
+
+# single train
+python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task train
+
+# single eval
+python research/classification/Classifier.py --config research/classification/configs/Classifier_ImageNet_AlexNet.py --task test
+```
+
+
```

### Comparing `tw-3.8.1/tw/nn/filter.py` & `tw-3.9.0/tw/nn/filter.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/pooling.py` & `tw-3.9.0/tw/nn/pooling.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/functional.py` & `tw-3.9.0/tw/nn/functional.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/nms.py` & `tw-3.9.0/tw/nn/nms.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/convert.py` & `tw-3.9.0/tw/nn/convert.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/initialize.py` & `tw-3.9.0/tw/nn/initialize.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/rnn.py` & `tw-3.9.0/tw/nn/rnn.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/normalize.py` & `tw-3.9.0/tw/nn/normalize.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/drop.py` & `tw-3.9.0/tw/nn/drop.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/sample.py` & `tw-3.9.0/tw/nn/sample.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/search.py` & `tw-3.9.0/tw/nn/search.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/attention.py` & `tw-3.9.0/tw/nn/attention.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/keypoints.py` & `tw-3.9.0/tw/nn/keypoints.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/head.py` & `tw-3.9.0/tw/nn/head.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/fft.py` & `tw-3.9.0/tw/nn/fft.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/__init__.py` & `tw-3.9.0/tw/nn/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
 from .convert import EmptyConv2d
 from .convert import EmptyConvTranspose2d
 from .convert import EmptyBatchNorm2d
 from .convert import EmptyLayer
 from .convert import FrozenBatchNorm2d
 
+from .correlation import CorrLookup
+
 from .drop import DropBlock2d
 from .drop import DropPath
 
 from .embedding import AngleLinear
 
 from . import initialize
 from . import losses
@@ -84,14 +86,24 @@
 from .losses import DIoULoss
 from .losses import GIoULoss
 from .losses import IoULoss
 
 from .losses import MonotonicityRelatedLoss
 from .losses import PLCCLoss
 
+from .losses import LaplacianLoss
+from .losses import NMELoss
+from .losses import WingLoss
+from .losses import SmoothWingLoss
+from .losses import WiderWingLoss
+from .losses import NormalizedWiderWingLoss
+
+from .losses import MultiLevelEPELoss
+from .losses import MultiLevelCharbonnierLoss
+
 from .nms import MulticlassNMS
 from .nms import MultiLabelNonMaxSuppression
 from .nms import NonMaxSuppression
 
 from .normalize import L2Norm
 from .normalize import Scale
```

### Comparing `tw-3.8.1/tw/nn/losses.py` & `tw-3.9.0/tw/nn/losses.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-r"""Losses collections
+"""Losses collections
 """
 
 import itertools
 import math
+
+import scipy.sparse as sp
 import numpy as np
+
 import torch
 from torch import nn
 import torch.nn.functional as F
+from torch.nn.modules.loss import _Loss
 
 # for autograd
 from torch.autograd.function import once_differentiable
 
 try:
   from tw import _C
 except ImportError:
@@ -56,14 +60,22 @@
     "SigmoidFocalLoss",
     "OrderSensitiveMetricLoss",
     "MutualChannelLoss",
     "LabelSmoothLoss",
     "EBMLoss",
     "MonotonicityRelatedLoss",
     "PLCCLoss",
+    "LaplacianLoss",
+    "NMELoss",
+    "WingLoss",
+    "SmoothWingLoss",
+    "WiderWingLoss",
+    "NormalizedWiderWingLoss",
+    "MultiLevelEPELoss",
+    "MultiLevelCharbonnierLoss",
 ]
 
 
 #!<-----------------------------------------------------------------------------
 #!<  spatial Loss
 #!<-----------------------------------------------------------------------------
 
@@ -1582,7 +1594,609 @@
         inputs ([N, C]): inputs value
         targets ([N, C]): targets value
     """
     bs = inputs.size(0)
     assert inputs.ndim == targets.ndim == 2
     assert bs > 1, "at least input number larger than 2."
     return (1 - torch.cosine_similarity(inputs.t() - torch.mean(inputs), targets.t() - torch.mean(targets))[0]) / 2
+
+#!<-----------------------------------------------------------------------------
+#!< Face alignment related loss
+#!< https://github.com/BeierZhu/Sturcture-Coherency-Face-Alignment
+#!<-----------------------------------------------------------------------------
+
+
+def gen_laplacian_matrix(num_points, top_k):
+  """
+  Return 106 x 106 matrix
+  """
+  if num_points == 98:
+    connection = np.loadtxt(f'utils/face_graph/{num_points}pts_top{top_k}.txt')
+  else:
+    connection = np.loadtxt(f'utils/face_graph/{num_points}pts.txt')
+
+  return adj_mx_from_list(connection, num_points)
+
+
+def adj_mx_from_list(connection, num_points):
+  edges = connection[:, :2]
+  return adj_mx_from_weighted_edges(num_points, edges)
+
+
+def adj_mx_from_weighted_edges(num_pts, edges):
+  edges = np.array(edges, dtype=np.int32)
+  weights = np.ones(edges.shape[0])
+  data, i, j = weights, edges[:, 0], edges[:, 1]
+  adj_mx = sp.coo_matrix((data, (i, j)), shape=(num_pts, num_pts), dtype=np.float32).todense()
+
+  np.fill_diagonal(adj_mx, 0)
+  row_sum = adj_mx.sum(axis=1)
+  row_sum[row_sum == 0] = 1
+  adj_mx /= row_sum
+  np.fill_diagonal(adj_mx, -1)
+
+  adj_mx = torch.tensor(adj_mx, dtype=torch.float)
+  return adj_mx.unsqueeze(0)
+
+
+class LaplacianLoss(_Loss):
+  def __init__(self, loss, num_points, reduction="mean"):
+    super(LaplacianLoss, self).__init__(reduction=reduction)
+    self.loss = loss
+    self.num_points = num_points
+    self.laplacian_matrix = gen_laplacian_matrix(num_points, 3).cuda()  # 106x106
+
+  def forward(self, prediction, target):
+    prediction = prediction.reshape(-1, self.num_points, 2)
+    target = target.reshape(-1, self.num_points, 2)
+    prediction = torch.matmul(self.laplacian_matrix, prediction)
+    target = torch.matmul(self.laplacian_matrix, target)
+    prediction = prediction.reshape(-1, self.num_points*2)
+    target = target.reshape(-1, self.num_points*2)
+
+    return self.loss(prediction, target)
+
+
+def nme_loss(prediction: torch.Tensor, target: torch.Tensor, num_points, image_size=256, reduction="mean"):
+  """
+  normalized_wider_wing = 
+      1. C/d * |x|                           , if |x| < thres1
+      2. C/d * (thres2*ln(1+|x|/curvature) + B), if |x| >= thres2
+  """
+  assert prediction.size() == target.size(), 'input tensors must have the same size'
+
+  # Calculate Euclidean distances between actual and target locations
+  diff = prediction - target
+  diff = diff.reshape(diff.size(0), -1, 2)
+  dist_sq = diff.pow(2).sum(-1, keepdim=False)
+  loss = dist_sq.sqrt()  # shape (B x N)
+
+  if num_points == 29:
+    le_idx = [8]
+    re_idx = [9]
+
+  if num_points == 68:
+    le_idx = [36]  # le = left eye
+    re_idx = [45]  # re = right eye
+
+  if num_points == 98:
+    le_idx = [60]
+    re_idx = [72]
+
+  target = target.reshape(-1, num_points, 2)
+  le_loc = torch.mean(target[:, le_idx, :], dim=1)  # batchsize x 2
+  re_loc = torch.mean(target[:, re_idx, :], dim=1)
+
+  norm_dist = torch.sqrt(torch.sum((le_loc - re_loc)**2, dim=1))  # batchsize
+  factor = image_size/norm_dist
+
+  if reduction == "sum":
+    loss = loss.sum(dim=1)
+    loss *= factor
+    loss = loss.sum()
+
+  if reduction == "mean":
+    loss = loss.mean(dim=1)
+    loss *= factor
+    loss = loss.mean()
+
+  return loss
+
+
+class NMELoss(_Loss):
+  """docstring for NMELoss"""
+
+  def __init__(self, num_points, image_size, reduction="mean"):
+    super(NMELoss, self).__init__(reduction=reduction)
+    self.num_points = num_points
+    self.image_size = image_size
+
+  def forward(self, prediction, target):
+    return nme_loss(prediction, target,
+                    num_points=self.num_points,
+                    image_size=self.image_size,
+                    reduction=self.reduction)
+
+
+def wing_loss(prediction: torch.Tensor, target: torch.Tensor, width=5, curvature=0.5, reduction="mean"):
+  """
+  https://arxiv.org/pdf/1711.06753.pdf
+  :param prediction:
+  :param target:
+  :param width:
+  :param curvature:
+  :param reduction:
+  :return:
+  """
+  diff_abs = (target - prediction).abs()
+  loss = diff_abs.clone()
+
+  idx_smaller = diff_abs < width
+  idx_bigger = diff_abs >= width
+
+  loss[idx_smaller] = width * torch.log(1 + diff_abs[idx_smaller] / curvature)
+
+  C = width - width * math.log(1 + width / curvature)
+  loss[idx_bigger] = loss[idx_bigger] - C
+
+  if reduction == "sum":
+    loss = loss.sum()
+
+  if reduction == "mean":
+    loss = loss.mean()
+
+  return loss
+
+
+class WingLoss(_Loss):
+  def __init__(self, width=5, curvature=0.5, reduction="mean"):
+    super(WingLoss, self).__init__(reduction=reduction)
+    self.width = width
+    self.curvature = curvature
+
+  def forward(self, prediction, target):
+    return wing_loss(prediction, target, self.width, self.curvature, self.reduction)
+
+
+def smooth_wing_loss(prediction: torch.Tensor, target: torch.Tensor, thres1=2, thres2=20, curvature=2, reduction="mean"):
+  """
+  smooth_wing = 
+      1. |x|                           , if |x| < thres1
+      2. thres2*ln(1+|x|/curvature) + B, if A <= |x| < thres2
+      3. |x| - C                       , if |x| >= thres2
+  """
+  loss = (target - prediction).abs()
+
+  idx_small = loss < thres1
+  idx_normal = (loss >= thres1) * (loss < thres2)
+  idx_big = loss >= thres2
+
+  B = thres1 - thres2 * math.log(1 + thres1 / curvature)
+  loss[idx_normal] = thres2 * torch.log(1 + loss[idx_normal] / curvature) + B
+
+  C = thres2 - thres2 * math.log(1 + thres2 / curvature) - B
+  loss[idx_big] = loss[idx_big] - C
+
+  if reduction == "sum":
+    loss = loss.sum()
+  if reduction == "mean":
+    loss = loss.mean()
+
+  return loss
+
+
+class SmoothWingLoss(_Loss):
+  """docstring for SmoothWingLoss"""
+
+  def __init__(self, thres1=2, thres2=20, curvature=2, reduction="mean"):
+    super(SmoothWingLoss, self).__init__(reduction=reduction)
+    self.thres1 = thres1
+    self.thres2 = thres2
+    self.curvature = curvature
+
+  def forward(self, prediction, target):
+    return smooth_wing_loss(prediction, target, self.thres1, self.thres2, self.curvature, self.reduction)
+
+
+def wider_wing_loss(prediction: torch.Tensor, target: torch.Tensor, thres1=2, thres2=20, curvature=2, reduction="mean"):
+  """
+  wider_wing = 
+      1. |x|                           , if |x| < thres1
+      2. thres2*ln(1+|x|/curvature) + B, if |x| >= thres2
+  """
+  loss = (target - prediction).abs()
+
+  idx_small = loss < thres1
+  idx_big = loss >= thres1
+
+  B = thres1 - thres2 * math.log(1 + thres1 / curvature)
+  loss[idx_big] = thres2 * torch.log(1 + loss[idx_big] / curvature) + B
+
+  if reduction == "sum":
+    loss = loss.sum()
+  if reduction == "mean":
+    loss = loss.mean()
+
+  return loss
+
+
+class WiderWingLoss(_Loss):
+  """docstring for WiderWingLoss"""
+
+  def __init__(self, thres1=2, thres2=20, curvature=2, reduction="mean"):
+    super(WiderWingLoss, self).__init__(reduction=reduction)
+    self.thres1 = thres1
+    self.thres2 = thres2
+    self.curvature = curvature
+
+  def forward(self, prediction, target):
+    return wider_wing_loss(prediction, target, self.thres1, self.thres2, self.curvature, self.reduction)
+
+
+def normalized_wider_wing_loss(prediction: torch.Tensor, target: torch.Tensor, num_points, image_size=256, thres1=2, thres2=20, curvature=2, reduction="mean"):
+  """
+  normalized_wider_wing = 
+      1. C/d * |x|                           , if |x| < thres1
+      2. C/d * (thres2*ln(1+|x|/curvature) + B), if |x| >= thres2
+  """
+  loss = (target - prediction).abs()
+
+  idx_small = loss < thres1
+  idx_big = loss >= thres1
+
+  B = thres1 - thres2 * math.log(1 + thres1 / curvature)
+  loss[idx_big] = thres2 * torch.log(1 + loss[idx_big] / curvature) + B
+
+  if num_points == 29:
+    le_idx = [8]
+    re_idx = [9]
+
+  if num_points == 68:
+    le_idx = [36]  # le = left eye
+    re_idx = [45]  # re = right eye
+
+  if num_points == 98:
+    le_idx = [60]
+    re_idx = [72]
+
+  target = target.reshape(-1, num_points, 2)
+  le_loc = torch.mean(target[:, le_idx, :], dim=1)  # batchsize x 2
+  re_loc = torch.mean(target[:, re_idx, :], dim=1)
+
+  norm_dist = torch.sqrt(torch.sum((le_loc - re_loc)**2, dim=1))  # batchsize
+  factor = image_size/norm_dist
+
+  if reduction == "sum":
+    loss = loss.sum(dim=1)
+    loss *= factor
+    loss = loss.sum()
+
+  if reduction == "mean":
+    loss = loss.mean(dim=1)
+    loss *= factor
+    loss = loss.mean()
+
+  return loss
+
+
+class NormalizedWiderWingLoss(_Loss):
+  """docstring for NormalizedWiderWingLoss"""
+
+  def __init__(self, thres1=2, thres2=20, curvature=2, num_points=98, image_size=256, reduction="mean"):
+    super(NormalizedWiderWingLoss, self).__init__(reduction=reduction)
+    self.thres1 = thres1
+    self.thres2 = thres2
+    self.curvature = curvature
+
+    self.num_points = num_points
+    self.image_size = image_size
+
+  def forward(self, prediction, target):
+    return normalized_wider_wing_loss(prediction, target, self.num_points, self.image_size, self.thres1, self.thres2, self.curvature, self.reduction)
+
+#!<-----------------------------------------------------------------------------
+#!< EPE error: optical flow
+#!<-----------------------------------------------------------------------------
+
+
+def endpoint_error(pred, target, p=2, q=None, eps=None):
+  """Calculate end point errors between prediction and ground truth.
+
+  If not define q, the loss function is
+  .. math::
+    loss = \Vert \mathbf{u}-\mathbf{u_gt} \Vert^p
+
+  otherwise,
+  .. math::
+    loss = (\Vert \mathbf{u}-\mathbf{u_gt} \Vert^p+eps)^q
+
+  For PWC-Net L2 norm loss: p=2, for the robust loss function p=1, q=0.4,
+  eps=0.01.
+
+  Args:
+      pred (torch.Tensor): output flow map from flow_estimator
+          shape(B, 2, H, W).
+      target (torch.Tensor): ground truth flow map shape(B, 2, H, W).
+      p (int): norm degree for loss. Options are 1 or 2. Defaults to 2.
+      q (float, optional): used to give less penalty to outliers when
+          fine-tuning model. Defaults to 0.4.
+      eps (float, optional): a small constant to numerical stability when
+          fine-tuning model. Defaults to 0.01.
+
+  Returns:
+      Tensor: end-point error map with the shape (B, H, W).
+  """
+
+  assert pred.shape == target.shape, (f'pred shape {pred.shape} does not match target shape {target.shape}.')
+
+  epe_map = torch.norm(pred - target, p, dim=1)  # shape (B, H, W).
+
+  if q is not None and eps is not None:
+    epe_map = (epe_map + eps)**q
+
+  return epe_map
+
+
+class MultiLevelEPELoss(nn.Module):
+  """Multi-level end point error loss.
+
+  Args:
+
+    p (int): norm degree for loss. Options are 1 or 2. Defaults to 2.
+    q (float): used to give less penalty to outliers when fine-tuning model. Defaults to None.
+    eps (float): a small constant to numerical stability when fine-tuning model. Defaults to None.
+    weights (dict): manual rescaling weights given to the loss of flow map
+        at each level, and the keys in weights must correspond to predicted
+        dict. Defaults to dict(level6=0.32, level5=0.08, level4=0.02, level3=0.01, level2=0.005).
+    flow_div (float): the divisor used to scale down ground truth. Defaults to 20.
+    max_flow (float): maximum value of optical flow, if some pixel's flow
+        of target is larger than it, this pixel is not valid. Default to float('inf').
+    resize_flow (str): mode for reszing flow: 'downsample' and 'upsample',
+        as multi-level predicted outputs don't match the ground truth.
+        If set to 'downsample', it will downsample the ground truth, and
+        if set to 'upsample' it will upsample the predicted flow, and
+        'upsample' is used for sparse flow map as no generic interpolation
+        mode can resize a ground truth of sparse flow correctly. Default to 'downsample'.
+    scale_as_level (bool): Whether flow for each level is at its native
+        spatial resolution. If `'scale_as_level'` is True, the ground
+        truth is scaled at different levels, if it is False, the ground truth will not be scaled. Default to False.
+    reduction (str): the reduction to apply to the output:'none', 'mean',
+        'sum'. 'none': no reduction will be applied and will return a
+        full-size epe map, 'mean': the mean of the epe map is taken, 'sum':
+        the epe map will be summed but averaged by batch_size. Default: 'sum'.
+
+    """
+
+  def __init__(self, p=2,
+               q=None,
+               eps=None,
+               weights=[0.32, 0.08, 0.02, 0.01, 0.005],
+               flow_div=20.,
+               max_flow=float('inf'),
+               resize_flow='downsample',
+               scale_as_level=False,
+               reduction='sum'):
+    super(MultiLevelEPELoss, self).__init__()
+    assert p == 1 or p == 2
+    self.p = p
+    self.q = q
+    if self.q is not None:
+      assert self.q > 0
+
+    self.eps = eps
+    if self.eps is not None:
+      assert eps > 0
+
+    assert flow_div > 0
+    self.flow_div = flow_div
+
+    assert isinstance(weights, list)
+    self.weights = weights
+
+    assert max_flow > 0.
+    self.max_flow = max_flow
+
+    assert resize_flow in ('downsample', 'upsample')
+    self.resize_flow = resize_flow
+
+    assert isinstance(scale_as_level, bool)
+    self.scale_as_level = scale_as_level
+
+    assert reduction in ('mean', 'sum')
+    self.reduction = reduction
+
+  def forward(self, pred_list, target, valid=None):
+    """Forwar function for MultiLevelCharbonnierLoss.
+
+    Args:
+        pred_list (list): Multi-level output of predicted optical flow,
+            and the contain in dict is a Tensor or list of Tensor with
+            shape (B, 2, H_l, W_l), where l indicates the level.
+        target (Tensor): Ground truth of optical flow with shape (B, 2, H, W).
+        valid (Tensor, optional): Valid mask for optical flow. Defaults to None.
+
+    Returns:
+        Tensor: value of pixel-wise generalized Charbonnier loss.
+
+    """
+    # compute valid optical flow (avoid to outlier)
+    if valid is None:
+      valid = torch.ones_like(target[:, 0, :, :])
+    else:
+      mag = torch.sum(target**2, dim=1).sqrt()
+      valid = ((valid >= 0.5) & (mag < self.max_flow)).to(target)
+
+    # normalize
+    th, tw = target.shape[2:]
+    target_div = target / self.flow_div
+
+    # optical flow target shape
+    c_org, h_org, w_org = target.shape[1:]
+    assert c_org == 2, f'The channels ground truth must be 2, but got {c_org}'
+
+    # over for each level: from top to bottom
+    loss = 0
+    for level, cur_weight in enumerate(self.weights):
+      cur_pred = pred_list[level] / self.flow_div
+      b, _, h, w = cur_pred.shape
+
+      if self.resize_flow == 'downsample':
+        # down sample ground truth following irr solution
+        # https://github.com/visinf/irr/blob/master/losses.py#L16
+        cur_target = F.adaptive_avg_pool2d(target_div, [h, w])
+        if self.scale_as_level:
+          cur_target[:, 0] /= (tw / w)
+          cur_target[:, 1] /= (th / h)
+        cur_valid = F.adaptive_max_pool2d(valid, [h, w])
+      else:
+        cur_target = target_div
+        cur_valid = valid
+
+      if self.resize_flow == 'upsample':
+        # up sample predicted flow following pwcnet and irr solution
+        # https://github.com/visinf/irr/blob/master/losses.py#L20
+        # when training sparse flow dataset, as no generic
+        # interpolation mode can resize a ground truth of sparse flow correctly.
+        cur_pred = F.interpolate(cur_pred, size=cur_target.shape[2:], mode='bilinear', align_corners=False)
+        if self.scale_as_level:
+          cur_pred[:, 0] *= (tw / w)
+          cur_pred[:, 1] *= (th / h)
+
+      loss_map = endpoint_error(cur_pred, cur_target, p=self.p, q=self.q, eps=self.eps) * cur_valid
+
+      if self.reduction == 'mean':
+        loss += loss_map.sum() / (cur_valid.sum() + 1e-8) * cur_weight
+      elif self.reduction == 'sum':
+        loss += loss_map.sum() / b * cur_weight
+
+    return loss
+
+
+def charbonnier_loss(pred, target, q=0.2, eps=0.01):
+  """Generalized Charbonnier loss function between output and ground truth.
+
+  The loss function is
+  .. math::
+    loss = ((u-u_gt)^2+(v-v_gt)^2+eps)^q
+
+  Generalized Charbonnier loss was used in LiteFlowNet when fine tuning,
+  with eps=0.01 q=0.2.
+
+  Args:
+      pred (torch.Tensor): output flow map from flow_estimator
+          shape(B, 2, H, W).
+      target (torch.Tensor): ground truth flow map shape(B, 2, H, W).
+      q (float): the exponent in charbonnier loss.
+      eps (float): small constant to numerical stability when
+          fine-tuning model. Defaults to 0.01.
+
+  Returns:
+      Tensor: loss map with the shape (B, H, W).
+  """
+
+  assert pred.shape == target.shape, (f'pred shape {pred.shape} does not match target shape {target.shape}.')
+  diff = torch.add(pred, -target)
+  loss_map = (torch.sum(diff * diff, dim=1) + eps)**q  # shape (B, H, W).
+  return loss_map
+
+
+class MultiLevelCharbonnierLoss(nn.Module):
+
+  def __init__(self, q=0.2,
+               eps=0.01,
+               flow_div=20.,
+               weights=[0.32, 0.08, 0.02, 0.01, 0.005],
+               max_flow=float('inf'),
+               resize_flow='downsample',
+               scale_as_level=False,
+               reduction='sum'):
+    super(MultiLevelCharbonnierLoss, self).__init__()
+
+    assert isinstance(q, float) and q > 0.
+    self.q = q
+
+    assert isinstance(eps, float) and eps > 0.
+    self.eps = eps
+
+    assert flow_div > 0
+    self.flow_div = flow_div
+
+    assert isinstance(weights, list)
+    self.weights = weights
+
+    assert max_flow > 0.
+    self.max_flow = max_flow
+
+    assert resize_flow in ('downsample', 'upsample')
+    self.resize_flow = resize_flow
+
+    assert isinstance(scale_as_level, bool)
+    self.scale_as_level = scale_as_level
+
+    assert reduction in ('mean', 'sum')
+    self.reduction = reduction
+
+  def forward(self, pred_list, target, valid=None):
+    """Forwar function for MultiLevelCharbonnierLoss.
+
+    Args:
+        preds_list (list): Multi-level output of predicted optical flow,
+            and the contain in dict is a Tensor or list of Tensor with
+            shape (B, 2, H_l, W_l), where l indicates the level.
+        target (Tensor): Ground truth of optical flow with shape (B, 2, H, W).
+        valid (Tensor, optional): Valid mask for optical flow. Defaults to None.
+
+    Returns:
+        Tensor: value of pixel-wise generalized Charbonnier loss.
+
+    """
+    # compute valid optical flow (avoid to outlier)
+    if valid is None:
+      valid = torch.ones_like(target[:, 0, :, :])
+    else:
+      mag = torch.sum(target**2, dim=1).sqrt()
+      valid = ((valid >= 0.5) & (mag < self.max_flow)).to(target)
+
+    # normalize
+    th, tw = target.shape[2:]
+    target_div = target / self.flow_div
+
+    # optical flow target shape
+    c_org, h_org, w_org = target.shape[1:]
+    assert c_org == 2, f'The channels ground truth must be 2, but got {c_org}'
+
+    # over for each level: from top to bottom
+    loss = 0
+    for level, cur_weight in enumerate(self.weights):
+      cur_pred = pred_list[level] / self.flow_div
+      b, _, h, w = cur_pred.shape
+
+      if self.resize_flow == 'downsample':
+        # down sample ground truth following irr solution
+        # https://github.com/visinf/irr/blob/master/losses.py#L16
+        cur_target = F.adaptive_avg_pool2d(target_div, [h, w])
+        if self.scale_as_level:
+          cur_target[:, 0] /= (tw / w)
+          cur_target[:, 1] /= (th / h)
+        cur_valid = F.adaptive_max_pool2d(valid, [h, w])
+      else:
+        cur_target = target_div
+        cur_valid = valid
+
+      if self.resize_flow == 'upsample':
+        # up sample predicted flow following pwcnet and irr solution
+        # https://github.com/visinf/irr/blob/master/losses.py#L20
+        # when training sparse flow dataset, as no generic
+        # interpolation mode can resize a ground truth of sparse flow correctly.
+        cur_pred = F.interpolate(cur_pred, size=cur_target.shape[2:], mode='bilinear', align_corners=False)
+        if self.scale_as_level:
+          cur_pred[:, 0] *= (tw / w)
+          cur_pred[:, 1] *= (th / h)
+
+      loss_map = charbonnier_loss(cur_pred, cur_target, q=self.q, eps=self.eps) * cur_valid
+
+      if self.reduction == 'mean':
+        loss += loss_map.sum() / (cur_valid.sum() + 1e-8) * cur_weight
+      elif self.reduction == 'sum':
+        loss += loss_map.sum() / b * cur_weight
+
+    return loss
```

### Comparing `tw-3.8.1/tw/nn/embedding.py` & `tw-3.9.0/tw/nn/embedding.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/conv.py` & `tw-3.9.0/tw/nn/conv.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/bbox.py` & `tw-3.9.0/tw/nn/bbox.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/transformer.py` & `tw-3.9.0/tw/nn/transformer.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/anchor.py` & `tw-3.9.0/tw/nn/anchor.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/fpn.py` & `tw-3.9.0/tw/nn/fpn.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/interpolate.py` & `tw-3.9.0/tw/nn/interpolate.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/nn/activation.py` & `tw-3.9.0/tw/nn/activation.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/media/raw.py` & `tw-3.9.0/tw/media/raw.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/media/media.py` & `tw-3.9.0/tw/media/media.py`

 * *Files 18% similar despite different names*

```diff
@@ -206,14 +206,90 @@
 def video_resize(video_path: str, target_h, target_w, output_path):
   cmd = 'ffmpeg -y -i {} -vsync 0 -threads 16 -vf scale={}:{} -pix_fmt yuvj420p -strict -2 {}'.format(
       video_path, target_w, target_h, output_path)
   logger.info(cmd)
   return subprocess.call(cmd, shell=True)
 
 
+class YuvReader():
+  def __init__(self, path: str, height: int, width: int, separate=False):
+    assert os.path.exists(path)
+    self.size = height * width + height * width // 2
+    self.handle = open(path, 'rb')
+    self.count = os.path.getsize(path) // self.size
+
+    assert height > 0 and height % 2 == 0
+    assert width > 0 and width % 2 == 0
+    self.height = height
+    self.width = width
+    self.separate = separate
+
+    # preload first
+    h, w = height, width
+    s = width * height
+    uPlanePos = s
+    vPlanePos = s + (width // 2) * (height // 2)
+
+    self.frames = []
+    for i in range(self.count):
+      arr = np.array([i for i in self.handle.read(self.size)]).astype('uint8')
+      y = arr[:uPlanePos]
+      u = arr[uPlanePos: vPlanePos]
+      v = arr[vPlanePos:]
+      y = np.reshape(y, [h, w])
+      u = u.reshape(h // 2, w // 2)
+      v = v.reshape(h // 2, w // 2)
+      if self.separate:
+        self.frames.append([y, u, v])
+      else:
+        u = cv2.resize(u, dsize=(w, h))
+        v = cv2.resize(v, dsize=(w, h))
+        yuv = np.stack([y, u, v], axis=2)
+        self.frames.append(yuv)
+
+  def __len__(self):
+    return len(self.frames)
+
+  def __getitem__(self, idx):
+    return self.frames[idx]
+
+  def __enter__(self):
+    return self
+
+  def __exit__(self, exc_type, exc_value, exc_traceback):
+    self.handle.close()
+
+
+class YuvWriter():
+  def __init__(self, path: str, height: int, width: int):
+    assert height > 0 and height % 2 == 0
+    assert width > 0 and width % 2 == 0
+    self.height = height
+    self.width = width
+    self.handle = open(path, 'wb')
+
+  def __len__(self):
+    return len(self.frames)
+
+  def __enter__(self):
+    return self
+
+  def __exit__(self, exc_type, exc_value, exc_traceback):
+    self.handle.close()
+
+  def write(self, y: np.ndarray, u: np.ndarray, v: np.ndarray):
+    assert y.shape[0] == self.height and y.shape[1] == self.width
+    assert u.shape[0] == self.height // 2 and u.shape[1] == self.width // 2
+    assert v.shape[0] == self.height // 2 and v.shape[1] == self.width // 2
+
+    self.handle.write(y.astype('uint8').tobytes())
+    self.handle.write(u.astype('uint8').tobytes())
+    self.handle.write(v.astype('uint8').tobytes())
+
+
 class VideoReader():
 
   def __init__(self, path: str, to_rgb=False, to_tensor=False):
     self.cap = cv2.VideoCapture(path)
     self.frame = None
     self.to_rgb = to_rgb
     self.to_tensor = to_tensor
```

### Comparing `tw-3.8.1/tw/media/__init__.py` & `tw-3.9.0/tw/media/__init__.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/media/ply.py` & `tw-3.9.0/tw/media/ply.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_landmark/__init__.py` & `tw-3.9.0/tw/contrib/face_landmark/__init__.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_landmark/mobileface.py` & `tw-3.9.0/tw/contrib/face_landmark/mobileface.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/__init__.py` & `tw-3.9.0/tw/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/s3fd/nets.py` & `tw-3.9.0/tw/contrib/face_detection/s3fd/nets.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/s3fd/box_utils.py` & `tw-3.9.0/tw/contrib/face_detection/s3fd/box_utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/s3fd/s3fd.py` & `tw-3.9.0/tw/contrib/face_detection/s3fd/s3fd.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/retinaface/nets.py` & `tw-3.9.0/tw/contrib/face_detection/retinaface/nets.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/retinaface/box_utils.py` & `tw-3.9.0/tw/contrib/face_detection/retinaface/box_utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/retinaface/retinaface.py` & `tw-3.9.0/tw/contrib/face_detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/retinaface/data_utils.py` & `tw-3.9.0/tw/contrib/face_detection/retinaface/data_utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/__init__.py` & `tw-3.9.0/tw/contrib/face_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/pyramidbox/nets.py` & `tw-3.9.0/tw/contrib/face_detection/pyramidbox/nets.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/pyramidbox/box_utils.py` & `tw-3.9.0/tw/contrib/face_detection/pyramidbox/box_utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/pyramidbox/pyramidbox.py` & `tw-3.9.0/tw/contrib/face_detection/pyramidbox/pyramidbox.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/dsfd/nets.py` & `tw-3.9.0/tw/contrib/face_detection/dsfd/nets.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/dsfd/dsfd.py` & `tw-3.9.0/tw/contrib/face_detection/dsfd/dsfd.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/dsfd/box_utils.py` & `tw-3.9.0/tw/contrib/face_detection/dsfd/box_utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/tinyface/nets.py` & `tw-3.9.0/tw/contrib/face_detection/tinyface/nets.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/tinyface/box_utils.py` & `tw-3.9.0/tw/contrib/face_detection/tinyface/box_utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/tinyface/tinyface.py` & `tw-3.9.0/tw/contrib/face_detection/tinyface/tinyface.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/mtcnn/first_stage.py` & `tw-3.9.0/tw/contrib/face_detection/mtcnn/first_stage.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/mtcnn/nets.py` & `tw-3.9.0/tw/contrib/face_detection/mtcnn/nets.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/mtcnn/box_utils.py` & `tw-3.9.0/tw/contrib/face_detection/mtcnn/box_utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/mtcnn/mtcnn.py` & `tw-3.9.0/tw/contrib/face_detection/mtcnn/mtcnn.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/faceboxes/nets.py` & `tw-3.9.0/tw/contrib/face_detection/faceboxes/nets.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/faceboxes/faceboxes.py` & `tw-3.9.0/tw/contrib/face_detection/faceboxes/faceboxes.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/contrib/face_detection/faceboxes/box_utils.py` & `tw-3.9.0/tw/contrib/face_detection/faceboxes/box_utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/optim/warmup_multistep_lr.py` & `tw-3.9.0/tw/optim/warmup_multistep_lr.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/optim/poly_lr.py` & `tw-3.9.0/tw/optim/poly_lr.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/optim/__init__.py` & `tw-3.9.0/tw/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/widerface.py` & `tw-3.9.0/tw/datasets/widerface.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/coco.py` & `tw-3.9.0/tw/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/cifar.py` & `tw-3.9.0/tw/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/pil.py` & `tw-3.9.0/tw/datasets/pil.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/general.py` & `tw-3.9.0/tw/datasets/general.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """General datasets for common tasks.
 """
 import os
+import tqdm
 import glob
 import random
+import copy
 import torch
+import cv2
 import tw
 import tw.transform as T
 
 #!<----------------------------------------------------------------------------
 #!< General Datasets for Classification or Regression
 #!<----------------------------------------------------------------------------
 
@@ -99,128 +102,188 @@
 #!<----------------------------------------------------------------------------
 
 class ImagesDataset(torch.utils.data.Dataset):
 
   """Loading all jpg/png images at path folder.
   """
 
-  def __init__(self, path, transform=None):
-    self.transform = transform
-    self.filenames = []
+  def __init__(self, path, transform, is_preload=False, is_meta=True, **kwargs):
+    # check
+    self.is_preload = is_preload
+    self.is_meta = is_meta
+    self.targets = []
+    self.method = None
 
-    if os.path.isdir(path):
-      imgs, _ = tw.media.collect(item, salience=True)
-      self.filenames.extend(imgs)
-
-    elif os.path.isfile(path):
-      res, _ = tw.parser.parse_from_text(path, [str, ], [True, ])  # nopep8
-      for item in res[0]:
-        imgs, _ = tw.media.collect(item, salience=True)
-        self.filenames.extend(imgs)
+    # method-1: path = [lr_folder_list]
+    if isinstance(path, list):
+      for folder in path:
+        image_list, _ = tw.media.collect((folder))
+        self.targets.extend(image_list)
+      self.method = 'folder_list'
+
+    # method-2 path = protocal file
+    elif isinstance(path, str) and os.path.exists(path) and path.endswith(('.txt',)):
+      tw.fs.raise_path_not_exist(path)
+      res, _ = tw.parser.parse_from_text(path, [str, ], [True, ])
+      self.targets = []
+      for img_path in res[0]:
+        self.targets.append(img_path)
+      self.method = 'file'
 
     else:
       raise NotImplementedError(path)
 
-    tw.logger.info(f'Total loading {len(self.filenames)} images from {path}.')
+    if self.is_preload:
+      new_targets = []
+      for img_path in tqdm.tqdm(self.targets):
+        img = cv2.imread(img_path)
+        img = img.astype('float32')
+        assert img is not None
+        new_targets.append(img)
+      self.targets = new_targets
+
+    self.transform = transform
+    tw.logger.info(f'total load num of image: {len(self.targets)}.')
 
   def __len__(self):
-    return len(self.filenames)
+    return len(self.targets)
 
   def __getitem__(self, idx):
+    """fetch elements
+    """
+    img = self.targets[idx]
+
+    # preload or not
+    if self.is_preload:
+      meta = T.ImageMeta(binary=img.copy(), source=T.COLORSPACE.BGR)
 
-    img_meta = T.ImageMeta(path=self.filenames[idx])
-    img_meta.load().numpy()
+    else:
+      meta = T.ImageMeta(path=img, source=T.COLORSPACE.BGR)
+      meta.load().numpy()
 
-    return self.transform([img_meta, ])
+    # meta or not
+    if self.is_meta:
+      return self.transform([meta, ])
+    else:
+      return self.transform(meta.bin)
 
 
-class ImageEnhance(torch.utils.data.Dataset):
+class ImageRestoration(torch.utils.data.Dataset):
 
-  """General Image Enhancement: image to image translation
+  """General Image Restoration: image to image translation
 
     e.g. super resolution, denoise, sharpeness
 
-  Format:
-    input_image_path augmented_image_path
+    Method-1: path [
+      [lr_folder_1, lr_folder_2, ...],
+      [hr_folder_1, hr_folder_2, ...],
+    ]
+
+    Method-2: protocal.txt
+      lr_img_path1 hr_img_path1
+      lr_img_path2 hr_img_path2
+      ...
+
+    Method-3: binaryfile.pth
+      data = {
+        'pred': [n, h, w, 3],
+        'label': [n, h', w', 3],
+      }
+      patch is used in np.ndarray (BGR 0-255 format)
+
+    Note: 
+      different from ImageFolderEnhance, it first load all image into memory.
 
   """
 
-  def __init__(self, path, transform, **kwargs):
+  def __init__(self, path, transform, is_preload=False, is_meta=True, repeat=1, **kwargs):
     # check
-    tw.fs.raise_path_not_exist(path)
-    res, _ = tw.parser.parse_from_text(path, [str, str], [True, True])  # nopep8
-
+    self.is_preload = is_preload
+    self.is_meta = is_meta
     self.targets = []
-    for img_path, enhance_path in zip(res[0], res[1]):
-      self.targets.append((img_path, enhance_path))
-
-    self.transform = transform
-    tw.logger.info('Totally loading %d samples.' % len(self.targets))
-
-  def __len__(self):
-    return len(self.targets)
-
-  def __getitem__(self, idx):
-    # load image
-    img_meta = T.ImageMeta(path=self.targets[idx][0])
-    img_meta.load().numpy()
-    # load enhance
-    enhance_meta = T.ImageMeta(path=self.targets[idx][1])
-    enhance_meta.load().numpy()
-
-    return self.transform([img_meta, enhance_meta])
-
-
-class ImageFolderEnhance(torch.utils.data.Dataset):
-
-  """General Image Folder Enhancement: image to image translation
+    self.method = None
 
-    e.g. super resolution, denoise, sharpeness
-
-  Format:
-    input_image_folder augmented_image_folder
-
-  """
+    # method-1: path = [[lr_folder_list], [hr_folder_list]]
+    if isinstance(path, list) and len(path) == 2:
+      lr_folder_list, hr_folder_list = path
+      assert len(lr_folder_list) == len(hr_folder_list)
+      for lr_folder, hr_folder in zip(lr_folder_list, hr_folder_list):
+        lr_list = [os.path.join(lr_folder, f) for f in sorted(os.listdir(lr_folder))]
+        hr_list = [os.path.join(hr_folder, f) for f in sorted(os.listdir(hr_folder))]
+        self.targets.extend([*zip(lr_list, hr_list)])
+      self.method = 'folder_list'
+
+    # method-2 path = protocal file input-label
+    elif isinstance(path, str) and os.path.exists(path) and path.endswith(('.txt',)):
+      tw.fs.raise_path_not_exist(path)
+      res, _ = tw.parser.parse_from_text(path, [str, str], [True, True])
+      self.targets = []
+      for lr_path, hr_path in zip(res[0], res[1]):
+        self.targets.append((lr_path, hr_path))
+      self.method = 'file'
+
+    # method-3 binary file
+    elif isinstance(path, str) and os.path.exists(path) and path.endswith(('.pth',)):
+      data = torch.load(path)
+      assert data['pred'].shape[0] == data['label'].shape[0]
+      for i in tqdm.tqdm(range(data['pred'].shape[0])):
+        self.targets.append((data['pred'][i], data['label'][i]))
 
-  def __init__(self, path, transform, **kwargs):
-    # check
-    tw.fs.raise_path_not_exist(path)
-    res, _ = tw.parser.parse_from_text(path, [str, str], [True, True])  # nopep8
+    else:
+      raise NotImplementedError(path)
 
-    self.targets = []
-    total_img = 0
-    for _, (image_folder, enhance_folder) in enumerate(zip(*res)):
-      self.targets.append((
-          [os.path.join(image_folder, f) for f in sorted(os.listdir(image_folder))],
-          [os.path.join(enhance_folder, f) for f in sorted(os.listdir(enhance_folder))],
-      ))
-      total_img += len(self.targets[-1][0])
+    if self.is_preload:
+      new_targets = []
+      for lr_path, hr_path in tqdm.tqdm(self.targets):
+        lr_img = cv2.imread(lr_path)
+        lr_img = lr_img.astype('float32')
+        hr_img = cv2.imread(hr_path)
+        hr_img = hr_img.astype('float32')
+        assert lr_img is not None and hr_img is not None
+        new_targets.append((lr_img, hr_img))
+      self.targets = new_targets
+
+    # repeat dataset
+    if repeat > 1:
+      targets = []
+      for _ in range(repeat):
+        for target in self.targets:
+          targets.append(target)
+      self.targets = targets
 
     self.transform = transform
-    tw.logger.info(f'num of folder: {len(self)}, num of image: {total_img}.')
+    tw.logger.info(f'total load num of image: {len(self.targets)}.')
 
   def __len__(self):
     return len(self.targets)
 
   def __getitem__(self, idx):
-    # folder
-    img, enh = self.targets[idx]
-    assert len(img) <= len(enh), f"{len(img)} vs {len(enh)}."
-
-    # fetch image
-    i = random.randint(0, len(img) - 1)
-    img_meta = T.ImageMeta(path=img[i], source=T.COLORSPACE.BGR)
-    img_meta.load().numpy()
-    enh_meta = T.ImageMeta(path=enh[i], source=T.COLORSPACE.BGR)
-    enh_meta.load().numpy()
+    """fetch elements
+    """
+    lr, hr = self.targets[idx]
+
+    # preload or not
+    if self.is_preload:
+      lr_meta = T.ImageMeta(binary=lr.copy(), source=T.COLORSPACE.BGR)
+      hr_meta = T.ImageMeta(binary=hr.copy(), source=T.COLORSPACE.BGR)
 
-    return self.transform([img_meta, enh_meta])
+    else:
+      lr_meta = T.ImageMeta(path=lr, source=T.COLORSPACE.BGR)
+      lr_meta.load().numpy()
+      hr_meta = T.ImageMeta(path=hr, source=T.COLORSPACE.BGR)
+      hr_meta.load().numpy()
+
+    # meta or not
+    if self.is_meta:
+      return self.transform([lr_meta, hr_meta])
+    else:
+      return self.transform(lr_meta.bin, hr_meta.bin)
 
 
-class VideoFolderEnhance(torch.utils.data.Dataset):
+class VideoRestoration(torch.utils.data.Dataset):
 
   """General Video Folder Enhancement: video to video translation
 
     e.g. super resolution, denoise, sharpeness
 
   Format:
     input_video_folder augmented_video_folder
@@ -255,45 +318,7 @@
 
     i = random.randint(0, len(enh) - self.segment)
     img_meta = T.VideoMeta(path=img[i: i + self.segment])
     img_meta.load().numpy()
     enh_meta = T.VideoMeta(path=enh[i: i + self.segment])
     enh_meta.load().numpy()
     return self.transform([img_meta, enh_meta])
-
-
-
-class ImageBinaryPatchEnhance(torch.utils.data.Dataset):
-
-  """General Image Binary Patch Enhancement: image to image translation
-
-    e.g. super resolution, denoise, sharpeness
-
-  Format:
-    data = {
-      'pred': [n, h, w, 3],
-      'label': [n, h', w', 3],
-    }
-    patch is used in np.ndarray (BGR 0-255 format)
-
-  """
-
-  def __init__(self, path, transform, **kwargs):
-    # check
-    tw.fs.raise_path_not_exist(path)
-    data = torch.load(path)
-    self.targets = data
-    self.transform = transform
-    assert self.targets['pred'].shape[0] == self.targets['label'].shape[0]
-    tw.logger.info('Totally loading %d samples.' % len(self))
-
-  def __len__(self):
-    return self.targets['pred'].shape[0]
-
-  def __getitem__(self, idx):
-    # load image
-    img_meta = T.ImageMeta(binary=self.targets['pred'][idx].copy())
-    img_meta.numpy()
-    # load enhance
-    enhance_meta = T.ImageMeta(binary=self.targets['label'][idx].copy())
-    enhance_meta.numpy()
-    return self.transform([img_meta, enhance_meta])
```

### Comparing `tw-3.8.1/tw/datasets/point_cloud.py` & `tw-3.9.0/tw/datasets/point_cloud.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/imagenet.py` & `tw-3.9.0/tw/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/__init__.py` & `tw-3.9.0/tw/datasets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,40 +15,53 @@
 
 from .base import SampleCollator
 from .base import BatchMultiSampler
 
 from .mnist import Mnist
 from .cifar import Cifar10
 from .imagenet import ImageNet
-from .widerface import WiderFace, WiderFaceTest
 from .coco import CocoDetection
 
+from .face import WiderFace, WiderFaceTest
+from .face import Face300W
+# from .face import Face300W_LP
+# from .face import AFLW2000
+from .face import COFW
+from .face import JD106
+# from .face import WFLW
+
+from .facemesh import BigoFaceMesh
+from .facemesh import NoW
+
 from .avec2014 import Avec2014
 from .avec2014 import Avec2014Video
 
 from .general import ImageLabel
 from .general import ImageSalientDet
 from .general import ImagesDataset
-from .general import ImageEnhance
-from .general import ImageFolderEnhance
-from .general import VideoFolderEnhance
-from .general import ImageBinaryPatchEnhance
+from .general import ImageRestoration
+from .general import VideoRestoration
 
 from .quality_assess import PIPAL
 from .quality_assess import TID2013
 from .quality_assess import KonIQ10k
 from .quality_assess import SPAQ
 from .quality_assess import LIVEC
 from .quality_assess import LIVE2005
 from .quality_assess import LIVEMD
 from .quality_assess import CSIQ
 from .quality_assess import FLIVE
 from .quality_assess import VQA_III
 
+from .optical_flow import MPISintel
+from .optical_flow import FlyingChairs
+from .optical_flow import FlyingThings3D
 
 from .denoise import SIDD_sRGB
 
 from .point_cloud import SensatUrban
 
+from .super_resolution import Flickr1024
+
 from . import pil
 
 from torch.utils.data import *
```

### Comparing `tw-3.8.1/tw/datasets/base.py` & `tw-3.9.0/tw/datasets/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import os
 import torch
 from torch.utils import data as td
-from torch._six import int_classes as _int_classes
 import tw
 
 
 #!<---------------------------------------------------------------
 #!< COLLARTOR
 #!<---------------------------------------------------------------
 
@@ -54,16 +53,14 @@
 
   def __init__(self, samplers, batch_size, drop_last):
     assert isinstance(samplers, (tuple, list))
     assert drop_last
     for sampler in samplers:
       if not isinstance(sampler, td.Sampler):
         raise ValueError("sampler should be an instance of torch.utils.data.Sampler, but got sampler={}" .format(sampler))  # nopep8
-    if not isinstance(batch_size, _int_classes) or isinstance(batch_size, bool) or batch_size <= 0:  # nopep8
-      raise ValueError("batch_size should be a positive integer value, but got batch_size={}".format(batch_size))  # nopep8
     if not isinstance(drop_last, bool):
       raise ValueError("drop_last should be a boolean value, but got drop_last={}".format(drop_last))  # nopep8
 
     self.samplers = samplers
     self.total_samples = sum([len(s) for s in self.samplers])
     self.batch_size = batch_size
     self.drop_last = drop_last
```

### Comparing `tw-3.8.1/tw/datasets/super_resolution.py` & `tw-3.9.0/tw/tools/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-# Copyright 2021 The KaiJIN Authors. All Rights Reserved.
+# Copyright 2020 The KaiJIN Authors. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Image or Video Super Resolution Dataset
-"""
-import copy
-import os
-from collections import OrderedDict
-import torch
-import scipy
-import numpy as np
-import tw
-import tw.transform as T
-
+"""External command
 
-class BSD300():
-  pass
+  python -m tw.tools.monitor    : used for monitor hardware performance
+  python -m tw.tools.busy       : used for busy running invalid task
+  python -m tw.tools.media      : used for preprocessing
+  python -m tw.tools.event      : used for training log
+  python -m tw.tools.checkpoint : used for manipulating checkpoints
 
-
-class Set14():
-  pass
+"""
```

### Comparing `tw-3.8.1/tw/datasets/mnist.py` & `tw-3.9.0/tw/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/quality_assess.py` & `tw-3.9.0/tw/datasets/quality_assess.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/avec2014.py` & `tw-3.9.0/tw/datasets/avec2014.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/datasets/denoise.py` & `tw-3.9.0/tw/datasets/denoise.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Image or Video Denoise Dataset
 """
 import copy
 import os
-from numpy.lib.arraysetops import in1d
 import torch
 import scipy
 import numpy as np
 import tw
 import tw.transform as T
```

### Comparing `tw-3.8.1/tw/utils/checkpoint.py` & `tw-3.9.0/tw/utils/checkpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -116,30 +116,49 @@
 
     else:
       pass
 
   model.load_state_dict(curr_state_dict)
 
   if print_stat:
+    logger.sys('Checkpoint file total with %d tensors.' % len(state_dict))
     logger.sys(f'Loaded state_dict: {num_matched}/{num_total} matched')
 
   return model
 
 
 def print_trainable_variables(model: nn.Module):
   """fetch trainable variables
   """
   logger.net('TRAINABLE VARIABLES:')
-  logger.net('{:60} {:20} {:5}'.format('WEIGHT', 'SHAPE', 'TRAIN'))
+  max_len = max(max([len(name) for name, p in model.named_parameters()]), 60)
+  logger.net(('{:%d} {:20} {:^8} {:^8} {:^8}' % (max_len + 5)).format('WEIGHT', 'SHAPE', 'TRAIN', 'MEAN', 'STD'))
   for name, p in model.named_parameters():
-    logger.net('{:60} {:20} {:5}'.format(name, str(list(p.shape)), p.requires_grad))
+    logger.net(('{:%d} {:20} {:^8d} {:^8.4f} {:^8.4f}' % (max_len + 5)).format(
+        name, str(list(p.shape)), p.requires_grad, p.mean(), p.std()))
 
 
 def load_state_dict_from_url(model: nn.Module, path, **kwargs):
   """download and open checkpoint from url/path, and load into model.
 
   Args:
       model (nn.Module): model.
       path ([type]): url or file path.
   """
   state_dict = load(path)
   load_matched_state_dict(model, state_dict)
+
+
+def compare_tensor(*tensors, name=None):
+  """compare two tensor value with stat
+
+  Args:
+      tensors (torch.Tensor): any
+      name (str, optional): Defaults to None.
+
+  """
+  if name is None:
+    name = 'var'
+  for i, tensor in enumerate(tensors):
+    t = tensor.cpu()
+    logger.info('[{}] shape:{}, sum:{:.4f}, mean:{:.4f}, var:{:.4f}, max:{:.4f}, min:{:.4f}'.format(
+        f'{name}:{i}', str(t.shape), t.sum().item(), t.mean().item(), t.var().item(), t.max().item(), t.min().item()))
```

### Comparing `tw-3.8.1/tw/utils/stat.py` & `tw-3.9.0/tw/utils/stat.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/utils/runner.py` & `tw-3.9.0/tw/utils/runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,24 +16,34 @@
 import os
 import socket
 import shutil
 import argparse
 import random
 from multiprocessing import Process
 
+import numpy as np
+
 import torch
 from torch import multiprocessing as mp
 from torch import distributed as dist
 from torch.utils.collect_env import get_pretty_env_info
 
 import tw
 
 
+def seed_worker(worker_id):
+  """assign different seed for each worker
+  """
+  worker_seed = torch.initial_seed() % 2 ** 32
+  np.random.seed(worker_seed)
+  random.seed(worker_seed)
+
+
 def launch(parser: argparse.ArgumentParser, tasker, **kwargs):
-  r"""launch a routine
+  """launch a routine
   """
 
   # ---------------------------------------------
   #  USED BY CONTEXT
   # ---------------------------------------------
   parser.add_argument('--name', type=str, default='tw')
   parser.add_argument('--root', type=str, default=None, help="None for creating, otherwise specific root.")
@@ -65,15 +75,15 @@
     mp.spawn(dist_runner, nprocs=num_gpus, args=(args, tasker, addr, port), join=True)
 
   else:
     dist_runner(0, args, tasker)
 
 
 def dist_runner(rank, config, tasker, addr='localhost', port=12300):
-  r"""support distributed runner.
+  """support distributed runner.
   """
 
   if config.multiprocess:
     # distributed step
     os.environ['MASTER_ADDR'] = addr
     os.environ['MASTER_PORT'] = port
     dist.init_process_group("nccl", rank=rank, world_size=torch.cuda.device_count())
@@ -115,15 +125,15 @@
   # shutil.copytree('./', config.root + '/tw', symlinks=True, ignore=_ignore)
 
   # running runner
   tasker(config)()
 
 
 def multitask(kernel, tasks, num_proc, *args):
-  r"""split tasks(dict) into multiple process to running
+  """split tasks(dict) into multiple process to running
 
   Args:
     kernel: kernel(tid, tasks[start: end], *args):
     tasks: a dictionary
     num_proc:
 
   """
@@ -140,15 +150,15 @@
     p.start()
     plist.append(p)
   for p in plist:
     p.join()
 
 
 def log(keys, values, step, epoch, tag, **kwargs):
-  r"""Display information during training in terms of interval.
+  """Display information during training in terms of interval.
   """
 
   if hasattr(tw.logger, tag):
     taglog = getattr(tw.logger, tag)
   else:
     taglog = tw.logger.info
```

### Comparing `tw-3.8.1/tw/utils/export.py` & `tw-3.9.0/tw/utils/export.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/utils/flops.py` & `tw-3.9.0/tw/utils/flops.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/utils/parser.py` & `tw-3.9.0/tw/utils/parser.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/utils/__init__.py` & `tw-3.9.0/tw/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/utils/drawer.py` & `tw-3.9.0/tw/utils/drawer.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,22 +98,40 @@
   """Draw points on image
 
   Args:
       image ([np.ndarray]): [H, W, C] uint8
       points ([np.ndarray]): [N, 2(x, y)] float
 
   """
-  assert isinstance(image, np.ndarray) and image.ndim == 3
+  assert isinstance(image, np.ndarray) and image.ndim in [3, 2]
   assert isinstance(points, np.ndarray) and points.ndim == 2
 
   render = image.copy()
   radius = 5 if 'radius' not in kwargs else kwargs['radius']
-
-  for _, (x, y) in enumerate(points):
-    cv2.circle(render, (int(x), int(y)), radius=radius, color=(0, 255, 0), thickness=cv2.FILLED)
+  color = (0, 255, 0) if 'color' not in kwargs else kwargs['color']
+  labels = None if 'labels' not in kwargs else kwargs['labels']
+  scores = None if 'scores' not in kwargs else kwargs['scores']
+
+  font_type = cv2.FONT_HERSHEY_SIMPLEX
+  font_thick = 1
+  font_scale = 0.4
+
+  for i, (x, y) in enumerate(points):
+    cv2.circle(render, (int(x), int(y)), radius=radius, color=color, thickness=cv2.FILLED)
+
+    # render label
+    if labels is not None:
+      label = labels[i]
+      if scores is not None:
+        caption = '{}:{:.2f}'.format(label, scores[i])
+      else:
+        caption = '{}'.format(label)
+      # get the width and height of the text box
+      tw, th = cv2.getTextSize(text=caption, fontFace=font_type, fontScale=font_scale, thickness=font_thick)[0] # nopep8
+      cv2.putText(render, caption, (int(x), int(y) - 4), fontFace=font_type, fontScale=font_scale, color=[255, 255, 255], thickness=font_thick) # nopep8
 
   return render
 
 
 def binary_class_analysis(preds, label, legends=None, grid=100, dst=None):
   """binary class figure.
 
@@ -201,9 +219,9 @@
   plt.legend()
   plt.xlim([0, 1])
   plt.ylim([0, 1])
 
   plt.tight_layout()
   plt.savefig(dst)
   plt.close()
-  
+
   return results
```

### Comparing `tw-3.8.1/tw/utils/tensorboard.py` & `tw-3.9.0/tw/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/utils/logger.py` & `tw-3.9.0/tw/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/utils/timer.py` & `tw-3.9.0/tw/utils/timer.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/utils/filesystem.py` & `tw-3.9.0/tw/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/widerface.py` & `tw-3.9.0/tw/evaluator/widerface.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/detection.py` & `tw-3.9.0/tw/evaluator/detection.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/image.py` & `tw-3.9.0/tw/evaluator/image.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/segmentation.py` & `tw-3.9.0/tw/evaluator/segmentation.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/classification.py` & `tw-3.9.0/tw/evaluator/classification.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/verification.py` & `tw-3.9.0/tw/evaluator/verification.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/__init__.py` & `tw-3.9.0/tw/evaluator/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,7 +31,11 @@
 from .segmentation import MattingEvaluator
 from .segmentation import PointCloudSegmentEvaluator
 
 from .verification import VerificationEvaluator
 
 from .detection import CocoEvaluator
 from .widerface import WiderfaceEvaluator
+
+from .landmark import FaceLandmarkEvaluator
+
+from .optical_flow import OpticalFlowEvaluator
```

### Comparing `tw-3.8.1/tw/evaluator/base.py` & `tw-3.9.0/tw/evaluator/base.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/quality_assess.py` & `tw-3.9.0/tw/evaluator/quality_assess.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/evaluator/avec2014.py` & `tw-3.9.0/tw/evaluator/avec2014.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/__init__.py` & `tw-3.9.0/tw/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,17 @@
 from .utils import drawer
 from .utils import parser
 from .utils import export
 
 # media
 from .media import ply
 from .media import media
-from .media import raw
-from .media import yuv
+# from .media import raw
+from .media import flow
+from .media import mesh
 
 # 2 - utils level
 from .utils import checkpoint
 from .utils import runner
 from . import evaluator
 
 # 3 - transform level
```

### Comparing `tw-3.8.1/tw/tools/checkpoint.py` & `tw-3.9.0/tw/tools/checkpoint.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/tools/busy.py` & `tw-3.9.0/tw/tools/busy.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/tools/media.py` & `tw-3.9.0/tw/tools/media.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/tools/monitor.py` & `tw-3.9.0/tw/tools/monitor.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/tools/event.py` & `tw-3.9.0/tw/tools/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 import shutil
 import pickle
 import subprocess
 import psutil
 import xml.etree.ElementTree as ET
 import time
 
+import numpy as np
+
 import torch
 import torchvision
 import tw
 
 from tensorboard.backend.event_processing import event_accumulator
 
 import matplotlib.pyplot as plt
@@ -186,15 +188,15 @@
     ax.legend(list(v.keys()), fontsize=5)
     ax.set_title(k)
 
   plt.savefig(root + '/output.png', dpi=300)
 
 
 def plot(root):
-  training_dirs = sorted(glob.glob('%s/*' % root))
+  training_dirs = [*sorted(glob.glob('%s/*' % root)), root]
   for folder in training_dirs:
     if not os.path.isdir(folder):
       continue
     event = TFEventAccumulator(folder)
     print('MODEL:', event.root, 'EPOCH:', event.epoch)
     if event.epoch == 0:
       continue
@@ -213,15 +215,16 @@
     rows, cols = len(kvs), 1
     plt.figure(figsize=(16, 4 * rows))
     plb.gcf().suptitle(event.root, fontsize=14)
 
     # * plot each key
     for idx, (k, v) in enumerate(kvs.items()):
       ax = plt.subplot(rows, cols, idx + 1)
-      print(' [INFO] Render {}'.format(k))
+      print(' [INFO] Render {}, max: {} in epoch: {}, min: {} in epoch: {}'.format(
+        k, np.max(v[1]), v[0][np.argmax(v[1])], np.min(v[1]), v[0][np.argmin(v[1])]))
       if 'train' in k:
         ax.plot(v[0][100:], v[1][100:], label=k)
       else:
         ax.plot(v[0], v[1], label=k)
       ax.grid()
       ax.legend()
       ax.set_title(k)
```

### Comparing `tw-3.8.1/tw/transform/primitive/filter.py` & `tw-3.9.0/tw/transform/primitive/filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 @T.MetaWrapper(support=[T.ImageMeta])
 def _random_iso_noise_meta(metas: Sequence[T.MetaBase], color_shift=0.05, intensity=0.5, **kwargs):
 
   random_state = np.random.RandomState()
 
   for meta in metas:
 
-    if meta.source == T.COLORSPACE.HEATMAP:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       meta.bin = _random_iso_noise_np(meta.bin,
                                       color_shift=color_shift,
                                       intensity=intensity,
                                       random_state=random_state)
@@ -100,30 +100,31 @@
   elif T.IsTensor(inputs):
     raise NotImplementedError
   elif T.IsPilImage(inputs):
     raise NotImplementedError
 
 
 #!<----------------------------------------------------------------------------
-#!< GAUSSIAN NOISE
+#!< GAU32
+# \;lhgfdxszjhgfd4xszhgrcefdxwzfdsaxz2wqqaiuyr;kjSSIAN NOISE
 #!<----------------------------------------------------------------------------
 
 
 @T.MetaWrapper(support=[T.ImageMeta])
 def _random_gaussian_noise_meta(metas: Sequence[T.MetaBase], var_limit=(10.0, 50.0), mean=0.0, **kwargs):
   r"""Apply gaussian noise to the input image."""
   assert isinstance(var_limit, tuple), var_limit
 
   var = random.uniform(*var_limit)
   sigma = var ** 0.5
   random_state = np.random.RandomState()
 
   for meta in metas:
 
-    if meta.source == T.COLORSPACE.HEATMAP:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       gauss = random_state.normal(mean, sigma, meta.bin.shape)
       meta.bin = (meta.bin + gauss).clip(0, 255)
 
   return metas
@@ -157,15 +158,15 @@
   assert isinstance(sigma_limit, tuple), sigma_limit
 
   ks_t = random.choice(np.arange(ksize_limit[0], ksize_limit[1] + 1, 2))
   sigma_t = random.uniform(*sigma_limit)
 
   for meta in metas:
 
-    if meta.source == T.COLORSPACE.HEATMAP:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       meta.bin = cv2.GaussianBlur(meta.bin, ksize=(ks_t, ks_t), sigmaX=sigma_t)
 
   return metas
 
@@ -197,15 +198,15 @@
   else:
     ys, ye = random.randint(0, ksize - 1), random.randint(0, ksize - 1)
   cv2.line(kernel, (xs, ys), (xe, ye), 1, thickness=1)
   kernel = kernel.astype(np.float32) / np.sum(kernel)  # normalize kernel
 
   for meta in metas:
 
-    if meta.source == T.COLORSPACE.HEATMAP:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       meta.bin = cv2.filter2D(meta.bin, ddepth=-1, kernel=kernel)
 
   return metas
 
@@ -228,15 +229,15 @@
 @T.MetaWrapper(support=[T.ImageMeta])
 def _random_median_blur_meta(metas: Sequence[T.MetaBase]):
   r"""Blur the input image using using a median filter with a random aperture linear size."""
 
   ksize = random.choice(np.arange(3, 8, 2))
 
   for meta in metas:
-    if meta.source == T.COLORSPACE.HEATMAP:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       curr_dtype = meta.bin.dtype
       meta.bin = cv2.medianBlur(meta.bin.astype('uint8'), ksize=ksize).astype(curr_dtype)
 
   return metas
@@ -262,7 +263,66 @@
     raise NotImplementedError
   elif T.IsMeta(inputs):
     raise NotImplementedError
   elif T.IsTensor(inputs):
     return kornia.sobel(inputs)
   elif T.IsPilImage(inputs):
     raise NotImplementedError
+
+
+#!<----------------------------------------------------------------------------
+#!< RANDOM GAMMA
+#!<----------------------------------------------------------------------------
+
+def _adjust_gamma_np(img, gamma=1.0):
+  """Using gamma correction to process the image.
+
+  Args:
+      img (ndarray): Image to be adjusted. uint8 datatype.
+
+      gamma (float or int): Gamma value used in gamma correction. gamma is a
+          positive value. Note: gamma larger than 1 make the shadows darker,
+          while gamma smaller than 1 make dark regions lighter. Default: 1.0.
+  """
+
+  assert isinstance(gamma, float) or isinstance(gamma, int)
+  assert gamma > 0
+
+  dtype = img.dtype
+  table = ((np.arange(256) / 255.) ** gamma * (255 + 1 - 1e-3)).astype('uint8')
+
+  adjusted_img = cv2.LUT(img.astype('uint8'), table).astype(dtype)
+
+  return adjusted_img
+
+
+@T.MetaWrapper(support=[T.ImageMeta])
+def _adjust_gamma_meta(metas: Sequence[T.MetaBase], gamma):
+
+  for meta in metas:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
+      continue
+
+    if isinstance(meta, T.ImageMeta):
+      meta.bin = _adjust_gamma_np(meta.bin, gamma)
+
+  return metas
+
+
+def random_gamma(inputs, low=0.7, high=1.5, **kwargs):
+  """Random gamma correction of images.
+
+    Note: gamma larger than 1 make the shadows darker, while gamma smaller than
+    1 make dark regions lighter.
+
+  """
+  assert 0 <= low <= high
+  gamma = random.uniform(low, high)
+
+  if T.IsNumpy(inputs):
+    raise NotImplementedError
+  elif T.IsMeta(inputs):
+    return _adjust_gamma_meta(inputs, gamma=gamma, **kwargs)
+  elif T.IsTensor(inputs):
+    raise NotImplementedError
+  elif T.IsPilImage(inputs):
+    raise NotImplementedError
```

### Comparing `tw-3.8.1/tw/transform/primitive/crop.py` & `tw-3.9.0/tw/transform/primitive/crop.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/transform/primitive/normalize.py` & `tw-3.9.0/tw/transform/primitive/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 @T.MetaWrapper()
 def _to_tensor_meta(metas: Sequence[T.MetaBase], scale=None, mean=None, std=None, **kwargs):
   mean = torch.tensor(mean) if mean is not None else None
   std = torch.tensor(std) if std is not None else None
 
   for meta in metas:
 
-    if meta.source == T.COLORSPACE.HEATMAP:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       meta.bin = torch.from_numpy(meta.bin)
       continue
 
     if isinstance(meta, T.ImageMeta):
       # for image
       if meta.bin.ndim == 3:
         m = torch.from_numpy(np.ascontiguousarray(meta.bin.transpose((2, 0, 1))))
@@ -148,15 +148,15 @@
 #!< TO TENSOR
 #!<----------------------------------------------------------------------------
 
 @T.MetaWrapper()
 def _to_float_meta(metas: Sequence[T.MetaBase], **kwargs):
   for meta in metas:
     if isinstance(meta, T.ImageMeta):
-      if meta.source == T.COLORSPACE.HEATMAP:
+      if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
         continue
       meta.bin = meta.bin.astype('float32')
   return metas
 
 
 def to_float(inputs, **kwargs):
   """inputs format to float
@@ -263,15 +263,15 @@
 
 
 @T.MetaWrapper(support=[T.ImageMeta, T.VideoMeta])
 def _truncated_standardize_meta(metas: Sequence[T.MetaBase], **kwargs):
 
   for meta in metas:
 
-    if meta.source == T.COLORSPACE.HEATMAP:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       meta.bin = _truncated_standardize_np(meta.bin)
 
     if isinstance(meta, T.VideoMeta):
       if meta.bin.ndim == 4:
@@ -319,15 +319,15 @@
 
 
 @T.MetaWrapper(support=[T.ImageMeta])
 def _local_contrast_normalize_meta(metas: Sequence[T.MetaBase], p=3, q=3, c=1, **kwargs):
 
   for meta in metas:
 
-    if meta.source == T.COLORSPACE.HEATMAP:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       meta.bin = _local_contrast_normalize_np(meta.bin, p, q, c)
 
   return metas
```

### Comparing `tw-3.8.1/tw/transform/primitive/pad.py` & `tw-3.9.0/tw/transform/primitive/pad.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/transform/primitive/colorspace.py` & `tw-3.9.0/tw/transform/primitive/colorspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
 
 @T.MetaWrapper(support=[T.ImageMeta, T.VideoMeta, T.BoxListMeta, T.KpsListMeta])
 def _change_colorspace_meta(metas: Sequence[T.MetaBase], src: T.COLORSPACE, dst: T.COLORSPACE, **kwargs):
 
   for meta in metas:
 
-    if meta.source in [T.COLORSPACE.HEATMAP]:
+    if meta.source in [T.COLORSPACE.HEATMAP, T.COLORSPACE.FLOW]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       meta.bin = _change_colorspace_np(meta.bin, src, dst)
       meta.source = dst
 
     if isinstance(meta, T.VideoMeta):
@@ -323,16 +323,19 @@
                                         brightness_delta=32,
                                         contrast_range=(0.5, 1.5),
                                         saturation_range=(0.5, 1.5),
                                         hue_delta=18,
                                         **kwargs):
   """NOTE: different augmentation in batch of ImageMeta.
   """
+  seed = random.randint(0, 2**32-1)
 
   for meta in metas:
+    # all meta with same augmentation
+    random.seed(seed)
 
     if meta.source in [T.COLORSPACE.HEATMAP]:
       continue
 
     if isinstance(meta, T.ImageMeta):
       meta.bin = _random_photometric_distortion_numpy(meta.bin,
                                                       brightness_delta,
```

### Comparing `tw-3.8.1/tw/transform/primitive/bbox.py` & `tw-3.9.0/tw/transform/primitive/bbox.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/transform/primitive/resize.py` & `tw-3.9.0/tw/transform/primitive/resize.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/transform/primitive/morphology.py` & `tw-3.9.0/tw/transform/primitive/morphology.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/transform/pil.py` & `tw-3.9.0/tw/transform/pil.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/transform/meta.py` & `tw-3.9.0/tw/transform/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
   BGR = 1
   BGRA = 2
   RBGA = 3
   HLS = 4
   HSV = 5
   HEATMAP = 10
   GRAY = 11
+  FEATURE = 12
+  FLOW = 13
   BT709_FULLRANGE = 20
   BT601_FULLRANGE = 21
   BT709_VIDEORANGE = 22
   BT601_VIDEORANGE = 23
   BAYER = 31
   XTRANS = 32
 
@@ -169,15 +171,15 @@
 
 #!<-----------------------------------------------------------------------------
 #!< Image Meta
 #!<-----------------------------------------------------------------------------
 
 
 class ImageMeta(MetaBase):
-  r"""ImageMeta
+  """ImageMeta
 
   Args:
     name (string/int): the identifier
     source (string): 'image' for normal rgb, 'mask' for heatmap.
     path (string): path to source
     binary: binary format like nd.array
 
@@ -185,78 +187,73 @@
 
   def __init__(self, name='ImageMeta', source=COLORSPACE.BGR, path=None, binary=None):
     super(ImageMeta, self).__init__(name)
     self.source = source
 
     if path is not None:
       fs.raise_path_not_exist(path)
-    self.path = path  # path to image
 
-    self.h = 0
-    self.w = 0
-    self.c = 0
+    self.path = path  # path to image
     self.bin = binary   # raw inputs format
 
     self.label = []
     self.caption = []
     self.transform = []   # transform op
 
+  @property
+  def h(self):
+    return self.bin.shape[0]
+
+  @property
+  def w(self):
+    return self.bin.shape[1]
+
+  @property
+  def c(self):
+    if self.bin.ndim == 3:
+      return self.bin.shape[2]
+    elif self.bin.ndim == 2:
+      return 1
+    else:
+      return -1
+
   def __str__(self):
     s = '  ImageMeta => {}\n'.format(self.name)
     s += '    source: {}\n'.format(self.source)
     s += '    path: {}\n'.format(self.path)
-    s += '    shape: (h={}, w={}, c={})\n'.format(
-        self.h, self.w, self.c)
+    s += '    shape: (h={}, w={}, c={})\n'.format(self.h, self.w, self.c)
     if self.bin is not None:
-      if len(self.bin.shape) == 2:
-        h, w = self.bin.shape
-        c = 0
-      elif len(self.bin.shape) == 3:
-        h, w, c = self.bin.shape
-      else:
-        raise NotImplementedError(self.bin.shape)
-      s += '    binary: (h={}, w={}, c={}, type={})\n'.format(
-          h, w, c, self.bin.__class__.__name__)
-      s += '    numerical: (max={}, min={}, avg={})\n'.format(
-          self.bin.max(), self.bin.min(), self.bin.mean())
+      s += '    binary: (h={}, w={}, c={}, type={})\n'.format(self.h, self.w, self.c, self.bin.__class__.__name__)
+      s += '    numerical: (max={}, min={}, avg={})\n'.format(self.bin.max(), self.bin.min(), self.bin.mean())
     if self.label:
       s += '    label: {}\n'.format(self.label)
     if self.caption:
       s += '    captions: {}\n'.format(self.caption)
     if self.transform is not None:
       s += '    transform: {}\n'.format(self.transform)
     return s
 
   def numpy(self):
-    if self.source == COLORSPACE.HEATMAP:
+    if self.source in [COLORSPACE.HEATMAP, ]:
       self.bin = np.array(self.bin).astype('uint8')
     else:
       self.bin = np.array(self.bin).astype('float32')
     return self
 
   def load(self):
     # if binary file has existed, return self
     if self.bin is not None:
       return self
 
-    # if path is raw file load
+    # loading file in terms of their extension
     if os.path.splitext(os.path.basename(self.path))[1].upper() in ['.CR2', '.NEF', '.ARW']:
       self.bin = raw.read_raw(self.path)
       self.c, self.h, self.w = self.bin.shape
-
-    # else default to image
     else:
       self.bin = cv2.imread(self.path, cv2.IMREAD_UNCHANGED)
-      if len(self.bin.shape) == 2:
-        self.h, self.w = self.bin.shape
-        self.c = 1
-      elif len(self.bin.shape) == 3:
-        self.h, self.w, self.c = self.bin.shape
-      else:
-        raise NotImplementedError(self.bin.shape)
 
     return self
 
 #!<-----------------------------------------------------------------------------
 #!< BoxList Meta
 #!<-----------------------------------------------------------------------------
```

### Comparing `tw-3.8.1/tw/transform/__init__.py` & `tw-3.9.0/tw/transform/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 # augmentation
 from .primitive.affine import vflip
 from .primitive.affine import random_vflip
 from .primitive.affine import hflip
 from .primitive.affine import random_hflip
 from .primitive.affine import rotate
 from .primitive.affine import random_rotate
+from .primitive.affine import restoration_augment
+from .primitive.affine import random_affine
 
 from .primitive import bbox
 
 from .primitive.colorspace import change_colorspace
 from .primitive.colorspace import random_photometric_distortion
 
 from .primitive.crop import random_crop
@@ -81,14 +83,15 @@
 
 from .primitive.filter import random_iso_noise
 from .primitive.filter import random_gaussian_noise
 from .primitive.filter import random_gaussian_blur
 from .primitive.filter import random_median_blur
 from .primitive.filter import random_motion_blur
 from .primitive.filter import sobel
+from .primitive.filter import random_gamma
 
 from .primitive.morphology import random_alpha_to_trimap
 from .primitive.morphology import alpha_to_trimap
 
 from .primitive.normalize import to_tensor
 from .primitive.normalize import to_float
 from .primitive.normalize import equal_hist
```

### Comparing `tw-3.8.1/tw/models/transformer2d/vit.py` & `tw-3.9.0/tw/models/transformer2d/vit.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/res2net_v1b.py` & `tw-3.9.0/tw/models/res2net_v1b.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/ghostnet.py` & `tw-3.9.0/tw/models/ghostnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/mnasnet.py` & `tw-3.9.0/tw/models/mnasnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone3d/r2plus1d.py` & `tw-3.9.0/tw/models/backbone3d/r2plus1d.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone3d/c3d.py` & `tw-3.9.0/tw/models/backbone3d/c3d.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone3d/p3d.py` & `tw-3.9.0/tw/models/backbone3d/p3d.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone3d/i3d.py` & `tw-3.9.0/tw/models/backbone3d/i3d.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone3d/p3d_without_bn.py` & `tw-3.9.0/tw/models/backbone3d/p3d_without_bn.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone3d/r3d.py` & `tw-3.9.0/tw/models/backbone3d/r3d.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/resnets_deeplab.py` & `tw-3.9.0/tw/models/resnets_deeplab.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/mixnet.py` & `tw-3.9.0/tw/models/mixnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/alexnet.py` & `tw-3.9.0/tw/models/backbone2d/alexnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/vgg_cifar.py` & `tw-3.9.0/tw/models/backbone2d/vgg_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/mobilenet_v3.py` & `tw-3.9.0/tw/models/backbone2d/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/resnet_cifar.py` & `tw-3.9.0/tw/models/backbone2d/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/mobilenet_v2.py` & `tw-3.9.0/tw/models/backbone2d/mobilenet_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,19 @@
     # building last several layers
     features.append(ConvBNReLU(
         input_channel, self.last_channel, kernel_size=1))
     # make it nn.Sequential
     self.features = nn.Sequential(*features)
 
     # building classifier
-    self.classifier = nn.Sequential(
-        nn.Dropout(0.2),
-        nn.Linear(self.last_channel, num_classes),
-    )
+    if not output_backbone:
+      self.classifier = nn.Sequential(
+          nn.Dropout(0.2),
+          nn.Linear(self.last_channel, num_classes),
+      )
 
     # weight initialization
     for m in self.modules():
       if isinstance(m, nn.Conv2d):
         nn.init.kaiming_normal_(m.weight, mode='fan_out')
         if m.bias is not None:
           nn.init.zeros_(m.bias)
@@ -139,9 +140,9 @@
   Arguments:
       pretrained (bool): If True, returns a model pre-trained on ImageNet
       progress (bool): If True, displays a progress bar of the download to stderr
   """
   model = MobileNetV2(**kwargs)
   if pretrained:
     state_dict = load_state_dict_from_url(model_urls['mobilenet_v2'])
-    model.load_state_dict(state_dict)
+    model.load_state_dict(state_dict, strict=False)
   return model
```

### Comparing `tw-3.8.1/tw/models/backbone2d/resnet_tf.py` & `tw-3.9.0/tw/models/backbone2d/resnet_tf.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/shufflenet_v1_cifar.py` & `tw-3.9.0/tw/models/backbone2d/shufflenet_v1_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/squeezenet.py` & `tw-3.9.0/tw/models/backbone2d/squeezenet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/senet.py` & `tw-3.9.0/tw/models/backbone2d/senet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/efficientnet_cifar.py` & `tw-3.9.0/tw/models/backbone2d/efficientnet_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/shufflenet_v2_cifar.py` & `tw-3.9.0/tw/models/backbone2d/shufflenet_v2_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/vgg.py` & `tw-3.9.0/tw/models/backbone2d/vgg.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/mobilenet_v2_cifar.py` & `tw-3.9.0/tw/models/backbone2d/mobilenet_v2_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/senet_cifar.py` & `tw-3.9.0/tw/models/backbone2d/senet_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/mobilenet_v2_deeplab.py` & `tw-3.9.0/tw/models/backbone2d/mobilenet_v2_deeplab.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/googlenet.py` & `tw-3.9.0/tw/models/backbone2d/googlenet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/shufflenet_v2.py` & `tw-3.9.0/tw/models/backbone2d/shufflenet_v2.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/xception.py` & `tw-3.9.0/tw/models/backbone2d/xception.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/resnet.py` & `tw-3.9.0/tw/models/backbone2d/resnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/vgg_extractor.py` & `tw-3.9.0/tw/models/backbone2d/vgg_extractor.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/densenet.py` & `tw-3.9.0/tw/models/backbone2d/densenet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/bcnn.py` & `tw-3.9.0/tw/models/backbone2d/bcnn.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/inceptionresnetv2.py` & `tw-3.9.0/tw/models/backbone2d/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/densenet_cifar.py` & `tw-3.9.0/tw/models/backbone2d/densenet_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/backbone2d/efficientnet.py` & `tw-3.9.0/tw/models/backbone2d/efficientnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/__init__.py` & `tw-3.9.0/tw/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/mobilenet_v1.py` & `tw-3.9.0/tw/models/mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/inception.py` & `tw-3.9.0/tw/models/inception.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/res2net.py` & `tw-3.9.0/tw/models/res2net.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/fastscnn.py` & `tw-3.9.0/tw/models/segment2d/fastscnn.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/enet.py` & `tw-3.9.0/tw/models/segment2d/enet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/frvsr.py` & `tw-3.9.0/tw/models/segment2d/frvsr.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/espnet.py` & `tw-3.9.0/tw/models/segment2d/espnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/fenet.py` & `tw-3.9.0/tw/models/segment2d/fenet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/ocnet.py` & `tw-3.9.0/tw/models/segment2d/ocnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/bisenet.py` & `tw-3.9.0/tw/models/segment2d/bisenet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/deeplabv3p.py` & `tw-3.9.0/tw/models/segment2d/deeplabv3p.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/lenet.py` & `tw-3.9.0/tw/models/segment2d/lenet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/erfnet.py` & `tw-3.9.0/tw/models/segment2d/erfnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/poolnet.py` & `tw-3.9.0/tw/models/segment2d/poolnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/lednet.py` & `tw-3.9.0/tw/models/segment2d/lednet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/drn.py` & `tw-3.9.0/tw/models/segment2d/drn.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/icnet.py` & `tw-3.9.0/tw/models/segment2d/icnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/psanet.py` & `tw-3.9.0/tw/models/segment2d/psanet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/pspnet.py` & `tw-3.9.0/tw/models/segment2d/pspnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/dunet.py` & `tw-3.9.0/tw/models/segment2d/dunet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/ccnet.py` & `tw-3.9.0/tw/models/segment2d/ccnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/danet.py` & `tw-3.9.0/tw/models/segment2d/danet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/fcn.py` & `tw-3.9.0/tw/models/segment2d/fcn.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/encnet.py` & `tw-3.9.0/tw/models/segment2d/encnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/asffnet.py` & `tw-3.9.0/tw/models/segment2d/asffnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/utils.py` & `tw-3.9.0/tw/models/segment2d/utils.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/unet.py` & `tw-3.9.0/tw/models/segment2d/unet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/bgmv2.py` & `tw-3.9.0/tw/models/segment2d/bgmv2.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/segment2d/cgnet.py` & `tw-3.9.0/tw/models/segment2d/cgnet.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/moco.py` & `tw-3.9.0/tw/models/moco.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/tw/models/resnext_cifar.py` & `tw-3.9.0/tw/models/resnext_cifar.py`

 * *Files identical despite different names*

### Comparing `tw-3.8.1/setup.py` & `tw-3.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
       )
   ]
   return ext_modules
 
 
 setup(
     name="tw",
-    version="3.8.1",
+    version="3.9.0",
     author="Kai Jin",
     author_email="atranitell@gmail.com",
     description="TorchWrapper is a deep learning helper.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/atranitell/TensorWrapper",
     license="Apache 2.0 Licence",
@@ -124,19 +124,18 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     install_requires=[
         "matplotlib",
-        "opencv-python==3.*",
+        # "opencv-python==3.*",
         "numpy",
         "tensorboard",
         "tqdm",
         "cython",
         "scipy",
-        "rawpy",
-        "exifread"
-        # "kornia" corresponding to torch==1.4.0
+        # "rawpy",
+        # "exifread"
         # "kornia==0.2.2", # corresponding to torch==1.4.0
     ],
 )
```

