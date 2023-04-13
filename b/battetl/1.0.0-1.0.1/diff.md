# Comparing `tmp/battetl-1.0.0.tar.gz` & `tmp/battetl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battetl-1.0.0.tar", last modified: Tue Apr 11 20:16:08 2023, max compression
+gzip compressed data, was "battetl-1.0.1.tar", last modified: Thu Apr 13 23:31:40 2023, max compression
```

## Comparing `battetl-1.0.0.tar` & `battetl-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 20:16:08.725299 battetl-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-04-04 20:46:42.000000 battetl-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    14511 2023-04-11 20:16:08.718277 battetl-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13972 2023-04-11 19:33:26.000000 battetl-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 20:16:08.676636 battetl-1.0.0/battetl/
--rw-rw-rw-   0        0        0     7291 2023-04-10 18:26:06.000000 battetl-1.0.0/battetl/BattETL.py
--rw-rw-rw-   0        0        0      116 2023-04-05 19:58:40.000000 battetl-1.0.0/battetl/__init__.py
--rw-rw-rw-   0        0        0     8243 2023-04-05 19:58:40.000000 battetl-1.0.0/battetl/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:16:08.693015 battetl-1.0.0/battetl/extract/
--rw-rw-rw-   0        0        0    27305 2023-04-10 18:26:06.000000 battetl-1.0.0/battetl/extract/Extractor.py
--rw-rw-rw-   0        0        0       34 2023-04-05 19:58:40.000000 battetl-1.0.0/battetl/extract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:16:08.709038 battetl-1.0.0/battetl/load/
--rw-rw-rw-   0        0        0    33698 2023-04-11 19:33:26.000000 battetl-1.0.0/battetl/load/Loader.py
--rw-rw-rw-   0        0        0       28 2023-04-05 19:58:40.000000 battetl-1.0.0/battetl/load/__init__.py
--rw-rw-rw-   0        0        0     1573 2023-04-05 19:58:40.000000 battetl-1.0.0/battetl/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:16:08.717036 battetl-1.0.0/battetl/transform/
--rw-rw-rw-   0        0        0    23437 2023-04-10 18:26:06.000000 battetl-1.0.0/battetl/transform/Transformer.py
--rw-rw-rw-   0        0        0       38 2023-04-05 19:58:40.000000 battetl-1.0.0/battetl/transform/__init__.py
--rw-rw-rw-   0        0        0    12219 2023-04-05 19:58:40.000000 battetl-1.0.0/battetl/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:16:08.693015 battetl-1.0.0/battetl.egg-info/
--rw-rw-rw-   0        0        0    14511 2023-04-11 20:16:08.000000 battetl-1.0.0/battetl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-11 20:16:08.000000 battetl-1.0.0/battetl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 20:16:08.000000 battetl-1.0.0/battetl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 20:16:08.000000 battetl-1.0.0/battetl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 20:16:08.725299 battetl-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-11 20:13:07.000000 battetl-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.405179 battetl-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-04 20:46:42.000000 battetl-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    14919 2023-04-13 23:31:40.404173 battetl-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14366 2023-04-13 22:40:48.000000 battetl-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.378146 battetl-1.0.1/battetl/
+-rw-rw-rw-   0        0        0     7291 2023-04-10 18:26:06.000000 battetl-1.0.1/battetl/BattETL.py
+-rw-rw-rw-   0        0        0      116 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/__init__.py
+-rw-rw-rw-   0        0        0     8243 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.392654 battetl-1.0.1/battetl/extract/
+-rw-rw-rw-   0        0        0    27305 2023-04-10 18:26:06.000000 battetl-1.0.1/battetl/extract/Extractor.py
+-rw-rw-rw-   0        0        0       34 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/extract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.397666 battetl-1.0.1/battetl/load/
+-rw-rw-rw-   0        0        0    33698 2023-04-11 19:33:26.000000 battetl-1.0.1/battetl/load/Loader.py
+-rw-rw-rw-   0        0        0       28 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/load/__init__.py
+-rw-rw-rw-   0        0        0     1573 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.401142 battetl-1.0.1/battetl/transform/
+-rw-rw-rw-   0        0        0    23437 2023-04-10 18:26:06.000000 battetl-1.0.1/battetl/transform/Transformer.py
+-rw-rw-rw-   0        0        0       38 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/transform/__init__.py
+-rw-rw-rw-   0        0        0    12219 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.388146 battetl-1.0.1/battetl.egg-info/
+-rw-rw-rw-   0        0        0    14919 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 23:31:40.405179 battetl-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1140 2023-04-13 23:21:25.000000 battetl-1.0.1/setup.py
```

### Comparing `battetl-1.0.0/LICENSE` & `battetl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `battetl-1.0.0/PKG-INFO` & `battetl-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang and Chintan Pathak
 Author-email: info@battgenie.life
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BattETL
 
 BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
 
-<img src="./images/BattETL_Simple_System.svg">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
 
-### Overview
+## Overview
 
 - [Motivation](#motivation)
 - [Video Guides](#video-guides)
 - [Installation](#installation)
-    - [Requirements](#requirements)
-    - [Installation Instructions](#installation-instructions)
+  - [Requirements](#requirements)
+  - [Installation Instructions](#installation-instructions)
 - [Usage](#usage)
-    - [Config File](#config-file)
-    - [Env File](#env-file)
-    - [Data Export Requirements](#data-export-requirements)
-        - [Maccor](#maccor)
-        - [Arbin](#arbin)
-- [Overview](#overview)
-    - [System Diagram](#system-diagram)
-    - [Transformer](#transformer)
-    - [Extractor](#extractor)
-    - [Loader](#loader)
+  - [Config File](#config-file)
+  - [Env File](#env-file)
+  - [Data Export Requirements](#data-export-requirements)
+    - [Maccor](#maccor)
+    - [Arbin](#arbin)
+- [BattETL Overview](#battetl-overview)
+  - [System Diagram](#system-diagram)
+  - [Transformer](#transformer)
+  - [Extractor](#extractor)
+  - [Loader](#loader)
 - [Testing](#testing)
 - [Troubleshooting](#troubleshooting)
 
-# Motivation
+## Motivation
 
-## Why another battery cycler data ingesting tool?
+### Why another battery cycler data ingesting tool?
 
 There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
 
 ### Some features of BattETL
 
 - **A relational data destination.**
 
@@ -55,42 +56,50 @@
 
 Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
 
 - **Analytics built into the transformation step.**
 
 As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
 
-# Video Guides
+## Video Guides
 
 The following are video guides BattETL and BattDB:
 
 - [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
 - [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
 - [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
-# Installation
+## Installation
 
 A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
 
-## Requirements
+### Requirements
 
 BattETL requires Python 3.9 or 3.10. The specific package requirements are detailed in the `requirements.txt` file.
 
-## Installation Instructions
+### Installation Instructions
 
-Within the directory type the following into a terminal:
+Install BattETL using pip:
 
 ```sh
