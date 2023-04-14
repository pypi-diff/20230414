# Comparing `tmp/fameio-1.7.tar.gz` & `tmp/fameio-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fameio-1.7.tar", last modified: Mon Feb 20 14:00:30 2023, max compression
+gzip compressed data, was "fameio-1.8.tar", last modified: Fri Apr 14 14:12:01 2023, max compression
```

## Comparing `fameio-1.7.tar` & `fameio-1.8.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.883108 fameio-1.7/
--rw-rw-rw-   0        0        0    10389 2022-05-24 09:01:58.000000 fameio-1.7/LICENSE
--rw-rw-rw-   0        0        0    25405 2023-02-20 14:00:30.883108 fameio-1.7/PKG-INFO
--rw-rw-rw-   0        0        0    24738 2023-02-17 08:14:51.000000 fameio-1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-02-20 14:00:30.883108 fameio-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1766 2023-02-20 14:00:13.000000 fameio-1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.819706 fameio-1.7/src/
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.819706 fameio-1.7/src/fameio/
--rw-rw-rw-   0        0        0        0 2022-05-24 09:01:58.000000 fameio-1.7/src/fameio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.851781 fameio-1.7/src/fameio/scripts/
--rw-rw-rw-   0        0        0      708 2022-05-24 09:01:58.000000 fameio-1.7/src/fameio/scripts/__init__.py
--rw-rw-rw-   0        0        0     2949 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/scripts/convert_results.py
--rw-rw-rw-   0        0        0     1313 2023-02-20 12:43:52.000000 fameio-1.7/src/fameio/scripts/make_config.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.851781 fameio-1.7/src/fameio/source/
--rw-rw-rw-   0        0        0      164 2022-06-07 13:57:06.000000 fameio-1.7/src/fameio/source/__init__.py
--rw-rw-rw-   0        0        0     5448 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/cli.py
--rw-rw-rw-   0        0        0     7289 2023-02-20 12:43:52.000000 fameio-1.7/src/fameio/source/loader.py
--rw-rw-rw-   0        0        0     1815 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/logs.py
--rw-rw-rw-   0        0        0     1207 2022-06-07 09:46:52.000000 fameio-1.7/src/fameio/source/path_resolver.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.867439 fameio-1.7/src/fameio/source/results/
--rw-rw-rw-   0        0        0        0 2022-07-04 13:10:56.000000 fameio-1.7/src/fameio/source/results/__init__.py
--rw-rw-rw-   0        0        0     4207 2022-08-26 08:04:34.000000 fameio-1.7/src/fameio/source/results/agent_type.py
--rw-rw-rw-   0        0        0     4102 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/results/csv_writer.py
--rw-rw-rw-   0        0        0     6100 2022-08-26 08:04:34.000000 fameio-1.7/src/fameio/source/results/data_transformer.py
--rw-rw-rw-   0        0        0     3826 2022-08-26 08:04:34.000000 fameio-1.7/src/fameio/source/results/output_dao.py
--rw-rw-rw-   0        0        0     4677 2022-07-04 13:10:56.000000 fameio-1.7/src/fameio/source/results/reader.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.883108 fameio-1.7/src/fameio/source/scenario/
--rw-rw-rw-   0        0        0      258 2022-05-24 09:01:58.000000 fameio-1.7/src/fameio/source/scenario/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/scenario/agent.py
--rw-rw-rw-   0        0        0     4888 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/scenario/attribute.py
--rw-rw-rw-   0        0        0     8739 2023-02-20 08:27:27.000000 fameio-1.7/src/fameio/source/scenario/contract.py
--rw-rw-rw-   0        0        0     1341 2022-06-07 09:46:52.000000 fameio-1.7/src/fameio/source/scenario/exception.py
--rw-rw-rw-   0        0        0     1262 2022-05-24 09:01:58.000000 fameio-1.7/src/fameio/source/scenario/fameiofactory.py
--rw-rw-rw-   0        0        0     4479 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/scenario/generalproperties.py
--rw-rw-rw-   0        0        0     3468 2022-06-07 09:46:52.000000 fameio-1.7/src/fameio/source/scenario/scenario.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.883108 fameio-1.7/src/fameio/source/schema/
--rw-rw-rw-   0        0        0      156 2022-05-24 09:01:58.000000 fameio-1.7/src/fameio/source/schema/__init__.py
--rw-rw-rw-   0        0        0     3217 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/schema/agenttype.py
--rw-rw-rw-   0        0        0     8100 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/schema/attribute.py
--rw-rw-rw-   0        0        0      108 2022-05-24 09:01:58.000000 fameio-1.7/src/fameio/source/schema/exception.py
--rw-rw-rw-   0        0        0     1601 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/schema/schema.py
--rw-rw-rw-   0        0        0     1810 2022-06-07 09:46:52.000000 fameio-1.7/src/fameio/source/series.py
--rw-rw-rw-   0        0        0     6472 2022-06-07 09:46:52.000000 fameio-1.7/src/fameio/source/time.py
--rw-rw-rw-   0        0        0      516 2022-05-24 09:01:58.000000 fameio-1.7/src/fameio/source/tools.py
--rw-rw-rw-   0        0        0    11295 2022-06-07 09:46:52.000000 fameio-1.7/src/fameio/source/validator.py
--rw-rw-rw-   0        0        0    11519 2023-02-17 08:14:51.000000 fameio-1.7/src/fameio/source/writer.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:00:30.851781 fameio-1.7/src/fameio.egg-info/
--rw-rw-rw-   0        0        0    25405 2023-02-20 14:00:30.000000 fameio-1.7/src/fameio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2023-02-20 14:00:30.000000 fameio-1.7/src/fameio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 14:00:30.000000 fameio-1.7/src/fameio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-02-20 14:00:30.000000 fameio-1.7/src/fameio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-20 12:46:29.000000 fameio-1.7/src/fameio.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       76 2023-02-20 14:00:30.000000 fameio-1.7/src/fameio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-20 14:00:30.000000 fameio-1.7/src/fameio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.419520 fameio-1.8/
+-rw-rw-rw-   0        0        0    10391 2023-04-14 05:55:34.000000 fameio-1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    28055 2023-04-14 14:12:01.419520 fameio-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    27385 2023-04-14 14:10:34.000000 fameio-1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:12:01.420533 fameio-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2023-04-14 05:55:34.000000 fameio-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.293521 fameio-1.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.299522 fameio-1.8/src/fameio/
+-rw-rw-rw-   0        0        0      109 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.310521 fameio-1.8/src/fameio/scripts/
+-rw-rw-rw-   0        0        0      746 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3296 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/scripts/convert_results.py
+-rw-rw-rw-   0        0        0     1339 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/scripts/make_config.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.343526 fameio-1.8/src/fameio/source/
+-rw-rw-rw-   0        0        0      278 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/__init__.py
+-rw-rw-rw-   0        0        0     9376 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/source/cli.py
+-rw-rw-rw-   0        0        0     7403 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/loader.py
+-rw-rw-rw-   0        0        0     1929 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/logs.py
+-rw-rw-rw-   0        0        0     1321 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/path_resolver.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.367521 fameio-1.8/src/fameio/source/results/
+-rw-rw-rw-   0        0        0      109 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/__init__.py
+-rw-rw-rw-   0        0        0     4321 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/agent_type.py
+-rw-rw-rw-   0        0        0     3793 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/source/results/conversion.py
+-rw-rw-rw-   0        0        0     4216 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/csv_writer.py
+-rw-rw-rw-   0        0        0     6222 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/data_transformer.py
+-rw-rw-rw-   0        0        0     3960 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/output_dao.py
+-rw-rw-rw-   0        0        0     4791 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/reader.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.398531 fameio-1.8/src/fameio/source/scenario/
+-rw-rw-rw-   0        0        0      372 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/__init__.py
+-rw-rw-rw-   0        0        0     3830 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/agent.py
+-rw-rw-rw-   0        0        0     5002 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/attribute.py
+-rw-rw-rw-   0        0        0     8853 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/contract.py
+-rw-rw-rw-   0        0        0     1455 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/exception.py
+-rw-rw-rw-   0        0        0     1376 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/fameiofactory.py
+-rw-rw-rw-   0        0        0     4593 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/generalproperties.py
+-rw-rw-rw-   0        0        0     3582 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/scenario.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.418530 fameio-1.8/src/fameio/source/schema/
+-rw-rw-rw-   0        0        0      270 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/__init__.py
+-rw-rw-rw-   0        0        0     3331 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/agenttype.py
+-rw-rw-rw-   0        0        0     8214 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/attribute.py
+-rw-rw-rw-   0        0        0      224 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/exception.py
+-rw-rw-rw-   0        0        0     1715 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/schema.py
+-rw-rw-rw-   0        0        0     1924 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/series.py
+-rw-rw-rw-   0        0        0     6943 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/time.py
+-rw-rw-rw-   0        0        0      630 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/tools.py
+-rw-rw-rw-   0        0        0    11409 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/validator.py
+-rw-rw-rw-   0        0        0    11633 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/writer.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.309521 fameio-1.8/src/fameio.egg-info/
+-rw-rw-rw-   0        0        0    28055 2023-04-14 14:12:00.000000 fameio-1.8/src/fameio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1470 2023-04-14 14:12:01.000000 fameio-1.8/src/fameio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:12:00.000000 fameio-1.8/src/fameio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-04-14 14:12:01.000000 fameio-1.8/src/fameio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 14:12:00.000000 fameio-1.8/src/fameio.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-04-14 14:12:01.000000 fameio-1.8/src/fameio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 14:12:01.000000 fameio-1.8/src/fameio.egg-info/top_level.txt
```

### Comparing `fameio-1.7/LICENSE` & `fameio-1.8/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -171,8 +171,8 @@
       License. However, in accepting such obligations, You may act only
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
-   END OF TERMS AND CONDITIONS
+   END OF TERMS AND CONDITIONS
```

### Comparing `fameio-1.7/PKG-INFO` & `fameio-1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: fameio
-Version: 1.7
+Version: 1.8
 Summary: Python scripts for operation of FAME models
 Home-page: https://gitlab.com/fame-framework/fame-io/
 Author: Felix Nitsch, Christoph Schimeczek, Ulrich Frey, Marc Deissenroth-Uhrig, Benjamin Fuchs, A. Achraf El Ghazi
 Author-email: fame@dlr.de
 License: Apache License 2.0
 Keywords: FAME,agent-based modelling
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
+Provides-Extra: dev
+License-File: LICENSE.txt
 
