# Comparing `tmp/chelsa_cmip6-1.1.tar.gz` & `tmp/chelsa_cmip6-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/karger/scripts/chelsa_cmip6/dist/tmpng4palze/chelsa_cmip6-1.1.tar", last modified: Mon Oct 31 09:41:47 2022, max compression
+gzip compressed data, was "/home/karger/scripts/chelsa_cmip6/dist/tmpmv6702el/chelsa_cmip6-1.2.tar", last modified: Fri Apr 14 11:58:42 2023, max compression
```

## Comparing `chelsa_cmip6-1.1.tar` & `chelsa_cmip6-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 karger   (67351) karger   (69282)        0 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/
--rw-r--r--   0 karger   (67351) karger   (69282)    15889 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/PKG-INFO
--rw-rw-r--   0 karger   (67351) karger   (69282)      999 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/setup.cfg
--rw-rw-r--   0 karger   (67351) karger   (69282)    14844 2022-10-31 09:29:33.000000 chelsa_cmip6-1.1/README.md
--rw-rw-r--   0 karger   (67351) karger   (69282)     1214 2022-10-31 09:40:40.000000 chelsa_cmip6-1.1/setup.py
--rw-r--r--   0 karger   (67351) karger   (69282)    34523 2022-07-26 10:03:28.000000 chelsa_cmip6-1.1/LICENSE
-drwxr-xr-x   0 karger   (67351) karger   (69282)        0 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/src/
-drwxr-xr-x   0 karger   (67351) karger   (69282)        0 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/src/chelsa_cmip6.egg-info/
--rw-r--r--   0 karger   (67351) karger   (69282)       13 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/src/chelsa_cmip6.egg-info/top_level.txt
--rw-r--r--   0 karger   (67351) karger   (69282)    15889 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/src/chelsa_cmip6.egg-info/PKG-INFO
--rw-r--r--   0 karger   (67351) karger   (69282)      372 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/src/chelsa_cmip6.egg-info/SOURCES.txt
--rw-r--r--   0 karger   (67351) karger   (69282)        1 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/src/chelsa_cmip6.egg-info/dependency_links.txt
--rw-r--r--   0 karger   (67351) karger   (69282)       46 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/src/chelsa_cmip6.egg-info/requires.txt
-drwxr-xr-x   0 karger   (67351) karger   (69282)        0 2022-10-31 09:41:47.000000 chelsa_cmip6-1.1/src/chelsa_cmip6/
--rw-rw-r--   0 karger   (67351) karger   (69282)     3642 2022-10-31 09:29:33.000000 chelsa_cmip6-1.1/src/chelsa_cmip6/run_chelsa_cmip6.py
--rw-rw-r--   0 karger   (67351) karger   (69282)    17879 2022-10-31 09:29:33.000000 chelsa_cmip6-1.1/src/chelsa_cmip6/GetClim.py
--rw-r--r--   0 karger   (67351) karger   (69282)        0 2021-10-06 09:18:55.000000 chelsa_cmip6-1.1/src/chelsa_cmip6/__init__.py
--rw-r--r--   0 karger   (67351) karger   (69282)    21661 2022-07-11 09:37:17.000000 chelsa_cmip6-1.1/src/chelsa_cmip6/BioClim.py
--rw-r--r--   0 karger   (67351) karger   (69282)      103 2021-10-06 09:18:55.000000 chelsa_cmip6-1.1/pyproject.toml
+drwxr-xr-x   0 karger   (67351) karger   (69282)        0 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/
+-rw-r--r--   0 karger   (67351) karger   (69282)    20379 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/PKG-INFO
+-rw-r--r--   0 karger   (67351) karger   (69282)      999 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/setup.cfg
+-rw-r--r--   0 karger   (67351) karger   (69282)    19322 2023-04-14 11:47:35.000000 chelsa_cmip6-1.2/README.md
+-rw-r--r--   0 karger   (67351) karger   (69282)     1285 2023-04-14 11:58:30.000000 chelsa_cmip6-1.2/setup.py
+-rw-r--r--   0 karger   (67351) karger   (69282)    34523 2022-07-26 10:03:28.000000 chelsa_cmip6-1.2/LICENSE
+drwxr-xr-x   0 karger   (67351) karger   (69282)        0 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/src/
+drwxr-xr-x   0 karger   (67351) karger   (69282)        0 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/src/chelsa_cmip6.egg-info/
+-rw-r--r--   0 karger   (67351) karger   (69282)       13 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/src/chelsa_cmip6.egg-info/top_level.txt
+-rw-r--r--   0 karger   (67351) karger   (69282)    20379 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/src/chelsa_cmip6.egg-info/PKG-INFO
+-rw-r--r--   0 karger   (67351) karger   (69282)      372 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/src/chelsa_cmip6.egg-info/SOURCES.txt
+-rw-r--r--   0 karger   (67351) karger   (69282)        1 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/src/chelsa_cmip6.egg-info/dependency_links.txt
+-rw-r--r--   0 karger   (67351) karger   (69282)       66 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/src/chelsa_cmip6.egg-info/requires.txt
+drwxr-xr-x   0 karger   (67351) karger   (69282)        0 2023-04-14 11:58:42.000000 chelsa_cmip6-1.2/src/chelsa_cmip6/
+-rw-rw-r--   0 karger   (67351) karger   (69282)     3642 2022-10-31 09:29:33.000000 chelsa_cmip6-1.2/src/chelsa_cmip6/run_chelsa_cmip6.py
+-rw-r--r--   0 karger   (67351) karger   (69282)    19342 2023-04-14 11:47:35.000000 chelsa_cmip6-1.2/src/chelsa_cmip6/GetClim.py
+-rw-r--r--   0 karger   (67351) karger   (69282)        0 2021-10-06 09:18:55.000000 chelsa_cmip6-1.2/src/chelsa_cmip6/__init__.py
+-rw-r--r--   0 karger   (67351) karger   (69282)    21661 2022-07-11 09:37:17.000000 chelsa_cmip6-1.2/src/chelsa_cmip6/BioClim.py
+-rw-r--r--   0 karger   (67351) karger   (69282)      103 2021-10-06 09:18:55.000000 chelsa_cmip6-1.2/pyproject.toml
```

### Comparing `chelsa_cmip6-1.1/PKG-INFO` & `chelsa_cmip6-1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: chelsa_cmip6
-Version: 1.1
+Version: 1.2
 Summary: This package contains function to create monthly high-resolution climatologies for a selected geographic area for min-, max-, and mean temperature, precipitation rate and bioclimatic variables from anomalies and using CHELSA V2.1 as baseline high resolution climatology. Only works for GCMs for which tas, tasmax, tasmin, and pr are available.
 Home-page: https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
 Author: Dirk Nikolaus Karger
 Author-email: dirk.karger@wsl.ch
 License: GNU
 Download-URL: https://gitlabext.wsl.ch/karger/chelsa_cmip6/-/archive/v1.0/chelsa_cmip6-v1.0.tar.gz
 Project-URL: Bug Tracker, https://github.com/pypa/chelsa_cmip6/issues
 Keywords: CMIP6,climate,delta-change,CHELSA,bioclimate,growing degree days,gdd,bio
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 chelsa_cmip6
 -----------
 This package contains functions to creates monthly high-resolution 
@@ -46,79 +46,82 @@
 2. To install from the default repositories, enter the following:
 ```bash
 sudo apt-get install git
 ```
 
 3. you can now install the latest version from github by typing the following command in the terminal:
 ```bash
-python -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
+python3 -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
 ```
 
 #### From PyPI:
 If you want the latest release version, you can also install it from PyPI using:
 
 using pip:
 ```bash
-python -m pip install chelsa-cmip6
+python3 -m pip install chelsa-cmip6
 ```
 ## On Windows
 #### Install python:
 1. Check if python is already installed on your machine. To do so open the command line interface by:
 Press: Win + R
 
 2. This will open a run window:
 Type: cmd.exe and press enter
 This should open the command line interface of Windows
 
 3. In the command line interface type:
 ```bash
-python
+python3
 ```
 If python is already installed, you will automatically enter the command line interpreter of python. If
 Python is not already installed, a Microsoft Store window will open asking you to install Python. Click 'Get'
 and install Python. Make sure your version is at least 3.8.
 
 4. Verify your installation by typing the following in the command line interface:
 ```bash
-python --version
+python3 --version
 ```
 
 #### Install the chelsa-cmip6 package:
 ##### Using pip
 If you want the latest release version, you can also install it from PyPI using:
 
 ```bash
-python -m pip install chelsa-cmip6
+python3 -m pip install chelsa-cmip6
 ```
 
 ##### Using Git
 If you want the latest version, you can also install it from Github. If you dont have Git
 installed on your machine, you can find the installers here: 
 https://git-scm.com/download/win
 
 Follow the steps in the installer and after completion open a new command line interface in windows and type:
 ```bash
-python -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
+python3 -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
 ```
 