+pip install battetl
+```
+
+Install BattETL from source code:
+
+```sh
+git clone https://github.com/BattGenie/battetl.git
+cd battetl
 pip install -r requirements.txt
 pip install .
 ```
 
-Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb)] database to load the data to. Follow the instructions there for deploying the database.
+Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
 
-# Usage
+## Usage
 
 A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
 Using BattETL as an all-in-one ETL function is as easy as:
 
 ```python
 from battetl import BattETL
@@ -104,15 +113,15 @@
 
 Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
 
 For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
 
 > Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
 
-## Config File
+### Config File
 
 To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
 
 ```json
 {
     "timezone": "America/Los_Angeles",
     "data_file_path": [
@@ -147,34 +156,35 @@
             "manufacturer": "BattGenie",
             "model": "Cycler9000"
         }
     }
 }
 ```
 
-## Env File
+### Env File
 
 The .env contains the associated database credentials and is formatted as follows
 
 ```
 ENV=dev # dev, prod
 DB_TARGET=YOUR_DATABASE_NAME
 DB_USERNAME=YOUR_USERNAME
 DB_PASSWORD=YOUR_PASSWORD
 DB_HOSTNAME=localhost
 DB_PORT=5432
 ```
+
 An example .env file is given within `examples/.env.example`
 
-## Data Export Requirements
+### Data Export Requirements
 
 - [For Maccor Cycler](#maccor)
 - [For Arbin Cycler](#arbin)
 
-### Maccor
+#### Maccor
 
 From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
 
 The following columns are the minimum required for export:
 
 For Data Records:
 
@@ -184,34 +194,34 @@
 - Step Time : Header Label of StepTime(s), Units of seconds
 - Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
 - Energy : Header Label of Watt-hr, Units of Watt-hour
 - Current : Header Label of Current(A), Units of Amps
 - Voltage : Header Label of Voltage(V), Units of Volts
 - DPT Time : Header label of DPt Time
 
-<img src="./images/MaccorExport_DataRecords.png" width="85%" height="50%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
 
 For Cycle Statistics:
 
 - Cycle : Header Label of Cycle
 - Capacity Chg : Header label AH-IN, Units of Ahr
 - Capacity Dis : Header label AH-Out, Units of Ahr
 - DPT Time : Header Label of DPt Time
 
-<img src="./images/MaccorExport_CycleStats.png" width="85%" height="50%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
 
-### Arbin
+#### Arbin
 
 Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
 
-<img src="./images/ArbinExport.jpg" width="45%" height="25%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
 
-An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory. 
+An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
 
-# BattETL Overview
+## BattETL Overview
 
 A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
 
 BattETL bundles together the three independent submodules:
 
 - [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
 - [Transformer](#transformer) : Responsible for transforming cycler data
@@ -221,87 +231,87 @@
 
 - `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
 - `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
 - `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
 - `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
 - `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
 
-## System diagram
+### System diagram
 
-<img src="./images/BattETL_SystemDiagram.svg">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
 
-## Extractor
+### Extractor
 
 The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
 - `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
 - `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
 
-### Variables
+#### Variables
 
 - `cycler_make: str`: Cycler make  
 - `raw_test_data_meta_data: list[dict]`: Test data meta data  
 - `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
 - `raw_test_data: pandas.DataFrame`: Test data  
 - `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
 - `maccor_procedure: dict`: Maccor procedure  
 - `arbin_schedule: dict`: Arbin schedule  
 
-## Transformer
+### Transformer
 
 The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
 - `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
 
-### Variables
+#### Variables
 
 - `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
 - `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
 - `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
 - `test_data: pandas.DataFrame`: Transformed test data  
 - `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
 
-## Loader
+### Loader
 
 The `load` module provides an interface to load the extracted data into a database.
 
-Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the lastest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
 - `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
 
-# Testing
+## Testing
 
 To run the test suite, use the following commands:
 
 - Run all tests: `pytest`
 - Run Maccor tests: `pytest -m maccor`
 - Run Arbin tests: `pytest -m arbin`
 - Run database specific tests: `pytest -m database`
 - Run tests other than Arbin: `pytest -m "not arbin"`
 - Run Extractor tests: `pytest tests/test_extract_data.py`
 
 To show logs while testing, add the `-o log_cli=true` flag.
 
-# Troubleshooting
+## Troubleshooting
 
-## pip install psycopg2 error
+### pip install psycopg2 error
 
 If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
 
 ```sh
 sudo apt install libpq-dev
 ```
```

### Comparing `battetl-1.0.0/README.md` & `battetl-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # BattETL
 
 BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
 
-<img src="./images/BattETL_Simple_System.svg">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
 
-### Overview
+## Overview
 
 - [Motivation](#motivation)
 - [Video Guides](#video-guides)
 - [Installation](#installation)
-    - [Requirements](#requirements)
-    - [Installation Instructions](#installation-instructions)
+  - [Requirements](#requirements)
+  - [Installation Instructions](#installation-instructions)
 - [Usage](#usage)
-    - [Config File](#config-file)
-    - [Env File](#env-file)
-    - [Data Export Requirements](#data-export-requirements)
-        - [Maccor](#maccor)
-        - [Arbin](#arbin)
-- [Overview](#overview)
-    - [System Diagram](#system-diagram)
-    - [Transformer](#transformer)
-    - [Extractor](#extractor)
-    - [Loader](#loader)
+  - [Config File](#config-file)
+  - [Env File](#env-file)
+  - [Data Export Requirements](#data-export-requirements)
+    - [Maccor](#maccor)
+    - [Arbin](#arbin)
+- [BattETL Overview](#battetl-overview)
+  - [System Diagram](#system-diagram)
+  - [Transformer](#transformer)
+  - [Extractor](#extractor)
+  - [Loader](#loader)
 - [Testing](#testing)
 - [Troubleshooting](#troubleshooting)
 
-# Motivation
+## Motivation
 
-## Why another battery cycler data ingesting tool?
+### Why another battery cycler data ingesting tool?
 
 There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
 
 ### Some features of BattETL
 
 - **A relational data destination.**
 
@@ -41,42 +41,50 @@
 
 Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
 
 - **Analytics built into the transformation step.**
 
 As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
 
-# Video Guides
+## Video Guides
 
 The following are video guides BattETL and BattDB:
 
 - [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
 - [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
 - [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
-# Installation
+## Installation
 
 A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
 
-## Requirements
+### Requirements
 
 BattETL requires Python 3.9 or 3.10. The specific package requirements are detailed in the `requirements.txt` file.
 
-## Installation Instructions
+### Installation Instructions
 
-Within the directory type the following into a terminal:
+Install BattETL using pip:
 
 ```sh
+pip install battetl
+```
+
+Install BattETL from source code:
+
+```sh
+git clone https://github.com/BattGenie/battetl.git
+cd battetl
 pip install -r requirements.txt
 pip install .
 ```
 
-Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb)] database to load the data to. Follow the instructions there for deploying the database.
+Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
 
-# Usage
+## Usage
 
 A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
 Using BattETL as an all-in-one ETL function is as easy as:
 
 ```python
 from battetl import BattETL
@@ -90,15 +98,15 @@
 
 Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
 
 For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
 
 > Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
 
-## Config File
+### Config File
 
 To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
 
 ```json
 {
     "timezone": "America/Los_Angeles",
     "data_file_path": [
@@ -133,34 +141,35 @@
             "manufacturer": "BattGenie",
             "model": "Cycler9000"
         }
     }
 }
 ```
 
-## Env File
+### Env File
 
 The .env contains the associated database credentials and is formatted as follows
 
 ```
 ENV=dev # dev, prod
 DB_TARGET=YOUR_DATABASE_NAME
 DB_USERNAME=YOUR_USERNAME
 DB_PASSWORD=YOUR_PASSWORD
 DB_HOSTNAME=localhost
 DB_PORT=5432
 ```
+
 An example .env file is given within `examples/.env.example`
 
-## Data Export Requirements
+### Data Export Requirements
 
 - [For Maccor Cycler](#maccor)
 - [For Arbin Cycler](#arbin)
 
-### Maccor
+#### Maccor
 
 From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
 
 The following columns are the minimum required for export:
 
 For Data Records:
 
@@ -170,34 +179,34 @@
 - Step Time : Header Label of StepTime(s), Units of seconds
 - Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
 - Energy : Header Label of Watt-hr, Units of Watt-hour
 - Current : Header Label of Current(A), Units of Amps
 - Voltage : Header Label of Voltage(V), Units of Volts
 - DPT Time : Header label of DPt Time
 
-<img src="./images/MaccorExport_DataRecords.png" width="85%" height="50%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
 
 For Cycle Statistics:
 
 - Cycle : Header Label of Cycle
 - Capacity Chg : Header label AH-IN, Units of Ahr
 - Capacity Dis : Header label AH-Out, Units of Ahr
 - DPT Time : Header Label of DPt Time
 
-<img src="./images/MaccorExport_CycleStats.png" width="85%" height="50%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
 
-### Arbin
+#### Arbin
 
 Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
 
-<img src="./images/ArbinExport.jpg" width="45%" height="25%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
 
-An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory. 
+An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
 
-# BattETL Overview
+## BattETL Overview
 
 A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
 
 BattETL bundles together the three independent submodules:
 
 - [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
 - [Transformer](#transformer) : Responsible for transforming cycler data
@@ -207,87 +216,87 @@
 
 - `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
 - `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
 - `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
 - `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
 - `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
 
-## System diagram
+### System diagram
 
-<img src="./images/BattETL_SystemDiagram.svg">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
 
-## Extractor
+### Extractor
 
 The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
 - `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
 - `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
 
-### Variables
+#### Variables
 
 - `cycler_make: str`: Cycler make  
 - `raw_test_data_meta_data: list[dict]`: Test data meta data  
 - `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
 - `raw_test_data: pandas.DataFrame`: Test data  
 - `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
 - `maccor_procedure: dict`: Maccor procedure  
 - `arbin_schedule: dict`: Arbin schedule  
 
-## Transformer
+### Transformer
 
 The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
 - `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
 
-### Variables
+#### Variables
 
 - `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
 - `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
 - `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
 - `test_data: pandas.DataFrame`: Transformed test data  
 - `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
 
-## Loader
+### Loader
 
 The `load` module provides an interface to load the extracted data into a database.
 
-Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the lastest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
 - `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
 
-# Testing
+## Testing
 
 To run the test suite, use the following commands:
 
 - Run all tests: `pytest`
 - Run Maccor tests: `pytest -m maccor`
 - Run Arbin tests: `pytest -m arbin`
 - Run database specific tests: `pytest -m database`
 - Run tests other than Arbin: `pytest -m "not arbin"`
 - Run Extractor tests: `pytest tests/test_extract_data.py`
 
 To show logs while testing, add the `-o log_cli=true` flag.
 
-# Troubleshooting
+## Troubleshooting
 
-## pip install psycopg2 error
+### pip install psycopg2 error
 
 If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
 
 ```sh
 sudo apt install libpq-dev
 ```
```

### Comparing `battetl-1.0.0/battetl/BattETL.py` & `battetl-1.0.1/battetl/BattETL.py`

 * *Files identical despite different names*

### Comparing `battetl-1.0.0/battetl/constants.py` & `battetl-1.0.1/battetl/constants.py`

 * *Files identical despite different names*

### Comparing `battetl-1.0.0/battetl/extract/Extractor.py` & `battetl-1.0.1/battetl/extract/Extractor.py`

 * *Files identical despite different names*

### Comparing `battetl-1.0.0/battetl/load/Loader.py` & `battetl-1.0.1/battetl/load/Loader.py`

 * *Files identical despite different names*

### Comparing `battetl-1.0.0/battetl/logger.py` & `battetl-1.0.1/battetl/logger.py`

 * *Files identical despite different names*

### Comparing `battetl-1.0.0/battetl/transform/Transformer.py` & `battetl-1.0.1/battetl/transform/Transformer.py`

 * *Files identical despite different names*

### Comparing `battetl-1.0.0/battetl/utils.py` & `battetl-1.0.1/battetl/utils.py`

 * *Files identical despite different names*

### Comparing `battetl-1.0.0/battetl.egg-info/PKG-INFO` & `battetl-1.0.1/battetl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang and Chintan Pathak
 Author-email: info@battgenie.life
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BattETL
 
 BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
 
-<img src="./images/BattETL_Simple_System.svg">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
 
-### Overview
+## Overview
 
 - [Motivation](#motivation)
 - [Video Guides](#video-guides)
 - [Installation](#installation)
-    - [Requirements](#requirements)
-    - [Installation Instructions](#installation-instructions)
+  - [Requirements](#requirements)
+  - [Installation Instructions](#installation-instructions)
 - [Usage](#usage)
-    - [Config File](#config-file)
-    - [Env File](#env-file)
-    - [Data Export Requirements](#data-export-requirements)
-        - [Maccor](#maccor)
-        - [Arbin](#arbin)
-- [Overview](#overview)
-    - [System Diagram](#system-diagram)
-    - [Transformer](#transformer)
-    - [Extractor](#extractor)
-    - [Loader](#loader)
+  - [Config File](#config-file)
+  - [Env File](#env-file)
+  - [Data Export Requirements](#data-export-requirements)
+    - [Maccor](#maccor)
+    - [Arbin](#arbin)
+- [BattETL Overview](#battetl-overview)
+  - [System Diagram](#system-diagram)
+  - [Transformer](#transformer)
+  - [Extractor](#extractor)
+  - [Loader](#loader)
 - [Testing](#testing)
 - [Troubleshooting](#troubleshooting)
 
-# Motivation
+## Motivation
 
-## Why another battery cycler data ingesting tool?
+### Why another battery cycler data ingesting tool?
 
 There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
 
 ### Some features of BattETL
 
 - **A relational data destination.**
 
@@ -55,42 +56,50 @@
 
 Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
 
 - **Analytics built into the transformation step.**
 
 As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
 
-# Video Guides
+## Video Guides
 
 The following are video guides BattETL and BattDB:
 
 - [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
 - [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
 - [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
-# Installation
+## Installation
 
 A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
 
-## Requirements
+### Requirements
 
 BattETL requires Python 3.9 or 3.10. The specific package requirements are detailed in the `requirements.txt` file.
 
-## Installation Instructions
+### Installation Instructions
 
-Within the directory type the following into a terminal:
+Install BattETL using pip:
 
 ```sh
+pip install battetl
+```
+
+Install BattETL from source code:
+
+```sh
+git clone https://github.com/BattGenie/battetl.git
+cd battetl
 pip install -r requirements.txt
 pip install .
 ```
 
-Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb)] database to load the data to. Follow the instructions there for deploying the database.
+Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
 
-# Usage
+## Usage
 
 A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
 Using BattETL as an all-in-one ETL function is as easy as:
 
 ```python
 from battetl import BattETL
@@ -104,15 +113,15 @@
 
 Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
 
 For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
 
 > Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
 
-## Config File
+### Config File
 
 To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
 
 ```json
 {
     "timezone": "America/Los_Angeles",
     "data_file_path": [
@@ -147,34 +156,35 @@
             "manufacturer": "BattGenie",
             "model": "Cycler9000"
         }
     }
 }
 ```
 
-## Env File
+### Env File
 
 The .env contains the associated database credentials and is formatted as follows
 
 ```
 ENV=dev # dev, prod
 DB_TARGET=YOUR_DATABASE_NAME
 DB_USERNAME=YOUR_USERNAME
 DB_PASSWORD=YOUR_PASSWORD
 DB_HOSTNAME=localhost
 DB_PORT=5432
 ```
+
 An example .env file is given within `examples/.env.example`
 
-## Data Export Requirements
+### Data Export Requirements
 
 - [For Maccor Cycler](#maccor)
 - [For Arbin Cycler](#arbin)
 
-### Maccor
+#### Maccor
 
 From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
 
 The following columns are the minimum required for export:
 
 For Data Records:
 
@@ -184,34 +194,34 @@
 - Step Time : Header Label of StepTime(s), Units of seconds
 - Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
 - Energy : Header Label of Watt-hr, Units of Watt-hour
 - Current : Header Label of Current(A), Units of Amps
 - Voltage : Header Label of Voltage(V), Units of Volts
 - DPT Time : Header label of DPt Time
 
-<img src="./images/MaccorExport_DataRecords.png" width="85%" height="50%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
 
 For Cycle Statistics:
 
 - Cycle : Header Label of Cycle
 - Capacity Chg : Header label AH-IN, Units of Ahr
 - Capacity Dis : Header label AH-Out, Units of Ahr
 - DPT Time : Header Label of DPt Time
 
-<img src="./images/MaccorExport_CycleStats.png" width="85%" height="50%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
 
-### Arbin
+#### Arbin
 
 Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
 
-<img src="./images/ArbinExport.jpg" width="45%" height="25%">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
 
-An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory. 
+An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
 
-# BattETL Overview
+## BattETL Overview
 
 A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
 
 BattETL bundles together the three independent submodules:
 
 - [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
 - [Transformer](#transformer) : Responsible for transforming cycler data
@@ -221,87 +231,87 @@
 
 - `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
 - `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
 - `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
 - `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
 - `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
 
-## System diagram
+### System diagram
 
-<img src="./images/BattETL_SystemDiagram.svg">
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
 
-## Extractor
+### Extractor
 
 The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
 - `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
 - `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
 
-### Variables
+#### Variables
 
 - `cycler_make: str`: Cycler make  
 - `raw_test_data_meta_data: list[dict]`: Test data meta data  
 - `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
 - `raw_test_data: pandas.DataFrame`: Test data  
 - `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
 - `maccor_procedure: dict`: Maccor procedure  
 - `arbin_schedule: dict`: Arbin schedule  
 
-## Transformer
+### Transformer
 
 The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
 - `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
 
-### Variables
+#### Variables
 
 - `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
 - `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
 - `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
 - `test_data: pandas.DataFrame`: Transformed test data  
 - `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
 
-## Loader
+### Loader
 
 The `load` module provides an interface to load the extracted data into a database.
 
-Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the lastest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
 
 For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
 
-### Functions
+#### Functions
 
 - `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
 - `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
 
-# Testing
+## Testing
 
 To run the test suite, use the following commands:
 
 - Run all tests: `pytest`
 - Run Maccor tests: `pytest -m maccor`
 - Run Arbin tests: `pytest -m arbin`
 - Run database specific tests: `pytest -m database`
 - Run tests other than Arbin: `pytest -m "not arbin"`
 - Run Extractor tests: `pytest tests/test_extract_data.py`
 
 To show logs while testing, add the `-o log_cli=true` flag.
 
-# Troubleshooting
+## Troubleshooting
 
-## pip install psycopg2 error
+### pip install psycopg2 error
 
 If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
 
 ```sh
 sudo apt install libpq-dev
 ```
```

