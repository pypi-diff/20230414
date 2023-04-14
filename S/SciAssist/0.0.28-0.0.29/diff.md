# Comparing `tmp/SciAssist-0.0.28.tar.gz` & `tmp/SciAssist-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciAssist-0.0.28.tar", last modified: Wed Mar 15 16:23:56 2023, max compression
+gzip compressed data, was "SciAssist-0.0.29.tar", last modified: Fri Apr 14 07:34:22 2023, max compression
```

## Comparing `SciAssist-0.0.28.tar` & `SciAssist-0.0.29.tar`

### file list

```diff
@@ -1,133 +1,142 @@
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.999786 SciAssist-0.0.28/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.28/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.28/MANIFEST.in
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-03-15 16:23:55.999786 SciAssist-0.0.28/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.28/README.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1378 2023-03-15 15:28:06.000000 SciAssist-0.0.28/pyproject.toml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-03-15 16:23:55.999786 SciAssist-0.0.28/setup.cfg
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.28/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      677 2023-03-15 15:36:30.000000 SciAssist-0.0.28/src/SciAssist/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/config.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/s2orc.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.995786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.995786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.995786 SciAssist-0.0.28/src/SciAssist/bin/doc2json/scripts/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/bin/doc2json/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.995786 SciAssist-0.0.28/src/SciAssist/datamodules/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/datamodules/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4111 2023-03-07 08:16:44.000000 SciAssist-0.0.28/src/SciAssist/datamodules/acl_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.995786 SciAssist-0.0.28/src/SciAssist/datamodules/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/datamodules/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/datamodules/components/cora_label.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.28/src/SciAssist/datamodules/cora_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.28/src/SciAssist/datamodules/fid_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.28/src/SciAssist/datamodules/general_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.28/src/SciAssist/datamodules/longsumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3229 2023-03-08 01:59:56.000000 SciAssist-0.0.28/src/SciAssist/datamodules/mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7564 2023-03-04 17:22:45.000000 SciAssist-0.0.28/src/SciAssist/datamodules/mup_scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-02-20 01:29:35.000000 SciAssist-0.0.28/src/SciAssist/datamodules/scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.28/src/SciAssist/datamodules/test_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.28/src/SciAssist/datamodules/xsum_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.995786 SciAssist-0.0.28/src/SciAssist/models/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/models/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.995786 SciAssist-0.0.28/src/SciAssist/models/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/models/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/models/components/bart_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/models/components/bert_token_classifier.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    10090 2022-12-05 04:05:34.000000 SciAssist-0.0.28/src/SciAssist/models/components/fid_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-03-07 07:57:37.000000 SciAssist-0.0.28/src/SciAssist/models/components/flant5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1565 2022-11-21 03:52:20.000000 SciAssist-0.0.28/src/SciAssist/models/components/frost_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1590 2022-11-08 07:42:28.000000 SciAssist-0.0.28/src/SciAssist/models/components/longt5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.28/src/SciAssist/models/cora_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13466 2023-03-11 10:35:23.000000 SciAssist-0.0.28/src/SciAssist/models/mup_bart_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7880 2022-11-15 05:02:37.000000 SciAssist-0.0.28/src/SciAssist/models/mup_fid_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8141 2022-12-11 12:29:46.000000 SciAssist-0.0.28/src/SciAssist/models/mup_frost_module.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.995786 SciAssist-0.0.28/src/SciAssist/pipelines/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3358 2023-03-15 13:49:38.000000 SciAssist-0.0.28/src/SciAssist/pipelines/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.28/src/SciAssist/pipelines/pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.28/src/SciAssist/pipelines/reference_string_parsing.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13928 2023-03-02 03:17:19.000000 SciAssist-0.0.28/src/SciAssist/pipelines/summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-02-03 14:41:15.000000 SciAssist-0.0.28/src/SciAssist/pipelines/summarization_origin.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.28/src/SciAssist/pipelines/testing_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.28/src/SciAssist/pipelines/training_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.28/src/SciAssist/test.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.28/src/SciAssist/train.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.28/src/SciAssist/training_args.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.999786 SciAssist-0.0.28/src/SciAssist/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.28/src/SciAssist/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.999786 SciAssist-0.0.28/src/SciAssist/utils/collators/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.28/src/SciAssist/utils/collators/CollatorForFid.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.28/src/SciAssist/utils/collators/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.28/src/SciAssist/utils/data_reader.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    65129 2023-03-05 13:37:47.000000 SciAssist-0.0.28/src/SciAssist/utils/data_utils.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1751 2023-03-01 06:47:44.000000 SciAssist-0.0.28/src/SciAssist/utils/evaluate_sr.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      599 2023-02-23 04:13:53.000000 SciAssist-0.0.28/src/SciAssist/utils/extract_acl.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1912 2023-01-09 01:58:56.000000 SciAssist-0.0.28/src/SciAssist/utils/extract_keywords.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2430 2023-03-04 17:52:51.000000 SciAssist-0.0.28/src/SciAssist/utils/extract_keywords_flant5.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1679 2023-02-10 16:41:07.000000 SciAssist-0.0.28/src/SciAssist/utils/extract_keywords_yake.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3640 2023-01-08 13:42:08.000000 SciAssist-0.0.28/src/SciAssist/utils/pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1502 2023-03-07 08:47:10.000000 SciAssist-0.0.28/src/SciAssist/utils/testset.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2203 2023-03-08 02:07:35.000000 SciAssist-0.0.28/src/SciAssist/utils/windows_pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1327 2023-01-25 09:41:26.000000 SciAssist-0.0.28/src/SciAssist/utils/xml2txt.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.991786 SciAssist-0.0.28/src/SciAssist.egg-info/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-03-15 16:23:55.000000 SciAssist-0.0.28/src/SciAssist.egg-info/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5050 2023-03-15 16:23:55.000000 SciAssist-0.0.28/src/SciAssist.egg-info/SOURCES.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-03-15 16:23:55.000000 SciAssist-0.0.28/src/SciAssist.egg-info/dependency_links.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-03-15 16:23:55.000000 SciAssist-0.0.28/src/SciAssist.egg-info/entry_points.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      356 2023-03-15 16:23:55.000000 SciAssist-0.0.28/src/SciAssist.egg-info/requires.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       44 2023-03-15 16:23:55.000000 SciAssist-0.0.28/src/SciAssist.egg-info/top_level.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1321 2023-03-05 16:03:26.000000 SciAssist-0.0.28/src/chatsonic.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7944 2022-12-04 10:40:25.000000 SciAssist-0.0.28/src/convert_pegasus.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.28/src/process.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-03-15 16:23:55.999786 SciAssist-0.0.28/tests/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.28/tests/test_rsp.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.28/tests/test_summ.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.29/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.29/MANIFEST.in
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-14 07:34:22.097593 SciAssist-0.0.29/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.29/README.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1379 2023-04-14 07:14:09.000000 SciAssist-0.0.29/pyproject.toml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-14 07:34:22.101593 SciAssist-0.0.29/setup.cfg
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.29/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/config.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/s2orc.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/scripts/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/datamodules/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/datamodules/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.29/src/SciAssist/datamodules/acl_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/datamodules/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/datamodules/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/datamodules/components/cora_label.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.29/src/SciAssist/datamodules/cora_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/datamodules/dataset_extraction_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.29/src/SciAssist/datamodules/fid_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.29/src/SciAssist/datamodules/general_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.29/src/SciAssist/datamodules/longsumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.29/src/SciAssist/datamodules/mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.29/src/SciAssist/datamodules/mup_mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-04-14 07:04:55.000000 SciAssist-0.0.29/src/SciAssist/datamodules/mup_scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.29/src/SciAssist/datamodules/scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.29/src/SciAssist/datamodules/test_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.29/src/SciAssist/datamodules/xsum_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/models/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/models/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/models/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/models/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/models/components/bart_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/models/components/bert_dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/models/components/bert_token_classifier.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    10090 2022-12-05 04:05:34.000000 SciAssist-0.0.29/src/SciAssist/models/components/fid_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-14 06:59:33.000000 SciAssist-0.0.29/src/SciAssist/models/components/flant5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1565 2022-11-21 03:52:20.000000 SciAssist-0.0.29/src/SciAssist/models/components/frost_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1590 2022-11-08 07:42:28.000000 SciAssist-0.0.29/src/SciAssist/models/components/longt5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.29/src/SciAssist/models/cora_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/models/dataset_extraction_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.29/src/SciAssist/models/mup_bart_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7880 2022-11-15 05:02:37.000000 SciAssist-0.0.29/src/SciAssist/models/mup_fid_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8141 2023-04-14 07:09:36.000000 SciAssist-0.0.29/src/SciAssist/models/mup_frost_module.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/pipelines/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4193 2023-04-14 07:13:16.000000 SciAssist-0.0.29/src/SciAssist/pipelines/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/pipelines/dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.29/src/SciAssist/pipelines/pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.29/src/SciAssist/pipelines/reference_string_parsing.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    14508 2023-04-14 07:09:05.000000 SciAssist-0.0.29/src/SciAssist/pipelines/summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-04-14 07:08:00.000000 SciAssist-0.0.29/src/SciAssist/pipelines/summarization_origin.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.29/src/SciAssist/pipelines/testing_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.29/src/SciAssist/pipelines/training_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/test.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.29/src/SciAssist/train.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.29/src/SciAssist/training_args.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.29/src/SciAssist/utils/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2714 2023-03-25 10:51:15.000000 SciAssist-0.0.29/src/SciAssist/utils/acl.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/utils/collators/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.29/src/SciAssist/utils/collators/CollatorForFid.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.29/src/SciAssist/utils/collators/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.29/src/SciAssist/utils/data_reader.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    75293 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/utils/data_utils.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    60999 2023-04-14 06:53:22.000000 SciAssist-0.0.29/src/SciAssist/utils/data_utils2.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1751 2023-03-01 06:47:44.000000 SciAssist-0.0.29/src/SciAssist/utils/evaluate_sr.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      661 2023-03-25 10:26:12.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_acl.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5324 2023-03-30 02:58:27.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keysents.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1912 2023-01-09 01:58:56.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keywords.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2655 2023-04-05 08:52:04.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_flant5.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1573 2023-03-19 09:05:48.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_tfidf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1703 2023-04-05 08:45:37.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_yake.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5041 2023-03-25 10:36:56.000000 SciAssist-0.0.29/src/SciAssist/utils/pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1502 2023-03-07 08:47:10.000000 SciAssist-0.0.29/src/SciAssist/utils/testset.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2261 2023-03-27 00:48:06.000000 SciAssist-0.0.29/src/SciAssist/utils/windows_pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1499 2023-03-22 11:40:06.000000 SciAssist-0.0.29/src/SciAssist/utils/xml2txt.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist.egg-info/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5460 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/SOURCES.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/dependency_links.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/entry_points.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      356 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/requires.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       65 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/top_level.txt
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)     1321 2023-03-05 16:03:26.000000 SciAssist-0.0.29/src/chatsonic.py
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)     7944 2022-12-04 10:40:25.000000 SciAssist-0.0.29/src/convert_pegasus.py
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.29/src/process.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/tests/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.29/tests/test_rsp.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.29/tests/test_summ.py
```

### Comparing `SciAssist-0.0.28/LICENSE` & `SciAssist-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/PKG-INFO` & `SciAssist-0.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.28
+Version: 0.0.29
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.28/README.md` & `SciAssist-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/pyproject.toml` & `SciAssist-0.0.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SciAssist"
-version = "0.0.28"
+version = "0.0.29"
 authors = [
   { name="WING-NUS", email="dingyixi@hotmail.com" },
 ]
 maintainers = [
   { name="Yixi Ding", email="dingyixi@hotmail.com" },
 ]
 description = "A toolkit for Scientific Document Processing"