+<!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+
+SPDX-License-Identifier: Apache-2.0 -->
 [![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4501190.svg)](https://doi.org/10.5281/zenodo.4501190)
+[![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
+[![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
 [![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
 [![pipeline status](https://gitlab.com/fame-framework/fame-io/badges/main/pipeline.svg)](https://gitlab.com/fame-framework/fame-io/commits/main)
 [![coverage report](https://gitlab.com/fame-framework/fame-io/badges/main/coverage.svg)](https://gitlab.com/fame-framework/fame-io/-/commits/main)
+[![REUSE status](https://api.reuse.software/badge/gitlab.com/fame-framework/fame-io)](https://api.reuse.software/info/gitlab.com/fame-framework/fame-io)
 
 # FAME-Io
 Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
 Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
 The package is also formerly known as [FAME-Py](https://doi.org/10.5281/zenodo.4314338).
 
 # Installation
@@ -535,20 +540,36 @@
 | `-l` or `--log` <option>             | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
 | `-lf` or `--logfile` <file>          | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
 | `-a` or `--agents` <list-of-agents>  | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
 | `-o` or `--output`                   | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
 | `-se` or `--single-export`           | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
 | `-m` or `--memory-saving`            | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
 | `-cc` or `--complex-column` <option> | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
+| `-t` or `--time` <option>            | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
+
+Additionally, you may merge TimeSteps of a certain range of steps in the output files to
+  i) associate multiple time steps with a common logical time in your simulation
+  ii) reduce number of lines in output files
+
+For this, add the option `merge-times` and specify the arguments as follows:
+
+| Command                   | Action                                                                                   |
+|---------------------------|------------------------------------------------------------------------------------------|
+| `-fp` or `--focal-point`  | TimeStep on which `steps-before` earlier and `steps-after` later TimeSteps are merged on |
+| `-sb` or `--steps-before` | Range of TimeSteps before the `focal-point` they get merged to                           |
+| `-sa` or `--steps-after`  | Range of TimeSteps after the `focal-point` they get merged to                            |
 
 This could look as follows:
 
-    convertFameResults -f <./path/to/protobuf_file.pb> -l debug -lf <path/to/output.log> -a AgentType1 AgentType2 -o myCsvFolder -m -cc SPLIT
+    convertFameResults -f <./path/to/protobuf_file.pb> -l debug -lf <path/to/output.log> -a AgentType1 AgentType2 -o myCsvFolder -m -cc SPLIT merge-times -fp 0 -sb 1799 -sa 1800
 
-You may also call the conversion script from any Python script with
+Make sure that in the range of time steps you specify for merging there is only one value per column in the merged time range.
+If multiple values per column are merged values will get concatenated and might yield unexpected results.
+
+You may also call the conversion script from any Python script with:
 
 ```python
 from fameio.scripts.convert_results import run as convert_results
 
 convert_results("./path/to/protobuf_file.pb")
 ```
 
@@ -561,29 +582,56 @@
 run_config = {Options.LOG_LEVEL: "info",
               Options.LOG_FILE: "scenario.log",
               Options.OUTPUT: "Output",
               Options.AGENT_LIST: ['AgentType1', 'AgentType2'],
               Options.MEMORY_SAVING: False,
               Options.SINGLE_AGENT_EXPORT: False,
               Options.RESOLVE_COMPLEX_FIELD: "SPLIT",
+              Options.TIME: "INT",
+              Options.TIME_MERGING: {},
               }
 
 convert_results("./path/to/protobuf_file.pb", run_config)
 ```
 
-# Contribute
+## Cite FAME-Io
+If you use FAME-Io for academic work, please cite as follows.
+
+Bibtex entry:
+```
+@article{fameio2023joss,
+  author  = {Felix Nitsch and Christoph Schimeczek and Ulrich Frey and Benjamin Fuchs},
+  title   = {FAME-Io: Configuration tools for complex agent-based simulations},
+  journal = {Journal of Open Source Software},
+  year    = {2023},
+  doi     = {doi: https://doi.org/10.21105/joss.04958}
+}
+```
+
+## Contribute
 Please read the Contributors License Agreement `cla.md`, sign it and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing.
 
 ## Testing changes locally
 
 Once some changes have been performed on the local git clone, use the following command to override your local installation with your modified copy in order to test the result:
 
 ```bash
 python3 setup.py bdist_wheel && pip3 install --force-reinstall --no-dependencies ./dist/*.whl
 ```
 
 ## Code style
 
 We use the code formatting library [`black`](https://pypi.org/project/black/).
-The maximum line length is defined as 120 characters. 
+The maximum line length is defined as 120 characters.
 Therefore, before committing, run `black --line-length 120 .`
 
+## Pre-Commit hooks
+
+FAME-Io uses several pre-commit hooks to ensure high code quality.
+To use them, install `dev` packages and then initialise pre-commit in FAME-Io's base folder:
+
+```
+    pip install fameio[dev]
+    pre-commit install -t pre-commit -t pre-push
+```
+
+
```

### Comparing `fameio-1.7/README.md` & `fameio-1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+<!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+
+SPDX-License-Identifier: Apache-2.0 -->
 [![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4501190.svg)](https://doi.org/10.5281/zenodo.4501190)
+[![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
+[![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
 [![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
 [![pipeline status](https://gitlab.com/fame-framework/fame-io/badges/main/pipeline.svg)](https://gitlab.com/fame-framework/fame-io/commits/main)
 [![coverage report](https://gitlab.com/fame-framework/fame-io/badges/main/coverage.svg)](https://gitlab.com/fame-framework/fame-io/-/commits/main)
+[![REUSE status](https://api.reuse.software/badge/gitlab.com/fame-framework/fame-io)](https://api.reuse.software/info/gitlab.com/fame-framework/fame-io)
 
 # FAME-Io
 Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
 Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
 The package is also formerly known as [FAME-Py](https://doi.org/10.5281/zenodo.4314338).
 
 # Installation
@@ -517,20 +522,36 @@
 | `-l` or `--log` <option>             | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
 | `-lf` or `--logfile` <file>          | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
 | `-a` or `--agents` <list-of-agents>  | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
 | `-o` or `--output`                   | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
 | `-se` or `--single-export`           | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
 | `-m` or `--memory-saving`            | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
 | `-cc` or `--complex-column` <option> | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
+| `-t` or `--time` <option>            | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
+
+Additionally, you may merge TimeSteps of a certain range of steps in the output files to
+  i) associate multiple time steps with a common logical time in your simulation
+  ii) reduce number of lines in output files
+
+For this, add the option `merge-times` and specify the arguments as follows:
+
+| Command                   | Action                                                                                   |
+|---------------------------|------------------------------------------------------------------------------------------|
+| `-fp` or `--focal-point`  | TimeStep on which `steps-before` earlier and `steps-after` later TimeSteps are merged on |
+| `-sb` or `--steps-before` | Range of TimeSteps before the `focal-point` they get merged to                           |
+| `-sa` or `--steps-after`  | Range of TimeSteps after the `focal-point` they get merged to                            |
 
 This could look as follows:
 
-    convertFameResults -f <./path/to/protobuf_file.pb> -l debug -lf <path/to/output.log> -a AgentType1 AgentType2 -o myCsvFolder -m -cc SPLIT
+    convertFameResults -f <./path/to/protobuf_file.pb> -l debug -lf <path/to/output.log> -a AgentType1 AgentType2 -o myCsvFolder -m -cc SPLIT merge-times -fp 0 -sb 1799 -sa 1800
+
+Make sure that in the range of time steps you specify for merging there is only one value per column in the merged time range.
+If multiple values per column are merged values will get concatenated and might yield unexpected results.
 
-You may also call the conversion script from any Python script with
+You may also call the conversion script from any Python script with:
 
 ```python
 from fameio.scripts.convert_results import run as convert_results
 
 convert_results("./path/to/protobuf_file.pb")
 ```
 
@@ -543,28 +564,54 @@
 run_config = {Options.LOG_LEVEL: "info",
               Options.LOG_FILE: "scenario.log",
               Options.OUTPUT: "Output",
               Options.AGENT_LIST: ['AgentType1', 'AgentType2'],
               Options.MEMORY_SAVING: False,
               Options.SINGLE_AGENT_EXPORT: False,
               Options.RESOLVE_COMPLEX_FIELD: "SPLIT",
+              Options.TIME: "INT",
+              Options.TIME_MERGING: {},
               }
 
 convert_results("./path/to/protobuf_file.pb", run_config)
 ```
 
-# Contribute
+## Cite FAME-Io
+If you use FAME-Io for academic work, please cite as follows.
+
+Bibtex entry:
+```
+@article{fameio2023joss,
+  author  = {Felix Nitsch and Christoph Schimeczek and Ulrich Frey and Benjamin Fuchs},
+  title   = {FAME-Io: Configuration tools for complex agent-based simulations},
+  journal = {Journal of Open Source Software},
+  year    = {2023},
+  doi     = {doi: https://doi.org/10.21105/joss.04958}
+}
+```
+
+## Contribute
 Please read the Contributors License Agreement `cla.md`, sign it and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing.
 
 ## Testing changes locally
 
 Once some changes have been performed on the local git clone, use the following command to override your local installation with your modified copy in order to test the result:
 
 ```bash
 python3 setup.py bdist_wheel && pip3 install --force-reinstall --no-dependencies ./dist/*.whl
 ```
 
 ## Code style
 
 We use the code formatting library [`black`](https://pypi.org/project/black/).
-The maximum line length is defined as 120 characters. 
-Therefore, before committing, run `black --line-length 120 .`
+The maximum line length is defined as 120 characters.
+Therefore, before committing, run `black --line-length 120 .`
+
+## Pre-Commit hooks
+
+FAME-Io uses several pre-commit hooks to ensure high code quality.
+To use them, install `dev` packages and then initialise pre-commit in FAME-Io's base folder:
+
+```
+    pip install fameio[dev]
+    pre-commit install -t pre-commit -t pre-push
+```
```

### Comparing `fameio-1.7/setup.py` & `fameio-1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="fameio",
-    version="1.7",
+    version="1.8",
     description="Python scripts for operation of FAME models",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["FAME", "agent-based modelling"],
     url="https://gitlab.com/fame-framework/fame-io/",
     author=", ".join(__author__),
     author_email=__email__,
@@ -49,12 +49,12 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "pandas",
         "fameprotobuf>=1.2,<1.3",  # noqa
         "pyyaml",
     ],
-    extras_require={"test": ["pytest", "google.protobuf", "mockito"]},
+    extras_require={"dev": ["pytest", "mockito", "pre-commit"]},
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
 )
```

### Comparing `fameio-1.7/src/fameio/scripts/__init__.py` & `fameio-1.8/src/fameio/scripts/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
-
+import sys
 
 from fameio.scripts.convert_results import DEFAULT_CONFIG as DEFAULT_CONVERT_CONFIG
 from fameio.scripts.convert_results import run as convert_results
 from fameio.scripts.make_config import DEFAULT_CONFIG as DEFAULT_MAKE_CONFIG
 from fameio.scripts.make_config import run as make_config
 from fameio.source.cli import arg_handling_convert_results, arg_handling_make_config
 
 
 def makeFameRunConfig():
-    input_file, run_config = arg_handling_make_config(DEFAULT_MAKE_CONFIG)
+    input_file, run_config = arg_handling_make_config(sys.argv[1:], DEFAULT_MAKE_CONFIG)
     make_config(input_file, run_config)
 
 
 def convertFameResults():
-    input_file, run_config = arg_handling_convert_results(DEFAULT_CONVERT_CONFIG)
+    input_file, run_config = arg_handling_convert_results(sys.argv[1:], DEFAULT_CONVERT_CONFIG)
     convert_results(input_file, run_config)
```

### Comparing `fameio-1.7/src/fameio/scripts/convert_results.py` & `fameio-1.8/src/fameio/scripts/convert_results.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 #!/usr/bin/env python
 
 import logging as log
+import sys
 from pathlib import Path
 from typing import Union
 
 from fameio.source.cli import (
     Options,
     ResolveOptions,
     arg_handling_convert_results,
-    get_config_or_default,
+    update_default_config,
+    TimeOptions,
 )
 from fameio.source.logs import log_and_raise_critical, set_up_logger
 from fameio.source.results.agent_type import AgentTypeLog
+from fameio.source.results.conversion import apply_time_option, apply_time_merging
 from fameio.source.results.csv_writer import CsvWriter
 from fameio.source.results.data_transformer import DataTransformer
 from fameio.source.results.output_dao import OutputDAO
 from fameio.source.results.reader import Reader
 
 DEFAULT_CONFIG = {
     Options.LOG_LEVEL: "info",
     Options.LOG_FILE: None,
     Options.AGENT_LIST: None,
     Options.OUTPUT: None,
     Options.SINGLE_AGENT_EXPORT: False,
     Options.MEMORY_SAVING: False,
     Options.RESOLVE_COMPLEX_FIELD: ResolveOptions.SPLIT.name,
+    Options.TIME: TimeOptions.UTC.name,
+    Options.TIME_MERGING: {},
 }
 
-
 ERR_MEMORY_ERROR = "Out of memory. Try using `-m` or `--memory-saving` option."
 ERR_MEMORY_SEVERE = "Out of memory despite memory-saving mode. Reduce output interval in `FAME-Core` and rerun model"
 
 
 def run(file_path: Union[str, Path], config: dict = None) -> None:
     """Reads file in protobuf format at given `file_path` and extracts its content to .csv file(s)"""
-    config = get_config_or_default(config, DEFAULT_CONFIG)
+    config = update_default_config(config, DEFAULT_CONFIG)
     set_up_logger(level_name=config[Options.LOG_LEVEL], file_name=config[Options.LOG_FILE])
 
     writer = CsvWriter(config[Options.OUTPUT], Path(file_path), config[Options.SINGLE_AGENT_EXPORT])
     file_stream = open(Path(file_path), "rb")
 
     if config[Options.MEMORY_SAVING]:
         log.info("Memory saving mode enabled: Disable on conversion of small files for performance improvements.")
@@ -49,21 +53,23 @@
     data_transformer = DataTransformer.build(config[Options.RESOLVE_COMPLEX_FIELD])
     try:
         while data_storages := reader.read():
             output = OutputDAO(data_storages, agent_type_log)
             for agent_name in output.get_sorted_agents_to_extract():
                 log.debug(f"Extracting data for {agent_name}...")
                 data_frames = output.get_agent_data(agent_name, data_transformer)
+                apply_time_merging(data_frames, config[Options.TIME_MERGING])
+                apply_time_option(data_frames, config[Options.TIME])
                 log.debug(f"Writing data for {agent_name}...")
                 writer.write_to_files(agent_name, data_frames)
         log.info("Data conversion completed.")
     except MemoryError:
         log_and_raise_critical(ERR_MEMORY_SEVERE if Options.MEMORY_SAVING else ERR_MEMORY_ERROR)
 
     file_stream.close()
     if not agent_type_log.has_any_agent_type():
         log.error("Provided file did not contain any output data.")
 
 
 if __name__ == "__main__":
-    input_file, run_config = arg_handling_convert_results(DEFAULT_CONFIG)
+    input_file, run_config = arg_handling_convert_results(sys.argv[1:], DEFAULT_CONFIG)
     run(input_file, run_config)
```

### Comparing `fameio-1.7/src/fameio/scripts/make_config.py` & `fameio-1.8/src/fameio/scripts/make_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 import logging as log
+import sys
 from pathlib import Path
 from typing import Union
 
-from fameio.source.cli import Options, arg_handling_make_config, get_config_or_default
+from fameio.source.cli import Options, arg_handling_make_config, update_default_config
 from fameio.source.loader import load_yaml, check_for_yaml_file_type
 from fameio.source.logs import set_up_logger
 from fameio.source.scenario import Scenario
 from fameio.source.validator import SchemaValidator
 from fameio.source.writer import ProtoWriter
 
 DEFAULT_CONFIG = {
@@ -15,22 +16,22 @@
     Options.LOG_FILE: None,
     Options.OUTPUT: Path("config.pb"),
 }
 
 
 def run(file: Union[str, Path], config: dict = None) -> None:
     """Executes the main workflow for the building of a FAME configuration file"""
-    config = get_config_or_default(config, DEFAULT_CONFIG)
+    config = update_default_config(config, DEFAULT_CONFIG)
     set_up_logger(level_name=config[Options.LOG_LEVEL], file_name=config[Options.LOG_FILE])
 
     check_for_yaml_file_type(Path(file))
     scenario = Scenario.from_dict(load_yaml(Path(file)))
     SchemaValidator.ensure_is_valid_scenario(scenario)
     writer = ProtoWriter(config[Options.OUTPUT])
     writer.write_validated_scenario(scenario)
 
     log.info("Configuration completed.")
 
 
 if __name__ == "__main__":
-    input_file, run_config = arg_handling_make_config(DEFAULT_CONFIG)
+    input_file, run_config = arg_handling_make_config(sys.argv[1:], DEFAULT_CONFIG)
     run(input_file, run_config)
```

### Comparing `fameio-1.7/src/fameio/source/loader.py` & `fameio-1.8/src/fameio/source/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 import os
 from pathlib import Path
 from fnmatch import fnmatch
 from typing import IO, Any, Callable
 
 import yaml
```

### Comparing `fameio-1.7/src/fameio/source/logs.py` & `fameio-1.8/src/fameio/source/logs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 from pathlib import Path
 from typing import NoReturn
 
 LOG_LEVELS = {
     "critical": log.CRITICAL,
     "error": log.ERROR,
```

### Comparing `fameio-1.7/src/fameio/source/path_resolver.py` & `fameio-1.8/src/fameio/source/path_resolver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import glob
 import os
 from typing import List, Optional
 
 
 class PathResolver:
     """Class responsible for locating files referenced in a scenario.
```

### Comparing `fameio-1.7/src/fameio/source/results/agent_type.py` & `fameio-1.8/src/fameio/source/results/agent_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import List, Dict, Set, Union, Tuple
 
 from fameprotobuf.Services_pb2 import Output
 
 
 class AgentType:
     """Provides information derived from an underlying protobuf AgentType"""
```

### Comparing `fameio-1.7/src/fameio/source/results/csv_writer.py` & `fameio-1.8/src/fameio/source/results/csv_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 from pathlib import Path
 from typing import Dict, Union
 
 import pandas as pd
 
 from fameio.source.results.data_transformer import INDEX
```

### Comparing `fameio-1.7/src/fameio/source/results/data_transformer.py` & `fameio-1.8/src/fameio/source/results/data_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from abc import ABC
 from builtins import staticmethod
-from typing import List, Dict, Tuple, Union
+from typing import List, Dict, Tuple, Union, Optional
 
 import pandas as pd
 from fameprotobuf.Services_pb2 import Output
 from pandas import DataFrame
 
 from fameio.source.cli import ResolveOptions
 from fameio.source.results.agent_type import AgentType
@@ -24,19 +28,19 @@
 
     @staticmethod
     def build(complex_column_mode: ResolveOptions) -> "DataTransformer":
         return DataTransformer.MODES[complex_column_mode]()
 
     def extract_agent_data(
         self, series: List[Output.Series], agent_type: AgentType
-    ) -> Dict[Union[str, None], pd.DataFrame]:
+    ) -> Dict[Optional[str], pd.DataFrame]:
         """
         Returns dict of DataFrame(s) containing all data from given `series` of given `agent_type`.
         When ResolveOption is `SPLIT`, the dict maps each complex column's name to the associated DataFrame.
-        In any case, the dict maps `None` to a DataFrame with the content of all simple column / merged columns
+        In any case, the dict maps `None` to a DataFrame with the content of all simple column / merged columns.
         """
         container = self._extract_agent_data(series, agent_type)
         data_frames = {}
         for column_id, agent_data in container.items():
             data_frame = DataFrame.from_dict(agent_data, orient="index")
             column_name = agent_type.get_column_name_for_id(column_id)
             if column_id == DataTransformer.SIMPLE_COLUMN_INDEX:
```

### Comparing `fameio-1.7/src/fameio/source/results/output_dao.py` & `fameio-1.8/src/fameio/source/results/output_dao.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from typing import List, Dict, Iterable
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
+from typing import List, Dict, Iterable, Optional
 
 import pandas as pd
 from fameprotobuf.DataStorage_pb2 import DataStorage
 from fameprotobuf.Services_pb2 import Output
 
 from fameio.source.results.agent_type import AgentTypeLog
 from fameio.source.results.data_transformer import DataTransformer
@@ -52,15 +56,15 @@
 
     def _get_agent_names_by_series_count_ascending(self) -> List[str]:
         """Returns list of agent type names sorted by their amount of series"""
         length_per_agent_types = {agent_name: len(value) for agent_name, value in self._all_series.items()}
         sorted_dict = sorted(length_per_agent_types.items(), key=lambda item: item[1])
         return [agent_name for agent_name, _ in sorted_dict]
 
-    def get_agent_data(self, agent_name: str, data_transformer: DataTransformer) -> Dict[str, pd.DataFrame]:
+    def get_agent_data(self, agent_name: str, data_transformer: DataTransformer) -> Dict[Optional[str], pd.DataFrame]:
         """
         Returns DataFrame(s) containing all data of given `agent` - data is removed after the first call
         Depending on the chosen ResolveOption the dict contains one DataFrame for the simple (and merged columns),
         or, in `SPLIT` mode, additional DataFrames mapped to each complex column's name.
         """
         agent_series = self._all_series.pop(agent_name) if agent_name in self._all_series else []
         agent_type = self._agent_type_log.get_agent_type(agent_name)
```

### Comparing `fameio-1.7/src/fameio/source/results/reader.py` & `fameio-1.8/src/fameio/source/results/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 import struct
 import typing
 from abc import ABC, abstractmethod
 from typing import IO, List
 
 from fameprotobuf.DataStorage_pb2 import DataStorage
```

### Comparing `fameio-1.7/src/fameio/source/scenario/agent.py` & `fameio-1.8/src/fameio/source/scenario/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict
 
 from fameio.source.scenario.attribute import Attribute
 from fameio.source.scenario.exception import (
     assert_or_raise,
     get_or_default,
     get_or_raise,
```

### Comparing `fameio-1.7/src/fameio/source/scenario/attribute.py` & `fameio-1.8/src/fameio/source/scenario/attribute.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 from typing import Any, Dict, List
 
 from fameio.source.scenario.exception import log_and_raise
 
 
 class Attribute:
```

### Comparing `fameio-1.7/src/fameio/source/scenario/contract.py` & `fameio-1.8/src/fameio/source/scenario/contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 from typing import Any, Dict, List, Optional
 
 from fameio.source.scenario.attribute import Attribute
 from fameio.source.scenario.exception import get_or_default, get_or_raise, log_and_raise
 from fameio.source.time import FameTime
 from fameio.source.tools import ensure_is_list, keys_to_lower
```

### Comparing `fameio-1.7/src/fameio/source/scenario/exception.py` & `fameio-1.8/src/fameio/source/scenario/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 
 from fameio.source.logs import log_error_and_raise
 
 
 def log_and_raise(message: str):
     """Raises ScenarioException with given `message`"""
```

### Comparing `fameio-1.7/src/fameio/source/scenario/fameiofactory.py` & `fameio-1.8/src/fameio/source/scenario/fameiofactory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from fameio.source.schema.schema import Schema
 from fameio.source.scenario.generalproperties import GeneralProperties
 from fameio.source.scenario.agent import Agent
 from fameio.source.scenario.contract import Contract
 
 
 class FameIOFactory:
```

### Comparing `fameio-1.7/src/fameio/source/scenario/generalproperties.py` & `fameio-1.8/src/fameio/source/scenario/generalproperties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 
 from fameio.source.scenario.exception import get_or_default, get_or_raise
 from fameio.source.time import FameTime
 from fameio.source.tools import keys_to_lower
```

### Comparing `fameio-1.7/src/fameio/source/scenario/scenario.py` & `fameio-1.8/src/fameio/source/scenario/scenario.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import List
 
 from fameio.source.scenario.agent import Agent
 from fameio.source.scenario.contract import Contract
 from fameio.source.scenario.exception import get_or_default, get_or_raise
 from fameio.source.scenario.fameiofactory import FameIOFactory
 from fameio.source.scenario.generalproperties import GeneralProperties
```

### Comparing `fameio-1.7/src/fameio/source/schema/agenttype.py` & `fameio-1.8/src/fameio/source/schema/agenttype.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 from typing import Dict, List, Any
 
 from fameio.source.logs import log_error_and_raise
 from fameio.source.schema.exception import SchemaException
 from fameio.source.schema.attribute import AttributeSpecs
 from fameio.source.tools import keys_to_lower
```

### Comparing `fameio-1.7/src/fameio/source/schema/attribute.py` & `fameio-1.8/src/fameio/source/schema/attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 import typing
 from enum import Enum, auto
 from typing import Any, Dict
 
 from fameio.source.schema.exception import SchemaException
 from fameio.source.time import FameTime
```

### Comparing `fameio-1.7/src/fameio/source/schema/schema.py` & `fameio-1.8/src/fameio/source/schema/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Dict
 
 from fameio.source.logs import log_error_and_raise
 from fameio.source.schema.agenttype import AgentType
 from fameio.source.schema.exception import SchemaException
 from fameio.source.tools import keys_to_lower
```

### Comparing `fameio-1.7/src/fameio/source/series.py` & `fameio-1.8/src/fameio/source/series.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Dict, Union
 
 from fameio.source.logs import log_error_and_raise
 
 
 class SeriesManagementException(Exception):
     """Indicates that an error occurred during management of time series"""
```

### Comparing `fameio-1.7/src/fameio/source/time.py` & `fameio-1.8/src/fameio/source/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import datetime as dt
 import math
 import re
 from enum import Enum
 from typing import Union
 
 from fameio.source.logs import log_error_and_raise
@@ -61,14 +65,15 @@
     """Handles conversion of TimeSteps and TimeDurations into TimeStamps and vice versa"""
 
     _TIME_UNIT_UNKNOWN = "TimeUnit conversion of '{}' not implemented."
     _FORMAT_INVALID = "'{}' is not recognised as time stamp string - check its format."
     _INVALID_TIMESTAMP = "Cannot convert time stamp string '{}' - check its format."
     _INVALID_TOO_LARGE = "Cannot convert time stamp string '{}' - last day of leap year is Dec 30th!"
     _NO_TIMESTAMP = "Time value expected, but '{}' is neither a time stamp string nor an integer."
+    _INVALID_DATE_FORMAT = "Received invalid date format '{}'."
 
     @staticmethod
     def convert_datetime_to_fame_time_step(datetime_string: str) -> int:
         """Converts real Datetime string to FAME time step"""
         if not FameTime.is_datetime(datetime_string):
             log_error_and_raise(ConversionException(FameTime._FORMAT_INVALID.format(datetime_string)))
         datetime = FameTime._convert_to_datetime(datetime_string)
@@ -86,23 +91,29 @@
         """Converts given `datetime_string` to real-world datetime"""
         try:
             return dt.datetime.strptime(datetime_string, DATE_FORMAT)
         except ValueError:
             log_error_and_raise(ConversionException(FameTime._INVALID_TIMESTAMP.format(datetime_string)))
 
     @staticmethod
-    def convert_fame_time_step_to_datetime(fame_time_steps: int) -> str:
-        """Converts given `fame_time_steps` to corresponding real-world datetime string"""
+    def convert_fame_time_step_to_datetime(fame_time_steps: int, date_format: str = DATE_FORMAT) -> str:
+        """
+        Converts given `fame_time_steps` to corresponding real-world datetime string in `date_format`,
+        raises ConversionException if invalid `date_format` received.
+        """
         years_since_start_time = math.floor(fame_time_steps / Constants.STEPS_PER_YEAR)
         current_year = years_since_start_time + Constants.FIRST_YEAR
         beginning_of_year = dt.datetime(year=current_year, month=1, day=1, hour=0, minute=0, second=0)
         steps_in_current_year = fame_time_steps - years_since_start_time * Constants.STEPS_PER_YEAR
         seconds_in_current_year = steps_in_current_year / Constants.STEPS_PER_SECOND
         datetime = beginning_of_year + dt.timedelta(seconds=seconds_in_current_year)
-        return datetime.strftime(DATE_FORMAT)
+        try:
+            return datetime.strftime(date_format)
+        except ValueError:
+            log_error_and_raise(ConversionException(FameTime._INVALID_DATE_FORMAT.format(date_format)))
 
     @staticmethod
     def convert_time_span_to_fame_time_steps(value: int, unit: TimeUnit) -> int:
         """Converts value of `TimeUnit.UNIT` to fame time steps"""
         steps = Constants.steps_per_unit.get(unit)
         if steps:
             return steps * value
```

### Comparing `fameio-1.7/src/fameio/source/tools.py` & `fameio-1.8/src/fameio/source/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict
 
 
 def keys_to_lower(dictionary: Dict[str, Any]) -> Dict[str, Any]:
     """Returns new dictionary content of given `dictionary` but its `keys` in lower case"""
     return {keys.lower(): value for keys, value in dictionary.items()}
```

### Comparing `fameio-1.7/src/fameio/source/validator.py` & `fameio-1.8/src/fameio/source/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 from collections import Counter
 from typing import Any, Dict, List
 
 from fameio.source.logs import log_error_and_raise
 from fameio.source.scenario import Agent, Attribute, Contract, Scenario
 from fameio.source.schema.agenttype import AgentType
```

### Comparing `fameio-1.7/src/fameio/source/writer.py` & `fameio-1.8/src/fameio/source/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging as log
 import os.path
 from pathlib import Path
 from typing import Any, Dict
 
 import pandas as pd
 from fameio.source.logs import log_error_and_raise
```

### Comparing `fameio-1.7/src/fameio.egg-info/PKG-INFO` & `fameio-1.8/src/fameio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: fameio
-Version: 1.7
+Version: 1.8
 Summary: Python scripts for operation of FAME models
 Home-page: https://gitlab.com/fame-framework/fame-io/
 Author: Felix Nitsch, Christoph Schimeczek, Ulrich Frey, Marc Deissenroth-Uhrig, Benjamin Fuchs, A. Achraf El Ghazi
 Author-email: fame@dlr.de
 License: Apache License 2.0
 Keywords: FAME,agent-based modelling
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
+Provides-Extra: dev
+License-File: LICENSE.txt
 
+<!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+
+SPDX-License-Identifier: Apache-2.0 -->
 [![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4501190.svg)](https://doi.org/10.5281/zenodo.4501190)
+[![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
+[![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
 [![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
 [![pipeline status](https://gitlab.com/fame-framework/fame-io/badges/main/pipeline.svg)](https://gitlab.com/fame-framework/fame-io/commits/main)
 [![coverage report](https://gitlab.com/fame-framework/fame-io/badges/main/coverage.svg)](https://gitlab.com/fame-framework/fame-io/-/commits/main)
+[![REUSE status](https://api.reuse.software/badge/gitlab.com/fame-framework/fame-io)](https://api.reuse.software/info/gitlab.com/fame-framework/fame-io)
 
 # FAME-Io
 Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
 Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
 The package is also formerly known as [FAME-Py](https://doi.org/10.5281/zenodo.4314338).
 
 # Installation
@@ -535,20 +540,36 @@
 | `-l` or `--log` <option>             | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
 | `-lf` or `--logfile` <file>          | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
 | `-a` or `--agents` <list-of-agents>  | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
 | `-o` or `--output`                   | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
 | `-se` or `--single-export`           | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
 | `-m` or `--memory-saving`            | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
 | `-cc` or `--complex-column` <option> | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
+| `-t` or `--time` <option>            | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
+
+Additionally, you may merge TimeSteps of a certain range of steps in the output files to
+  i) associate multiple time steps with a common logical time in your simulation
+  ii) reduce number of lines in output files
+
+For this, add the option `merge-times` and specify the arguments as follows:
+
+| Command                   | Action                                                                                   |
+|---------------------------|------------------------------------------------------------------------------------------|
+| `-fp` or `--focal-point`  | TimeStep on which `steps-before` earlier and `steps-after` later TimeSteps are merged on |
+| `-sb` or `--steps-before` | Range of TimeSteps before the `focal-point` they get merged to                           |
+| `-sa` or `--steps-after`  | Range of TimeSteps after the `focal-point` they get merged to                            |
 
 This could look as follows:
 
-    convertFameResults -f <./path/to/protobuf_file.pb> -l debug -lf <path/to/output.log> -a AgentType1 AgentType2 -o myCsvFolder -m -cc SPLIT
+    convertFameResults -f <./path/to/protobuf_file.pb> -l debug -lf <path/to/output.log> -a AgentType1 AgentType2 -o myCsvFolder -m -cc SPLIT merge-times -fp 0 -sb 1799 -sa 1800
 
-You may also call the conversion script from any Python script with
+Make sure that in the range of time steps you specify for merging there is only one value per column in the merged time range.
+If multiple values per column are merged values will get concatenated and might yield unexpected results.
+
+You may also call the conversion script from any Python script with:
 
 ```python
 from fameio.scripts.convert_results import run as convert_results
 
 convert_results("./path/to/protobuf_file.pb")
 ```
 
@@ -561,29 +582,56 @@
 run_config = {Options.LOG_LEVEL: "info",
               Options.LOG_FILE: "scenario.log",
               Options.OUTPUT: "Output",
               Options.AGENT_LIST: ['AgentType1', 'AgentType2'],
               Options.MEMORY_SAVING: False,
               Options.SINGLE_AGENT_EXPORT: False,
               Options.RESOLVE_COMPLEX_FIELD: "SPLIT",
+              Options.TIME: "INT",
+              Options.TIME_MERGING: {},
               }
 
 convert_results("./path/to/protobuf_file.pb", run_config)
 ```
 
-# Contribute
+## Cite FAME-Io
+If you use FAME-Io for academic work, please cite as follows.
+
+Bibtex entry:
+```
+@article{fameio2023joss,
+  author  = {Felix Nitsch and Christoph Schimeczek and Ulrich Frey and Benjamin Fuchs},
+  title   = {FAME-Io: Configuration tools for complex agent-based simulations},
+  journal = {Journal of Open Source Software},
+  year    = {2023},
+  doi     = {doi: https://doi.org/10.21105/joss.04958}
+}
+```
+
+## Contribute
 Please read the Contributors License Agreement `cla.md`, sign it and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing.
 
 ## Testing changes locally
 
 Once some changes have been performed on the local git clone, use the following command to override your local installation with your modified copy in order to test the result:
 
 ```bash
 python3 setup.py bdist_wheel && pip3 install --force-reinstall --no-dependencies ./dist/*.whl
 ```
 
 ## Code style
 
 We use the code formatting library [`black`](https://pypi.org/project/black/).
-The maximum line length is defined as 120 characters. 
+The maximum line length is defined as 120 characters.
 Therefore, before committing, run `black --line-length 120 .`
 
+## Pre-Commit hooks
+
+FAME-Io uses several pre-commit hooks to ensure high code quality.
+To use them, install `dev` packages and then initialise pre-commit in FAME-Io's base folder:
+
+```
+    pip install fameio[dev]
+    pre-commit install -t pre-commit -t pre-push
+```
+
+
```

### Comparing `fameio-1.7/src/fameio.egg-info/SOURCES.txt` & `fameio-1.8/src/fameio.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE
+LICENSE.txt
 README.md
 setup.py
 src/fameio/__init__.py
 src/fameio.egg-info/PKG-INFO
 src/fameio.egg-info/SOURCES.txt
 src/fameio.egg-info/dependency_links.txt
 src/fameio.egg-info/entry_points.txt
@@ -20,14 +20,15 @@
 src/fameio/source/series.py
 src/fameio/source/time.py
 src/fameio/source/tools.py
 src/fameio/source/validator.py
 src/fameio/source/writer.py
 src/fameio/source/results/__init__.py
 src/fameio/source/results/agent_type.py
+src/fameio/source/results/conversion.py
 src/fameio/source/results/csv_writer.py
 src/fameio/source/results/data_transformer.py
 src/fameio/source/results/output_dao.py
 src/fameio/source/results/reader.py
 src/fameio/source/scenario/__init__.py
 src/fameio/source/scenario/agent.py
 src/fameio/source/scenario/attribute.py
```