-##### GDAL and rasterio
-chelsa-cmip6 depends on rasterio, which in turn depends on GDAL. Sometimes these two modules can create problems with the 
+##### GDAL and rasterio in chelsa-cmip6 V.1.0 & V1.1
+chelsa-cmip6 up to version  1.1. depends on rasterio, which in turn depends on GDAL. Sometimes these two modules can create problems with the 
 installation routine. If the installation hangs while installing the rasterio module, you can try installing both modules manually
 before installing chelsa-cmip6.
 
 GDAL can be quite complex to build and install, particularly on Windows and MacOS
 If you run into problems follow the steps provided for your respective system here:
 
 You can get information how to install GDAL on your system here: https://pypi.org/project/GDAL/
 
 After the manual installation of GDAL you can install rasterio by:
 ```bash
-python -m pip install rasterio
+python3 -m pip install rasterio
 ```
 
+starting V.1.2 chelsa-cmip6 does not rely on rasterio anymore, but uses byte wise connections to remote CHELSA
+data stored in netcdf files.
+
 # HOW TO USE
 ----------
 The chelsa_cmip6 module provides functions to create monthly climatologies from climate
 simulation data from CMIP6 using climate observation data from CHELSA V.2.1
 at a 0.0083333° grid resolution for a given area of choice.
 
 The GetClim module contains classes and functions to connect to CMIP6 data
@@ -140,27 +143,45 @@
 are available for both the reference and the future period.
 
 The standard reference period is 1981-01-01 - 2010-12-31. If another reference period is 
 chosen, the code conducts a delta change for this period as well. Best practice would be to 
 choose the standard reference period.
 
 
-EXAMPLE: 
+
+
+
+EXAMPLES: 
 ------------
 You can use the package in two ways 1. by importing the module in python, and 2. by using
 the run_chelsa_cmip6.py wrapper function in the terminal (Linux, MAC) or command prompt (Windows).
 
+Figure 1 gives an visual example of the different model parameters for Example 1. 
+
+
+![explanation of the delta change method](/figs/Fig1-1.png)*Example of the delta change method applied on the model MPI-ESM1-2-LR for ssp585, the reference period 1981-2010, and the future period 2041-2070 (Example 1). The MPI-ESM1-2-LP gives the low resolution reference period temperature tas_low^ref  and the low resolution future period temperature tas_low^fut. The difference between these two temperatures is interpolated to 30 arcsec resolution using a qubic-spline CS(Δtas_fut^ref) and then added to the high resolution reference temperature tas_high^ref to get tas_high^fut. The parameters that need to be set to achieve the shown delta change downscaling are shown in the upper left corner. Both tas_high^ref and tas_high^fut are given as output for a specific region that is specified using the arguments: --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 .*
+
+
+
+EXAMPLE 1: 
+------------
+
 To create future climate data within python, first import the main function by:
 
 ## Using python
 ------------
 ```python
 from chelsa_cmip6.GetClim import chelsa_cmip6
 ```
 
+Creating long term climatological normals and the related bioclimatic variables that are commonly used in species distribution modeling 
+is controlled via the fefps and fefpe parameters of the chelsa_cmip6 function. You can use function by running the following command 
+in python a python prompt. Open a python prompt by either typing python 
+in your terminal in Linux, or a command prompt in Windows.
+
 You can then set the parameters of the chelsa_cmip6 function to create the climate data for the CMIP6 model you want.
 If we want to create climatologies and bioclimatic variables for the model MPI-ESM1-2-LR and ssp585 for the years
 2041-2070 for the region between 5.3° - 10.4° longitude, and 46.0° - 47.5° latitude and save them in your home 
 directory (~/, on a linux system), we need to set the parameters of the function as follows: 
 ```python
 chelsa_cmip6(activity_id='ScenarioMIP', 
              table_id='Amon', 
@@ -181,41 +202,74 @@
 #### on Windows:
 If you are on a windows system the 'output' parameter should be in the form windows requires it, e.g.
 
 ```python
 output='C:/Users/your_user_name/' # the directory you want the output to be saved in 
 ```
 
+Important: Plese be aware that depending on the computer you use the function will only run if you have access to the internet, and it might take a considerable amount of time to finish as the data transfer needed is relativly large.
+
+
+EXAMPLE 2: 
+------------
+
+Creating a monthly timeseries for the same model requires only an adaptation of the fefps, and fefpe parameter 
+of the function. Here we show an example using a simple loop in python. The output will be a netCDF files for each 
+month from 2016, 2100 for tas, tasmax, tasmin, and pr, and an annual timeseries for the bioclimatic variables.
+```python
+for year in range(2016,2101):
+    chelsa_cmip6(activity_id='ScenarioMIP', 
+                 table_id='Amon', 
+                 experiment_id='ssp585', 
+                 institution_id='MPI-M', 
+                 source_id='MPI-ESM1-2-LR', 
+                 member_id='r1i1p1f1', 
+                 refps='1981-01-15', 
+                 refpe='2010-12-15', 
+                 fefps=str(year) + '-01-01', 
+                 fefpe=str(year) + '-12-31', 
+                 xmin=5.3, 
+                 xmax=10.4,
+                 ymin=46.0, 
+                 ymax=47.5,
+                 output='~/')
+```
+
+
 ## Use chelsa_cmip6 without using python directly
 ------------
 You can also use the function directly from the terminal if you like. The chelsa_cmip6 package comes with a wrapper function,
 run_chelsa_cmip6.py that allows you to simply use it via the terminal without any python knowledge required. It means however that you have to add directory where the wrapper function run_chelsa_cmip6.py is located to your PATH variable, so that your system knows where to look for it. 
 
 #### on Linux
 1. Find the directory in which chelsa_cmip6 is located by typing the following in the terminal:
 ```bash
-python -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
+python3 -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
 ```
 The printed path without the '\__init__.py' at the end is the path you will need to add to your PATH variable.
 
 2. You can now add it to your PATH variable by using:
 ```bash
 export PATH="your_path:$PATH"
 ```
 
 3. Restart your terminal. You should now be able to use chelsa_cmip6 by running e.g. the following in the terminal:
 ```bash 
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "~/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "~/"
 ```
 
 #### on Windows
 On Windows you need to first find out where the python package is installed. You can do so by typing the following in the command line interface:
 
 ```bash
-python -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
+python3 -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
 ```
 
 The printed path without the '\__init__.py' at the end is the path you will need to add to your path variable. On my machine it 
 looks like this:
 
 ```bash 
 C:\Users\Administrator\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.10_qbz5n2kfra8p0\LocalCache\local-packages\Python310\site-packages\chelsa_cmip6\__init__.py
@@ -228,56 +282,89 @@
 
 4. Type the following in the command prompt, replacing C:\your\path\here with the your local path
 ```bash 
 setx /M path "%path%;C:\your\path\here"
 ```
 5. Close the command prompt and open a new one. You now should be able to run the the function now by e.g. typing:
 ```bash 
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "C:/Users/<your_user_name>/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "C:/Users/<your_user_name>/"
 ```
 
 ```bash
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "~/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "~/"
 ```
 
 important is that the combination of activity_id 'ScenarioMIP' and e.g. experiment_id 'ssp585' is set to a combination that exists.
 You can also get historical data but in that case, activity_ID, experiment_id, and fefps and fefps need to be changed. E.g. 
 
 ```bash
-run_chelsa_cmip6.py --activity_id "CMIP" --table_id "Amon" --experiment_id "historical" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "1851-01-15" --fefpe "1880-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '~/'
+run_chelsa_cmip6.py --activity_id "CMIP" --table_id "Amon" \
+--experiment_id "historical" --institution_id "MPI-M" \
+--source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" \
+--refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "1851-01-15" --fefpe "1880-12-15" \
+--xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '~/'
 ```
 
 it is also important that your fefps and fefpe are covered by the experiment_id and activity_id.
 
 These reference periods are possible for example:
 
 'ScenarioMIP' - 2016-01-01 - 2100-12-31
 
 'CMIP' - 1850-01-01 - 2015-12-31
 
 refps and refpe need to be in the range 1850-01-01 - 2015-12-31.
 
 ## chelsa_cmip6 in R via the reticulate package
 ------------