@@ -38,15 +38,15 @@
     "seaborn~=0.11.2",
     "setuptools>=61.0",
     "torch>=1.12.0",
     "torchmetrics>=0.7.0",
     "transformers~=4.19.2",
     "wandb~=0.12.19",
     "pdfminer.six",
-    "pandas~=1.4.3"
+    "pandas~=1.4.3",
 ]
 
 
 [project.scripts]
 setup_grobid = "SciAssist.bin:setup_grobid"
 run_grobid = "SciAssist.bin:run_grobid"
```

### Comparing `SciAssist-0.0.28/setup.cfg` & `SciAssist-0.0.29/setup.cfg`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/__init__.py` & `SciAssist-0.0.29/src/SciAssist/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import os
 import platform
 
 ROOT_DIR = os.getcwd()
 BASE_OUTPUT_DIR = os.path.join(ROOT_DIR, "output/result")
 BASE_TEMP_DIR = os.path.join(ROOT_DIR,"output/.temp")
+os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 USER_DIR_MAP = {
     "linux": "HOME",
+    "darwin": "HOME",
     "windows": "USERPROFILE"
 }
 USER_DIR = os.environ[USER_DIR_MAP[platform.system().lower()]]
 # Directory for cached files, including checkpoints, model dicts, tokenizers involved in pipelines.
 # Unlike `cache_dir` set in config files, this is for users.
 
 BASE_CACHE_DIR = os.path.join(USER_DIR, ".cache/sciassist")
 
 
 from SciAssist.pipelines.reference_string_parsing import ReferenceStringParsing
-from SciAssist.pipelines.summarization import Summarization
+from SciAssist.pipelines.summarization import Summarization
+from SciAssist.pipelines.dataset_extraction import DatasetExtraction
```

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/__init__.py` & `SciAssist-0.0.29/src/SciAssist/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/LICENSE` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/s2orc.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/s2orc.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh` & `SciAssist-0.0.29/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/acl_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/acl_datamodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,29 +41,29 @@
 
         # Prepare keywords
         text = []
         summ = []
         kw = []
         id = []
         lengths = []
-        with open("/home/dingyx/project/SciAssist/data/pdfs/test.csv", 'r', newline='', encoding='ISO-8859-1') as f:
+        with open("/home/yixi/project/sciassist/data/pdfs/text/test.csv", 'r', newline='', encoding='ISO-8859-1') as f:
             rows = csv.reader(f)
             # Get Column names
             keys = next(rows)
             # Add values by column
             for row in rows:
 
                 kws = row[2].split(",")
 
                 kws = [kws[0]]
 
-                with open("/home/dingyx/project/SciAssist/data/pdfs/summary_flant5/" + row[0] + ".txt" , "w") as f:
+                with open("/home/yixi/project/sciassist/data/pdfs/summary_ours/" + row[0] + ".txt" , "w") as f:
                     f.write(" ".join(kws) + " => ")
                 # for i in range(5):
-                    with open("/home/dingyx/project/SciAssist/data/pdfs/" + row[1], "r") as t:
+                    with open("/home/yixi/project/sciassist/data/pdfs/text/" + row[1], "r") as t:
                         txt = t.readlines()
                         txt = " ".join(txt)
                         text.append(txt)
                     summ.append("a")
                     kw.append(kws)
                     id.append(int(row[0]))
                     lengths.append(100)
```

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/cora_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/cora_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/fid_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/fid_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/general_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/general_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/longsumm_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/longsumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/mup_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/mup_datamodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Optional
 
 import datasets
 from datasets import Dataset, DatasetDict
 from pytorch_lightning import LightningDataModule
 from torch.utils.data import DataLoader
 