-You can also use the chelsa_cmip6 package in R if you want to itegrate it into your R workflow. To do so open an R console or R Studio and follow the steps below. Important: You still need to have python and the chelsa_cmip6 package installed (see instructions above).
+You can also use the chelsa_cmip6 package in R if you want to integrate it into your R workflow. To do so open an R console or R Studio and follow the steps below. Important: You still need to have python and the chelsa_cmip6 package installed (see instructions above).
+Tested with R 4.2.1 in Windows 10
 
 Install and load the reticulate package
 ```R
 install.packages("reticulate",dependencies = TRUE)
 library(reticulate)
 ```
 
+Install and load the chelsa-cmip6 package
+```R
+py_install("chelsa-cmip6", pip=T)
+```
+
 The import() function enables you to import the chelsa_cmip6 module and call it’s functions directly from R.
 ```R
 chelsa_cmip6 <- import('chelsa_cmip6')
 ```
 
-You can then use the chelsa_cmip6 function in R the same you would in python.
+You can then use the chelsa_cmip6 function in R the same you would in python. Be aware that the function might run for a while before it creates any output.
 ```R
-
+chelsa_cmip6$GetClim$chelsa_cmip6(activity_id='ScenarioMIP', 
+                                  table_id='Amon', 
+                                  experiment_id='ssp585', 
+                                  institution_id='MPI-M', 
+                                  source_id='MPI-ESM1-2-LR', 
+                                  member_id='r1i1p1f1', 
+                                  refps='1981-01-15', 
+                                  refpe='2010-12-15', 
+                                  fefps='2041-01-15', 
+                                  fefpe='2070-12-15', 
+                                  xmin=5.3, 
+                                  xmax=10.4,
+                                  ymin=46.0, 
+                                  ymax=47.5,
+                                  output='~/')
 ```
 
 
 # REQUIREMENTS
 ------------
 chelsa_cmip6 is written in Python 3. It has been tested to run well with the
 following Python release and package versions. The dependencies will be installed automatically.
@@ -287,25 +374,37 @@
 - numpy 1.19.5
 - rasterio 1.2.1
 - pandas 1.1.5
 - zarr 2.6.1
 - gcsfs 0.7.2
 - datetime 3.9.2
 - scipy 0.19.1
+- fsspec
+- dask
+- netcdf4
+- h5netcdf
+
 
 
 ## SINGULARITY
 ------------
 All dependencies are also resolved in the singularity container '/singularity/chelsa_cmip6.sif'. Singularity needs to be installed on the respective linux system you are using. 
 An installation guide can be found here: https://sylabs.io/guides/3.3/user-guide/quick_start.html#quick-installation-steps
 
+The singularity container is available only here: https://gitlabext.wsl.ch/karger/chelsa_cmip6/-/blob/master/singularity/chelsa_cmip6.sif
+
 If you use chelsa_cmip6 together with singularity the command should be slightly modified:
 
 ```bash
-singularity exec /singularity/chelsa_cmip6.sif python3 chelsa_cmip6.py --activity_id 'CMIP' --table_id 'Amon' --experiment_id 'historical' --institution_id 'MPI-M' --source_id 'MPI-ESM1-2-LR' --member_id 'r1i1p1f1' --refps '1981-01-15' --refpe '2010-12-15' --fefps '1851-01-15' --fefpe '1880-12-15' --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '/home/karger/scratch/'
+singularity exec /singularity/chelsa_cmip6.sif python3 chelsa_cmip6.py \
+--activity_id 'CMIP' --table_id 'Amon' --experiment_id 'historical' \
+--institution_id 'MPI-M' --source_id 'MPI-ESM1-2-LR' --member_id 'r1i1p1f1' \
+--refps '1981-01-15' --refpe '2010-12-15' --fefps '1851-01-15' \
+--fefpe '1880-12-15' --xmin 5.3 --xmax 10.4 --ymin 46.0 \
+--ymax 47.5 --output '/home/karger/scratch/'
 ```
 
 tested with singularity version 3.3.0-809.g78ec427cc
 but newer versions usually work as well.
 
 
 ## CHECKING IF ALL NEEDED INPUT IS AVAILABLE
@@ -330,14 +429,22 @@
 ------------
 The output consist of netCDF4 files. There will be different files for each variable and seperatly for
 the reference (refps - refpe) and the future period (fefps - fefpe). 
 Additionally, there will be netCDF4 files for the 
 different bioclimatic variables each for both the reference (refps - refpe) and the future period (fefps - fefpe). 
 
 
+##  CAVEATS
+------------
+Important: 
+1. Please be aware that depending on the computer you use the function will only run if you have access to the internet. 
+2. It might take a considerable amount of time to finish as the data transfer needed is relativly large.
+3. You will need a considerable amount of RAM depending on the geographical size you choose. The example given runs with 16 GB of RAM. Below that we cannot garantee that the function will succeed.
+
+
 # COPYRIGHT
 ---------
 (C) 2022 Dirk Nikolaus Karger
 
 
 # LICENSE
 -------
```

### Comparing `chelsa_cmip6-1.1/setup.cfg` & `chelsa_cmip6-1.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chelsa_cmip6
-version = 1.1
+version = 1.2
 author = Dirk Nikolaus Karger
 author_email = dirk.karger@wsl.ch
 description = This package contains function to create monthly high-resolution climatologies
 	for a selected geographic area for min-, max-, and mean temperature, precipitation rate
 	and bioclimatic variables from anomalies and using CHELSA V2.1 as
 	baseline high resolution climatology. Only works for GCMs for
 	which tas, tasmax, tasmin, and pr are available.
```

### Comparing `chelsa_cmip6-1.1/README.md` & `chelsa_cmip6-1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,79 +27,82 @@
 2. To install from the default repositories, enter the following:
 ```bash
 sudo apt-get install git
 ```
 
 3. you can now install the latest version from github by typing the following command in the terminal:
 ```bash
-python -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
+python3 -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
 ```
 
 #### From PyPI:
 If you want the latest release version, you can also install it from PyPI using:
 
 using pip:
 ```bash
-python -m pip install chelsa-cmip6
+python3 -m pip install chelsa-cmip6
 ```
 ## On Windows
 #### Install python:
 1. Check if python is already installed on your machine. To do so open the command line interface by:
 Press: Win + R
 
 2. This will open a run window:
 Type: cmd.exe and press enter
 This should open the command line interface of Windows
 
 3. In the command line interface type:
 ```bash
-python
+python3
 ```
 If python is already installed, you will automatically enter the command line interpreter of python. If
 Python is not already installed, a Microsoft Store window will open asking you to install Python. Click 'Get'
 and install Python. Make sure your version is at least 3.8.
 
 4. Verify your installation by typing the following in the command line interface:
 ```bash
-python --version
+python3 --version
 ```
 
 #### Install the chelsa-cmip6 package:
 ##### Using pip
 If you want the latest release version, you can also install it from PyPI using:
 
 ```bash
-python -m pip install chelsa-cmip6
+python3 -m pip install chelsa-cmip6
 ```
 
 ##### Using Git
 If you want the latest version, you can also install it from Github. If you dont have Git
 installed on your machine, you can find the installers here: 
 https://git-scm.com/download/win
 
 Follow the steps in the installer and after completion open a new command line interface in windows and type:
 ```bash
-python -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
+python3 -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
 ```
 
-##### GDAL and rasterio
-chelsa-cmip6 depends on rasterio, which in turn depends on GDAL. Sometimes these two modules can create problems with the 
+##### GDAL and rasterio in chelsa-cmip6 V.1.0 & V1.1
+chelsa-cmip6 up to version  1.1. depends on rasterio, which in turn depends on GDAL. Sometimes these two modules can create problems with the 
 installation routine. If the installation hangs while installing the rasterio module, you can try installing both modules manually
 before installing chelsa-cmip6.
 
 GDAL can be quite complex to build and install, particularly on Windows and MacOS
 If you run into problems follow the steps provided for your respective system here:
 
 You can get information how to install GDAL on your system here: https://pypi.org/project/GDAL/
 
 After the manual installation of GDAL you can install rasterio by:
 ```bash
-python -m pip install rasterio
+python3 -m pip install rasterio
 ```
 
+starting V.1.2 chelsa-cmip6 does not rely on rasterio anymore, but uses byte wise connections to remote CHELSA
+data stored in netcdf files.
+
 # HOW TO USE
 ----------
 The chelsa_cmip6 module provides functions to create monthly climatologies from climate
 simulation data from CMIP6 using climate observation data from CHELSA V.2.1
 at a 0.0083333° grid resolution for a given area of choice.
 
 The GetClim module contains classes and functions to connect to CMIP6 data
@@ -121,27 +124,45 @@
 are available for both the reference and the future period.
 
 The standard reference period is 1981-01-01 - 2010-12-31. If another reference period is 
 chosen, the code conducts a delta change for this period as well. Best practice would be to 
 choose the standard reference period.
 
 
-EXAMPLE: 
+
+
+
+EXAMPLES: 
 ------------
 You can use the package in two ways 1. by importing the module in python, and 2. by using
 the run_chelsa_cmip6.py wrapper function in the terminal (Linux, MAC) or command prompt (Windows).
 
+Figure 1 gives an visual example of the different model parameters for Example 1. 
+
+
+![explanation of the delta change method](/figs/Fig1-1.png)*Example of the delta change method applied on the model MPI-ESM1-2-LR for ssp585, the reference period 1981-2010, and the future period 2041-2070 (Example 1). The MPI-ESM1-2-LP gives the low resolution reference period temperature tas_low^ref  and the low resolution future period temperature tas_low^fut. The difference between these two temperatures is interpolated to 30 arcsec resolution using a qubic-spline CS(Δtas_fut^ref) and then added to the high resolution reference temperature tas_high^ref to get tas_high^fut. The parameters that need to be set to achieve the shown delta change downscaling are shown in the upper left corner. Both tas_high^ref and tas_high^fut are given as output for a specific region that is specified using the arguments: --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 .*
+
+
+
+EXAMPLE 1: 
+------------
+
 To create future climate data within python, first import the main function by:
 
 ## Using python
 ------------
 ```python
 from chelsa_cmip6.GetClim import chelsa_cmip6
 ```
 
+Creating long term climatological normals and the related bioclimatic variables that are commonly used in species distribution modeling 
+is controlled via the fefps and fefpe parameters of the chelsa_cmip6 function. You can use function by running the following command 
+in python a python prompt. Open a python prompt by either typing python 
+in your terminal in Linux, or a command prompt in Windows.
+
 You can then set the parameters of the chelsa_cmip6 function to create the climate data for the CMIP6 model you want.
 If we want to create climatologies and bioclimatic variables for the model MPI-ESM1-2-LR and ssp585 for the years
 2041-2070 for the region between 5.3° - 10.4° longitude, and 46.0° - 47.5° latitude and save them in your home 
 directory (~/, on a linux system), we need to set the parameters of the function as follows: 
 ```python
 chelsa_cmip6(activity_id='ScenarioMIP', 
              table_id='Amon', 
@@ -162,41 +183,74 @@
 #### on Windows:
 If you are on a windows system the 'output' parameter should be in the form windows requires it, e.g.
 
 ```python
 output='C:/Users/your_user_name/' # the directory you want the output to be saved in 
 ```
 
+Important: Plese be aware that depending on the computer you use the function will only run if you have access to the internet, and it might take a considerable amount of time to finish as the data transfer needed is relativly large.
+
+
+EXAMPLE 2: 
+------------
+
+Creating a monthly timeseries for the same model requires only an adaptation of the fefps, and fefpe parameter 
+of the function. Here we show an example using a simple loop in python. The output will be a netCDF files for each 
+month from 2016, 2100 for tas, tasmax, tasmin, and pr, and an annual timeseries for the bioclimatic variables.
+```python
+for year in range(2016,2101):
+    chelsa_cmip6(activity_id='ScenarioMIP', 
+                 table_id='Amon', 
+                 experiment_id='ssp585', 
+                 institution_id='MPI-M', 
+                 source_id='MPI-ESM1-2-LR', 
+                 member_id='r1i1p1f1', 
+                 refps='1981-01-15', 
+                 refpe='2010-12-15', 
+                 fefps=str(year) + '-01-01', 
+                 fefpe=str(year) + '-12-31', 
+                 xmin=5.3, 
+                 xmax=10.4,
+                 ymin=46.0, 
+                 ymax=47.5,
+                 output='~/')
+```
+
+
 ## Use chelsa_cmip6 without using python directly
 ------------
 You can also use the function directly from the terminal if you like. The chelsa_cmip6 package comes with a wrapper function,
 run_chelsa_cmip6.py that allows you to simply use it via the terminal without any python knowledge required. It means however that you have to add directory where the wrapper function run_chelsa_cmip6.py is located to your PATH variable, so that your system knows where to look for it. 
 
 #### on Linux
 1. Find the directory in which chelsa_cmip6 is located by typing the following in the terminal:
 ```bash
-python -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
+python3 -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
 ```
 The printed path without the '\__init__.py' at the end is the path you will need to add to your PATH variable.
 
 2. You can now add it to your PATH variable by using:
 ```bash
 export PATH="your_path:$PATH"
 ```
 
 3. Restart your terminal. You should now be able to use chelsa_cmip6 by running e.g. the following in the terminal:
 ```bash 
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "~/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "~/"
 ```
 
 #### on Windows
 On Windows you need to first find out where the python package is installed. You can do so by typing the following in the command line interface:
 
 ```bash
-python -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
+python3 -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
 ```
 
 The printed path without the '\__init__.py' at the end is the path you will need to add to your path variable. On my machine it 
 looks like this:
 
 ```bash 
 C:\Users\Administrator\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.10_qbz5n2kfra8p0\LocalCache\local-packages\Python310\site-packages\chelsa_cmip6\__init__.py
@@ -209,56 +263,89 @@
 
 4. Type the following in the command prompt, replacing C:\your\path\here with the your local path
 ```bash 
 setx /M path "%path%;C:\your\path\here"
 ```
 5. Close the command prompt and open a new one. You now should be able to run the the function now by e.g. typing:
 ```bash 
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "C:/Users/<your_user_name>/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "C:/Users/<your_user_name>/"
 ```
 
 ```bash
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "~/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "~/"
 ```
 
 important is that the combination of activity_id 'ScenarioMIP' and e.g. experiment_id 'ssp585' is set to a combination that exists.
 You can also get historical data but in that case, activity_ID, experiment_id, and fefps and fefps need to be changed. E.g. 
 
 ```bash
-run_chelsa_cmip6.py --activity_id "CMIP" --table_id "Amon" --experiment_id "historical" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "1851-01-15" --fefpe "1880-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '~/'
+run_chelsa_cmip6.py --activity_id "CMIP" --table_id "Amon" \
+--experiment_id "historical" --institution_id "MPI-M" \
+--source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" \
+--refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "1851-01-15" --fefpe "1880-12-15" \
+--xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '~/'
 ```
 
 it is also important that your fefps and fefpe are covered by the experiment_id and activity_id.
 
 These reference periods are possible for example:
 
 'ScenarioMIP' - 2016-01-01 - 2100-12-31
 
 'CMIP' - 1850-01-01 - 2015-12-31
 
 refps and refpe need to be in the range 1850-01-01 - 2015-12-31.
 
 ## chelsa_cmip6 in R via the reticulate package
 ------------
-You can also use the chelsa_cmip6 package in R if you want to itegrate it into your R workflow. To do so open an R console or R Studio and follow the steps below. Important: You still need to have python and the chelsa_cmip6 package installed (see instructions above).
+You can also use the chelsa_cmip6 package in R if you want to integrate it into your R workflow. To do so open an R console or R Studio and follow the steps below. Important: You still need to have python and the chelsa_cmip6 package installed (see instructions above).
+Tested with R 4.2.1 in Windows 10
 
 Install and load the reticulate package
 ```R
 install.packages("reticulate",dependencies = TRUE)
 library(reticulate)
 ```
 