-from SciAssist.utils.data_reader import csv_reader
 from SciAssist.utils.data_utils import DataUtilsForSeq2Seq
 
 
 class MupDataModule(LightningDataModule):
     def __init__(
         self,
         data_repo: str,
@@ -35,15 +34,15 @@
     def prepare_data(self) -> DatasetDict:
         raw_datasets = datasets.load_dataset(
             self.hparams.data_repo,
             cache_dir=self.data_cache_dir
         )
 
         # Get test from csv
-        raw_datasets["test"] = csv_reader("data/mup/test-release.csv")
+        # raw_datasets["test"] = csv_reader("data/mup/test-release.csv")
         return raw_datasets
 
     def setup(self, stage: Optional[str] = None):
         if not self.data_train and not self.data_val and not self.data_test:
             processed_datasets = self.prepare_data()
             tokenized_datasets = processed_datasets.map(
                 lambda x: self.data_utils.tokenize_and_align_labels(x, inputs_column="text", labels_column="summary"),
```

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/mup_scisumm_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/mup_mup_datamodule.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,41 +100,45 @@
 
     def prepare_data(self) -> DatasetDict:
 
         # Prepare keywords
         summ = []
         kw = []
         text = []
-        with open("/home/dingyx/project/SciAssist/data/Task2/From-ScisummNet-2019/mup_flant5_target_Entities_sci2.csv", 'r', newline='', encoding='ISO-8859-1') as f:
+        with open("/home/yixi/project/sciassist/data/train2.csv", 'r', newline='', encoding='ISO-8859-1') as f:
             rows = csv.reader(f)
             # Get Column names
             keys = next(rows)
             # Add values by column
             for row in rows:
-
-                kws = row[4].split(",")
-                summ.append(row[2])
-                kw.append(kws)
-                text.append(row[3])
+                if row[0].isnumeric():
+                    kws = row[4].split(",")
+                    kws = list(set(kws))
+                    summ.append(row[2])
+                    kw.append(kws)
+                    text.append(row[3])
                 # lengths.append(100)
 
         lengths = [len(s.split(" ")) for s in summ]
         lengths = [50*math.ceil(s/50) for s in lengths]
 
         mask1=[]
         mask2=[]
-        for i in range(len(text)/2):
-            mask1.append(random.randint(0, len(text)))
-        for i in range(len(text)/2):
-            mask2.append(random.randint(0, len(text)))
+        mask1 = random.sample(range(0, int(len(text))), int(len(text) / 3))
+        mask2 = random.sample(range(0, int(len(text))), int(len(text) / 5))
+
+        # for i in range(int(len(text)/3)):
+        #     mask2.append(random.randint(0, len(text)-1))
 
         for i in mask1:
-            kw[i] = None
+            if len(kw[i])<=1:
+                kw[i] = None
         for i in mask2:
-            lengths[i] = None
+            if lengths[i] <= 100:
+                lengths[i] = None
 
         raw_datasets = DatasetDict()
         raw_datasets["train"] = {
             "text": text,
             "summary": summ,
             "keywords": kw,
             "length": lengths
```

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/scisumm_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/test_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/datamodules/xsum_datamodule.py` & `SciAssist-0.0.29/src/SciAssist/datamodules/xsum_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/components/bart_summarization.py` & `SciAssist-0.0.29/src/SciAssist/models/components/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/components/bert_token_classifier.py` & `SciAssist-0.0.29/src/SciAssist/models/components/bert_token_classifier.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/components/fid_summarization.py` & `SciAssist-0.0.29/src/SciAssist/models/components/fid_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/components/flant5_summarization.py` & `SciAssist-0.0.29/src/SciAssist/models/components/flant5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/components/frost_summarization.py` & `SciAssist-0.0.29/src/SciAssist/models/components/frost_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/components/longt5_summarization.py` & `SciAssist-0.0.29/src/SciAssist/models/components/longt5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/cora_module.py` & `SciAssist-0.0.29/src/SciAssist/models/cora_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/mup_bart_module.py` & `SciAssist-0.0.29/src/SciAssist/models/mup_bart_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # main developer: Yixi Ding <dingyixi@hotmail.com>
 import math
 import os
 from pathlib import Path
 from typing import Any, List
 
-import numpy
+import bert_score
 import numpy as np
+import pandas as pd
 import torch
 from pytorch_lightning import LightningModule
 from scipy.stats import pearsonr
 from torchmetrics import MaxMetric
-from torchmetrics.text.rouge import ROUGEScore
 from torchmetrics.text.bert import BERTScore
+from torchmetrics.text.rouge import ROUGEScore
 from transformers import AutoModelForSeq2SeqLM
-import pandas as pd
 
 from SciAssist.utils.data_utils import DataUtilsForSeq2Seq
-import bert_score
+
 
 class MupBartLitModule(LightningModule):
     def __init__(
         self,
         model: AutoModelForSeq2SeqLM,
         data_utils = DataUtilsForSeq2Seq,
         lr: float = 2e-5,
     ):
         super().__init__()
         self.save_hyperparameters(logger=False)
         self.data_utils = data_utils
         self.model = model
-        self.model.load_state_dict(torch.load("/home/dingyx/project/SciAssist/src/pretrained/flant5_mup/flant5-base-mup.pt"))
 
         self.val_metric = ROUGEScore(use_stemmer=True)
         self.val_best_Rouge1 = MaxMetric()
         self.val_best_bertscore = MaxMetric()
         self.test_bertscore = BERTScore(use_stemmer=True)
         self.test_metric = ROUGEScore(use_stemmer=True)
         self.test_best_Rouge1 = MaxMetric()
@@ -152,15 +151,15 @@
         self.log("val/gen_len", self.val_gen_len, on_step=False, on_epoch=True, prog_bar=True)
         self.log("val/best_rouge1", self.val_best_Rouge1.compute(), on_epoch=True, prog_bar=True)
 
     def test_step(self, batch: Any, batch_idx: int):
         input_ids = batch["input_ids"]
         attention_mask = batch["attention_mask"]
         result = {}
-        # torch.save(self.model.state_dict(), "/home/dingyx/project/SciAssist/src/pretrained/flant5_mup_scisumm/latest.pt")
+        # torch.save(self.model.state_dict(), "/home/yixi/project/sciassist/src/pretrained/flant5_mup/negative.pt")
         # torch.save(self.model,"/home/dingyx/project/SciAssist/src/pretrained/flant5_mup/checkpoints/epoch_001.ckpt")
         # print("finished")
 
         if "labels" not in batch.keys():
             # Simply do prediction
             preds = self.model.generate(input_ids=input_ids, attention_mask=attention_mask)
             decoded_preds = self.data_utils.tokenizer.batch_decode(preds, skip_special_tokens=True)
```

### Comparing `SciAssist-0.0.28/src/SciAssist/models/mup_fid_module.py` & `SciAssist-0.0.29/src/SciAssist/models/mup_fid_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/models/mup_frost_module.py` & `SciAssist-0.0.29/src/SciAssist/models/mup_frost_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/pipelines/__init__.py` & `SciAssist-0.0.29/src/SciAssist/pipelines/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # main developer: Yixi Ding <dingyixi@hotmail.com>
 
 from typing import Dict
 
 import torch
 
 from SciAssist import BASE_CACHE_DIR
-from SciAssist.models.components.bart_summarization import BartForSummarization
 from SciAssist.models.components.bert_token_classifier import BertForTokenClassifier
 from SciAssist.models.components.flant5_summarization import FlanT5ForSummarization
+from SciAssist.models.components.bert_dataset_extraction import BertForDatasetExtraction
 from SciAssist.utils.data_utils import (
     DataUtilsForTokenClassification,
     DataUtilsForSeq2Seq, DataUtilsForFlanT5, DataUtilsForT5,
+    DataUtilsForSeq2Seq,
+    DataUtilsForDatasetExtraction
 )
 
 # Provided models for each task
 TASKS = {
     "reference-string-parsing": {
         "scibert-on-cora":  {
             "model": BertForTokenClassifier,
@@ -54,15 +56,30 @@
     "controlled-summarization": {
         "default": {
             "model": FlanT5ForSummarization,
             "model_dict_url": "https://huggingface.co/spaces/dyxohjl666/Controlled-summarization/resolve/main/flant5-mup-scisumm.pt",
             # "model_dict_url": None,
             "data_utils": DataUtilsForFlanT5,
         }
-    }
+    },
+    "dataset-extraction": {
+        "default": {
+            "model": BertForDatasetExtraction,
+            "model_dict_url": "https://huggingface.co/spaces/wing-nus/SciAssist/resolve/main/dataset-extraction.pt",
+            "data_utils": DataUtilsForDatasetExtraction,
+        },
+    },
+
+    # "controlled-summarization": {
+    #     "default": {
+    #         "model": FrostForSummarization,
+    #         "model_dict_url": None,
+    #         "data_utils": DataUtilsForFrost,
+    #     }
+    # }
 
 }
 
 def load_model(config: Dict, cache_dir=BASE_CACHE_DIR, device="gpu"):
     '''
 
     Args:
@@ -81,10 +98,15 @@
     print("Loading the model...")
     model_class = config["model"]
     model = model_class(cache_dir=cache_dir)
     map_location = None if torch.cuda.is_available() and device in ["gpu","cuda"] else torch.device("cpu")
     if config["model_dict_url"]!=None:
         state_dict = torch.hub.load_state_dict_from_url(config["model_dict_url"], model_dir=cache_dir, map_location=map_location)
         model.load_state_dict(state_dict)
+    else:
+        # You can also choose to load your local trained model:
+        # model.load_state_dict(torch.load("/home/linxiao/SciAssist-scibert-0223/src/models/scibert_ner/2023-03-25_02-27-17/scibert_dataset_extraction.pt"))
+        pass
+
     model.eval()
 
     return model
```

### Comparing `SciAssist-0.0.28/src/SciAssist/pipelines/pipeline.py` & `SciAssist-0.0.29/src/SciAssist/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/pipelines/reference_string_parsing.py` & `SciAssist-0.0.29/src/SciAssist/pipelines/reference_string_parsing.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/pipelines/summarization.py` & `SciAssist-0.0.29/src/SciAssist/pipelines/summarization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # main developer: Yixi Ding <dingyixi@hotmail.com>
 import json
+import math
 import os
 from typing import List, Tuple, Optional, Dict
 
-import torch
 from datasets import Dataset
 
 from SciAssist import BASE_TEMP_DIR, BASE_OUTPUT_DIR
 from SciAssist.pipelines.pipeline import Pipeline
+from SciAssist.pipelines.testing_pipeline import test
 from SciAssist.utils.pdf2text import process_pdf_file, get_bodytext
 from SciAssist.utils.windows_pdf2text import windows_get_bodytext
-from SciAssist.pipelines.testing_pipeline import test
+
 
 class Summarization(Pipeline):
     """
     The pipeline for single document summarization.
 
     Args:
         model_name (`str`, *optional*):
@@ -62,17 +63,19 @@
             os_name=None,
     ):
         super().__init__(task_name="controlled-summarization", model_name=model_name, device=device,
                          cache_dir=cache_dir, output_dir=output_dir, temp_dir=temp_dir)
         # self.model.load_state_dict(
         #     torch.load("/home/dingyx/project/SciAssist/src/pretrained/flant5_scisumm_mup/flant5-base-mix-mup-scisumm-keywords.pt"))
         # self.model.load_state_dict(
-        #     torch.load("/home/dingyx/project/SciAssist/src/pretrained/flant5_mup_scisumm/latest.pt")
+        #     torch.load("/home/yixi/project/sciassist/src/pretrained/flant5_mup/flant5-base-mup-scisumm-repeat10.pt")
+        # )
+        # self.model.load_state_dict(
+        #     torch.load("/home/yixi/project/sciassist/src/pretrained/flant5_mup/flant5-base.pt")
         # )
-
         self.data_utils = self.data_utils(
             tokenizer=tokenizer,
             model_class=self.config["model"],
             checkpoint=checkpoint,
             model_max_length=model_max_length,
             max_source_length=max_source_length,
             max_target_length=max_target_length
@@ -224,16 +227,20 @@
             num_beams (`int`): Number of beams for beam search. 1 means no beam search.
             num_return_sequences(`int`): The number of independently computed returned sequences for each element in the batch.
         Returns:
            `Tuple[str, str]`:
                 Predicted summarization and source text.
 
         """
+        num = 10
         res = self._summarize([example], num_beams, num_return_sequences,length=length, keywords=keywords)
-
+        if length is not None:
+            num = 5*math.ceil(length/50)
+        # if keywords is not None:
+        #     example = extract_related_sentences(example,keywords[0],num)
         return {"summary": res, "raw_text": example}
 
     def _summarize_for_text(
             self,
             filename: str,
             num_beams: int = 1,
             num_return_sequences: int = 1,
@@ -250,20 +257,23 @@
             num_return_sequences(`int`): The number of independently computed returned sequences for each element in the batch.
 
         Returns:
             `Tuple[str, str]`:
                 Predicted summarization and source text.
 
         """
-
+        num = 10
+        if length is not None:
+            num = 5 * math.ceil(length / 50)
         with open(filename, "r") as f:
             examples = f.readlines()
         examples = [" ".join(examples)]
         res = self._summarize(examples, num_beams, num_return_sequences,length=length,keywords=keywords)
-
+        # if keywords is not None:
+        #     examples = [extract_related_sentences(examples[0], keywords[0],num)]
         return {"summary": res, "raw_text": examples[0]}
 
     def _summarize_for_pdf(
             self,
             filename: str,
             temp_dir: Optional[str] = BASE_TEMP_DIR,
             output_dir: Optional[str] = BASE_OUTPUT_DIR,
```

### Comparing `SciAssist-0.0.28/src/SciAssist/pipelines/summarization_origin.py` & `SciAssist-0.0.29/src/SciAssist/pipelines/summarization_origin.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/pipelines/testing_pipeline.py` & `SciAssist-0.0.29/src/SciAssist/pipelines/testing_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/pipelines/training_pipeline.py` & `SciAssist-0.0.29/src/SciAssist/pipelines/training_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/test.py` & `SciAssist-0.0.29/src/SciAssist/test.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/train.py` & `SciAssist-0.0.29/src/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/training_args.py` & `SciAssist-0.0.29/src/SciAssist/training_args.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/__init__.py` & `SciAssist-0.0.29/src/SciAssist/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/collators/CollatorForFid.py` & `SciAssist-0.0.29/src/SciAssist/utils/collators/CollatorForFid.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/data_reader.py` & `SciAssist-0.0.29/src/SciAssist/utils/data_reader.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/data_utils.py` & `SciAssist-0.0.29/src/SciAssist/utils/data_utils2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import math
 from typing import List, Dict
 
 import nltk
 import numpy as np
 import torch
-from SciAssist.models.components.fid_summarization import FiDT5
 from torch.utils.data import DataLoader
 from transformers import AutoTokenizer
 from transformers import DataCollatorForSeq2Seq
 
 from SciAssist import BASE_CACHE_DIR
 from SciAssist.datamodules.components.cora_label import label2id as cora_label2id
 from SciAssist.models.components.bart_summarization import BartForSummarization
@@ -368,340 +366,14 @@
             batch_size=8,
             collate_fn=self.collator(),
         )
 
         return dataloader
 
 
-class DataUtilsForFiD():
-    """
-
-    Args:
-        tokenizer (`PretrainedTokenizer`, default to None):
-            The tokenizer for tokenization.
-        checkpoint (`str`):
-            The checkpoint from which the tokenizer is loaded.
-        model_max_length (`int`, *optional*): The max sequence length the model accepts.
-        max_source_length (`int`, *optional*): The max length of the input text.
-        max_target_length (`int`, *optional*): The max length of the generated summary.
-    """
-
-    def __init__(self, tokenizer = None, model_class = FiDT5,
-                 checkpoint = "google/flan-t5-large",
-                 model_max_length = 64,
-                 max_source_length = 64,
-                 max_target_length = 128,
-                 ):
-
-        self.checkpoint = checkpoint
-        self.model_max_length = model_max_length
-        self.max_source_length = max_source_length
-        self.max_target_length = max_target_length
-        self.model_class = model_class
-
-        if tokenizer is None:
-            self.tokenizer = AutoTokenizer.from_pretrained(
-                self.checkpoint,
-                model_max_length = self.model_max_length,
-                cache_dir=BASE_CACHE_DIR,
-            )
-        else:
-            self.tokenizer = tokenizer
-
-
-    def tokenize_and_align_labels(self, examples, inputs_column="text", labels_column="summary", token_per_paragraph=50):
-
-        """
-
-        Process the dataset for model input, for example, do tokenization and prepare label_ids.
-
-        Args:
-            examples (`Dataset`): { "text": [s1, s2, ...], "summary": [l1, l2, ...]}
-            inputs (`str`): The name of input column
-            labels (`str`): The name of target column
-
-        Returns:
-            `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
-
-        """
-
-        # Select input column
-        inputs = examples[inputs_column]
-        dataset = {"paragraphs": []}
-
-        for input in inputs:
-            texts = ["Please give a summary of the following text: "]
-            tokens = input.split(" ")
-            index = 0
-            while index+token_per_paragraph < min(len(tokens),120*token_per_paragraph):
-                p = " ".join(tokens[index:index+token_per_paragraph])
-                texts.append(p)
-                index += token_per_paragraph
-            texts.append(" ".join(tokens[index:index+token_per_paragraph]))
-            dataset["paragraphs"].append(texts)
-
-
-        # Select target column
-        if labels_column in examples.keys():
-            labels = examples[labels_column]
-            dataset["labels"] = labels
-
-        return dataset
-
-    def collator(self):
-
-        """
-
-        The collating function.
-
-        Returns:
-            `function`: A collating function.
-
-            For example, **DataCollatorForSeq2Seq(...)**.
-
-            You can also custom a collating function, but remember that `collator()` needs to return a **function**.
-        """
-
-        from SciAssist.utils.collators.CollatorForFid import DataCollatorForFid
-
-        return DataCollatorForFid(self.max_source_length, self.tokenizer, self.max_target_length)
-
-    def postprocess(self, preds, labels):
-
-        """
-        Process model's outputs and get the final results rather than simple ids.
-
-        Args:
-            preds (Tensor): Prediction labels, the output of the model.
-            labels (Tensor): True labels
-
-        Returns:
-            `(LongTensor, LongTensor)`: decoded_preds, decoded_labels
-
-        """
-
-        decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
-
-        labels = np.array(labels.to("cpu"))
-        # Replace -100 in the labels as we can't decode them.
-        labels = np.where(labels != -100, labels, self.tokenizer.pad_token_id)
-
-        decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=True)
-
-        decoded_preds = [pred.strip() for pred in decoded_preds]
-        decoded_labels = [label.strip() for label in decoded_labels]
-
-        # rougeLSum expects newline after each sentence
-        decoded_preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in decoded_preds]
-        decoded_labels = ["\n".join(nltk.sent_tokenize(label)) for label in decoded_labels]
-
-        return decoded_preds, decoded_labels
-
-    def get_dataloader(self, dataset, inputs_column="text", labels_column="summary"):
-
-        """
-        Generate DataLoader for a dataset.
-
-        Args:
-            dataset (`Dataset`): The raw dataset.
-            inputs_column (`str`): Column name of the inputs.
-            labels_column (`str`): Column name of the labels.
-
-        Returns:
-            `DataLoader`: A dataloader for the dataset. Will be used for inference.
-        """
-
-        tokenized_example = dataset.map(
-            lambda x: self.tokenize_and_align_labels(x, inputs_column=inputs_column, labels_column=labels_column),
-            batched=True,
-            remove_columns=dataset.column_names
-        )
-        dataloader = DataLoader(
-            dataset=tokenized_example,
-            batch_size=8,
-            collate_fn=self.collator(),
-        )
-
-        return dataloader
-
-#
-#
-# class DataUtilsForFrost():
-#     """
-#
-#     Args:
-#         tokenizer (`PretrainedTokenizer`, default to None):
-#             The tokenizer for tokenization.
-#         checkpoint (`str`):
-#             The checkpoint from which the tokenizer is loaded.
-#         model_max_length (`int`, *optional*): The max sequence length the model accepts.
-#         max_source_length (`int`, *optional*): The max length of the input text.
-#         max_target_length (`int`, *optional*): The max length of the generated summary.
-#     """
-#
-#
-#     def __init__(self, tokenizer = None, model_class = FrostForSummarization,
-#                  checkpoint = "pegasus/frost",
-#                  model_max_length = 1024,
-#                  max_source_length = 1024,
-#                  max_target_length = 128,
-#                  ):
-#
-#         self.checkpoint = checkpoint
-#         self.model_max_length = model_max_length
-#         self.max_source_length = max_source_length
-#         self.max_target_length = max_target_length
-#         self.model_class = model_class
-#
-#         if tokenizer is None:
-#             self.tokenizer = PegasusTokenizer.from_pretrained(
-#                 self.checkpoint,
-#                 cache_dir=BASE_CACHE_DIR,
-#                 model_max_length=self.model_max_length,
-#             )
-#         else:
-#             self.tokenizer = tokenizer
-#
-#         # FROST Constants
-#         self.ENTITYCHAIN_START_TOKEN = "[CONTENT]"
-#         self.SUMMARY_START_TOKEN = "[SUMMARY]"
-#         self.ENTITY_SEPARATOR = " | "
-#         self.ENTITY_SENTENCE_SEPARATOR = " ||| "
-#
-#         # Prepare Spacy processor
-#         self.SPACY_MODEL_OR_PATH = "en_core_web_sm"
-#         self.SPACY_PROCESSOR = spacy.load(self.SPACY_MODEL_OR_PATH)
-#
-#     def get_frost_labels(self, text):
-#         """Gets Spacy Frost processor."""
-#         entity_plans = []
-#         for text_sent in self.SPACY_PROCESSOR(text.replace("\n", " ")).sents:
-#             entity_plans.append(
-#                 self.ENTITY_SEPARATOR.join(
-#                     [entity.text for entity in self.SPACY_PROCESSOR(text_sent.text).ents]))
-#         text_with_entityplans = (
-#                 self.ENTITYCHAIN_START_TOKEN + " " +
-#                 self.ENTITY_SENTENCE_SEPARATOR.join(entity_plans) + " " +
-#                 self.SUMMARY_START_TOKEN + " " + text)
-#         return text_with_entityplans
-#
-#
-#     def tokenize_and_align_labels(self, examples, inputs_column="text", labels_column="summary"):
-#
-#         """
-#
-#         Process the dataset for model input, for example, do tokenization and prepare label_ids.
-#
-#         Args:
-#             examples (`Dataset`): { "text": [s1, s2, ...], "summary": [l1, l2, ...]}
-#             inputs (`str`): The name of input column
-#             labels (`str`): The name of target column
-#
-#         Returns:
-#             `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
-#
-#         """
-#
-#         # Select input column
-#         inputs = examples[inputs_column]
-#
-#         # Setup the tokenizer for inputs
-#         model_inputs = self.tokenizer(inputs, max_length=self.max_target_length, padding="max_length", truncation=True)
-#
-#         # Select target column
-#         if labels_column in examples.keys():
-#             labels = examples[labels_column]
-#             labels = [self.get_frost_labels(label) for label in labels]
-#
-#             # Setup the tokenizer for targets
-#             with self.tokenizer.as_target_tokenizer():
-#                 labels = self.tokenizer(labels, max_length=self.max_target_length, padding="max_length", truncation=True)
-#                 # Ignore padding in the loss
-#                 labels["input_ids"] = [
-#                     [(l if l != self.tokenizer.pad_token_id else -100) for l in label] for label in labels["input_ids"]
-#                 ]
-#
-#             model_inputs["labels"] = labels["input_ids"]
-#
-#         return model_inputs
-#
-#     def collator(self):
-#
-#         """
-#
-#         The collating function.
-#
-#         Returns:
-#             `function`: A collating function.
-#
-#             For example, **DataCollatorForSeq2Seq(...)**.
-#
-#             You can also custom a collating function, but remember that `collator()` needs to return a **function**.
-#         """
-#
-#
-#         return DataCollatorForSeq2Seq(self.tokenizer, model=self.model_class, pad_to_multiple_of=8)
-#
-#     def postprocess(self, preds, labels):
-#
-#         """
-#         Process model's outputs and get the final results rather than simple ids.
-#
-#         Args:
-#             preds (Tensor): Prediction labels, the output of the model.
-#             labels (Tensor): True labels
-#
-#         Returns:
-#             `(LongTensor, LongTensor)`: decoded_preds, decoded_labels
-#
-#         """
-#
-#         decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
-#
-#         labels = np.array(labels.to("cpu"))
-#         # Replace -100 in the labels as we can't decode them.
-#         labels = np.where(labels != -100, labels, self.tokenizer.pad_token_id)
-#
-#         decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=False)
-#
-#         decoded_preds = [pred.strip() for pred in decoded_preds]
-#         decoded_labels = [label.strip() for label in decoded_labels]
-#
-#         # rougeLSum expects newline after each sentence
-#         decoded_preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in decoded_preds]
-#         decoded_labels = ["\n".join(nltk.sent_tokenize(label)) for label in decoded_labels]
-#
-#         return decoded_preds, decoded_labels
-#
-#     def get_dataloader(self, dataset, inputs_column="text", labels_column="summary"):
-#
-#         """
-#         Generate DataLoader for a dataset.
-#
-#         Args:
-#             dataset (`Dataset`): The raw dataset.
-#             inputs_column (`str`): Column name of the inputs.
-#             labels_column (`str`): Column name of the labels.
-#
-#         Returns:
-#             `DataLoader`: A dataloader for the dataset. Will be used for inference.
-#         """
-#
-#         tokenized_example = dataset.map(
-#             lambda x: self.tokenize_and_align_labels(x, inputs_column=inputs_column, labels_column=labels_column),
-#             batched=True,
-#             remove_columns=dataset.column_names
-#         )
-#         dataloader = DataLoader(
-#             dataset=tokenized_example,
-#             batch_size=8,
-#             collate_fn=self.collator(),
-#         )
-#
-#         return dataloader
 
 class DataUtilsForT5():
     """
 
     Args:
         tokenizer (`PretrainedTokenizer`, default to None):
             The tokenizer for tokenization.
@@ -879,25 +551,26 @@
         self.checkpoint = checkpoint
         self.model_max_length = model_max_length
         self.max_source_length = max_source_length
         self.max_target_length = max_target_length
         self.model_class = model_class
         self.prompt = prompt
 
+
+
         if tokenizer is None:
             self.tokenizer = AutoTokenizer.from_pretrained(
                 self.checkpoint,
                 model_max_length = self.model_max_length,
                 cache_dir=BASE_CACHE_DIR,
                 use_fast=True
             )
         else:
             self.tokenizer = tokenizer
 
-
     def tokenize_and_align_labels(self, examples, inputs_column="text", labels_column="summary"):
 
         """
 
         Process the dataset for model input, for example, do tokenization and prepare label_ids.
 
         Args:
@@ -909,42 +582,197 @@
             `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
 
         """
 
         inputs = examples[inputs_column]
         prompts = [ self.prompt for i in inputs ]
 
-        import random
-        from random import randint
         # kw_instructions = ["{}"]
         def kw(prompt, keyword):
             # i = randint(1,10)
-            return "Keywords: " + str(", ".join(keyword)) + ". " + prompt + "talking about these keywords " if keyword is not None else prompt
-
+            if keyword is not None:
+                return "Keywords: " + str(", ".join(keyword)) + ". " + prompt + "based on these keywords " if keyword is not None else prompt
+            return prompt
             # return prompt + "that focuses on " + str(", ".join(keyword)) + " " if keyword is not None else prompt
         def leng(prompt, length):
-            return prompt + ", which has less than " + str(length) + " words " if length is not None else prompt
-
+            if length is not None:
+                return prompt + ", which has less than " + str(length) + " words " if length is not None else prompt
+            return prompt
+
+        # def k_str(k_list):
+        #     if k_list is not None:
+        #         return ", ".join(k_list)
+        #     return None
+        # def sents_num(l):
+        #     if l is not None:
+        #         return 5*math.ceil(l/50)
+        #     return 10
         if "keywords" in examples.keys():
             keywords = examples["keywords"]
             if keywords is not None:
                 prompts = [ kw(prompt,keyword) for (prompt,keyword) in zip(prompts,keywords) ]
+                # keywords = [k_str(k) for k in keywords]
+                # if "length" in examples.keys() and examples["length"] is not None:
+                #     inputs = [extract_related_sentences(t,k,sents_num(l)) for (t,k,l) in zip(inputs,keywords,examples["length"])]
+                # else:
+                #     inputs = [extract_related_sentences(t, k, 10) for (t, k) in zip(inputs, keywords)]
         if "length" in examples.keys():
             if examples["length"] is not None:
                 lengths = examples["length"]
                 prompts = [ leng(prompt,length) for (prompt,length) in zip(prompts,lengths)]
+
         # kwords = ["" for i in inputs]
         # if "keywords" in examples.keys():
         #     keywords = examples["keywords"]
         #     if keywords is not None:
         #         keywords = [ keyword if keyword is not None else [] for keyword in keywords ]
         #         # print(keywords)
         #         kwords = [ " ".join(keyword) for keyword in keywords ]
         inputs = [ prompt + ": " + raw_text for (prompt,raw_text) in zip(prompts, inputs) ]
-        # print(inputs[0][:200])
+        print(inputs[0:3][:200])
+
+
+        # Setup the tokenizer for inputs
+
+        model_inputs = self.tokenizer(inputs, max_length=self.max_source_length, padding="max_length", truncation=True)
+
+        # Select target column
+        if labels_column in examples.keys():
+            labels = examples[labels_column]
+            # Setup the tokenizer for targets
+            with self.tokenizer.as_target_tokenizer():
+                labels = self.tokenizer(labels, max_length=self.max_target_length, padding="max_length", truncation=True)
+                # Ignore padding in the loss
+                labels["input_ids"] = [
+                    [(l if l != self.tokenizer.pad_token_id else -100) for l in label] for label in labels["input_ids"]
+                ]
+            model_inputs["labels"] = labels["input_ids"]
+
+        #when test
+        # if "id" in examples.keys():
+        #     model_inputs["id"] = examples["id"]
+        # if "length" in examples.keys() and examples["length"] is not None:
+        #     if examples["length"][0] is not None:
+        #         model_inputs["length"] = examples["length"]
+        return model_inputs
+
+    def tokenize_and_align_labels2(self, examples, inputs_column="text", labels_column="summary"):
+
+        """
+
+        Process the dataset for model input, for example, do tokenization and prepare label_ids.
+
+        Args:
+            examples (`Dataset`): { "text": [s1, s2, ...], "summary": [l1, l2, ...]}
+            inputs (`str`): The name of input column
+            labels (`str`): The name of target column
+
+        Returns:
+            `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
+
+        """
+
+        inputs = examples[inputs_column]
+        def trunc(text):
+            text = text.strip().split()
+            return " ".join(text[:800])
+        inputs = [trunc(text) for text in inputs]
+
+
+        # kw_instructions = ["{}"]
+        def kw(i,text, keyword):
+
+            if keyword is None:
+                lists = [
+                    f"Write a summary for this text: {text}\n\nSummary:",
+                    f"Summarize this scientific article: {text}\n\nSummary:",
+                    f"Generate a summary this text:\n{text}\n\nSummary:",
+                    f"What is a shorter version of this:\n\n{text}\n\nSummary:",
+                    f"{text}\n\nWhat is a summary of the above text?",
+                    f"{text}\nSummarize the aforementioned text.",
+                    f"{text}\nCan you generate a summary of the above scientific text?",
+                    f"Here is a scientific article: {text}\nA summary of this is?",
+                    f"Scientific article:\n\n{text}\nWhat is a shorter version of the above article?",
+                    f"{text}\n\nWrite a summary.",
+                    f"Article:\n{text}Summary:",
+                ]
+            else:
+                keywords = ", ".join(keyword)
+                lists = [
+                    f"Keywords:{keywords}\n\nWrite a summary that includes all these keywords for this text: {text}\n\nSummary:",
+                    f"Keywords:{keywords}\n\nSummarize this scientific article based on these keywords: {text}\n\nSummary:",
+                    f"Here are some concepts: {keywords}\n\nGenerate a summary about these concepts for this text:\n{text}\n\nSummary:",
+                    f"What is a shorter version of this which mentions all :\n\n{text}\n\nSummary:",
+                    f"{text}\n\nWhat is a summary of the above text which mentions all of these concepts: {keywords}",
+                    f"{text}\nSummarize the aforementioned text about the following things: \n\n{keywords}.",
+                    f"{text}\nCan you generate a summary of the above scientific text that includes all the following words: {keywords}",
+                    f"Here is a scientific article: {text}\nA summary of this is?",
+                    f"Scientific article:\n\n{text}\nWhat is a shorter version of the above article?",
+                    f"{text}\n\nWrite a summary talking about these keywords: {keywords}",
+                    f"Keywords:{keywords}\n\nArticle:\n{text}Summary:",
+                ]
+            tot = len(lists) - 1
+            i = i%tot
+
+            return lists[i]
+            # return prompt + "that focuses on " + str(", ".join(keyword)) + " " if keyword is not None else prompt
+        def leng(i,text, length):
+
+            if length is None:
+                lists = [
+                    f"Write a summary for this text: {text}\n\nSummary:",
+                    f"Summarize this scientific article: {text}\n\nSummary:",
+                    f"Generate a summary this text:\n{text}\n\nSummary:",
+                    f"What is a shorter version of this:\n\n{text}\n\nSummary:",
+                    f"{text}\n\nWhat is a summary of the above text?",
+                    f"{text}\nSummarize the aforementioned text.",
+                    f"{text}\nCan you generate a summary of the above scientific text?",
+                    f"Here is a scientific article: {text}\nA summary of this is?",
+                    f"Scientific article:\n\n{text}\nWhat is a shorter version of the above article?",
+                    f"{text}\n\nWrite a summary.",
+                    f"Article:\n{text}Summary:",
+                ]
+            else:
+                lists = [
+                    f"Write a summary that has less than {length} words for this text: {text}\n\nSummary:",
+                    f"Summarize this scientific article within {length} words: {text}\n\nSummary:",
+                    f"Generate a summary of {length} words for this text:\n{text}\n\nSummary:",
+                    f"{text}\n\nWhat is a summary of the above text which has about {length} words?",
+                    f"{text}\nSummarize the aforementioned text within {length} words.",
+                    f"{text}\nCan you generate a summary of the above scientific text that includes {length} words?",
+                    f"Here is a scientific article: {text}\nA summary of {length} words of this is?",
+                    f"Scientific article:\n\n{text}\nWhat is a {length} words version of the above article?",
+                    f"{text}\n\nWrite a summary within {length} words.",
+                    f"Length:{length} words\n\nArticle:\n{text}Summary:",
+                ]
+            tot = len(lists) - 1
+            i = i%tot
+
+            return lists[i]
+
+
+        keywords = examples["keywords"]
+        lengths = examples["length"]
+        def convert(i,keyw, length, text):
+
+            if keyw is None and length is None:
+                 return f"Summarize this scientific article: {text}\n\nSummary:"
+
+            elif keyw is not None and length is not None:
+                return f"Keywords:{keyw}\n\nSummarize this scientific article within {length} words based on these keywords : {text}\n\nSummary:"
+
+            elif keyw is not None:
+                return kw(i,text,keyw)
+
+            elif length is not None:
+                return leng(i,text,length)
+
+        inputs = [convert(i,e[0],e[1],e[2]) for i,e in enumerate(zip(keywords,lengths,inputs))]
+
+        print(inputs[0][:150])
 
 
         # Setup the tokenizer for inputs
 
         model_inputs = self.tokenizer(inputs, max_length=self.max_source_length, padding="max_length", truncation=True)
 
         # Select target column
@@ -956,19 +784,19 @@
                 # Ignore padding in the loss
                 labels["input_ids"] = [
                     [(l if l != self.tokenizer.pad_token_id else -100) for l in label] for label in labels["input_ids"]
                 ]
             model_inputs["labels"] = labels["input_ids"]
 
         #when test
-        if "id" in examples.keys():
-            model_inputs["id"] = examples["id"]
-        if "length" in examples.keys() and examples["length"] is not None:
-            if examples["length"][0] is not None:
-                model_inputs["length"] = examples["length"]
+        # if "id" in examples.keys():
+        #     model_inputs["id"] = examples["id"]
+        # if "length" in examples.keys() and examples["length"] is not None:
+        #     if examples["length"][0] is not None:
+        #         model_inputs["length"] = examples["length"]
         return model_inputs
 
     def collator(self):
 
         """
 
         The collating function.
@@ -1582,16 +1410,14 @@
             `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
 
         """
 
         inputs = examples[inputs_column]
         prompts = [ self.prompt for i in inputs ]
 
-        import random
-        from random import randint
         # kw_instructions = ["{}"]
         def kw(prompt, keyword):
             # i = randint(1,10)
             return "Keywords: " + str(", ".join(keyword)) + ". " + prompt + "talking about these keywords " if keyword is not None else prompt
 
             # return prompt + "that focuses on " + str(", ".join(keyword)) + " " if keyword is not None else prompt
         def leng(prompt, length):
```

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/evaluate_sr.py` & `SciAssist-0.0.29/src/SciAssist/utils/evaluate_sr.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/extract_keywords.py` & `SciAssist-0.0.29/src/SciAssist/utils/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/extract_keywords_flant5.py` & `SciAssist-0.0.29/src/SciAssist/utils/acl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,84 @@
-import yake
+import random
+
 import datasets
 import pandas as pd
 import os
 from tqdm import tqdm
 from transformers import AutoModelForSeq2SeqLM, AutoTokenizer
-
+device = "cuda:1"
 model = AutoModelForSeq2SeqLM.from_pretrained("google/flan-t5-xl")
 tokenizer = AutoTokenizer.from_pretrained("google/flan-t5-xl", max_length=1024, truncation=True)
-
+model.to(device)
 
 
 file_list = []
 
-# root_dir = "/home/dingyx/project/SciAssist/data/"
-# root_dir = "/home/dingyx/project/SciAssist/data/Task2/From-ScisummNet-2019/"
-
+summ = []
+root_dir = "/home/yixi/project/sciassist/data/pdfs/text"
+# root_dir = "/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019/"
 # for dirpath,dirnames,files in os.walk(root_dir):
-#     file_list = dirnames
+#     file_l = files
 #     break
+# file_l.sort()
+# file_list=[]
+# for i in file_l:
+#     if i[-4:]==".txt":
+#         file_list.append(i)
 
-root_dir = "/home/dingyx/project/SciAssist/data/"
 for dirpath,dirnames,files in os.walk(root_dir):
-    file_l = files
+    file_list = files
     break
-file_l.sort()
-file_list=[]
-for i in file_l:
-    if i[-4:]==".txt":
-        file_list.append(i)
+file_list.sort()
 
 def keyword_extraction(input_text):
-    # with open(os.path.join(root_dir,input_text),"r") as f:
-    # # with open(os.path.join(root_dir, input_text, "summary",input_text + ".scisummnet_human.txt"), "r") as f:
-    #     input_text = f.readlines()
-    #     input_text= " ".join(input_text)
-    inputs = tokenizer("What entities does this scientific document talk about?" + input_text + "Entities: ", return_tensors="pt", max_length=1024, truncation=True)
+    with open(os.path.join(root_dir,input_text),"r") as f:
+    # with open(os.path.join(root_dir, input_text, "summary",input_text + ".scisummnet_human.txt"), "r") as f:
+        input_text = f.readlines()
+        input_text= " ".join(input_text)
+    input_text = input_text.replace("\t"," ")
+    input_text = input_text.replace("\n","  ")
+
+    inputs = tokenizer("What key entities does this scientific document include?" + input_text + "Entities: ", return_tensors="pt", max_length=1024, truncation=True)
+    inputs.to(device)
     outputs = model.generate(**inputs)
-    keywords_res = tokenizer.batch_decode(outputs, skip_special_tokens=True)
-    keywords_res = [ k.strip().split() for k in keywords_res ]
-    keywords_res = [ " ".join(k) for k in keywords_res]
+    keywords_res = tokenizer.batch_decode(outputs, skip_special_tokens=True)[0]
+    print(keywords_res)
+    keywords_res = keywords_res.strip().split(",")
+    keywords_res = [k.strip() for k in keywords_res]
+    keywords_res = [k for k in keywords_res if k!=""]
     keywords_res = list(set(keywords_res))
+
+
     keyword_str = ",".join(keywords_res)
     # print(keyword_str)
+
     return keyword_str
 
 
 # In[197]:
 
 
 # ### Different setting of keyword extraction
 
 # In[841]:
 
-raw_datasets = datasets.load_dataset(
-    "allenai/mup",
-    cache_dir="/home/dingyx/.cache/sciassist"
-)
+# raw_datasets = datasets.load_dataset(
+#     "allenai/mup",
+#     cache_dir="/home/yixi/.cache/sciassist"
+# )
 
 print("loading finished.")
-file_list = raw_datasets["train"]
+# file_list = raw_datasets["train"]
 # file_list = raw_datasets["validation"].select(range(1000))
 
-summ = file_list["summary"]
-# scisumm = {"File": file_list}
+# summ = file_list["summary"]
+scisumm = {"File": file_list}
+print(file_list)
 # print(scisumm["File"])
-scisumm = {"title": file_list["paper_name"], "summary":summ, "text":file_list["text"] }
+# scisumm = {"title": file_list["paper_name"], "summary":summ, "text":file_list["text"] }
 scisumm = pd.DataFrame(scisumm)
 tqdm.pandas(desc='progress bar')
-scisumm['keyword']=scisumm["summary"].progress_apply(keyword_extraction,args=())
+scisumm['keyword']=scisumm["File"].progress_apply(keyword_extraction,args=())
 # scisumm['keyword']=scisumm["File"].progress_apply(keyword_extraction,args=())
-scisumm.to_csv(os.path.join(root_dir,"train.csv"), index=True)
+# scisumm["summary"]=summ
+scisumm.to_csv(os.path.join(root_dir,"test.csv"), index=True)
```

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/extract_keywords_yake.py` & `SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_yake.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 
 import pandas as pd
 import os
 from tqdm import tqdm
 
 file_list = []
 
-root_dir = "/home/dingyx/project/SciAssist/data/Task2/From-ScisummNet-2019/"
+root_dir = "/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019/"
 for dirpath,dirnames,files in os.walk(root_dir):
     file_list = dirnames
     break
 
 
 def keyword_extraction(input_text, kw_extractor):
-    with open(os.path.join(root_dir,input_text,input_text+".txt"),"r") as f:
-    # with open(os.path.join(root_dir, input_text, "summary",input_text + ".scisummnet_human.txt"), "r") as f:
+    # with open(os.path.join(root_dir,input_text,input_text+".txt"),"r") as f:
+    with open(os.path.join(root_dir, input_text, "summary",input_text + ".scisummnet_human.txt"), "r") as f:
         input_text = f.readlines()
-        input_text= " ".join(input_text)
+        input_text= " ".join(input_text[1:])
     keywords_res = kw_extractor.extract_keywords(input_text)
-    keyword_str = "#".join([kw[0] for kw in keywords_res])
+    keyword_str = ",".join([kw[0] for kw in keywords_res])
     return keyword_str
 
 
 # In[197]:
 
 
 # ### Different setting of keyword extraction
 
 # In[841]:
 
 
 language = "en"  # 文档语言
-max_ngram_size = 2  # N-grams
-deduplication_thresold = 0.5  # 筛选阈值,越小关键词越少
+max_ngram_size = 3  # N-grams
+deduplication_thresold = 0.3  # 筛选阈值,越小关键词越少
 deduplication_algo = 'seqm'
 windowSize = 3
-numOfKeywords = 10  # 最大数量
+numOfKeywords = 5  # 最大数量
 
 kw_extractor = yake.KeywordExtractor(lan=language,
                                      n=max_ngram_size,
                                      dedupLim=deduplication_thresold,
                                      dedupFunc=deduplication_algo,
                                      windowsSize=windowSize,
                                      top=numOfKeywords)
```

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/pdf2text.py` & `SciAssist-0.0.29/src/SciAssist/utils/pdf2text.py`

 * *Files 17% similar despite different names*

```diff
@@ -53,29 +53,64 @@
     os.makedirs(output_dir, exist_ok=True)
     assert json_file[-4:] == "json"
     if suffix is None:
         suffix = "_" + "_".join(section)
     output_path = os.path.join(output_dir, os.path.basename(json_file)[:-5] + suffix + ".txt")
     strings_file = open(output_path,"w")
 
-    section = section.lower()
+    section = [s.lower() for s in section]
     with open(json_file,'r') as f:
         data = json.load(f)
         for context in data["pdf_parse"]["body_text"]:
             sent = context["text"]
-            if sent != "" and context["section"].lower() in section:
-                sent = nltk.word_tokenize(sent)
-                strings_file.write(" ".join(sent))
-                strings_file.write(" ")
-            else:
-                break
+            for j in section:
+                if sent != "" and j in context["section"].lower():
+                    sent = nltk.word_tokenize(sent)
+                    strings_file.write(" ".join(sent))
+                    strings_file.write(" ")
+                else:
+                    continue
 
     strings_file.close()
     return output_path
 
+def get_IC(json_file: str, output_dir: str = BASE_OUTPUT_DIR, suffix=None):
+    os.makedirs(output_dir, exist_ok=True)
+    section=["Introduction","Conclusion"]
+    assert json_file[-4:] == "json"
+    if suffix is None:
+        suffix = "_" + "_".join(section)
+    output_path = os.path.join(output_dir, os.path.basename(json_file)[:-5] + suffix + ".txt")
+    strings_file = open(output_path,"w")
+    res=[]
+    section = [s.lower() for s in section]
+    flag=0
+    with open(json_file,'r') as f:
+        data = json.load(f)
+        for context in data["pdf_parse"]["body_text"]:
+            sent = context["text"]
+            for j in section:
+                if sent != "" and j in context["section"].lower():
+                    if j=="introduction":
+                        flag=1
+                    sent = nltk.word_tokenize(sent)
+                    res.extend(sent)
+                else:
+                    continue
+        if flag==0:
+            res=[]
+            for context in data["pdf_parse"]["body_text"]:
+                sent = context["text"]
+                if sent != "":
+                    sent = nltk.word_tokenize(sent)
+                    res.extend(sent)
+    strings_file.write(" ".join(res[:800]))
+    strings_file.write(" ")
+    strings_file.close()
+    return output_path
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Extracting strings from JSON")
     parser.add_argument("--input_file", required=True, help="path to the input json file")
     parser.add_argument("--temp_dir", default=BASE_TEMP_DIR, help="path to the temp dir for putting json files")
     parser.add_argument("--output_dir", default=BASE_OUTPUT_DIR, help="path to the output dir for putting text files")
```

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/testset.py` & `SciAssist-0.0.29/src/SciAssist/utils/testset.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/windows_pdf2text.py` & `SciAssist-0.0.29/src/SciAssist/utils/windows_pdf2text.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,24 @@
     raw_text = []
     res = {
         "title":"",
         "author":[],
         "body_text":[],
         "reference":[]
     }
+    print(path)
+    fp = open(path, 'rb')
     for page_layout in extract_pages(path):
         for element in page_layout:
             if "get_text" in dir(element):
                 text = element.get_text().replace("\n","")
                 text = text.strip()
                 if text.isdigit() == False and text != "":
                     raw_text.append(text)
-
+    fp.close()
     res["title"] = raw_text[0]
 
     i = 1 # the index of the current text in raw_text
 
     while i<len(raw_text):
         if raw_text[i] in ["abstract","Abstract", "ABSTRACT"]:
             i += 1
```

### Comparing `SciAssist-0.0.28/src/SciAssist/utils/xml2txt.py` & `SciAssist-0.0.29/src/SciAssist/utils/xml2txt.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import xml.etree.ElementTree as ET
 import os
 file_list = []
 
-root_dir = "/home/dingyx/project/SciAssist/data/Task2/From-ScisummNet-2019/"
+root_dir = "/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019"
 for dirpath,dirnames,files in os.walk(root_dir):
     file_list = dirnames
     break
-
+filter_files=[]
 
 def parse_rec(filename):
     file = os.path.join(root_dir,filename,"Reference_XML",filename+".xml")
     tree = ET.parse(file)  # 解析读取xml函数
 
 
     # Element.findall()查找当前元素的直接子元素中带有指定标签的元素
     # Element.find()找带有特定标签的第一个子级
     # Elemtn.text 访问元素的文本内容
     # Element.get 访问元素的属性。
     body_text = ""
+
     if len(tree.findall('SECTION'))>0:
         for section in tree.findall('SECTION'):
-            if "Introduction" in section.get("title") or "Conclusion" in section.get("title"):
+            if "Introduction" in section.get("title") or "Conclusion" in section.get("title") or "1" in section.get("title"):
                 for s in section.findall("S"):
                     body_text += s.text
                     body_text += " "
     else:
-        for s in tree.findall("S"):
-            if s.text is not None:
-                body_text += s.text
-                body_text += " "
+        filter_files.append(filename)
+    # else:
+        # for s in tree.findall("S"):
+        #     if s.text is not None:
+        #         body_text += s.text
+        #         body_text += " "
+        # print(filename)
 
     with open(os.path.join(root_dir,filename,filename+".txt"),"w") as f:
         f.write(body_text)
 
     return body_text
 
 for file in file_list:
     s = parse_rec(file)
 
 print("Finished.")
-
-
+print(filter_files)
```

### Comparing `SciAssist-0.0.28/src/SciAssist.egg-info/PKG-INFO` & `SciAssist-0.0.29/src/SciAssist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.28
+Version: 0.0.29
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.28/src/SciAssist.egg-info/SOURCES.txt` & `SciAssist-0.0.29/src/SciAssist.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -56,50 +56,59 @@
 src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
 src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
 src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
 src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
 src/SciAssist/datamodules/__init__.py
 src/SciAssist/datamodules/acl_datamodule.py
 src/SciAssist/datamodules/cora_datamodule.py
+src/SciAssist/datamodules/dataset_extraction_datamodule.py
 src/SciAssist/datamodules/fid_datamodule.py
 src/SciAssist/datamodules/general_datamodule.py
 src/SciAssist/datamodules/longsumm_datamodule.py
 src/SciAssist/datamodules/mup_datamodule.py
+src/SciAssist/datamodules/mup_mup_datamodule.py
 src/SciAssist/datamodules/mup_scisumm_datamodule.py
 src/SciAssist/datamodules/scisumm_datamodule.py
 src/SciAssist/datamodules/test_datamodule.py
 src/SciAssist/datamodules/xsum_datamodule.py
 src/SciAssist/datamodules/components/__init__.py
 src/SciAssist/datamodules/components/cora_label.py
 src/SciAssist/models/__init__.py
 src/SciAssist/models/cora_module.py
+src/SciAssist/models/dataset_extraction_module.py
 src/SciAssist/models/mup_bart_module.py
 src/SciAssist/models/mup_fid_module.py
 src/SciAssist/models/mup_frost_module.py
 src/SciAssist/models/components/__init__.py
 src/SciAssist/models/components/bart_summarization.py
+src/SciAssist/models/components/bert_dataset_extraction.py
 src/SciAssist/models/components/bert_token_classifier.py
 src/SciAssist/models/components/fid_summarization.py
 src/SciAssist/models/components/flant5_summarization.py
 src/SciAssist/models/components/frost_summarization.py
 src/SciAssist/models/components/longt5_summarization.py
 src/SciAssist/pipelines/__init__.py
+src/SciAssist/pipelines/dataset_extraction.py
 src/SciAssist/pipelines/pipeline.py
 src/SciAssist/pipelines/reference_string_parsing.py
 src/SciAssist/pipelines/summarization.py
 src/SciAssist/pipelines/summarization_origin.py
 src/SciAssist/pipelines/testing_pipeline.py
 src/SciAssist/pipelines/training_pipeline.py
 src/SciAssist/utils/__init__.py
+src/SciAssist/utils/acl.py
 src/SciAssist/utils/data_reader.py
 src/SciAssist/utils/data_utils.py
+src/SciAssist/utils/data_utils2.py
 src/SciAssist/utils/evaluate_sr.py
 src/SciAssist/utils/extract_acl.py
+src/SciAssist/utils/extract_keysents.py
 src/SciAssist/utils/extract_keywords.py
 src/SciAssist/utils/extract_keywords_flant5.py
+src/SciAssist/utils/extract_keywords_tfidf.py
 src/SciAssist/utils/extract_keywords_yake.py
 src/SciAssist/utils/pdf2text.py
 src/SciAssist/utils/testset.py
 src/SciAssist/utils/windows_pdf2text.py
 src/SciAssist/utils/xml2txt.py
 src/SciAssist/utils/collators/CollatorForFid.py
 src/SciAssist/utils/collators/__init__.py
```

### Comparing `SciAssist-0.0.28/src/chatsonic.py` & `SciAssist-0.0.29/src/chatsonic.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/convert_pegasus.py` & `SciAssist-0.0.29/src/convert_pegasus.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/src/process.py` & `SciAssist-0.0.29/src/process.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/tests/test_rsp.py` & `SciAssist-0.0.29/tests/test_rsp.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.28/tests/test_summ.py` & `SciAssist-0.0.29/tests/test_summ.py`

 * *Files identical despite different names*