+Install and load the chelsa-cmip6 package
+```R
+py_install("chelsa-cmip6", pip=T)
+```
+
 The import() function enables you to import the chelsa_cmip6 module and call it’s functions directly from R.
 ```R
 chelsa_cmip6 <- import('chelsa_cmip6')
 ```
 
-You can then use the chelsa_cmip6 function in R the same you would in python.
+You can then use the chelsa_cmip6 function in R the same you would in python. Be aware that the function might run for a while before it creates any output.
 ```R
-
+chelsa_cmip6$GetClim$chelsa_cmip6(activity_id='ScenarioMIP', 
+                                  table_id='Amon', 
+                                  experiment_id='ssp585', 
+                                  institution_id='MPI-M', 
+                                  source_id='MPI-ESM1-2-LR', 
+                                  member_id='r1i1p1f1', 
+                                  refps='1981-01-15', 
+                                  refpe='2010-12-15', 
+                                  fefps='2041-01-15', 
+                                  fefpe='2070-12-15', 
+                                  xmin=5.3, 
+                                  xmax=10.4,
+                                  ymin=46.0, 
+                                  ymax=47.5,
+                                  output='~/')
 ```
 
 
 # REQUIREMENTS
 ------------
 chelsa_cmip6 is written in Python 3. It has been tested to run well with the
 following Python release and package versions. The dependencies will be installed automatically.
@@ -268,25 +355,37 @@
 - numpy 1.19.5
 - rasterio 1.2.1
 - pandas 1.1.5
 - zarr 2.6.1
 - gcsfs 0.7.2
 - datetime 3.9.2
 - scipy 0.19.1
+- fsspec
+- dask
+- netcdf4
+- h5netcdf
+
 
 
 ## SINGULARITY
 ------------
 All dependencies are also resolved in the singularity container '/singularity/chelsa_cmip6.sif'. Singularity needs to be installed on the respective linux system you are using. 
 An installation guide can be found here: https://sylabs.io/guides/3.3/user-guide/quick_start.html#quick-installation-steps
 
+The singularity container is available only here: https://gitlabext.wsl.ch/karger/chelsa_cmip6/-/blob/master/singularity/chelsa_cmip6.sif
+
 If you use chelsa_cmip6 together with singularity the command should be slightly modified:
 
 ```bash
-singularity exec /singularity/chelsa_cmip6.sif python3 chelsa_cmip6.py --activity_id 'CMIP' --table_id 'Amon' --experiment_id 'historical' --institution_id 'MPI-M' --source_id 'MPI-ESM1-2-LR' --member_id 'r1i1p1f1' --refps '1981-01-15' --refpe '2010-12-15' --fefps '1851-01-15' --fefpe '1880-12-15' --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '/home/karger/scratch/'
+singularity exec /singularity/chelsa_cmip6.sif python3 chelsa_cmip6.py \
+--activity_id 'CMIP' --table_id 'Amon' --experiment_id 'historical' \
+--institution_id 'MPI-M' --source_id 'MPI-ESM1-2-LR' --member_id 'r1i1p1f1' \
+--refps '1981-01-15' --refpe '2010-12-15' --fefps '1851-01-15' \
+--fefpe '1880-12-15' --xmin 5.3 --xmax 10.4 --ymin 46.0 \
+--ymax 47.5 --output '/home/karger/scratch/'
 ```
 
 tested with singularity version 3.3.0-809.g78ec427cc
 but newer versions usually work as well.
 
 
 ## CHECKING IF ALL NEEDED INPUT IS AVAILABLE
@@ -311,14 +410,22 @@
 ------------
 The output consist of netCDF4 files. There will be different files for each variable and seperatly for
 the reference (refps - refpe) and the future period (fefps - fefpe). 
 Additionally, there will be netCDF4 files for the 
 different bioclimatic variables each for both the reference (refps - refpe) and the future period (fefps - fefpe). 
 
 
+##  CAVEATS
+------------
+Important: 
+1. Please be aware that depending on the computer you use the function will only run if you have access to the internet. 
+2. It might take a considerable amount of time to finish as the data transfer needed is relativly large.
+3. You will need a considerable amount of RAM depending on the geographical size you choose. The example given runs with 16 GB of RAM. Below that we cannot garantee that the function will succeed.
+
+
 # COPYRIGHT
 ---------
 (C) 2022 Dirk Nikolaus Karger
 
 
 # LICENSE
 -------
```

### Comparing `chelsa_cmip6-1.1/setup.py` & `chelsa_cmip6-1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from distutils.core import setup
 setup(
   name = 'chelsa_cmip6',         
   packages = ['chelsa_cmip6'],  
-  version = '1.1',
+  version = '1.2',
   license='GNU',
   description = "This package contains function to create monthly high-resolution climatologies for a selected geographic area for min-, max-, and mean temperature, precipitation rate and bioclimatic variables from anomalies and using CHELSA V2.1 as baseline high resolution climatology. Only works for GCMs for which tas, tasmax, tasmin, and pr are available.", 
   author = 'Dirk Nikolaus Karger',                  
   author_email = 'dirk.karger@wsl.ch',     
   url = 'https://gitlabext.wsl.ch/karger/chelsa_cmip6.git',
   download_url = 'https://gitlabext.wsl.ch/karger/chelsa_cmip6/-/archive/v1.0/chelsa_cmip6-v1.0.tar.gz', 
   keywords = ['CMIP6', 'climate', 'delta-change', 'CHELSA', 'bioclimate', 'growing degree days', 'gdd', 'bio'],  
   install_requires=[
           'numpy',
           'xarray',
-          'rasterio',
           'pandas',
           'zarr',
           'gcsfs',
-          'scipy'
+          'scipy',
+          'fsspec',
+          'dask',
+          'netcdf4',
+          'h5netcdf'
       ],
   classifiers=[
-    'Development Status :: 3 - Alpha',      
-    'Intended Audience :: Developers',      
-    'Topic :: Software Development :: Build Tools'
+    'Development Status :: 5 - Production/Stable',      
+    'Intended Audience :: Science/Research',      
+    'Topic :: Scientific/Engineering :: GIS'
   ],
 )
```

### Comparing `chelsa_cmip6-1.1/LICENSE` & `chelsa_cmip6-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chelsa_cmip6-1.1/src/chelsa_cmip6.egg-info/PKG-INFO` & `chelsa_cmip6-1.2/src/chelsa_cmip6.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: chelsa-cmip6
-Version: 1.1
+Version: 1.2
 Summary: This package contains function to create monthly high-resolution climatologies for a selected geographic area for min-, max-, and mean temperature, precipitation rate and bioclimatic variables from anomalies and using CHELSA V2.1 as baseline high resolution climatology. Only works for GCMs for which tas, tasmax, tasmin, and pr are available.
 Home-page: https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
 Author: Dirk Nikolaus Karger
 Author-email: dirk.karger@wsl.ch
 License: GNU
 Download-URL: https://gitlabext.wsl.ch/karger/chelsa_cmip6/-/archive/v1.0/chelsa_cmip6-v1.0.tar.gz
 Project-URL: Bug Tracker, https://github.com/pypa/chelsa_cmip6/issues
 Keywords: CMIP6,climate,delta-change,CHELSA,bioclimate,growing degree days,gdd,bio
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 chelsa_cmip6
 -----------
 This package contains functions to creates monthly high-resolution 
@@ -46,79 +46,82 @@
 2. To install from the default repositories, enter the following:
 ```bash
 sudo apt-get install git
 ```
 
 3. you can now install the latest version from github by typing the following command in the terminal:
 ```bash
-python -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
+python3 -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
 ```
 
 #### From PyPI:
 If you want the latest release version, you can also install it from PyPI using:
 
 using pip:
 ```bash
-python -m pip install chelsa-cmip6
+python3 -m pip install chelsa-cmip6
 ```
 ## On Windows
 #### Install python:
 1. Check if python is already installed on your machine. To do so open the command line interface by:
 Press: Win + R
 
 2. This will open a run window:
 Type: cmd.exe and press enter
 This should open the command line interface of Windows
 
 3. In the command line interface type:
 ```bash
-python
+python3
 ```
 If python is already installed, you will automatically enter the command line interpreter of python. If
 Python is not already installed, a Microsoft Store window will open asking you to install Python. Click 'Get'
 and install Python. Make sure your version is at least 3.8.
 
 4. Verify your installation by typing the following in the command line interface:
 ```bash
-python --version
+python3 --version
 ```
 
 #### Install the chelsa-cmip6 package:
 ##### Using pip
 If you want the latest release version, you can also install it from PyPI using:
 
 ```bash
-python -m pip install chelsa-cmip6
+python3 -m pip install chelsa-cmip6
 ```
 
 ##### Using Git
 If you want the latest version, you can also install it from Github. If you dont have Git
 installed on your machine, you can find the installers here: 
 https://git-scm.com/download/win
 
 Follow the steps in the installer and after completion open a new command line interface in windows and type:
 ```bash
-python -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
+python3 -m pip install git+https://gitlabext.wsl.ch/karger/chelsa_cmip6.git
 ```
 
-##### GDAL and rasterio
-chelsa-cmip6 depends on rasterio, which in turn depends on GDAL. Sometimes these two modules can create problems with the 
+##### GDAL and rasterio in chelsa-cmip6 V.1.0 & V1.1
+chelsa-cmip6 up to version  1.1. depends on rasterio, which in turn depends on GDAL. Sometimes these two modules can create problems with the 
 installation routine. If the installation hangs while installing the rasterio module, you can try installing both modules manually
 before installing chelsa-cmip6.
 
 GDAL can be quite complex to build and install, particularly on Windows and MacOS
 If you run into problems follow the steps provided for your respective system here:
 
 You can get information how to install GDAL on your system here: https://pypi.org/project/GDAL/
 
 After the manual installation of GDAL you can install rasterio by:
 ```bash
-python -m pip install rasterio
+python3 -m pip install rasterio
 ```
 
+starting V.1.2 chelsa-cmip6 does not rely on rasterio anymore, but uses byte wise connections to remote CHELSA
+data stored in netcdf files.
+
 # HOW TO USE
 ----------
 The chelsa_cmip6 module provides functions to create monthly climatologies from climate
 simulation data from CMIP6 using climate observation data from CHELSA V.2.1
 at a 0.0083333° grid resolution for a given area of choice.
 
 The GetClim module contains classes and functions to connect to CMIP6 data
@@ -140,27 +143,45 @@
 are available for both the reference and the future period.
 
 The standard reference period is 1981-01-01 - 2010-12-31. If another reference period is 
 chosen, the code conducts a delta change for this period as well. Best practice would be to 
 choose the standard reference period.
 
 
-EXAMPLE: 
+
+
+
+EXAMPLES: 
 ------------
 You can use the package in two ways 1. by importing the module in python, and 2. by using
 the run_chelsa_cmip6.py wrapper function in the terminal (Linux, MAC) or command prompt (Windows).
 
+Figure 1 gives an visual example of the different model parameters for Example 1. 
+
+
+![explanation of the delta change method](/figs/Fig1-1.png)*Example of the delta change method applied on the model MPI-ESM1-2-LR for ssp585, the reference period 1981-2010, and the future period 2041-2070 (Example 1). The MPI-ESM1-2-LP gives the low resolution reference period temperature tas_low^ref  and the low resolution future period temperature tas_low^fut. The difference between these two temperatures is interpolated to 30 arcsec resolution using a qubic-spline CS(Δtas_fut^ref) and then added to the high resolution reference temperature tas_high^ref to get tas_high^fut. The parameters that need to be set to achieve the shown delta change downscaling are shown in the upper left corner. Both tas_high^ref and tas_high^fut are given as output for a specific region that is specified using the arguments: --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 .*
+
+
+
+EXAMPLE 1: 
+------------
+
 To create future climate data within python, first import the main function by:
 
 ## Using python
 ------------
 ```python
 from chelsa_cmip6.GetClim import chelsa_cmip6
 ```
 
+Creating long term climatological normals and the related bioclimatic variables that are commonly used in species distribution modeling 
+is controlled via the fefps and fefpe parameters of the chelsa_cmip6 function. You can use function by running the following command 
+in python a python prompt. Open a python prompt by either typing python 
+in your terminal in Linux, or a command prompt in Windows.
+
 You can then set the parameters of the chelsa_cmip6 function to create the climate data for the CMIP6 model you want.
 If we want to create climatologies and bioclimatic variables for the model MPI-ESM1-2-LR and ssp585 for the years
 2041-2070 for the region between 5.3° - 10.4° longitude, and 46.0° - 47.5° latitude and save them in your home 
 directory (~/, on a linux system), we need to set the parameters of the function as follows: 
 ```python
 chelsa_cmip6(activity_id='ScenarioMIP', 
              table_id='Amon', 
@@ -181,41 +202,74 @@
 #### on Windows:
 If you are on a windows system the 'output' parameter should be in the form windows requires it, e.g.
 
 ```python
 output='C:/Users/your_user_name/' # the directory you want the output to be saved in 
 ```
 
+Important: Plese be aware that depending on the computer you use the function will only run if you have access to the internet, and it might take a considerable amount of time to finish as the data transfer needed is relativly large.
+
+
+EXAMPLE 2: 
+------------
+
+Creating a monthly timeseries for the same model requires only an adaptation of the fefps, and fefpe parameter 
+of the function. Here we show an example using a simple loop in python. The output will be a netCDF files for each 
+month from 2016, 2100 for tas, tasmax, tasmin, and pr, and an annual timeseries for the bioclimatic variables.
+```python
+for year in range(2016,2101):
+    chelsa_cmip6(activity_id='ScenarioMIP', 
+                 table_id='Amon', 
+                 experiment_id='ssp585', 
+                 institution_id='MPI-M', 
+                 source_id='MPI-ESM1-2-LR', 
+                 member_id='r1i1p1f1', 
+                 refps='1981-01-15', 
+                 refpe='2010-12-15', 
+                 fefps=str(year) + '-01-01', 
+                 fefpe=str(year) + '-12-31', 
+                 xmin=5.3, 
+                 xmax=10.4,
+                 ymin=46.0, 
+                 ymax=47.5,
+                 output='~/')
+```
+
+
 ## Use chelsa_cmip6 without using python directly
 ------------
 You can also use the function directly from the terminal if you like. The chelsa_cmip6 package comes with a wrapper function,
 run_chelsa_cmip6.py that allows you to simply use it via the terminal without any python knowledge required. It means however that you have to add directory where the wrapper function run_chelsa_cmip6.py is located to your PATH variable, so that your system knows where to look for it. 
 
 #### on Linux
 1. Find the directory in which chelsa_cmip6 is located by typing the following in the terminal:
 ```bash
-python -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
+python3 -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
 ```
 The printed path without the '\__init__.py' at the end is the path you will need to add to your PATH variable.
 
 2. You can now add it to your PATH variable by using:
 ```bash
 export PATH="your_path:$PATH"
 ```
 
 3. Restart your terminal. You should now be able to use chelsa_cmip6 by running e.g. the following in the terminal:
 ```bash 
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "~/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "~/"
 ```
 
 #### on Windows
 On Windows you need to first find out where the python package is installed. You can do so by typing the following in the command line interface:
 
 ```bash
-python -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
+python3 -c "import chelsa_cmip6; print(chelsa_cmip6.__file__);"
 ```
 
 The printed path without the '\__init__.py' at the end is the path you will need to add to your path variable. On my machine it 
 looks like this:
 
 ```bash 
 C:\Users\Administrator\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.10_qbz5n2kfra8p0\LocalCache\local-packages\Python310\site-packages\chelsa_cmip6\__init__.py
@@ -228,56 +282,89 @@
 
 4. Type the following in the command prompt, replacing C:\your\path\here with the your local path
 ```bash 
 setx /M path "%path%;C:\your\path\here"
 ```
 5. Close the command prompt and open a new one. You now should be able to run the the function now by e.g. typing:
 ```bash 
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "C:/Users/<your_user_name>/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "C:/Users/<your_user_name>/"
 ```
 
 ```bash
-run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" --experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output "~/"
+run_chelsa_cmip6.py --activity_id "ScenarioMIP" --table_id "Amon" \
+--experiment_id "ssp585" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" \
+--member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "2041-01-15" --fefpe "2070-12-15" --xmin 5.3 --xmax 10.4 \
+--ymin 46.0 --ymax 47.5 --output "~/"
 ```
 
 important is that the combination of activity_id 'ScenarioMIP' and e.g. experiment_id 'ssp585' is set to a combination that exists.
 You can also get historical data but in that case, activity_ID, experiment_id, and fefps and fefps need to be changed. E.g. 
 
 ```bash
-run_chelsa_cmip6.py --activity_id "CMIP" --table_id "Amon" --experiment_id "historical" --institution_id "MPI-M" --source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" --refps "1981-01-15" --refpe "2010-12-15" --fefps "1851-01-15" --fefpe "1880-12-15" --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '~/'
+run_chelsa_cmip6.py --activity_id "CMIP" --table_id "Amon" \
+--experiment_id "historical" --institution_id "MPI-M" \
+--source_id "MPI-ESM1-2-LR" --member_id "r1i1p1f1" \
+--refps "1981-01-15" --refpe "2010-12-15" \
+--fefps "1851-01-15" --fefpe "1880-12-15" \
+--xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '~/'
 ```
 
 it is also important that your fefps and fefpe are covered by the experiment_id and activity_id.
 
 These reference periods are possible for example:
 
 'ScenarioMIP' - 2016-01-01 - 2100-12-31
 
 'CMIP' - 1850-01-01 - 2015-12-31
 
 refps and refpe need to be in the range 1850-01-01 - 2015-12-31.
 
 ## chelsa_cmip6 in R via the reticulate package
 ------------
-You can also use the chelsa_cmip6 package in R if you want to itegrate it into your R workflow. To do so open an R console or R Studio and follow the steps below. Important: You still need to have python and the chelsa_cmip6 package installed (see instructions above).
+You can also use the chelsa_cmip6 package in R if you want to integrate it into your R workflow. To do so open an R console or R Studio and follow the steps below. Important: You still need to have python and the chelsa_cmip6 package installed (see instructions above).
+Tested with R 4.2.1 in Windows 10
 
 Install and load the reticulate package
 ```R
 install.packages("reticulate",dependencies = TRUE)
 library(reticulate)
 ```
 
+Install and load the chelsa-cmip6 package
+```R
+py_install("chelsa-cmip6", pip=T)
+```
+
 The import() function enables you to import the chelsa_cmip6 module and call it’s functions directly from R.
 ```R
 chelsa_cmip6 <- import('chelsa_cmip6')
 ```
 
-You can then use the chelsa_cmip6 function in R the same you would in python.
+You can then use the chelsa_cmip6 function in R the same you would in python. Be aware that the function might run for a while before it creates any output.
 ```R
-
+chelsa_cmip6$GetClim$chelsa_cmip6(activity_id='ScenarioMIP', 
+                                  table_id='Amon', 
+                                  experiment_id='ssp585', 
+                                  institution_id='MPI-M', 
+                                  source_id='MPI-ESM1-2-LR', 
+                                  member_id='r1i1p1f1', 
+                                  refps='1981-01-15', 
+                                  refpe='2010-12-15', 
+                                  fefps='2041-01-15', 
+                                  fefpe='2070-12-15', 
+                                  xmin=5.3, 
+                                  xmax=10.4,
+                                  ymin=46.0, 
+                                  ymax=47.5,
+                                  output='~/')
 ```
 
 
 # REQUIREMENTS
 ------------
 chelsa_cmip6 is written in Python 3. It has been tested to run well with the
 following Python release and package versions. The dependencies will be installed automatically.
@@ -287,25 +374,37 @@
 - numpy 1.19.5
 - rasterio 1.2.1
 - pandas 1.1.5
 - zarr 2.6.1
 - gcsfs 0.7.2
 - datetime 3.9.2
 - scipy 0.19.1
+- fsspec
+- dask
+- netcdf4
+- h5netcdf
+
 
 
 ## SINGULARITY
 ------------
 All dependencies are also resolved in the singularity container '/singularity/chelsa_cmip6.sif'. Singularity needs to be installed on the respective linux system you are using. 
 An installation guide can be found here: https://sylabs.io/guides/3.3/user-guide/quick_start.html#quick-installation-steps
 
+The singularity container is available only here: https://gitlabext.wsl.ch/karger/chelsa_cmip6/-/blob/master/singularity/chelsa_cmip6.sif
+
 If you use chelsa_cmip6 together with singularity the command should be slightly modified:
 
 ```bash
-singularity exec /singularity/chelsa_cmip6.sif python3 chelsa_cmip6.py --activity_id 'CMIP' --table_id 'Amon' --experiment_id 'historical' --institution_id 'MPI-M' --source_id 'MPI-ESM1-2-LR' --member_id 'r1i1p1f1' --refps '1981-01-15' --refpe '2010-12-15' --fefps '1851-01-15' --fefpe '1880-12-15' --xmin 5.3 --xmax 10.4 --ymin 46.0 --ymax 47.5 --output '/home/karger/scratch/'
+singularity exec /singularity/chelsa_cmip6.sif python3 chelsa_cmip6.py \
+--activity_id 'CMIP' --table_id 'Amon' --experiment_id 'historical' \
+--institution_id 'MPI-M' --source_id 'MPI-ESM1-2-LR' --member_id 'r1i1p1f1' \
+--refps '1981-01-15' --refpe '2010-12-15' --fefps '1851-01-15' \
+--fefpe '1880-12-15' --xmin 5.3 --xmax 10.4 --ymin 46.0 \
+--ymax 47.5 --output '/home/karger/scratch/'
 ```
 
 tested with singularity version 3.3.0-809.g78ec427cc
 but newer versions usually work as well.
 
 
 ## CHECKING IF ALL NEEDED INPUT IS AVAILABLE
@@ -330,14 +429,22 @@
 ------------
 The output consist of netCDF4 files. There will be different files for each variable and seperatly for
 the reference (refps - refpe) and the future period (fefps - fefpe). 
 Additionally, there will be netCDF4 files for the 
 different bioclimatic variables each for both the reference (refps - refpe) and the future period (fefps - fefpe). 
 
 
+##  CAVEATS
+------------
+Important: 
+1. Please be aware that depending on the computer you use the function will only run if you have access to the internet. 
+2. It might take a considerable amount of time to finish as the data transfer needed is relativly large.
+3. You will need a considerable amount of RAM depending on the geographical size you choose. The example given runs with 16 GB of RAM. Below that we cannot garantee that the function will succeed.
+
+
 # COPYRIGHT
 ---------
 (C) 2022 Dirk Nikolaus Karger
 
 
 # LICENSE
 -------
```

### Comparing `chelsa_cmip6-1.1/src/chelsa_cmip6/run_chelsa_cmip6.py` & `chelsa_cmip6-1.2/src/chelsa_cmip6/run_chelsa_cmip6.py`

 * *Files identical despite different names*

### Comparing `chelsa_cmip6-1.1/src/chelsa_cmip6/GetClim.py` & `chelsa_cmip6-1.2/src/chelsa_cmip6/GetClim.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 
 import numpy as np
 import xarray as xr
 import pandas as pd
 import gcsfs
 import datetime
+import fsspec
+from dask.diagnostics import ProgressBar
 from chelsa_cmip6.BioClim import BioClim
 
 
 def _get_cmip(activity_id, table_id, variable_id, experiment_id, instituion_id, source_id, member_id):
     """
     Get CMIP model from Google Cloud storage via lazy loading.
 
@@ -66,15 +68,15 @@
     :rtype: xarray
     """
     def __init__(self, ds, template):
         self.ds = ds
         self.template = template
 
     def interpolate(self):
-        res = self.ds.interp(lat=self.template["y"], lon=self.template["x"])
+        res = self.ds.interp(lat=self.template["lat"], lon=self.template["lon"])
         return res
 
 
 class chelsaV2:
     """ 
     Class to download and clip data from the CHELSA V2.1 normals (climatologies)
     for a specific bounding box delimited by minimum and maximum latitude and longitude
@@ -97,36 +99,53 @@
         """
         clip xarray
         
         :param ds: a xarray to_dataset
         :return: clipped xarray
         :rtype: xarray
         """
-        mask_lon = (ds.x >= self.xmin) & (ds.x <= self.xmax)
-        mask_lat = (ds.y >= self.ymin) & (ds.y <= self.ymax)
+        mask_lon = (ds.lon >= self.xmin) & (ds.lon <= self.xmax)
+        mask_lat = (ds.lat >= self.ymin) & (ds.lat <= self.ymax)
         cropped_ds = ds.where(mask_lon & mask_lat, drop=True)
         return cropped_ds
 
     def get_chelsa(self):
         """
         download chelsa
         
         :return: cropped xarray
         :rtype: xarray
         """
+
         a = []
         for month in range(1, 13):
-            url = 'https://envicloud.os.zhdk.cloud.switch.ch/chelsa/chelsa_V2/GLOBAL/climatologies/1981-2010/' + self.variable_id + '/CHELSA_' + self.variable_id + '_' + '%02d' % (month,) + '_1981-2010_V.2.1.tif'
-            a.append(url)
+            url = 'https://os.zhdk.cloud.switch.ch/envicloud/chelsa/chelsa_V2/GLOBAL/climatologies/1981-2010/ncdf/CHELSA_' + self.variable_id + '_' + '%02d' % (
+                month,) + '_1981-2010_V.2.1.nc'
+            with fsspec.open(url) as fobj:
+                ds = xr.open_dataset(fobj).chunk({'lat': 500, 'lon': 500})
+                ds = self._crop_ds_(ds)
+                ds.load()
+            a.append(ds)
+
+        ds = xr.concat([i for i in a], 'time')
+
+        #ds = self._crop_ds_(xr.concat([i for i in a], 'time'))
+
+        # old version using rasterio
+        #a = []
+        #for month in range(1, 13):
+        #    url = 'https://envicloud.os.zhdk.cloud.switch.ch/chelsa/chelsa_V2/GLOBAL/climatologies/1981-2010/' + self.variable_id + '/CHELSA_' + self.variable_id + '_' + '%02d' % (month,) + '_1981-2010_V.2.1.tif'
+        #    a.append(url)
 
-        ds = self._crop_ds_(xr.concat([xr.open_rasterio(i) for i in a], 'time'))
+        #ds = self._crop_ds_(xr.concat([xr.open_rasterio(i) for i in a], 'time'))
         if self.variable_id == "tas" or self.variable_id == 'tasmin' or self.variable_id == 'tasmax':
-            res = ds / 10 - 273.15
+            res = ds.assign(Band1=ds['Band1'] * 0.1)
         if self.variable_id == 'pr':
-            res = ds / 10
+            res = ds.assign(Band1=ds['Band1'] * 0.01)
+
         return res
 
 
 class cmip6_clim:
     """ 
     Climatology class for monthly climatologies for CMIP6 data 
     
@@ -214,14 +233,15 @@
     :param xmin: Minimum longitude [Decimal degree]
     :param xmax: Maximum longitude [Decimal degree]
     :param ymin: Minimum latitude [Decimal degree]
     :param ymax: Maximum latitude [Decimal degree]
     """
     def __init__(self, xmin, xmax, ymin, ymax):
         for var in ['pr', 'tas', 'tasmax', 'tasmin']:
+            print("getting variable: " + var)
             setattr(self, var, chelsaV2(xmin, xmax, ymin, ymax, var).get_chelsa())
 
 
 class CmipClimat:
     """ 
     Climatology data class for monthly cmip 6 climatological normals
     
@@ -271,18 +291,22 @@
         self.fefpe = fefpe
         self.hist_year = np.mean([int(datetime.datetime.strptime(refps, '%Y-%m-%d').year), 
                                  int(datetime.datetime.strptime(refpe, '%Y-%m-%d').year)]).__round__()
         self.futr_year = np.mean([int(datetime.datetime.strptime(fefps, '%Y-%m-%d').year), 
                                  int(datetime.datetime.strptime(fefpe, '%Y-%m-%d').year)]).__round__()
 
         for per in ['futr', 'hist']:
-            setattr(self, str(per + '_pr'), getattr(ChelsaClimat, 'pr').to_dataset(name='pr').rename({'time': 'month'}).drop('band') * interpol(
+            #setattr(self, str(per + '_pr'), getattr(ChelsaClimat, 'pr').to_dataset(name='pr').rename({'time': 'month'}).drop('band') * interpol(
+            #        getattr(CmipClimat, 'pr').get_anomaly(per), getattr(ChelsaClimat, 'pr')).interpolate())
+            setattr(self, str(per + '_pr'), getattr(ChelsaClimat, 'pr').rename({'time': 'month', 'Band1': 'pr'}) * interpol(
                     getattr(CmipClimat, 'pr').get_anomaly(per), getattr(ChelsaClimat, 'pr')).interpolate())
             for var in ['tas', 'tasmax', 'tasmin']:
-                setattr(self, str(per + '_' + var), getattr(ChelsaClimat, var).to_dataset(name=var).rename({'time': 'month'}).drop('band') + interpol(
+                #setattr(self, str(per + '_' + var), getattr(ChelsaClimat, var).to_dataset(name=var).rename({'time': 'month'}).drop('band') + interpol(
+                #        getattr(CmipClimat, var).get_anomaly(per), getattr(ChelsaClimat, var)).interpolate())
+                setattr(self, str(per + '_' + var), getattr(ChelsaClimat, var).rename({'time': 'month', 'Band1': var}) + interpol(
                         getattr(CmipClimat, var).get_anomaly(per), getattr(ChelsaClimat, var)).interpolate())
 
         for var in ['tas', 'tasmax', 'tasmin', 'pr']:
             getattr(self, str('futr_' + var))['month'] = [datetime.datetime(self.futr_year, month, 15) for month in getattr(self, str(per + '_' + var))['month'].values]
             getattr(self, str('hist_' + var))['month'] = [datetime.datetime(self.hist_year, month, 15) for month in getattr(self, str(per + '_' + var))['month'].values]
 
         if output:
@@ -330,34 +354,38 @@
     :param fefpe: End date of the future_period
     :param xmin: Minimum longitude [Decimal degree]
     :param xmax: Maximum longitude [Decimal degree]
     :param ymin: Minimum latitude [Decimal degree]
     :param ymax: Maximum latitude [Decimal degree]
     :param output: output directory, string
     """
-    #print('starting downloading CMIP data:')
-    cm_climat = CmipClimat(activity_id, table_id,
-                           experiment_id,
-                           institution_id, source_id,
-                           member_id, refps,
-                           refpe, fefps,
-                           fefpe)
+    print('start downloading CMIP data:')
+    with ProgressBar():
+        cm_climat = CmipClimat(activity_id, table_id,
+                               experiment_id,
+                               institution_id, source_id,
+                               member_id, refps,
+                               refpe, fefps,
+                               fefpe)
 
-    #print('starting downloading CHELSA data:')
+    print('start downloading CHELSA data (depending on your internet speed this might take a while...)')
     ch_climat = ChelsaClimat(xmin, xmax, ymin, ymax)
 
-    dc = DeltaChangeClim(ch_climat, cm_climat, refps,
-                         refpe, fefps,
-                         fefpe, output)
-
-    #print('starting building climatologies data:')
-    biohist = BioClim(dc.hist_pr, dc.hist_tas, dc.hist_tasmax, dc.hist_tasmin)
-    biofutr = BioClim(dc.futr_pr, dc.futr_tas, dc.futr_tasmax, dc.futr_tasmin)
+    print('applying delta change:')
+    with ProgressBar():
+        dc = DeltaChangeClim(ch_climat, cm_climat, refps,
+                             refpe, fefps,
+                             fefpe, output)
+
+    print('start building climatologies data:')
+    with ProgressBar():
+        biohist = BioClim(dc.hist_pr, dc.hist_tas, dc.hist_tasmax, dc.hist_tasmin)
+        biofutr = BioClim(dc.futr_pr, dc.futr_tas, dc.futr_tasmax, dc.futr_tasmin)
 
-    #print('saving bioclims:')
+    print('saving bioclims:')
     for n in range(1, 20):
         name = output + 'CHELSA' + '_' + cm_climat.tas.institution_id + '_' \
                + cm_climat.tas.source_id + '_' + str('bio' + str(n)) + '_' \
                + cm_climat.tas.experiment_id + '_' + cm_climat.tas.member_id \
                + '_' + cm_climat.tas.refps + '_' + cm_climat.tas.refpe + '.nc'
         getattr(biohist, 'bio' + str(n))().to_netcdf(name)
```

### Comparing `chelsa_cmip6-1.1/src/chelsa_cmip6/BioClim.py` & `chelsa_cmip6-1.2/src/chelsa_cmip6/BioClim.py`

 * *Files identical despite different names*

