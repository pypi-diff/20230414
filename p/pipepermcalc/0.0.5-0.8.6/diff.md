# Comparing `tmp/pipepermcalc-0.0.5.tar.gz` & `tmp/pipepermcalc-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipepermcalc-0.0.5.tar", last modified: Wed Mar 29 12:02:13 2023, max compression
+gzip compressed data, was "pipepermcalc-0.8.6.tar", last modified: Fri Apr 14 08:16:51 2023, max compression
```

## Comparing `pipepermcalc-0.0.5.tar` & `pipepermcalc-0.8.6.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 12:02:13.394076 pipepermcalc-0.0.5/
--rw-rw-rw-   0        0        0     1087 2023-01-25 10:21:46.000000 pipepermcalc-0.0.5/LICENSE
--rw-rw-rw-   0        0        0        0 2023-01-25 10:21:46.000000 pipepermcalc-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      843 2023-03-29 12:02:13.394076 pipepermcalc-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-29 09:00:30.000000 pipepermcalc-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-29 12:02:13.306078 pipepermcalc-0.0.5/pipepermcalc/
--rw-rw-rw-   0        0        0        0 2023-01-25 10:21:46.000000 pipepermcalc-0.0.5/pipepermcalc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:02:13.386079 pipepermcalc-0.0.5/pipepermcalc/database/
--rw-rw-rw-   0        0        0       49 2023-03-29 10:03:05.000000 pipepermcalc-0.0.5/pipepermcalc/database/__init__.py
--rw-rw-rw-   0        0        0    28943 2023-03-23 11:07:34.000000 pipepermcalc-0.0.5/pipepermcalc/database/ppc_database.csv
--rw-rw-rw-   0        0        0    49916 2023-03-29 10:38:14.000000 pipepermcalc-0.0.5/pipepermcalc/pipe.py
--rw-rw-rw-   0        0        0      815 2023-02-17 10:47:18.000000 pipepermcalc-0.0.5/pipepermcalc/project_path.py
--rw-rw-rw-   0        0        0    27148 2023-03-29 09:51:58.000000 pipepermcalc-0.0.5/pipepermcalc/segment.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:02:13.370077 pipepermcalc-0.0.5/pipepermcalc.egg-info/
--rw-rw-rw-   0        0        0      843 2023-03-29 12:02:13.000000 pipepermcalc-0.0.5/pipepermcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-03-29 12:02:13.000000 pipepermcalc-0.0.5/pipepermcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 12:02:13.000000 pipepermcalc-0.0.5/pipepermcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-03-29 12:02:13.000000 pipepermcalc-0.0.5/pipepermcalc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-29 12:02:13.000000 pipepermcalc-0.0.5/pipepermcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-03-29 11:13:19.000000 pipepermcalc-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 12:02:13.394076 pipepermcalc-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-03-29 12:01:45.000000 pipepermcalc-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:02:13.394076 pipepermcalc-0.0.5/tests/
--rw-rw-rw-   0        0        0    24654 2023-03-29 09:50:55.000000 pipepermcalc-0.0.5/tests/test_pipepermcalc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:16:51.362171 pipepermcalc-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 08:16:51.362171 pipepermcalc-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:16:51.362171 pipepermcalc-0.8.6/pipepermcalc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/pipepermcalc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:16:51.362171 pipepermcalc-0.8.6/pipepermcalc/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/pipepermcalc/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28502 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/pipepermcalc/database/ppc_database.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    53427 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/pipepermcalc/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27171 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/pipepermcalc/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:16:51.362171 pipepermcalc-0.8.6/pipepermcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 08:16:51.000000 pipepermcalc-0.8.6/pipepermcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 08:16:51.000000 pipepermcalc-0.8.6/pipepermcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:16:51.000000 pipepermcalc-0.8.6/pipepermcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 08:16:51.000000 pipepermcalc-0.8.6/pipepermcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 08:16:51.000000 pipepermcalc-0.8.6/pipepermcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:16:51.362171 pipepermcalc-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:16:51.362171 pipepermcalc-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23952 2023-04-14 08:16:37.000000 pipepermcalc-0.8.6/tests/test_pipepermcalc.py
```

### Comparing `pipepermcalc-0.0.5/LICENSE` & `pipepermcalc-0.8.6/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 KWR-Water
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 KWR-Water
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pipepermcalc-0.0.5/pipepermcalc/database/ppc_database.csv` & `pipepermcalc-0.8.6/pipepermcalc/database/ppc_database.csv`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,441 +1,441 @@
-CAS_number,chemical_name_NL,chemical_name_EN,molecular_weight,solubility,log_octanol_water_partitioning_coefficient,log_distribution_coefficient,chemical_group,chemical_group_number,molecular_volume,Drinking_water_norm
-,,,M,Cwsat,LOG Kow,LOG Kd,group,,Vm,
-,,,g/mol,g/m3,(-),(-),,,cm3/mol,g/m3
-66-25-1, Hexaldehyde, Hexaldehyde,100.16,6000,1.78,,overige,3,,
-71-55-6,"1,1,1-Trichloorethaan","1,1,1-Trichloroethane",133.4,2343.333333,2.8,0.760444292,ClAlk,1,,0.001
-79-34-5,"1,1,2,2-Tetrachloorethaan","1,1,2,2-Tetrachloroethane",167.85,2900,2.39,,ClAlk,1,,
-79-00-5,"1,1,2-Trichloorethaan","1,1,2-Trichloroethane",133.4,3055,1.89,0.753447145,ClAlk,1,,0.001
-75342,"1,1-Dichloorethaan","1,1-Dichloroethane",98.96499987,5223.690293,1.79,0.360665595,ClAlk,1,,0.001
-,"1,1-dichlooretheen","1,1-dichlooretheen",97,1824,2.13,0.589733613,ClAlk,1,,0.001
-,"1,2,3,4-tetrachlorobenzene","1,2,3,4-tetrachlorobenzene",215.9,3.399273364,4.64,2.67369577,ClArom,1,,0.001
-,"1,2,3,5-tetrachlorobenzene","1,2,3,5-tetrachlorobenzene",215.9,2.614957562,4.66,2.333981434,ClArom,1,,0.001
-87-61-6,"1,2,3-Trichloorbenzeen","1,2,3-Trichlorobenzene",181.439995,13.62398701,4.14,1.994666142,ClArom,1,,0.001
-96184,"1,2,3-trichloorpropaan","1,2,3-trichloropropane",147.43,1750,2.27,,,,,
-526738,"1,2,3-trimethylbenzeen","1,2,3-trimethylbenzene",120.19,75.2,3.66,,,,,
-,"1,2,3-Trimethylbenzene","1,2,3-Trimethylbenzene",120.19,75,3.6,,MAK,1,139.6,
-,"1,2,4,5-tetrachlorobenzene","1,2,4,5-tetrachlorobenzene",215.9,0.68248085,4.6,2.533894299,ClArom,1,,0.001
-120-82-1,"1,2,4-Trichloorbenzeen","1,2,4-Trichlorobenzene",181.439995,28.80802015,4.05,2.044515105,ClArom,1,,0.001
-95636,"1,2,4-trimethylbenzeen","1,2,4-trimethylbenzene",120.19,57,3.78,,,,,
-95-50-1,"1,2-Dichloorbenzeen","1,2-Dichlorobenzene",147.0024999,140.218586,3.43,1.36831917,ClArom,1,,0.001
-107-06-2,"1,2-Dichloorethaan","1,2-Dichloroethane",98.97333154,10188.83247,1.47,0.311244667,ClAlk,1,79.4,0.003
-156-59-2,"1,2-Dichlooretheen(cis)","1,2-dichloro-, (Z)-Ethene",96.95,775.6,1.906666667,0.625232261,ClAlk,1,,0.001
-540-59-0,"1,2-dichlooretheen(cisentrans)","1,2-dichloroEthene",96.95,775.6,1.27,,ClAlk,1,,
-156-60-5,"1,2-dichlooretheen(trans)","1,2-dichloro-, (1E)-Ethene",96.95,581.7,1.09,0.627641144,ClAlk,1,,0.001
-,"1,2-Dichloorfenol","1,2-Dichloorphenol",163,904.5313384,2.84,1.436666667,Cl,3,,
-78-87-5,"1,2-dichloorpropaan","1,2-Dichloropropane",113,1469,1.99,0.392478925,ClAlk,1,,0.001
-,"1,2-dimethylnaphthalene","1,2-dimethylnaphthalene",156,,4.31,,PAK,1,154.2,
-108-70-3,"1,3,5-Trichloorbenzeen","1,3,5-Trichlorobenzene",181.4249983,4.711953407,4.19,2.744256831,ClArom,1,,0.001
-108-67-8,"1,3,5-Trimethylbenzeen","1,3,5-Trimethylbenzene",120.19,11.45,3.51,,MAK,1,,
-541-73-1,"1,3-Dichloorbenzeen","1,3-Dichlorobenzene",147,114.3333333,3.4,1.546462047,ClArom,1,,0.001
-,"1,3-dichloorpropaan","1,3-dichloropropane",113,1469,1.99,0.392478925,ClAlk,1,,0.001
-,"1,3-dimethylnaphthalene","1,3-dimethylnaphthalene",156,,4.42,,PAK,1,155.8,
-,"1,4,6,7-tetramethylnaphthalene","1,4,6,7-tetramethylnaphthalene",184,,5.36,,PAK,1,186,
-106-46-7,"1,4-Dichloorbenzeen","1,4-Dichlorobenzene",147.0019999,60.52630716,3.44,1.586462047,ClArom,1,,0.001
-,"1,4-dimethylnaphthalene","1,4-dimethylnaphthalene",156,,4.37,,PAK,1,155.6,
-123-91-1,"1,4-Dioxane {p-dioxane} ","1,4-Dioxane ",88.11,1000000,-0.27,,overige,3,,
-,"1,8-dimethylnaphthalene","1,8-dimethylnaphthalene",156,,4.32,,PAK,1,155.6,
-71-36-3,1-Butanol,1-Butanol,74.12,63200,0.88,,O2,3,,
-109693,1-chloorbutaan,1-chlorobutane,92.57,0.87,2.39,,,,,
-90131,1-chloornaftaleen,1-chloornaphthalene,162.6059998,16.80146852,4.1,2.18418207,Cl,3,,0.001
-,1-Chloronaphthalene,1-Chloronaphthalene,162.62,17.4,4,,ClArom,1,137.7,
- 111-27-3 ,1-Hexanol {Hexylalcohol},1-Hexanol,102.18,5900,2.03,,O2,3,,
-,1-methylfluorene,1-methylfluorene,180,,4.97,,PAK,1,169.4,
-,1-methylnaphthalene,1-methylnaphthalene,142,,3.87,,PAK,1,139.9,
-,1-methylphenanthrene,1-methylphenanthrene,192,,5.08,,PAK,1,175.9,
-,1-methylpyrene,1-methylpyrene,216,,5.48,,PAK,1,197.7,
-71-41-0,1-Pentanol,1-Pentanol,88.15,22000,1.51,,O2,3,,
-,2-(2-Hydroxy-3.t-butyl-5-methylphenyl-5-Chloro-benztriazol (Tinuvin 326),2-(2-Hydroxy-3.t-butyl-5-methylphenyl-5-Chloro-benztriazol,315.8,,,,overige,3,,
-25167-70-8,"2,2,4-Trimethylpentaan","2,2,4-Trimethylpentane",112.21,14.2,4.37,,Alk,1,,
-15950-66-0,"2,3,4-Trichloorfenol","2,3,4-Trichlorophenol",197.5,71.1,3.8,1.845017825,Cl,3,,0.001
-,"2,3,5,6,-Tetramethyl-phenol","2,3,5,6,-Tetramethyl-phenol",150,,,,overige,3,,
-935-95-5,"2,3,5,6-Tetrachloorfenol","2,3,5,6-Tetrachlorophenol",231.9,4.79,3.88,2.10431794,Cl,3,,0.001
-,"2,3,5-trimethylnaphthalene","2,3,5-trimethylnaphthalene",170,,4.81,,PAK,1,170.2,
-,"2,3,6-trimethylnaphthalene","2,3,6-trimethylnaphthalene",170,,4.73,,PAK,1,170.3,
-,"2,3,7-TriCDD","2,3,7-TriCDD",287.5,0.14409133,6.1,,overige,3,179.9,
-,"2,3-Benzopyrole (Indole)","2,3-Benzopyrole",117,,,,onbekend,3,,
-,"2,3-Dichloor-5-nitrotolueen","2,3-Dichloor-5-nitrotolueen",,,,,Cl,3,,
-88-06-2,"2,4,6-Trichloorfenol","2,4,6-Trichlorophenol",197.46,243,3.695,2.234096671,Cl,3,,0.001
-,"2,4-dichloorfenol","2,4-dichloorphenol",163,1907.107928,3.06,1.308828347,ClAlk,1,,0.001
-,"2,5-dichloorfenol","2,5-dichloorphenol",163,420.9082483,3.06,1.596225694,ClAlk,1,,0.001
-,"2,6-dichloorfenol","2,6-dichloorphenol",163,534.106534,2.75,1.397831352,ClAlk,1,,0.001
-,"2,6-dimethylnaphthalene","2,6-dimethylnaphthalene",156,,4.31,,PAK,1,155.9,
-,"2,6-Di-tert-butyl-4-methyl-phenol (BHT)","2,6-Di-tert-butyl-4-methyl-phenol",220,,,,overige,3,,
-,"2,7/8-DiCDD","2,7/8-DiCDD",253.1,0.201044476,5.6,,overige,3,168.5,
-,2-CDD,2-CDD,218.6,1.736401521,5.2,,overige,3,156.4,
-95-51-2,2-Chlooraniline,2-Chloroaniline,127.57,8160,1.9,,Cl,3,,
-,2-chloorfenol,2-chloorphenol,128.5899988,8708.954334,2.15,0.398828347,ClAlk,1,,0.001
-91587,2-chloornaftaleen,2-chloornaphthalene,162.6099997,9.71436827,4.14,2.184177182,Cl,3,,0.001
-,2-ethylanthracene,2-ethylanthracene,206,,5.85,,PAK,1,191.2,
- 626-93-7,2-Hexanol,2-Hexanol,102.18,14350,1.76,,O2,3,,
-,2-Hydroxy-4-ethandiol methyl-thioacetic acid ester,2-Hydroxy-4-ethandiol methyl-thioacetic acid ester,346,,,,overige,3,,
-,2-Methoxy-4-propenyl-phenol,2-Methoxy-4-propenyl-phenol,164,,,,overige,3,,
-,2-methylanthracene,2-methylanthracene,192.15,1.661036915,4.85,,PAK,1,174.8,
-,2-methylnaphthalene,2-methylnaphthalene,167.15,1.661036915,4.28,,PAK,1,158.25,
-,2-methylphenanthrene,2-methylphenanthrene,192,,5.01,,PAK,1,176,
-6032-29-7,2-Pentanol,2-Pentanol,88.15,166000,1.25,,O2,3,,
-,2-Phenly-ehtyl-alcohol,2-Phenly-ehtyl-alcohol,122,,,,O2,3,,
-67-63-0,2-Propanol {isopropyl alcohol},2-Propanol,60.1,1000000,0.05,,O2,3,,
-,"3-(3,5-di-tert-butyl-4-hydroxy phenyl)-propionate (Irganox 1076)","3-(3,5-di-tert-butyl-4-hydroxy phenyl)-propionate",531,,,,onbekend,3,,
-609-19-8,"3,4,5-Trichloorfenol","3,4,5-Trichlorophenol",197.45,34.6,4.01,2.304002415,Cl,3,,0.001
-,"3,6-dimethylphenanthrene","3,6-dimethylphenanthrene",206.15,0.635183529,5.17,,PAK,1,192.2,
-,"3,7-Dimehtyl-octane-3-ol","3,7-Dimehtyl-octane-3-ol",158,,,,O2,3,,
-,"3,7-Dimethyl-6-octene-al","3,7-Dimethyl-6-octene-al",154,,,,O2,3,,
-108-42-9,3-Chlooraniline,3-Chloroaniline,127.57,5400,1.88,,Cl,3,,
-,3-chloorfenol,3-chloorphenol,128.5899988,7969.660322,2.5,0.748828347,ClAlk,1,,0.001
- 96-14-0 ,3-Methylpentane,3-Methylpentane,86.18,18,3.6,,Alk,1,,
-,3-Octene-2-one,3-Octene-2-one,126,,,,O2,3,,
-,3-Phenyl-1-propanol,3-Phenyl-1-propanol,136,,,,O2,3,,
-106-47-8,4-Chlooraniline,4-Chloroaniline,127.57,3900,1.83,,Cl,3,,
-,4-chloorfenol,4-chloorphenol,128.5899988,7667.192707,2.39,0.638828347,ClAlk,1,,0.001
-,4-Isopropenyl-1-methyl-1-cyclohexene (Limonene),4-Isopropenyl-1-methyl-1-cyclohexene,136,,,,overige,3,,
-,4-Isopropyl-tuluene,4-Isopropyl-tuluene,134,,,,MAK,1,,
-,6-methylchrysene,6-methylchrysene,242,,6.07,,PAK,1,211.9,
-,"7,12-dimethylbenz[a]anthracene","7,12-dimethylbenz[a]anthracene",256,,6.62,,PAK,1,226,
-,7-methylbenz[a]anthracene,7-methylbenz[a]anthracene,242,,6.07,,PAK,1,210.3,
-,7-Methyl-chinoline,7-Methyl-chinoline,143,,,,onbekend,3,,
-,"9,10-dimethylanthracene","9,10-dimethylanthracene",206.15,0.635183529,5.295,,PAK,1,190.15,
-,9-methylanthracene,9-methylanthracene,192,,5.07,,PAK,1,174.3,
-,acenaphthene,acenaphthene,154.1,22.06400634,3.96,,PAK,1,141.8,
-,acenaphthylene,acenaphthylene,152.2,,3.9,,PAK,1,223.1,
-67-64-1,Acetone,Acetone,58.08,790000,-0.24,,O2,3,74,
-75-05-8,Acetonitrile,Acetonitrile,41.05,1000000,-0.34,,overige,3,,
-,aldrin,aldrin,364.9,0.916587359,6.3,2.7036797,overige,3,240.1,0.00003
-463-49-0,Allene,Allene,40.065,,1.45,,Alk,1,,
-62-53-3,Aniline,Anilin,93.13,35333.33333,0.988,,overige,3,,
-,Antraceen,anthracene,178.1,4.350184731,4.525,3.063556603,PAK,1,158.9,0.0001
-1912249,atrazine,atrazine,215.6966666,38.13236662,2.61,0.975115324,overige,3,,0.0001
-,BDE-1,BDE-1,249.1,2.491,4.6,,BDE,3,174.7,
-,BDE-100,BDE-100,564.7,0.014184623,7.3,,BDE,3,232,
-,BDE-126,BDE-126,564.7,0.011267246,7.4,,BDE,3,233.7,
-,BDE-15,BDE-15,328,0.519844967,5.2,,BDE,3,189.9,
-,BDE-153,BDE-153,643.6,0.004060841,8,,BDE,3,246.6,
-,BDE-154,BDE-154,643.6,0.004060841,8,,BDE,3,246.5,
-,BDE-17,BDE-17,406.9,0.203933085,5.8,,BDE,3,202.1,
-,BDE-2,BDE-2,249.1,1.978671633,4.5,,BDE,3,173,
-,BDE-28,BDE-28,406.9,0.161989808,5.8,,BDE,3,203.8,
-,BDE-47,BDE-47,485.8,0.04858,6.5,,BDE,3,217.6,
-,BDE-66,BDE-66,485.8,0.04858,6.5,,BDE,3,218.2,
-,BDE-71,BDE-71,485.8,0.04858,6.6,,BDE,3,217,
-,BDE-85,BDE-85,564.7,0.014184623,7.2,,BDE,3,231.6,
-,BDE-99,BDE-99,564.7,0.014184623,7.2,,BDE,3,232.1,
-,benz[a]anthracene,benz[a]anthracene,228.15,0.138965154,5.78,4.553465774,PAK,1,194.9,0.0001
-00-52-7,Benzaldehyde,Benzaldehyde,106.13,6950,1.48,,overige,3,,
-71-43-2,Benzeen,Benzene,78.10666652,1988.898826,2.13,0.659555885,MAK,1,89.4,0.001
-,benzo(a)perylene,benzo(a)perylene,252.3,,,,PAK,1,218.2,
-,"benzo(g,h,i)perylene","benzo(g,h,i)perylene",276.3,0.000186,6.22,5.193463434,PAK,1,241.3,0.0001
-,benzo[a]pyrene,benzo[a]pyrene,252.15,0.026200963,6.115,4.583465572,PAK,1,218.05,0.00001
-,benzo[b]fluoranthene,benzo[b]fluoranthene,252.15,0.026200963,5.84,4.103471294,PAK,1,231.8,0.0001
-,benzo[e]pyrene,benzo[e]pyrene,252.15,0.026200963,6.27,,PAK,1,219.45,
-,benzo[ghi]perylene,benzo[ghi]perylene,276,,6.7,,PAK,1,241,
-,benzo[k]fluoranthene,benzo[k]fluoranthene,252.15,0.026200963,6.005,,PAK,1,229.3,
-100-51-6,Benzyl alcohol,Benzyl alcohol,108.14,42900,1.1,,overige,3,,
-100-44-7,Benzylchloride,Benzyl chloride,126.59,476.5,2.3,,ClArom,1,,
-101-84-8  (= bifenyl oxide ??),bifenly ether,diphenyl ether,170.21,20,4.21,,O2,3,,
- 92-52-4 ,Bifenyl,Biphenyl,154.21,6.476666667,4.045,,PAK,1,,
-71-36-3,Butylalcohol {Butanol],Butylalcohol ,74.12,77000,0.84,,O2,3,,
-,butylated hydroxyanisol,butylated hydroxyanisol,180.2,,,,overige,3,175.7,
-,butylated hydroxytoluene,butylated hydroxytoluene,220.4,,,,overige,3,235,
-104518,butylbenzeen,butylbenzene,134.22,11.8,4.38,,,,,
-85687,butylbenzylftalaat(BBP),benzyl butyl phthalate (BBP),312.3966666,4.218630438,4.91,2.673692963,overige,3,,0.0001
-,Butyraldehyde,Butyraldehyde,72.11,71000,0.88,,O2,3,89.6,
-123-72-8,Butyraldehyde (butanal),Butyraldehyde,72.11,37000,0.88,,O2,3,,
-63252,carbaryl,carbaryl,201.2066664,81.56328382,2.36,1.043401359,overige,3,,0.0001
-1563662,carbofuran,carbofuran,221.2899993,376.0966593,1.63,0.444356263,overige,3,,0.0001
-,Cedrylacetate,Cedrylacetate,264,,,,overige,3,,
-,Chloordaan,Chlordane,410,0.14,5.8,3.363509843,overige,3,,0.0001
-75-00-3,chloorethaan,Chloroethane,64.515,6710,1.485,,ClAlk,1,,
-540545,chloorpentaan,chloropentane,106.59,197,2.73,,,,,
-,Chlorobenzene,Chlorobenzene,112.56,498,2.84,,ClArom,1,102.2,
-,Chloroform,Chloroform,119.38,7950,1.97,0.465300972,ClAlk,1,,0.001
-,chrysene,chrysene,228.15,0.138965154,5.755,4.483466305,PAK,1,196.3,0.0001
- 928-96-1 ,cis-Hex-3-en-1-ol,cis-Hex-3-en-1-ol,100.16,19300,1.61,,O2,3,,
-110-82-7,Cyclohexaan,Cyclohexane,84.16,49,3.48,,Alk,1,104.7,
-108941,cyclohexanon,cyclohexanon,98.14499563,18990.75095,0.81,-0.087766146,overige,3,,0.0001
- 75-19-4 ,Cyclopopane,Cyclopopane,42.08,502000,1.72,,overige,3,,
-,d10-fluoranthene,d10-fluoranthene,212,,,,PAK,1,,
-,d10-fluorene,d10-fluorene,176,,,,PAK,1,,
-,d12-benz[a]anthracene,d12-benz[a]anthracene,228.15,0.138965154,5.78,,PAK,1,,
-,d12-perylene,d12-perylene,264,,,,PAK,1,,
-117817,di(2-ethylhexyl)ftalaat,di(2-ethylhexyl)phthalate,390.5866662,0.045738942,7.45,4.133470728,overige,3,,0.0001
-,dibenz[ah]anthracene,dibenz[ah]anthracene,278,,6.8,,PAK,1,243.8,
-,"dibenzo(a,h)anthracene","dibenzo(a,h)anthracene",278.3,,,,PAK,1,244.2,
-84742,dibuthylftalaat(DBP),dibutyl phthalate,278.35,2.351,4.72,1.745420579,overige,3,,0.0001
-75-09-2,Dichloormethaan / Methyleenchloride,Dichloromethane,84.93,20000,1.25,0.088839633,ClAlk,1,64.5,0.001
-,"Didodecyl-3,3-thio-dipropionate","Didodecyl-3,3-thio-dipropionate",514,,,,onbekend,3,,
-,dieldrin,dieldrin,380.9,4.795246894,5.5,2.753654239,overige,3,253.7,0.00003
-60297,di-ethylether,di-ethylether,74.12,60400,0.89,,,,,
-84662,diethylftalaat(DEP),Diethyl phthalate (DEP),222.24,287.2,2.47,1.407730396,overige,3,,0.0001
-84753,dihexylftalaat(DHP),Dihexyl phthalate (DHP),334.5,0.01151,6.85,3.413505198,overige,3,,0.0001
-,di-isobutylftalaat(DIBP),Diisobutyl phthalate,278.35,9.6,4.46,2.00453864,overige,3,,0.0001
-108-20-3,Di-isopropylether,Diisopropyl ether,102.18,8900,1.52,,O2,3,,
-565-80-0,Di-isopropylketon,Di-isopropylketon,114.18,5700,1.86,,O2,3,,
-,Dimehtyl-phthalate,Dimehtyl-phthalate,194,,,,O2,3,,
- 67-68-5 ,Dimethyl sulfoxide,Dimethyl sulfoxide,78.14,1000000,-1.35,,overige,3,,
-,Dimethyl-benzyl-carbinol,Dimethyl-benzyl-carbinol,150,,,,onbekend,3,,
-,Dimethylftalaat,dimethylftalaat(DMP),194.19,2014,1.56,,O2,3,,
-131113,dimethylftalaat(DMP),Dimethyl phthalate,194.19,2014,1.56,1.023864247,overige,3,,0.0001
-,Diphenyl-oxide,Diphenyl-oxide,170,,,,overige,3,,
-,Docosane,Docosane,310,,,,onbekend,3,,
-,Eicosane,Eicosane,282,,,,onbekend,3,,
-,endosulfan sulphate,endosulfan sulphate,422.9,,5.1,,overige,3,239.8,
-,endrin,endrin,380.9,1.204511561,5,2.713672709,overige,3,253.7,0.0001
-,endrin aldehyde,endrin aldehyde,380.9,,5.5,,overige,3,253.2,
-,endrin ketone,endrin ketone,364.5,,6.8,,overige,3,,
-,ETBE (Ethyl tert-butyl ether) ,Ethyl tert-butyl ether,102.17476,5030.868137,1.88,,O2,3,,0.001
-74-84-0,Ethane,Ethane,30.07,62,1.81,,Alk,1,,
-64-17-5,Ethanol,Ethanol,46.07,1000000,-0.305,,O2,3,,
-141-78-6 ,Ethylacetaat,Ethylacetaat,88.1,62100,0.73,,O2,3,,
-100-41-4,Ethylbenzeen,Ethylbenzene,106.186665,159.4494297,3.15,1.299931656,MAK,1,,0.001
-74-85-1,Ethylene,Ethylene,28.05,130,1.13,,Alk,1,,
- 105-37-3 ,Ethylpropionate,Ethylpropionate,102.13,17000,1.21,,O2,3,,
-85-01-8,Fenanthreen,Phenanthrene,178.21,0.85,4.47,2.993573044,PAK,1,,0.0001
-108-95-2,Fenol,Phenol,94.10499987,65559.5567,1.48,0.336603308,O2,3,,0.001
-,fluoranthene,fluoranthene,202.15,0.836365063,5.08,3.943475119,PAK,1,195.85,0.0001
-,fluorene,fluorene,166.1,9.822703148,4.14,,PAK,1,154.6,
-,gasoline,gasoline,,,,,Arom,1,,
-,HCB,HCB,284.8,0.358541957,5.6,,overige,3,161.2,
-142-82-5,Heptaan (n-heptaan),n-Heptane,100.2,2.6,4.58,,Alk,1,,
-,heptachlor,heptachlor,373.3,1.180478251,6,3.213533128,overige,3,230.8,0.00003
-,heptachlor epoxide,heptachlor epoxide,389.3,4.900996628,5.4,1.705641075,overige,3,233.7,0.00003
-53535-33-4,Heptanol,Heptanol,116.21,1940,2.62,,O2,3,,
-110-54-3,Hexaan,Hexane,86.18,23,3.888,,Alk,1,,
-118741,Hexachloorbenzeen,Hexachlorobenzene,284.8,0.0117,5.73,2.823626427,ClArom,1,,0.001
- 66-25-1 ,Hexaldehyde,Hexaldehyde,100.16,6000,1.78,,O2,3,,
-25264-93-1,Hexene,Hexene,84.16,50,3.07,,Alk,1,,
-,δ-HCH,δ-HCH,290.8,115.7695652,3.9,2.134261869,overige,3,178,0.0001
-98-07-7,"α,α,α-Trichloortolueen",Benzotrichloride,195.475,51.5,2.92,,ClArom,1,,
-,α-endosulfan,α-endosulfan,406.9,2.567365435,4.9,1.874913747,overige,3,236.3,0.0001
-,α-HCH,α-HCH,290.8,91.95903436,3.9,2.09433891,overige,3,178,0.0001
-,β-HCH,β-HCH,290.8,460.8869404,3.9,2.134261869,overige,3,178,0.0001
-,γ-HCH,γ-HCH,290.8,73.04565743,3.8,1.755373969,overige,3,178,0.0001
-,"indeno[1,2,3-cd]pyrene","indeno[1,2,3-cd]pyrene",276,0.000265,6.7,4.783464526,PAK,1,253.4,0.0001
-103651,i-propylbenzeen,i-propylbenzene,120.19,61.3,3.66,,,,,
-115-11-7,Isobutyleen,Isobutylene,56.11,388,2.35,,Alk,1,,
-108-41-8,m-Chloortolueen,mo-Chlorotoluene,126.586,117,3.764,,ClArom,1,,
-,MCPA,MCPA,200.6,622,2.68,0.573466342,overige,3,,0.0001
-108394,m-Cresol,m-Cresol,108.1166641,6321.665372,1.96,0.517742126,overige,3,,0.001
- 74-82-8 ,Methaan,Methane,16.05,26000,1.09,,Alk,1,,
-67-56-1,Methanol,Methanol,32,1056000,-0.7,,O2,3,,
-100-66-3,Methoxybenzeen,methoxybenzene,108.14,1040,2.11,,O2,3,,
-,Methoxybenzene,Methoxybenzene,108.14,1741,2.11,,O2,3,109.3,
-,methoxychlor,methoxychlor,345.7,0.173260427,5.1,,overige,3,260.5,
-000108-10-1,Methyl iso-Buthyl Ketone,Methyl isobutyl ketone (MIBK),100.16,19000,1.31,,O2,3,125.8,
-1634-04-4,Methyl tert-butyl ether {MTBE},Methyl tert-butyl ether,88.15,51000,0.94,-0.043843695,O2,3,,0.001
-78-93-3,Methylethylketon {Butanone},2-Butanone,72,352800,0.2755,,O2,3,90.2,
-,Methyl-octacosanate,Methyl-octacosanate,438,,,,onbekend,3,,
-,Methyl-tricosanante,Methyl-tricosanante,368,,,,onbekend,3,,
-,me-triclosan,me-triclosan,303.6,2.411580521,5.4,,overige,3,214.2,
-,Minerale olie (C10),10,122,0.1,5.28,4.164492244,Alk,1,,0.001
-,Minerale olie (C10-C12),Mineral oil (C10-C12),132,0.028183829,5.73,,Alk,1,,
-,Minerale olie (C11),11,134,0.028183829,5.73,4.164492244,Alk,1,,0.001
-,Minerale olie (C12),12,146,0.007943282,6.18,4.164492244,Alk,1,,0.001
-,Minerale olie (C12-C16),Mineral oil (C12-C16),168,0.000630957,7.08,,Alk,1,,
-,Minerale olie (C13),13,158,0.002238721,6.63,5.463590432,Alk,1,,0.001
-,Minerale olie (C14),14,170,0.000630957,7.08,5.463590432,Alk,1,,0.001
-,Minerale olie (C15),15,182,0.000177828,7.53,5.463590432,Alk,1,,0.001
-,Minerale olie (C16),16,194,5.01E-05,7.98,5.463590432,Alk,1,,0.001
-,Minerale olie (C16-C21),Mineral oil (C16-C21),300,2.11E-06,9.105,,Alk,1,,
-,Minerale olie (C17),17,206,1.41E-05,8.43,7.763487393,Alk,1,,0.001
-,Minerale olie (C18),18,218,3.98E-06,8.88,7.763487393,Alk,1,,0.001
-,Minerale olie (C19),19,230,1.12E-06,9.33,7.763487393,Alk,1,,0.001
-,Minerale olie (C20),20,242,3.16E-07,9.78,7.763487393,Alk,1,,0.001
-,Minerale olie (C21),21,254,8.91E-08,10.23,7.763487393,Alk,1,,0.001
-,Minerale olie (C21-C30),Mineral oil (C21-C30),390,5.62E-10,12.03,,Alk,1,,
-,Minerale olie (C22),22,266,2.51E-08,10.68,,Alk,1,,0.001
-,Minerale olie (C23),23,278,7.08E-09,11.13,,Alk,1,,0.001
-,Minerale olie (C24),24,290,2.00E-09,11.58,,Alk,1,,0.001
-,Minerale olie (C25),25,302,5.62E-10,12.03,,Alk,1,,0.001
-,Minerale olie (C26),26,314,1.58E-10,12.48,,Alk,1,,0.001
-,Minerale olie (C27),27,326,4.47E-11,12.93,,Alk,1,,0.001
-,Minerale olie (C28),28,338,1.26E-11,13.38,,Alk,1,,0.001
-,Minerale olie (C29),29,350,3.55E-12,13.83,,Alk,1,,0.001
-,Minerale olie (C30),30,362,1.00E-12,14.28,,Alk,1,,0.001
-,Minerale olie (C31),31,374,2.82E-13,14.73,,Alk,1,,0.001
-,Minerale olie (C32),32,386,7.94E-14,15.18,,Alk,1,,0.001
-,Minerale olie (C33),33,398,2.24E-14,15.63,,Alk,1,,0.001
-,Minerale olie (C34),34,410,6.31E-15,16.08,,Alk,1,,0.001
-,Minerale olie (C35),35,422,1.78E-15,16.53,,Alk,1,,0.001
-,Minerale olie (C36),36,434,5.01E-16,16.98,,Alk,1,,0.001
-,Minerale olie (C37),37,446,1.41E-16,17.43,,Alk,1,,0.001
-,Minerale olie (C38),38,458,3.98E-17,17.88,,Alk,1,,0.001
-,Minerale olie (C39),39,470,1.12E-17,18.33,,Alk,1,,0.001
-,Minerale olie (C40),40,482,3.16E-18,18.78,,Alk,1,,0.001
- 99-09-2,m-Nitroaniline,3-Nitroaniline,138.13,1200,1.37,,overige,3,,
-,Monochlooranilinen,Monochlooranilinen,127.6,3470,1.88,1.308827992,Cl,3,,0.001
-108-90-7,Monochloorbenzeen,Chlorobenzene,112.5899987,507.425862,2.89,1.112564971,ClArom,1,,0.001
- 108-38-3 ,m-Xyleen,m-Xylene,106.1899991,197.4065205,3.2,1.181562839,MAK,1,,0.001
-91-20-3,Naftaleen,Naphthalene,128.19,31.8,3.3,1.745433577,PAK,1,124.6,0.001
-,naphthalene,naphthalene,128,,3.3,,PAK,1,128.2,
-106-97-8,n-Butaan {Butaan},Butane,58.12,61,2.89,,Alk,1,,
-,n-Decanal,n-Decanal,156,,,,O2,3,,
-,n-Dodecane,n-Dodecane,170,,,,Alk,1,,
- 75-83-2 ,Neohexane,Neohexane,86.18,,3.82,,Alk,1,,
-106-97-8,Neopentaan,Neopentane,72.15,33,3.11,,Alk,1,,
-98-95-3,Nitrobenzeen,Nitrobenzene,123.11,2026.666667,1.845,,overige,3,,
-100-61-8,n-Methylaniline,N-Methylaniline,107.16,5620,1.66,,overige,3,,
-,n-Nonanal,n-Nonanal,142,,,,O2,3,,
-,n-nonylphenol,n-nonylphenol,220.4,1.104616663,4.5,,overige,3,238.8,
-,n-nonylphenol-tech,n-nonylphenol-tech,,,,,overige,3,,
-,n-Octanal,n-Octanal,128,,,,O2,3,,
-,n-octylphenol,n-octylphenol,206.3,5.182021708,4,,overige,3,222.3,
-111842,nonaan,Nonane ,128.25,0.22,5.65,,,,,
-,nonylphenol-d4,nonylphenol-d4,,,,,overige,3,,
-109-66-0,n-Pentaan,Pentane,72.15,39.25,3.42,,Alk,1,,
-109-66-0,n-Pentane,n-Pentane,72.15,40,3.39,,Alk,1,,
-,n-Tetradecane,n-Tetradecane,198,,,,Alk,1,,
-,"o,p’-DDD","o,p’-DDD",320.1,0.3201,6.8,3.943475106,overige,3,224.8,0.0001
-,"o,p’-DDE","o,p’-DDE",318,0.400338281,7.1,4.1134711,overige,3,221.1,0.0001
-,"o,p’-DDT","o,p’-DDT",354.5,0.177670874,6.4,4.343467663,overige,3,237.7,0.0001
-95-49-8,o-Chloortolueen,o-Chlorotoluene,126.586,154,3.2,,ClArom,1,,
-95487,o-Cresol,o-Cresol,108.1166641,14858.86058,1.95,0.399094472,overige,3,,0.001
-111-65-9,Octaan,Octane,114.23,0.7,5.15,,Alk,1,,
-,octylphenol-d17,octylphenol-d17,,,,,overige,3,,
- 95-47-6 ,o-Xyleen,o-Xylene,106.186665,218.9335957,3.12,0.956771645,MAK,1,,0.001
-,"p,p’-DDD","p,p’-DDD",320.1,0.804054847,6.3,,overige,3,227.1,
-,"p,p’-DDE","p,p’-DDE",318,0.252596379,6.9,,overige,3,222.4,
-,"p,p’-DDMU","p,p’-DDMU",283.6,,6.2,,overige,3,210.4,
-,"p,p’-DDT","p,p’-DDT",354.5,0.141128992,6.4,,overige,3,240.1,
-,PCB 1,PCB 1,,,4.46,,PCB,2,163.2,
-,PCB 10,PCB 10,223.1,1.772146292,4.85,,PCB,2,223.1,
-,PCB 100,PCB 100,,,6.23,,PCB,2,212.1,
-,PCB 101,PCB 101,325.1617,0.057913166,6.316,4.293468622,PCB,2,212.15,0.0001
-,PCB 103,PCB 103,,,6.22,,PCB,2,212,
-,PCB 104,PCB 104,326.4,0.205944477,5.85,,PCB,2,360.9,
-,PCB 105,PCB 105,326.4,0.025926874,6.716666667,,PCB,2,209.9,
-,PCB 107,PCB 107,,,6.71,,PCB,2,210.5,
-,PCB 110,PCB 110,326.4,0.03264,6.526666667,,PCB,2,209.7,
-,PCB 118,PCB 118,341.3406,0.032261293,6.5081,5.113463578,PCB,2,210.25,0.0001
-,PCB 119,PCB 119,,,6.58,,PCB,2,210.75,
-,PCB 128,PCB 128,360.9,0.018087847,6.746666667,,PCB,2,222.6,
-,PCB 129,PCB 129,360.9,0.018087847,6.75,,PCB,2,360.9,
-,PCB 132,PCB 132,,,6.58,,PCB,2,222.65,
-,PCB 134,PCB 134,,,6.55,,PCB,2,222.2,
-,PCB 135,PCB 135,,,6.64,,PCB,2,222.9,
-,PCB 136,PCB 136,,,6.22,,PCB,2,221.7,
-,PCB 137,PCB 137,360.9,0.014367688,6.85,,PCB,2,360.9,
-,PCB 138,PCB 138,360.3746,0.017903781,6.7341,4.473466391,PCB,2,223.25,0.0001
-,PCB 14,PCB 14,223.1,0.560401863,5.3,,PCB,2,,
-,PCB 141,PCB 141,360.9,0.014367688,6.84,,PCB,2,223.55,
-,PCB 143,PCB 143,360.9,0.022771251,6.65,,PCB,2,,
-,PCB 145,PCB 145,360.9,0.072009017,6.3,,PCB,2,,
-,PCB 146,PCB 146,,,6.89,,PCB,2,223.7,
-,PCB 149,PCB 149,360.9,0.022771251,6.75,,PCB,2,360.9,
-,PCB 151,PCB 151,360.9,0.022771251,6.646666667,,PCB,2,223.15,
-,PCB 153,PCB 153,374.6501,0.012145224,6.9036,4.63346528,PCB,2,223.75,0.0001
-,PCB 155,PCB 155,360.9,0.01141266,6.67,,PCB,2,223.85,
-,PCB 156,PCB 156,360.9,0.00571988,7.226666667,,PCB,2,222.05,
-,PCB 158,PCB 158,,,7.02,,PCB,2,221.6,
-,PCB 16,PCB 16,,,5.16,,PCB,2,187.4,
-,PCB 163,PCB 163,,,6.99,,PCB,2,221.5,
-,PCB 170,PCB 170,395.3,0.004976532,7.35,,PCB,2,360.9,
-,PCB 171,PCB 171,,,7.11,,PCB,2,234.1,
-,PCB 172,PCB 172,,,7.33,,PCB,2,235.1,
-,PCB 174,PCB 174,,,7.11,,PCB,2,234,
-,PCB 177,PCB 177,,,7.08,,PCB,2,234,
-,PCB 178,PCB 178,,,7.14,,PCB,2,234.7,
-,PCB 18,PCB 18,257.5,0.814286497,5.246666667,,PCB,2,188.35,
-,PCB 180,PCB 180,395.3,0.006265083,7.3,4.753464668,PCB,2,360.9,0.0001
-,PCB 183,PCB 183,,,7.2,,PCB,2,234.6,
-,PCB 185,PCB 185,,,7.11,,PCB,2,234.4,
-,PCB 187,PCB 187,395.3,0.006265083,7.25,,PCB,2,235,
-,PCB 192,PCB 192,,,7.52,,PCB,2,234,
-,PCB 194,PCB 194,429.8,,7.8,,PCB,2,246.55,
-,PCB 195,PCB 195,,,7.56,,PCB,2,245.5,
-,PCB 197,PCB 197,,,7.3,,PCB,2,245.6,
-,PCB 199,PCB 199,,,7.2,,PCB,2,246.2,
-,PCB 201,PCB 201,,,7.62,,PCB,2,245.5,
-,PCB 202,PCB 202,,,7.24,,PCB,2,245.3,
-,PCB 204,PCB 204,429.8,0.004298,7.35,,PCB,2,246.5,
-,PCB 205,PCB 205,,,8,,PCB,2,244.8,
-,PCB 206,PCB 206,,,8.09,,PCB,2,257.4,
-,PCB 207,PCB 207,,,7.74,,PCB,2,257,
-,PCB 208,PCB 208,,,7.71,,PCB,2,256.9,
-,PCB 21,PCB 21,257.5,0.324173294,5.55,,PCB,2,257.5,
-,PCB 22,PCB 22,,,5.58,,PCB,2,186.8,
-,PCB 24,PCB 24,,,5.35,,PCB,2,186.1,
-,PCB 25,PCB 25,,,5.67,,PCB,2,187.6,
-,PCB 26,PCB 26,,,5.66,,PCB,2,187.4,
-,PCB 27,PCB 27,,,5.44,,PCB,2,186.6,
-,PCB 28,PCB 28,257.5,0.20453952,5.65,3.373509124,PCB,2,257.5,0.0001
-,PCB 29,PCB 29,257.5,0.324173294,5.633333333,,PCB,2,187.5,
-,PCB 3,PCB 3,,,4.69,,PCB,2,162.4,
-,PCB 30,PCB 30,257.5,0.408109997,5.45,,PCB,2,257.5,
-,PCB 31,PCB 31,257.5,0.20453952,5.75,,PCB,2,292,
-,PCB 32,PCB 32,,,5.44,,PCB,2,186.6,
-,PCB 37,PCB 37,,,5.83,,PCB,2,185.8,
-,PCB 4,PCB 4,223.1,2.808662594,4.7,,PCB,2,,
-,PCB 40,PCB 40,,,5.66,,PCB,2,199,
-,PCB 41,PCB 41,,,5.69,,PCB,2,199.2,
-,PCB 42,PCB 42,,,5.76,,PCB,2,199.8,
-,PCB 43,PCB 43,,,5.75,,PCB,2,199.9,
-,PCB 44,PCB 44,292,0.231943845,5.783333333,,PCB,2,199.95,
-,PCB 45,PCB 45,,,5.53,,PCB,2,198.8,
-,PCB 46,PCB 46,,,5.53,,PCB,2,198.8,
-,PCB 47,PCB 47,292,0.146346672,5.9,,PCB,2,292,
-,PCB 49,PCB 49,292,0.146346672,5.9,,PCB,2,292,
-,PCB 50,PCB 50,292,0.292,5.65,,PCB,2,292,
-,PCB 51,PCB 51,,,5.63,,PCB,2,199.6,
-,PCB 52,PCB 52,292,0.116247294,5.85,3.463500793,PCB,2,,0.0001
-,PCB 55,PCB 55,292,0.073347084,6.15,,PCB,2,292,
-,PCB 56,PCB 56,292,0.073347084,6.136666667,,PCB,2,198.35,
-,PCB 6,PCB 6,,,5.06,,PCB,2,175.2,
-,PCB 60,PCB 60,,,6.11,,PCB,2,198.5,
-,PCB 63,PCB 63,,,6.17,,PCB,2,199.2,
-,PCB 64,PCB 64,,,5.95,,PCB,2,198.3,
-,PCB 66,PCB 66,292,0.05826166,6.25,,PCB,2,,
-,PCB 69,PCB 69,292,0.092338508,6.046666667,,PCB,2,199.2,
-,PCB 71,PCB 71,,,5.98,,PCB,2,198,
-,PCB 74,PCB 74,292,,6.2,,PCB,2,199.25,
-,PCB 77,PCB 77,,,6.36,,PCB,2,197.2,
-,PCB 78,PCB 78,292,0.036760622,6.4,,PCB,2,326.4,
-,PCB 8,PCB 8,223.1,1.407665836,5.1,,PCB,2,,
-,PCB 81,PCB 81,,,6.36,,PCB,2,197.6,
-,PCB 82,PCB 82,,,6.2,,PCB,2,210.8,
-,PCB 83,PCB 83,,,6.26,,PCB,2,211.5,
-,PCB 85,PCB 85,326.4,0.051730914,6.333333333,,PCB,2,211.85,
-,PCB 87,PCB 87,326.4,0.051730914,6.33,,PCB,2,211.7,
-,PCB 89,PCB 89,,,6.07,,PCB,2,210.5,
-,PCB 91,PCB 91,,,6.13,,PCB,2,211.2,
-,PCB 97,PCB 97,326.4,0.051730914,6.33,,PCB,2,211.45,
-,PCB 99,PCB 99,326.4,0.041091325,6.45,,PCB,2,326.4,
-106-48-9,p-Chloorfenol,P-chlorophenol,128.56,25500,2.27,,Cl,3,,
-106-43-4,p-Chloortolueen,p-Chlorotoluene,126.586,123,3.33,,ClArom,1,,
-106445,p-Cresol,p-Cresol,108.1099991,28640.96526,1.94,0.444357034,overige,3,,0.001
-608-93-5,Pentachloorbenzeen,Pentachlorobenzene,250.1297785,0.322818462,5.076666667,2.683710051,ClArom,1,,0.001
-87-86-5,Pentachloorfenol,Pentachlorophenol,266.33,4.28,5.12,1.964642345,Cl,3,,0.001
-110-62-3,Pentanal,Pentanal,86.13,14000,1.31,,O2,3,,
-,Pentylbenzeen,Penthylbenzene,148.25,3.37,4.9,,MAK,1,,
-,perylene,perylene,252.15,0.026200963,6.175,,PAK,1,219.45,
-,phenanthrene,phenanthrene,178.1,4.350184731,4.48,,PAK,1,160.35,
- 74-98-6 ,Propaan,Propane,44.1,75,2.36,,Alk,1,,
-107-12-0,Propionitrile,Propionitrile,55.08,103000,0.16,,overige,3,,
- 103-65-1,Propylbenzeen,Propylbenzene,120.19,54.00633333,3.71,,MAK,1,,
-115-07-1,Propylene (Propeen??),Propylene,42.08,292,1.77,,Alk,1,,
-,p-Xyleen,p-Xylene,106.186665,210.9384616,3.15,1.428036212,MAK,1,123.9,0.001
-,pyrene,pyrene,202.15,0.836365063,4.94,,PAK,1,182.1,
-110861,pyridine,pyridine,79.1,665483.58,0.65,0.714917304,overige,3,,0.0001
-100-42-5,Styrene,Styrene,104.1485645,320.0573505,2.95,1.348594147,MAK,1,,0.001
-634-66-2,Tetrachloorbenzeen,Tetrachlorobenzene,216,4.16,4.6,2.51,ClArom,1,,
-127-18-4,Tetrachlooretheen,Tetrachloroethylene,165.8074995,118.8825037,3.4,1.194834616,ClAlk,1,,0.01
-56-23-5,Tetrachloormethaan,Tetrachloromethane,153.82,800,2.83,0.558949208,ClAlk,1,,0.001
-,Tetradecanol,Tetradecanol,214,,,,O2,3,,
- 75-73-0 ,Tetrafluoromethane,Tetrafluoromethane,88.01,20,1.18,,overige,3,,
-,tetrahydrofuran,tetrahydrofuran,72.10666651,405634.1962,0.47,-0.375336937,O2,3,,0.0001
-110010,tetrahydrothiophene,tetrahydrothiophene,88.17499986,12894.97733,1.61,0.232488206,overige,3,,0.0001
-,t-octylphenol,t-octylphenol,206.3,25.97163125,4.1,,overige,3,219.5,
-108-88-3,Tolueen,Toluene,92.14249285,610.5910523,2.73,0.870272715,MAK,1,106.9,0.001
-,Tribroommethaan,Tribromomethane,252.8,1719,2.67,0.946079776,overige,3,,0.0001
-79-01-6,Trichlooretheen,Trichloroethylene,131.4,1164.844161,2.61,0.842372721,ClAlk,1,,0.01
-,triclosan,triclosan,289.5,11.52520259,4.8,,overige,3,192.1,
-,UV1,UV1,214,,,,overige,3,,
-,UV10,UV10,585,,,,overige,3,,
-,UV2,UV2,258,,,,overige,3,,
-,UV3,UV3,326,,,,overige,3,,
-,UV4,UV4,332,,,,overige,3,,
-,UV5,UV5,346,,,,overige,3,,
-,UV6,UV6,388,,,,overige,3,,
-,UV7,UV7,388,,,,overige,3,,
-,UV8,UV8,445,,,,overige,3,,
-,UV9,UV9,551,,,,overige,3,,
-75-01-4,Vinylchloride,Vinyl chloride,62.5,428,1.52,0.734988789,ClAlk,1,,0.0001
-13-30-2-07,Xyleen,Xylene,120.208888,,3.74,,MAK,1,,
+CAS_number,chemical_name_NL,chemical_name_EN,molecular_weight,solubility,log_octanol_water_partitioning_coefficient,log_distribution_coefficient,chemical_group,chemical_group_number,molecular_volume,Drinking_water_norm
+,,,M,Cwsat,LOG Kow,LOG Kd,group,,Vm,
+,,,g/mol,g/m3,(-),(-),,,cm3/mol,g/m3
+66-25-1, Hexaldehyde, Hexaldehyde,100.16,6000,1.78,,overige,3,,
+71-55-6,"1,1,1-Trichloorethaan","1,1,1-Trichloroethane",133.4,2343.333333,2.8,0.760444292,ClAlk,1,,0.001
+79-34-5,"1,1,2,2-Tetrachloorethaan","1,1,2,2-Tetrachloroethane",167.85,2900,2.39,,ClAlk,1,,
+79-00-5,"1,1,2-Trichloorethaan","1,1,2-Trichloroethane",133.4,3055,1.89,0.753447145,ClAlk,1,,0.001
+75342,"1,1-Dichloorethaan","1,1-Dichloroethane",98.96499987,5223.690293,1.79,0.360665595,ClAlk,1,,0.001
+,"1,1-dichlooretheen","1,1-dichlooretheen",97,1824,2.13,0.589733613,ClAlk,1,,0.001
+,"1,2,3,4-tetrachlorobenzene","1,2,3,4-tetrachlorobenzene",215.9,3.399273364,4.64,2.67369577,ClArom,1,,0.001
+,"1,2,3,5-tetrachlorobenzene","1,2,3,5-tetrachlorobenzene",215.9,2.614957562,4.66,2.333981434,ClArom,1,,0.001
+87-61-6,"1,2,3-Trichloorbenzeen","1,2,3-Trichlorobenzene",181.439995,13.62398701,4.14,1.994666142,ClArom,1,,0.001
+96184,"1,2,3-trichloorpropaan","1,2,3-trichloropropane",147.43,1750,2.27,,,,,
+526738,"1,2,3-trimethylbenzeen","1,2,3-trimethylbenzene",120.19,75.2,3.66,,,,,
+,"1,2,3-Trimethylbenzene","1,2,3-Trimethylbenzene",120.19,75,3.6,,MAK,1,139.6,
+,"1,2,4,5-tetrachlorobenzene","1,2,4,5-tetrachlorobenzene",215.9,0.68248085,4.6,2.533894299,ClArom,1,,0.001
+120-82-1,"1,2,4-Trichloorbenzeen","1,2,4-Trichlorobenzene",181.439995,28.80802015,4.05,2.044515105,ClArom,1,,0.001
+95636,"1,2,4-trimethylbenzeen","1,2,4-trimethylbenzene",120.19,57,3.78,,,,,
+95-50-1,"1,2-Dichloorbenzeen","1,2-Dichlorobenzene",147.0024999,140.218586,3.43,1.36831917,ClArom,1,,0.001
+107-06-2,"1,2-Dichloorethaan","1,2-Dichloroethane",98.97333154,10188.83247,1.47,0.311244667,ClAlk,1,79.4,0.003
+156-59-2,"1,2-Dichlooretheen(cis)","1,2-dichloro-, (Z)-Ethene",96.95,775.6,1.906666667,0.625232261,ClAlk,1,,0.001
+540-59-0,"1,2-dichlooretheen(cisentrans)","1,2-dichloroEthene",96.95,775.6,1.27,,ClAlk,1,,
+156-60-5,"1,2-dichlooretheen(trans)","1,2-dichloro-, (1E)-Ethene",96.95,581.7,1.09,0.627641144,ClAlk,1,,0.001
+,"1,2-Dichloorfenol","1,2-Dichloorphenol",163,904.5313384,2.84,1.436666667,Cl,3,,
+78-87-5,"1,2-dichloorpropaan","1,2-Dichloropropane",113,1469,1.99,0.392478925,ClAlk,1,,0.001
+,"1,2-dimethylnaphthalene","1,2-dimethylnaphthalene",156,,4.31,,PAK,1,154.2,
+108-70-3,"1,3,5-Trichloorbenzeen","1,3,5-Trichlorobenzene",181.4249983,4.711953407,4.19,2.744256831,ClArom,1,,0.001
+108-67-8,"1,3,5-Trimethylbenzeen","1,3,5-Trimethylbenzene",120.19,11.45,3.51,,MAK,1,,
+541-73-1,"1,3-Dichloorbenzeen","1,3-Dichlorobenzene",147,114.3333333,3.4,1.546462047,ClArom,1,,0.001
+,"1,3-dichloorpropaan","1,3-dichloropropane",113,1469,1.99,0.392478925,ClAlk,1,,0.001
+,"1,3-dimethylnaphthalene","1,3-dimethylnaphthalene",156,,4.42,,PAK,1,155.8,
+,"1,4,6,7-tetramethylnaphthalene","1,4,6,7-tetramethylnaphthalene",184,,5.36,,PAK,1,186,
+106-46-7,"1,4-Dichloorbenzeen","1,4-Dichlorobenzene",147.0019999,60.52630716,3.44,1.586462047,ClArom,1,,0.001
+,"1,4-dimethylnaphthalene","1,4-dimethylnaphthalene",156,,4.37,,PAK,1,155.6,
+123-91-1,"1,4-Dioxane {p-dioxane} ","1,4-Dioxane ",88.11,1000000,-0.27,,overige,3,,
+,"1,8-dimethylnaphthalene","1,8-dimethylnaphthalene",156,,4.32,,PAK,1,155.6,
+71-36-3,1-Butanol,1-Butanol,74.12,63200,0.88,,O2,3,,
+109693,1-chloorbutaan,1-chlorobutane,92.57,0.87,2.39,,,,,
+90131,1-chloornaftaleen,1-chloornaphthalene,162.6059998,16.80146852,4.1,2.18418207,Cl,3,,0.001
+,1-Chloronaphthalene,1-Chloronaphthalene,162.62,17.4,4,,ClArom,1,137.7,
+ 111-27-3 ,1-Hexanol {Hexylalcohol},1-Hexanol,102.18,5900,2.03,,O2,3,,
+,1-methylfluorene,1-methylfluorene,180,,4.97,,PAK,1,169.4,
+,1-methylnaphthalene,1-methylnaphthalene,142,,3.87,,PAK,1,139.9,
+,1-methylphenanthrene,1-methylphenanthrene,192,,5.08,,PAK,1,175.9,
+,1-methylpyrene,1-methylpyrene,216,,5.48,,PAK,1,197.7,
+71-41-0,1-Pentanol,1-Pentanol,88.15,22000,1.51,,O2,3,,
+,2-(2-Hydroxy-3.t-butyl-5-methylphenyl-5-Chloro-benztriazol (Tinuvin 326),2-(2-Hydroxy-3.t-butyl-5-methylphenyl-5-Chloro-benztriazol,315.8,,,,overige,3,,
+25167-70-8,"2,2,4-Trimethylpentaan","2,2,4-Trimethylpentane",112.21,14.2,4.37,,Alk,1,,
+15950-66-0,"2,3,4-Trichloorfenol","2,3,4-Trichlorophenol",197.5,71.1,3.8,1.845017825,Cl,3,,0.001
+,"2,3,5,6,-Tetramethyl-phenol","2,3,5,6,-Tetramethyl-phenol",150,,,,overige,3,,
+935-95-5,"2,3,5,6-Tetrachloorfenol","2,3,5,6-Tetrachlorophenol",231.9,4.79,3.88,2.10431794,Cl,3,,0.001
+,"2,3,5-trimethylnaphthalene","2,3,5-trimethylnaphthalene",170,,4.81,,PAK,1,170.2,
+,"2,3,6-trimethylnaphthalene","2,3,6-trimethylnaphthalene",170,,4.73,,PAK,1,170.3,
+,"2,3,7-TriCDD","2,3,7-TriCDD",287.5,0.14409133,6.1,,overige,3,179.9,
+,"2,3-Benzopyrole (Indole)","2,3-Benzopyrole",117,,,,onbekend,3,,
+,"2,3-Dichloor-5-nitrotolueen","2,3-Dichloor-5-nitrotolueen",,,,,Cl,3,,
+88-06-2,"2,4,6-Trichloorfenol","2,4,6-Trichlorophenol",197.46,243,3.695,2.234096671,Cl,3,,0.001
+,"2,4-dichloorfenol","2,4-dichloorphenol",163,1907.107928,3.06,1.308828347,ClAlk,1,,0.001
+,"2,5-dichloorfenol","2,5-dichloorphenol",163,420.9082483,3.06,1.596225694,ClAlk,1,,0.001
+,"2,6-dichloorfenol","2,6-dichloorphenol",163,534.106534,2.75,1.397831352,ClAlk,1,,0.001
+,"2,6-dimethylnaphthalene","2,6-dimethylnaphthalene",156,,4.31,,PAK,1,155.9,
+,"2,6-Di-tert-butyl-4-methyl-phenol (BHT)","2,6-Di-tert-butyl-4-methyl-phenol",220,,,,overige,3,,
+,"2,7/8-DiCDD","2,7/8-DiCDD",253.1,0.201044476,5.6,,overige,3,168.5,
+,2-CDD,2-CDD,218.6,1.736401521,5.2,,overige,3,156.4,
+95-51-2,2-Chlooraniline,2-Chloroaniline,127.57,8160,1.9,,Cl,3,,
+,2-chloorfenol,2-chloorphenol,128.5899988,8708.954334,2.15,0.398828347,ClAlk,1,,0.001
+91587,2-chloornaftaleen,2-chloornaphthalene,162.6099997,9.71436827,4.14,2.184177182,Cl,3,,0.001
+,2-ethylanthracene,2-ethylanthracene,206,,5.85,,PAK,1,191.2,
+ 626-93-7,2-Hexanol,2-Hexanol,102.18,14350,1.76,,O2,3,,
+,2-Hydroxy-4-ethandiol methyl-thioacetic acid ester,2-Hydroxy-4-ethandiol methyl-thioacetic acid ester,346,,,,overige,3,,
+,2-Methoxy-4-propenyl-phenol,2-Methoxy-4-propenyl-phenol,164,,,,overige,3,,
+,2-methylanthracene,2-methylanthracene,192.15,1.661036915,4.85,,PAK,1,174.8,
+,2-methylnaphthalene,2-methylnaphthalene,167.15,1.661036915,4.28,,PAK,1,158.25,
+,2-methylphenanthrene,2-methylphenanthrene,192,,5.01,,PAK,1,176,
+6032-29-7,2-Pentanol,2-Pentanol,88.15,166000,1.25,,O2,3,,
+,2-Phenly-ehtyl-alcohol,2-Phenly-ehtyl-alcohol,122,,,,O2,3,,
+67-63-0,2-Propanol {isopropyl alcohol},2-Propanol,60.1,1000000,0.05,,O2,3,,
+,"3-(3,5-di-tert-butyl-4-hydroxy phenyl)-propionate (Irganox 1076)","3-(3,5-di-tert-butyl-4-hydroxy phenyl)-propionate",531,,,,onbekend,3,,
+609-19-8,"3,4,5-Trichloorfenol","3,4,5-Trichlorophenol",197.45,34.6,4.01,2.304002415,Cl,3,,0.001
+,"3,6-dimethylphenanthrene","3,6-dimethylphenanthrene",206.15,0.635183529,5.17,,PAK,1,192.2,
+,"3,7-Dimehtyl-octane-3-ol","3,7-Dimehtyl-octane-3-ol",158,,,,O2,3,,
+,"3,7-Dimethyl-6-octene-al","3,7-Dimethyl-6-octene-al",154,,,,O2,3,,
+108-42-9,3-Chlooraniline,3-Chloroaniline,127.57,5400,1.88,,Cl,3,,
+,3-chloorfenol,3-chloorphenol,128.5899988,7969.660322,2.5,0.748828347,ClAlk,1,,0.001
+ 96-14-0 ,3-Methylpentane,3-Methylpentane,86.18,18,3.6,,Alk,1,,
+,3-Octene-2-one,3-Octene-2-one,126,,,,O2,3,,
+,3-Phenyl-1-propanol,3-Phenyl-1-propanol,136,,,,O2,3,,
+106-47-8,4-Chlooraniline,4-Chloroaniline,127.57,3900,1.83,,Cl,3,,
+,4-chloorfenol,4-chloorphenol,128.5899988,7667.192707,2.39,0.638828347,ClAlk,1,,0.001
+,4-Isopropenyl-1-methyl-1-cyclohexene (Limonene),4-Isopropenyl-1-methyl-1-cyclohexene,136,,,,overige,3,,
+,4-Isopropyl-tuluene,4-Isopropyl-tuluene,134,,,,MAK,1,,
+,6-methylchrysene,6-methylchrysene,242,,6.07,,PAK,1,211.9,
+,"7,12-dimethylbenz[a]anthracene","7,12-dimethylbenz[a]anthracene",256,,6.62,,PAK,1,226,
+,7-methylbenz[a]anthracene,7-methylbenz[a]anthracene,242,,6.07,,PAK,1,210.3,
+,7-Methyl-chinoline,7-Methyl-chinoline,143,,,,onbekend,3,,
+,"9,10-dimethylanthracene","9,10-dimethylanthracene",206.15,0.635183529,5.295,,PAK,1,190.15,
+,9-methylanthracene,9-methylanthracene,192,,5.07,,PAK,1,174.3,
+,acenaphthene,acenaphthene,154.1,22.06400634,3.96,,PAK,1,141.8,
+,acenaphthylene,acenaphthylene,152.2,,3.9,,PAK,1,223.1,
+67-64-1,Acetone,Acetone,58.08,790000,-0.24,,O2,3,74,
+75-05-8,Acetonitrile,Acetonitrile,41.05,1000000,-0.34,,overige,3,,
+,aldrin,aldrin,364.9,0.916587359,6.3,2.7036797,overige,3,240.1,0.00003
+463-49-0,Allene,Allene,40.065,,1.45,,Alk,1,,
+62-53-3,Aniline,Anilin,93.13,35333.33333,0.988,,overige,3,,
+,Antraceen,anthracene,178.1,4.350184731,4.525,3.063556603,PAK,1,158.9,0.0001
+1912249,atrazine,atrazine,215.6966666,38.13236662,2.61,0.975115324,overige,3,,0.0001
+,BDE-1,BDE-1,249.1,2.491,4.6,,BDE,3,174.7,
+,BDE-100,BDE-100,564.7,0.014184623,7.3,,BDE,3,232,
+,BDE-126,BDE-126,564.7,0.011267246,7.4,,BDE,3,233.7,
+,BDE-15,BDE-15,328,0.519844967,5.2,,BDE,3,189.9,
+,BDE-153,BDE-153,643.6,0.004060841,8,,BDE,3,246.6,
+,BDE-154,BDE-154,643.6,0.004060841,8,,BDE,3,246.5,
+,BDE-17,BDE-17,406.9,0.203933085,5.8,,BDE,3,202.1,
+,BDE-2,BDE-2,249.1,1.978671633,4.5,,BDE,3,173,
+,BDE-28,BDE-28,406.9,0.161989808,5.8,,BDE,3,203.8,
+,BDE-47,BDE-47,485.8,0.04858,6.5,,BDE,3,217.6,
+,BDE-66,BDE-66,485.8,0.04858,6.5,,BDE,3,218.2,
+,BDE-71,BDE-71,485.8,0.04858,6.6,,BDE,3,217,
+,BDE-85,BDE-85,564.7,0.014184623,7.2,,BDE,3,231.6,
+,BDE-99,BDE-99,564.7,0.014184623,7.2,,BDE,3,232.1,
+,benz[a]anthracene,benz[a]anthracene,228.15,0.138965154,5.78,4.553465774,PAK,1,194.9,0.0001
+00-52-7,Benzaldehyde,Benzaldehyde,106.13,6950,1.48,,overige,3,,
+71-43-2,Benzeen,Benzene,78.10666652,1988.898826,2.13,0.659555885,MAK,1,89.4,0.001
+,benzo(a)perylene,benzo(a)perylene,252.3,,,,PAK,1,218.2,
+,"benzo(g,h,i)perylene","benzo(g,h,i)perylene",276.3,0.000186,6.22,5.193463434,PAK,1,241.3,0.0001
+,benzo[a]pyrene,benzo[a]pyrene,252.15,0.026200963,6.115,4.583465572,PAK,1,218.05,0.00001
+,benzo[b]fluoranthene,benzo[b]fluoranthene,252.15,0.026200963,5.84,4.103471294,PAK,1,231.8,0.0001
+,benzo[e]pyrene,benzo[e]pyrene,252.15,0.026200963,6.27,,PAK,1,219.45,
+,benzo[ghi]perylene,benzo[ghi]perylene,276,,6.7,,PAK,1,241,
+,benzo[k]fluoranthene,benzo[k]fluoranthene,252.15,0.026200963,6.005,,PAK,1,229.3,
+100-51-6,Benzyl alcohol,Benzyl alcohol,108.14,42900,1.1,,overige,3,,
+100-44-7,Benzylchloride,Benzyl chloride,126.59,476.5,2.3,,ClArom,1,,
+101-84-8  (= bifenyl oxide ??),bifenly ether,diphenyl ether,170.21,20,4.21,,O2,3,,
+ 92-52-4 ,Bifenyl,Biphenyl,154.21,6.476666667,4.045,,PAK,1,,
+71-36-3,Butylalcohol {Butanol],Butylalcohol ,74.12,77000,0.84,,O2,3,,
+,butylated hydroxyanisol,butylated hydroxyanisol,180.2,,,,overige,3,175.7,
+,butylated hydroxytoluene,butylated hydroxytoluene,220.4,,,,overige,3,235,
+104518,butylbenzeen,butylbenzene,134.22,11.8,4.38,,,,,
+85687,butylbenzylftalaat(BBP),benzyl butyl phthalate (BBP),312.3966666,4.218630438,4.91,2.673692963,overige,3,,0.0001
+,Butyraldehyde,Butyraldehyde,72.11,71000,0.88,,O2,3,89.6,
+123-72-8,Butyraldehyde (butanal),Butyraldehyde,72.11,37000,0.88,,O2,3,,
+63252,carbaryl,carbaryl,201.2066664,81.56328382,2.36,1.043401359,overige,3,,0.0001
+1563662,carbofuran,carbofuran,221.2899993,376.0966593,1.63,0.444356263,overige,3,,0.0001
+,Cedrylacetate,Cedrylacetate,264,,,,overige,3,,
+,Chloordaan,Chlordane,410,0.14,5.8,3.363509843,overige,3,,0.0001
+75-00-3,chloorethaan,Chloroethane,64.515,6710,1.485,,ClAlk,1,,
+540545,chloorpentaan,chloropentane,106.59,197,2.73,,,,,
+,Chlorobenzene,Chlorobenzene,112.56,498,2.84,,ClArom,1,102.2,
+,Chloroform,Chloroform,119.38,7950,1.97,0.465300972,ClAlk,1,,0.001
+,chrysene,chrysene,228.15,0.138965154,5.755,4.483466305,PAK,1,196.3,0.0001
+ 928-96-1 ,cis-Hex-3-en-1-ol,cis-Hex-3-en-1-ol,100.16,19300,1.61,,O2,3,,
+110-82-7,Cyclohexaan,Cyclohexane,84.16,49,3.48,,Alk,1,104.7,
+108941,cyclohexanon,cyclohexanon,98.14499563,18990.75095,0.81,-0.087766146,overige,3,,0.0001
+ 75-19-4 ,Cyclopopane,Cyclopopane,42.08,502000,1.72,,overige,3,,
+,d10-fluoranthene,d10-fluoranthene,212,,,,PAK,1,,
+,d10-fluorene,d10-fluorene,176,,,,PAK,1,,
+,d12-benz[a]anthracene,d12-benz[a]anthracene,228.15,0.138965154,5.78,,PAK,1,,
+,d12-perylene,d12-perylene,264,,,,PAK,1,,
+117817,di(2-ethylhexyl)ftalaat,di(2-ethylhexyl)phthalate,390.5866662,0.045738942,7.45,4.133470728,overige,3,,0.0001
+,dibenz[ah]anthracene,dibenz[ah]anthracene,278,,6.8,,PAK,1,243.8,
+,"dibenzo(a,h)anthracene","dibenzo(a,h)anthracene",278.3,,,,PAK,1,244.2,
+84742,dibuthylftalaat(DBP),dibutyl phthalate,278.35,2.351,4.72,1.745420579,overige,3,,0.0001
+75-09-2,Dichloormethaan / Methyleenchloride,Dichloromethane,84.93,20000,1.25,0.088839633,ClAlk,1,64.5,0.001
+,"Didodecyl-3,3-thio-dipropionate","Didodecyl-3,3-thio-dipropionate",514,,,,onbekend,3,,
+,dieldrin,dieldrin,380.9,4.795246894,5.5,2.753654239,overige,3,253.7,0.00003
+60297,di-ethylether,di-ethylether,74.12,60400,0.89,,,,,
+84662,diethylftalaat(DEP),Diethyl phthalate (DEP),222.24,287.2,2.47,1.407730396,overige,3,,0.0001
+84753,dihexylftalaat(DHP),Dihexyl phthalate (DHP),334.5,0.01151,6.85,3.413505198,overige,3,,0.0001
+,di-isobutylftalaat(DIBP),Diisobutyl phthalate,278.35,9.6,4.46,2.00453864,overige,3,,0.0001
+108-20-3,Di-isopropylether,Diisopropyl ether,102.18,8900,1.52,,O2,3,,
+565-80-0,Di-isopropylketon,Di-isopropylketon,114.18,5700,1.86,,O2,3,,
+,Dimehtyl-phthalate,Dimehtyl-phthalate,194,,,,O2,3,,
+ 67-68-5 ,Dimethyl sulfoxide,Dimethyl sulfoxide,78.14,1000000,-1.35,,overige,3,,
+,Dimethyl-benzyl-carbinol,Dimethyl-benzyl-carbinol,150,,,,onbekend,3,,
+,Dimethylftalaat,dimethylftalaat(DMP),194.19,2014,1.56,,O2,3,,
+131113,dimethylftalaat(DMP),Dimethyl phthalate,194.19,2014,1.56,1.023864247,overige,3,,0.0001
+,Diphenyl-oxide,Diphenyl-oxide,170,,,,overige,3,,
+,Docosane,Docosane,310,,,,onbekend,3,,
+,Eicosane,Eicosane,282,,,,onbekend,3,,
+,endosulfan sulphate,endosulfan sulphate,422.9,,5.1,,overige,3,239.8,
+,endrin,endrin,380.9,1.204511561,5,2.713672709,overige,3,253.7,0.0001
+,endrin aldehyde,endrin aldehyde,380.9,,5.5,,overige,3,253.2,
+,endrin ketone,endrin ketone,364.5,,6.8,,overige,3,,
+,ETBE (Ethyl tert-butyl ether) ,Ethyl tert-butyl ether,102.17476,5030.868137,1.88,,O2,3,,0.001
+74-84-0,Ethane,Ethane,30.07,62,1.81,,Alk,1,,
+64-17-5,Ethanol,Ethanol,46.07,1000000,-0.305,,O2,3,,
+141-78-6 ,Ethylacetaat,Ethylacetaat,88.1,62100,0.73,,O2,3,,
+100-41-4,Ethylbenzeen,Ethylbenzene,106.186665,159.4494297,3.15,1.299931656,MAK,1,,0.001
+74-85-1,Ethylene,Ethylene,28.05,130,1.13,,Alk,1,,
+ 105-37-3 ,Ethylpropionate,Ethylpropionate,102.13,17000,1.21,,O2,3,,
+85-01-8,Fenanthreen,Phenanthrene,178.21,0.85,4.47,2.993573044,PAK,1,,0.0001
+108-95-2,Fenol,Phenol,94.10499987,65559.5567,1.48,0.336603308,O2,3,,0.001
+,fluoranthene,fluoranthene,202.15,0.836365063,5.08,3.943475119,PAK,1,195.85,0.0001
+,fluorene,fluorene,166.1,9.822703148,4.14,,PAK,1,154.6,
+,gasoline,gasoline,,,,,Arom,1,,
+,HCB,HCB,284.8,0.358541957,5.6,,overige,3,161.2,
+142-82-5,Heptaan (n-heptaan),n-Heptane,100.2,2.6,4.58,,Alk,1,,
+,heptachlor,heptachlor,373.3,1.180478251,6,3.213533128,overige,3,230.8,0.00003
+,heptachlor epoxide,heptachlor epoxide,389.3,4.900996628,5.4,1.705641075,overige,3,233.7,0.00003
+53535-33-4,Heptanol,Heptanol,116.21,1940,2.62,,O2,3,,
+110-54-3,Hexaan,Hexane,86.18,23,3.888,,Alk,1,,
+118741,Hexachloorbenzeen,Hexachlorobenzene,284.8,0.0117,5.73,2.823626427,ClArom,1,,0.001
+ 66-25-1 ,Hexaldehyde,Hexaldehyde,100.16,6000,1.78,,O2,3,,
+25264-93-1,Hexene,Hexene,84.16,50,3.07,,Alk,1,,
+,δ-HCH,δ-HCH,290.8,115.7695652,3.9,2.134261869,overige,3,178,0.0001
+98-07-7,"α,α,α-Trichloortolueen",Benzotrichloride,195.475,51.5,2.92,,ClArom,1,,
+,α-endosulfan,α-endosulfan,406.9,2.567365435,4.9,1.874913747,overige,3,236.3,0.0001
+,α-HCH,α-HCH,290.8,91.95903436,3.9,2.09433891,overige,3,178,0.0001
+,β-HCH,β-HCH,290.8,460.8869404,3.9,2.134261869,overige,3,178,0.0001
+,γ-HCH,γ-HCH,290.8,73.04565743,3.8,1.755373969,overige,3,178,0.0001
+,"indeno[1,2,3-cd]pyrene","indeno[1,2,3-cd]pyrene",276,0.000265,6.7,4.783464526,PAK,1,253.4,0.0001
+103651,i-propylbenzeen,i-propylbenzene,120.19,61.3,3.66,,,,,
+115-11-7,Isobutyleen,Isobutylene,56.11,388,2.35,,Alk,1,,
+108-41-8,m-Chloortolueen,mo-Chlorotoluene,126.586,117,3.764,,ClArom,1,,
+,MCPA,MCPA,200.6,622,2.68,0.573466342,overige,3,,0.0001
+108394,m-Cresol,m-Cresol,108.1166641,6321.665372,1.96,0.517742126,overige,3,,0.001
+ 74-82-8 ,Methaan,Methane,16.05,26000,1.09,,Alk,1,,
+67-56-1,Methanol,Methanol,32,1056000,-0.7,,O2,3,,
+100-66-3,Methoxybenzeen,methoxybenzene,108.14,1040,2.11,,O2,3,,
+,Methoxybenzene,Methoxybenzene,108.14,1741,2.11,,O2,3,109.3,
+,methoxychlor,methoxychlor,345.7,0.173260427,5.1,,overige,3,260.5,
+000108-10-1,Methyl iso-Buthyl Ketone,Methyl isobutyl ketone (MIBK),100.16,19000,1.31,,O2,3,125.8,
+1634-04-4,Methyl tert-butyl ether {MTBE},Methyl tert-butyl ether,88.15,51000,0.94,-0.043843695,O2,3,,0.001
+78-93-3,Methylethylketon {Butanone},2-Butanone,72,352800,0.2755,,O2,3,90.2,
+,Methyl-octacosanate,Methyl-octacosanate,438,,,,onbekend,3,,
+,Methyl-tricosanante,Methyl-tricosanante,368,,,,onbekend,3,,
+,me-triclosan,me-triclosan,303.6,2.411580521,5.4,,overige,3,214.2,
+,Minerale olie (C10),10,122,0.1,5.28,4.164492244,Alk,1,,0.001
+,Minerale olie (C10-C12),Mineral oil (C10-C12),132,0.028183829,5.73,,Alk,1,,
+,Minerale olie (C11),11,134,0.028183829,5.73,4.164492244,Alk,1,,0.001
+,Minerale olie (C12),12,146,0.007943282,6.18,4.164492244,Alk,1,,0.001
+,Minerale olie (C12-C16),Mineral oil (C12-C16),168,0.000630957,7.08,,Alk,1,,
+,Minerale olie (C13),13,158,0.002238721,6.63,5.463590432,Alk,1,,0.001
+,Minerale olie (C14),14,170,0.000630957,7.08,5.463590432,Alk,1,,0.001
+,Minerale olie (C15),15,182,0.000177828,7.53,5.463590432,Alk,1,,0.001
+,Minerale olie (C16),16,194,5.01E-05,7.98,5.463590432,Alk,1,,0.001
+,Minerale olie (C16-C21),Mineral oil (C16-C21),300,2.11E-06,9.105,,Alk,1,,
+,Minerale olie (C17),17,206,1.41E-05,8.43,7.763487393,Alk,1,,0.001
+,Minerale olie (C18),18,218,3.98E-06,8.88,7.763487393,Alk,1,,0.001
+,Minerale olie (C19),19,230,1.12E-06,9.33,7.763487393,Alk,1,,0.001
+,Minerale olie (C20),20,242,3.16E-07,9.78,7.763487393,Alk,1,,0.001
+,Minerale olie (C21),21,254,8.91E-08,10.23,7.763487393,Alk,1,,0.001
+,Minerale olie (C21-C30),Mineral oil (C21-C30),390,5.62E-10,12.03,,Alk,1,,
+,Minerale olie (C22),22,266,2.51E-08,10.68,,Alk,1,,0.001
+,Minerale olie (C23),23,278,7.08E-09,11.13,,Alk,1,,0.001
+,Minerale olie (C24),24,290,2.00E-09,11.58,,Alk,1,,0.001
+,Minerale olie (C25),25,302,5.62E-10,12.03,,Alk,1,,0.001
+,Minerale olie (C26),26,314,1.58E-10,12.48,,Alk,1,,0.001
+,Minerale olie (C27),27,326,4.47E-11,12.93,,Alk,1,,0.001
+,Minerale olie (C28),28,338,1.26E-11,13.38,,Alk,1,,0.001
+,Minerale olie (C29),29,350,3.55E-12,13.83,,Alk,1,,0.001
+,Minerale olie (C30),30,362,1.00E-12,14.28,,Alk,1,,0.001
+,Minerale olie (C31),31,374,2.82E-13,14.73,,Alk,1,,0.001
+,Minerale olie (C32),32,386,7.94E-14,15.18,,Alk,1,,0.001
+,Minerale olie (C33),33,398,2.24E-14,15.63,,Alk,1,,0.001
+,Minerale olie (C34),34,410,6.31E-15,16.08,,Alk,1,,0.001
+,Minerale olie (C35),35,422,1.78E-15,16.53,,Alk,1,,0.001
+,Minerale olie (C36),36,434,5.01E-16,16.98,,Alk,1,,0.001
+,Minerale olie (C37),37,446,1.41E-16,17.43,,Alk,1,,0.001
+,Minerale olie (C38),38,458,3.98E-17,17.88,,Alk,1,,0.001
+,Minerale olie (C39),39,470,1.12E-17,18.33,,Alk,1,,0.001
+,Minerale olie (C40),40,482,3.16E-18,18.78,,Alk,1,,0.001
+ 99-09-2,m-Nitroaniline,3-Nitroaniline,138.13,1200,1.37,,overige,3,,
+,Monochlooranilinen,Monochlooranilinen,127.6,3470,1.88,1.308827992,Cl,3,,0.001
+108-90-7,Monochloorbenzeen,Chlorobenzene,112.5899987,507.425862,2.89,1.112564971,ClArom,1,,0.001
+ 108-38-3 ,m-Xyleen,m-Xylene,106.1899991,197.4065205,3.2,1.181562839,MAK,1,,0.001
+91-20-3,Naftaleen,Naphthalene,128.19,31.8,3.3,1.745433577,PAK,1,124.6,0.001
+,naphthalene,naphthalene,128,,3.3,,PAK,1,128.2,
+106-97-8,n-Butaan {Butaan},Butane,58.12,61,2.89,,Alk,1,,
+,n-Decanal,n-Decanal,156,,,,O2,3,,
+,n-Dodecane,n-Dodecane,170,,,,Alk,1,,
+ 75-83-2 ,Neohexane,Neohexane,86.18,,3.82,,Alk,1,,
+106-97-8,Neopentaan,Neopentane,72.15,33,3.11,,Alk,1,,
+98-95-3,Nitrobenzeen,Nitrobenzene,123.11,2026.666667,1.845,,overige,3,,
+100-61-8,n-Methylaniline,N-Methylaniline,107.16,5620,1.66,,overige,3,,
+,n-Nonanal,n-Nonanal,142,,,,O2,3,,
+,n-nonylphenol,n-nonylphenol,220.4,1.104616663,4.5,,overige,3,238.8,
+,n-nonylphenol-tech,n-nonylphenol-tech,,,,,overige,3,,
+,n-Octanal,n-Octanal,128,,,,O2,3,,
+,n-octylphenol,n-octylphenol,206.3,5.182021708,4,,overige,3,222.3,
+111842,nonaan,Nonane ,128.25,0.22,5.65,,,,,
+,nonylphenol-d4,nonylphenol-d4,,,,,overige,3,,
+109-66-0,n-Pentaan,Pentane,72.15,39.25,3.42,,Alk,1,,
+109-66-0,n-Pentane,n-Pentane,72.15,40,3.39,,Alk,1,,
+,n-Tetradecane,n-Tetradecane,198,,,,Alk,1,,
+,"o,p’-DDD","o,p’-DDD",320.1,0.3201,6.8,3.943475106,overige,3,224.8,0.0001
+,"o,p’-DDE","o,p’-DDE",318,0.400338281,7.1,4.1134711,overige,3,221.1,0.0001
+,"o,p’-DDT","o,p’-DDT",354.5,0.177670874,6.4,4.343467663,overige,3,237.7,0.0001
+95-49-8,o-Chloortolueen,o-Chlorotoluene,126.586,154,3.2,,ClArom,1,,
+95487,o-Cresol,o-Cresol,108.1166641,14858.86058,1.95,0.399094472,overige,3,,0.001
+111-65-9,Octaan,Octane,114.23,0.7,5.15,,Alk,1,,
+,octylphenol-d17,octylphenol-d17,,,,,overige,3,,
+ 95-47-6 ,o-Xyleen,o-Xylene,106.186665,218.9335957,3.12,0.956771645,MAK,1,,0.001
+,"p,p’-DDD","p,p’-DDD",320.1,0.804054847,6.3,,overige,3,227.1,
+,"p,p’-DDE","p,p’-DDE",318,0.252596379,6.9,,overige,3,222.4,
+,"p,p’-DDMU","p,p’-DDMU",283.6,,6.2,,overige,3,210.4,
+,"p,p’-DDT","p,p’-DDT",354.5,0.141128992,6.4,,overige,3,240.1,
+,PCB 1,PCB 1,,,4.46,,PCB,2,163.2,
+,PCB 10,PCB 10,223.1,1.772146292,4.85,,PCB,2,223.1,
+,PCB 100,PCB 100,,,6.23,,PCB,2,212.1,
+,PCB 101,PCB 101,325.1617,0.057913166,6.316,4.293468622,PCB,2,212.15,0.0001
+,PCB 103,PCB 103,,,6.22,,PCB,2,212,
+,PCB 104,PCB 104,326.4,0.205944477,5.85,,PCB,2,360.9,
+,PCB 105,PCB 105,326.4,0.025926874,6.716666667,,PCB,2,209.9,
+,PCB 107,PCB 107,,,6.71,,PCB,2,210.5,
+,PCB 110,PCB 110,326.4,0.03264,6.526666667,,PCB,2,209.7,
+,PCB 118,PCB 118,341.3406,0.032261293,6.5081,5.113463578,PCB,2,210.25,0.0001
+,PCB 119,PCB 119,,,6.58,,PCB,2,210.75,
+,PCB 128,PCB 128,360.9,0.018087847,6.746666667,,PCB,2,222.6,
+,PCB 129,PCB 129,360.9,0.018087847,6.75,,PCB,2,360.9,
+,PCB 132,PCB 132,,,6.58,,PCB,2,222.65,
+,PCB 134,PCB 134,,,6.55,,PCB,2,222.2,
+,PCB 135,PCB 135,,,6.64,,PCB,2,222.9,
+,PCB 136,PCB 136,,,6.22,,PCB,2,221.7,
+,PCB 137,PCB 137,360.9,0.014367688,6.85,,PCB,2,360.9,
+,PCB 138,PCB 138,360.3746,0.017903781,6.7341,4.473466391,PCB,2,223.25,0.0001
+,PCB 14,PCB 14,223.1,0.560401863,5.3,,PCB,2,,
+,PCB 141,PCB 141,360.9,0.014367688,6.84,,PCB,2,223.55,
+,PCB 143,PCB 143,360.9,0.022771251,6.65,,PCB,2,,
+,PCB 145,PCB 145,360.9,0.072009017,6.3,,PCB,2,,
+,PCB 146,PCB 146,,,6.89,,PCB,2,223.7,
+,PCB 149,PCB 149,360.9,0.022771251,6.75,,PCB,2,360.9,
+,PCB 151,PCB 151,360.9,0.022771251,6.646666667,,PCB,2,223.15,
+,PCB 153,PCB 153,374.6501,0.012145224,6.9036,4.63346528,PCB,2,223.75,0.0001
+,PCB 155,PCB 155,360.9,0.01141266,6.67,,PCB,2,223.85,
+,PCB 156,PCB 156,360.9,0.00571988,7.226666667,,PCB,2,222.05,
+,PCB 158,PCB 158,,,7.02,,PCB,2,221.6,
+,PCB 16,PCB 16,,,5.16,,PCB,2,187.4,
+,PCB 163,PCB 163,,,6.99,,PCB,2,221.5,
+,PCB 170,PCB 170,395.3,0.004976532,7.35,,PCB,2,360.9,
+,PCB 171,PCB 171,,,7.11,,PCB,2,234.1,
+,PCB 172,PCB 172,,,7.33,,PCB,2,235.1,
+,PCB 174,PCB 174,,,7.11,,PCB,2,234,
+,PCB 177,PCB 177,,,7.08,,PCB,2,234,
+,PCB 178,PCB 178,,,7.14,,PCB,2,234.7,
+,PCB 18,PCB 18,257.5,0.814286497,5.246666667,,PCB,2,188.35,
+,PCB 180,PCB 180,395.3,0.006265083,7.3,4.753464668,PCB,2,360.9,0.0001
+,PCB 183,PCB 183,,,7.2,,PCB,2,234.6,
+,PCB 185,PCB 185,,,7.11,,PCB,2,234.4,
+,PCB 187,PCB 187,395.3,0.006265083,7.25,,PCB,2,235,
+,PCB 192,PCB 192,,,7.52,,PCB,2,234,
+,PCB 194,PCB 194,429.8,,7.8,,PCB,2,246.55,
+,PCB 195,PCB 195,,,7.56,,PCB,2,245.5,
+,PCB 197,PCB 197,,,7.3,,PCB,2,245.6,
+,PCB 199,PCB 199,,,7.2,,PCB,2,246.2,
+,PCB 201,PCB 201,,,7.62,,PCB,2,245.5,
+,PCB 202,PCB 202,,,7.24,,PCB,2,245.3,
+,PCB 204,PCB 204,429.8,0.004298,7.35,,PCB,2,246.5,
+,PCB 205,PCB 205,,,8,,PCB,2,244.8,
+,PCB 206,PCB 206,,,8.09,,PCB,2,257.4,
+,PCB 207,PCB 207,,,7.74,,PCB,2,257,
+,PCB 208,PCB 208,,,7.71,,PCB,2,256.9,
+,PCB 21,PCB 21,257.5,0.324173294,5.55,,PCB,2,257.5,
+,PCB 22,PCB 22,,,5.58,,PCB,2,186.8,
+,PCB 24,PCB 24,,,5.35,,PCB,2,186.1,
+,PCB 25,PCB 25,,,5.67,,PCB,2,187.6,
+,PCB 26,PCB 26,,,5.66,,PCB,2,187.4,
+,PCB 27,PCB 27,,,5.44,,PCB,2,186.6,
+,PCB 28,PCB 28,257.5,0.20453952,5.65,3.373509124,PCB,2,257.5,0.0001
+,PCB 29,PCB 29,257.5,0.324173294,5.633333333,,PCB,2,187.5,
+,PCB 3,PCB 3,,,4.69,,PCB,2,162.4,
+,PCB 30,PCB 30,257.5,0.408109997,5.45,,PCB,2,257.5,
+,PCB 31,PCB 31,257.5,0.20453952,5.75,,PCB,2,292,
+,PCB 32,PCB 32,,,5.44,,PCB,2,186.6,
+,PCB 37,PCB 37,,,5.83,,PCB,2,185.8,
+,PCB 4,PCB 4,223.1,2.808662594,4.7,,PCB,2,,
+,PCB 40,PCB 40,,,5.66,,PCB,2,199,
+,PCB 41,PCB 41,,,5.69,,PCB,2,199.2,
+,PCB 42,PCB 42,,,5.76,,PCB,2,199.8,
+,PCB 43,PCB 43,,,5.75,,PCB,2,199.9,
+,PCB 44,PCB 44,292,0.231943845,5.783333333,,PCB,2,199.95,
+,PCB 45,PCB 45,,,5.53,,PCB,2,198.8,
+,PCB 46,PCB 46,,,5.53,,PCB,2,198.8,
+,PCB 47,PCB 47,292,0.146346672,5.9,,PCB,2,292,
+,PCB 49,PCB 49,292,0.146346672,5.9,,PCB,2,292,
+,PCB 50,PCB 50,292,0.292,5.65,,PCB,2,292,
+,PCB 51,PCB 51,,,5.63,,PCB,2,199.6,
+,PCB 52,PCB 52,292,0.116247294,5.85,3.463500793,PCB,2,,0.0001
+,PCB 55,PCB 55,292,0.073347084,6.15,,PCB,2,292,
+,PCB 56,PCB 56,292,0.073347084,6.136666667,,PCB,2,198.35,
+,PCB 6,PCB 6,,,5.06,,PCB,2,175.2,
+,PCB 60,PCB 60,,,6.11,,PCB,2,198.5,
+,PCB 63,PCB 63,,,6.17,,PCB,2,199.2,
+,PCB 64,PCB 64,,,5.95,,PCB,2,198.3,
+,PCB 66,PCB 66,292,0.05826166,6.25,,PCB,2,,
+,PCB 69,PCB 69,292,0.092338508,6.046666667,,PCB,2,199.2,
+,PCB 71,PCB 71,,,5.98,,PCB,2,198,
+,PCB 74,PCB 74,292,,6.2,,PCB,2,199.25,
+,PCB 77,PCB 77,,,6.36,,PCB,2,197.2,
+,PCB 78,PCB 78,292,0.036760622,6.4,,PCB,2,326.4,
+,PCB 8,PCB 8,223.1,1.407665836,5.1,,PCB,2,,
+,PCB 81,PCB 81,,,6.36,,PCB,2,197.6,
+,PCB 82,PCB 82,,,6.2,,PCB,2,210.8,
+,PCB 83,PCB 83,,,6.26,,PCB,2,211.5,
+,PCB 85,PCB 85,326.4,0.051730914,6.333333333,,PCB,2,211.85,
+,PCB 87,PCB 87,326.4,0.051730914,6.33,,PCB,2,211.7,
+,PCB 89,PCB 89,,,6.07,,PCB,2,210.5,
+,PCB 91,PCB 91,,,6.13,,PCB,2,211.2,
+,PCB 97,PCB 97,326.4,0.051730914,6.33,,PCB,2,211.45,
+,PCB 99,PCB 99,326.4,0.041091325,6.45,,PCB,2,326.4,
+106-48-9,p-Chloorfenol,P-chlorophenol,128.56,25500,2.27,,Cl,3,,
+106-43-4,p-Chloortolueen,p-Chlorotoluene,126.586,123,3.33,,ClArom,1,,
+106445,p-Cresol,p-Cresol,108.1099991,28640.96526,1.94,0.444357034,overige,3,,0.001
+608-93-5,Pentachloorbenzeen,Pentachlorobenzene,250.1297785,0.322818462,5.076666667,2.683710051,ClArom,1,,0.001
+87-86-5,Pentachloorfenol,Pentachlorophenol,266.33,4.28,5.12,1.964642345,Cl,3,,0.001
+110-62-3,Pentanal,Pentanal,86.13,14000,1.31,,O2,3,,
+,Pentylbenzeen,Penthylbenzene,148.25,3.37,4.9,,MAK,1,,
+,perylene,perylene,252.15,0.026200963,6.175,,PAK,1,219.45,
+,phenanthrene,phenanthrene,178.1,4.350184731,4.48,,PAK,1,160.35,
+ 74-98-6 ,Propaan,Propane,44.1,75,2.36,,Alk,1,,
+107-12-0,Propionitrile,Propionitrile,55.08,103000,0.16,,overige,3,,
+ 103-65-1,Propylbenzeen,Propylbenzene,120.19,54.00633333,3.71,,MAK,1,,
+115-07-1,Propylene (Propeen??),Propylene,42.08,292,1.77,,Alk,1,,
+,p-Xyleen,p-Xylene,106.186665,210.9384616,3.15,1.428036212,MAK,1,123.9,0.001
+,pyrene,pyrene,202.15,0.836365063,4.94,,PAK,1,182.1,
+110861,pyridine,pyridine,79.1,665483.58,0.65,0.714917304,overige,3,,0.0001
+100-42-5,Styrene,Styrene,104.1485645,320.0573505,2.95,1.348594147,MAK,1,,0.001
+634-66-2,Tetrachloorbenzeen,Tetrachlorobenzene,216,4.16,4.6,2.51,ClArom,1,,
+127-18-4,Tetrachlooretheen,Tetrachloroethylene,165.8074995,118.8825037,3.4,1.194834616,ClAlk,1,,0.01
+56-23-5,Tetrachloormethaan,Tetrachloromethane,153.82,800,2.83,0.558949208,ClAlk,1,,0.001
+,Tetradecanol,Tetradecanol,214,,,,O2,3,,
+ 75-73-0 ,Tetrafluoromethane,Tetrafluoromethane,88.01,20,1.18,,overige,3,,
+,tetrahydrofuran,tetrahydrofuran,72.10666651,405634.1962,0.47,-0.375336937,O2,3,,0.0001
+110010,tetrahydrothiophene,tetrahydrothiophene,88.17499986,12894.97733,1.61,0.232488206,overige,3,,0.0001
+,t-octylphenol,t-octylphenol,206.3,25.97163125,4.1,,overige,3,219.5,
+108-88-3,Tolueen,Toluene,92.14249285,610.5910523,2.73,0.870272715,MAK,1,106.9,0.001
+,Tribroommethaan,Tribromomethane,252.8,1719,2.67,0.946079776,overige,3,,0.0001
+79-01-6,Trichlooretheen,Trichloroethylene,131.4,1164.844161,2.61,0.842372721,ClAlk,1,,0.01
+,triclosan,triclosan,289.5,11.52520259,4.8,,overige,3,192.1,
+,UV1,UV1,214,,,,overige,3,,
+,UV10,UV10,585,,,,overige,3,,
+,UV2,UV2,258,,,,overige,3,,
+,UV3,UV3,326,,,,overige,3,,
+,UV4,UV4,332,,,,overige,3,,
+,UV5,UV5,346,,,,overige,3,,
+,UV6,UV6,388,,,,overige,3,,
+,UV7,UV7,388,,,,overige,3,,
+,UV8,UV8,445,,,,overige,3,,
+,UV9,UV9,551,,,,overige,3,,
+75-01-4,Vinylchloride,Vinyl chloride,62.5,428,1.52,0.734988789,ClAlk,1,,0.0001
+13-30-2-07,Xyleen,Xylene,120.208888,,3.74,,MAK,1,,
```

### Comparing `pipepermcalc-0.0.5/pipepermcalc/pipe.py` & `pipepermcalc-0.8.6/pipepermcalc/pipe.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,991 +1,1051 @@
-#%% ----------------------------------------------------------------------------
-# A. Hockin, January 2023
-# KWR 403230-003
-# Pipe permeation calculator
-# With Martin vd Schans, Bram Hillebrand, Lennart Brokx
-#
-# ------------------------------------------------------------------------------
-
-import numpy as np
-import pandas as pd
-import fuzzywuzzy.fuzz as fwf
-import fuzzywuzzy.process as fwp
-
-from pipepermcalc.segment import *
-from pipepermcalc.database import DATA_DIR 
-
-class Pipe:
-    '''
-    Pipe object class to make segments of the pipe and calculate the peak and
-    mean concentration of a chemical in groundwater and soil.
-
-    Attributes
-    -------
-    segment_list: list
-        list of the pipe segment objects which make up the pipe
-    _conditions_set: Boolean
-        Default False, True when the groundwater conditions have been set.
-    _flow_rate_set: Boolean
-        Default False, True when the flow rate has been set.
-    _concentration_groundwater_set: Boolean
-        Default False, True when the flow rate has been set.
-    _is_validated: Boolean
-        Default False, True when the flow rate has been set.
-    total_volume: float
-        Total volume of the pipe, summed from the pipe segments, m3
-    total_length': float
-        Total length of the pipe, summed from the pipe segments, m
-    flow_rate: float
-        Flow rate through pipe, m3/day.
-    CAS_number: string
-        CAS is a unique identification number assigned by the Chemical 
-        Abstracts Service (CAS)
-    chemical_name_EN: string
-        Name of the chemical in English
-    chemical_name_NL: string
-        Name of the chemical in Dutch
-    molecular_weight: float
-        Mass of one mole of a given chemical, g/mol
-    solubility:	float
-        solubility of given chemical in water, g/m3
-    log_octanol_water_partitioning_coefficient:	float,
-        Partition coefficient for the two-phase system consisting of 
-        n-octanol and water, Log Kow, [-]
-    log_distribution_coefficient: float
-        Ratio of the amount of chemical  adsorbed onto soil per amount 
-        of water, m3/g
-    chemical_group: string
-        Grouping of chemicals (expert opinion) with similar properties
-        for permeation: Group 1: PAK, MAK, ClArom, ClAlk, Arom, Alk, 
-        Group 2: PCB, Group 3: overig, onbekend, O2, Cl, BDE. See KWR 2016.056
-    chemical_group_number: integer
-        Integer corresponding to the chemical group 
-    molecular_volume: float
-        Volume occupied by one mole of the substance at a given 
-        temperature and pressure, cm3/mol.
-    Drinking_water_norm: float
-        Concentration allowable in the Dutch Drinking water decree, g/m3.
-    _Kd_known: Boolean
-        True when a distribution coefficient (Kd) for the chemical is known. 
-        Kd is needed to convert from soil to groundwater concentration.
-    concentration_groundwater: float
-        Concentration of the given chemical in groundwater, g/m3.
-    tolerance: float 
-        The allowable difference between the calculated and actual drinking 
-        water concentration, [-].
-    max_iterations: int
-        Maximum number of iterations allowed in the optimization scheme. 
-    temperature_groundwater: float
-        Temperature of the groundwater, degrees Celcius.
-    stagnation_time: float
-        Time in seconds which water in pipe is stagnant, unit of seconds. The 
-        stagnation factor is only valid for a stagnation time of 8 hours 
-        (28800 seconds), therefore using another other stagnation time is not advised.
-    concentration_peak_allowable_groundwater: float
-        Concentration in groundwater which, after a stagnation period, 
-        would not result in a peak concentration in drinking water exceeding 
-        the drinking water norm, g/m3.
-    concentration_mean_allowable_groundwater: float
-        Mean concentration in groundwater which would would not result in 
-        a mean daily (24 hours) concentration in drinking water exceeding 
-        the drinking water norm, g/m3.
-    mean_concentration_pipe_drinking_water: float 
-    #@martin, should these be returned as simply concentration_drinking_water to avoid confusion?
-        Calculates the mean concentration in drinking water for a 24 hour period
-        given a groundwater concentration.
-    peak_concentration_pipe_drinking_water: float
-        Calculates the peak (maximum) concentration in drinking water for a 
-        given a stagnation period given a groundwater concentration.
-    concentration_soil: float
-        Concentration of the given chemical in soil, mg/kg.
-    scale_factor_upper_limit: float
-        Scale factor used to set the upper limit of the bounds for calculating 
-        the mean concentration of drinking water or groundwater. Upper limit taken as the 
-        concentration of groundwater (solving for drinking water concentration) 
-        or solubility (solving for groundwater concentration) multiplied by the 
-        scale factor. Default value of 0.999 
-    scale_factor_lower_limit: float    
-        Scale factor used to set the upper limit of the bounds for calculating 
-        the mean concentration of drinking water or groundwater. Lower limit taken as the 
-        concentration of groundwater (solving for drinking water concentration) 
-        or solubility (solving for groundwater concentration) multiplied by the 
-        scale factor. Default value of 0.0001.  
-    ASSESSMENT_FACTOR_GROUNDWATER: float 
-        Factor used to correct calculations for observations in actual pipe 
-        permeation. Permeation of PE house connections in groundwater = 3, 
-        other pipe materials = 1. See section 7.2 in KWR 2016.056
-    ASSESSMENT_FACTOR_SOIL: float
-        Factor used to correct calculations for observations in actual pipe 
-        permeation. All pipe materials = 1.
-            
-    Note
-    ----
-    All parameters are in SI units: m, m2, g/m3 (equivalent to mg/L), seconds.
-
-    '''
-
-    #Constants for iterative calculations,
-    TOLERANCE_DEFAULT = 0.01
-    SCALE_FACTOR_UPPER_LIMIT = 0.999
-    SCALE_FACTOR_LOWER_LIMIT = 0.0001
-    MAX_ITERATIONS_DEFAULT = 1000
-    TEMPERATURE_GROUNDWATER_DEFAULT = 12 # degrees C
-    STAGNATION_TIME_DEFAULT = 8 * 60 * 60 # 8 hours in seconds
-    ASSESSMENT_FACTOR_GROUNDWATER = 3
-    ASSESSMENT_FACTOR_SOIL = 1
-    # FLOW_RATE_DEFAULT = 0.5/ 24 / 60 / 60 # 0.5 m3/day in seconds 
-    # @martin, do we want a default flow rate?
-
-    ppc_database = pd.read_csv(DATA_DIR + '/ppc_database.csv',  skiprows=[1, 2] ) 
-
-    #dictionary to check input parameter value and dtype
-    parameter_validation_dictionary = \
-        {
-        'name':     {'value_dtype': [str]}, 
-        'material': {'str_options': ['PE40', 'PE80', 'SBR', 'EPDM', 'PVC'],
-                    'value_dtype': [str]}, 
-        'permeation_direction': {'str_options': ['perpendicular', 'parallel'],
-                    'value_dtype': [str]}, 
-        'length': {'min_value': 0, 
-                'value_dtype': [float, int]}, 
-        'inner_diameter': {'min_value': 0, 
-                        'value_dtype': [float, int]}, 
-        'wall_thickness': {'min_value': 0, 
-                        'value_dtype': [float, int]},  
-        'diffusion_path_length': {'min_value': 0, 
-                                'value_dtype': [float, int]},
-        'max_iterations': {'min_value': 0, 
-                        'value_dtype': [float, int]}, 
-        'tolerance': {'min_value': 0,
-                    'max_value': 1, 
-                    'value_dtype': [float]},  
-        'stagnation_time': {'min_value': 0, 
-                            'value_dtype': [float, int]},  
-        'flow_rate': {'min_value': 0, 
-                    'value_dtype': [float, int]},  
-        'concentration_soil': {'min_value': 0, 
-                                    'value_dtype': [float, int]},  
-        'concentration_groundwater': {'min_value': 0, 
-                                    'value_dtype': [float, int]},  
-        'temperature_groundwater': {'min_value': 0, 
-                                    'value_dtype': [float, int]},  
-        'concentration_drinking_water': {'min_value': 0, 
-                                        'value_dtype': [float, int]},  
-        'chemical_name': {'value_dtype': [str]},  
-        'language': {'str_options': ['NL', 'EN'],
-                    'value_dtype': [str]}, 
-        }
-    
-    def __init__(self, 
-                 segment_list,
-                ):
-        '''
-        Attributes of the class added, default values of False added for the 
-        different conditions (flow rate, concentration groundwater, validation etc).
-
-        Attributes
-        ----------
-        segment_list: list
-            list of the segments objects
-        _conditions_set: Boolean
-            Default False, True when the groundwater conditions have been set.
-        _flow_rate_set: Boolean
-            Default False, True when the flow rate has been set.
-        _concentration_groundwater_set: Boolean
-            Default False, True when the flow rate has been set.
-        _is_validated: Boolean
-            Default False, True when the flow rate has been set.
-        total_volume: float
-            Total volume of the pipe, summed from the pipe segments, m3
-        total_length': float
-            Total length of the pipe, summed from the pipe segments, m
-                
-        ''' 
-
-        self.segment_list = segment_list
-        self._conditions_set = False
-        self._flow_rate_set = False
-        self._concentration_groundwater_set = False
-        self._is_validated = False
-        self._permeation_direction = False
-
-        sum_total_volume = 0
-        sum_total_length = 0
-        for segment in segment_list:
-            sum_total_length += segment.length
-            sum_total_volume += segment.volume
-
-        self.total_length = sum_total_length
-        self.total_volume = sum_total_volume
-    
-
-    def _validate_object(self, 
-                         check_object):
-        ''' Check that the input parameters are valid values and types for the 
-        input object, uses parameter_validation_dictionary to verify parameters.
-        
-        Parameters
-        ----------
-        check_object: object
-            Segment or Pipe object for which attributes must be validated.
-        '''
-
-        for k, v in self.parameter_validation_dictionary.items():
-            
-            if hasattr(check_object, k):
-                if (k == 'flow_rate' or k=='concentration_groundwater' or k=='concentration_soil') and getattr(check_object, k) is None:
-                    pass
-                else:
-                    if type(getattr(check_object, k)) not in v['value_dtype']:
-                        raise ValueError(f"Invalid value ~{getattr(check_object, k)}~ for parameter {k}. Input value should be a {v['value_dtype']}.")
-                    if 'min_value' in v.keys():
-                        if getattr(check_object, k) < v['min_value']:
-                            raise ValueError(f"Invalid value {getattr(check_object, k)} for parameter {k}. Input value should be a > {v['min_value']}.")
-                    if 'max_value' in v.keys():
-                        if getattr(check_object, k) > v['max_value']:
-                            raise ValueError(f"Invalid value ~{getattr(check_object, k)}~ for parameter {k}. Input value should be a < {v['max_value']}.")
-                    if 'str_options' in v.keys():
-                        if getattr(check_object, k) not in v['str_options']:
-                            raise ValueError(f"Invalid value ~{getattr(check_object, k)}~ for parameter {k}. Input value should be one of {v['str_options']}.")        
-
-
-    def validate_input_parameters(self,):
-        ''' Check that the input parameters are valid values and types for the 
-        Pipe and Segment objects'''
-
-        #check if 
-        if self._conditions_set is False:
-            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
-        else: 
-            #validate the segment attributes
-            for segment in self.segment_list:
-                self._validate_object(segment)
-                if segment.permeation_direction == 'perpendicular':
-                    self._permeation_direction = True # @alex this is a confusing name i would say _permeation_direction_set or something similar
-        
-            #validate the pipe attributes
-            self._validate_object(self)
-
-            if self._permeation_direction is False:
-                raise ValueError('Error, there must be atlease one pipe segment with permeation perpendicular to the flow rate.')
-            else:
-                self._is_validated=True
-
-
-    def _fuzzy_min_score(self, 
-                         chemical_name): 
-        """
-        This function calculates the minimum score required for a valid
-        match in fuzzywuzzy's extractOne function. The minimum score depends
-        on the length of 's' and is calculated based on the string lengths and
-        scores in the DEFAULT_MINSCORES dictionary. 
-        From Vincent Post. 
-
-        Parameters
-        ----------
-        chemical_name : str
-            String for which the minimum score must be determined, in our case 
-            the chemical name
-
-        Returns
-        -------
-        result : float
-            The minimum score for 'chemical_name'.
-        """
-        DEFAULT_FUZZY_MINSCORES = {1: 100, 3: 100, 4: 90, 5: 85, 6: 80, 8: 75}
-
-        xp = list(DEFAULT_FUZZY_MINSCORES.keys()) #@martin comment: #@@ maybe it's easier to enter a list directly, instead of extract the dictionary.
-        fp = [v for v in DEFAULT_FUZZY_MINSCORES.values()]
-        # Use the interp function from NumPy. By default this function
-        # yields fp[0] for x < xp[0] and fp[-1] for x > xp[-1]
-        return np.interp(len(chemical_name), xp, fp)
-
-
-    def _extract_matching_chemical_name(self, 
-                                        chemical_name, 
-                                        database):
-        
-        ''' Search and extract the highest matching chemical name from the 
-        database for the given input.
-
-        Parameters
-        ----------
-        chemical_name: str
-            String for which the minimum score/highest matching chemical name 
-            must be determined.
-        database: pandas df
-            Dataframe of the database of chemical information, including chemical 
-            name, CAS number, molecular weight, solubility, LKow, Kd etc. 
-
-        Returns
-        -------
-        matching_chemical_name : str
-            Name with the highest match for the input chemical name from the 
-            database.
-        '''
-
-        # Exctract the highest scoring chemical name matching the 
-        minscore = self._fuzzy_min_score(chemical_name=chemical_name)
-
-        # Return only the highest scoring item
-        fuzzy_score = fwp.extractOne(
-            query=chemical_name,
-            choices=database,
-            scorer=fwf.token_sort_ratio,
-            score_cutoff=minscore,
-        )
-        
-        matching_chemical_name = fuzzy_score[0]
-
-        return matching_chemical_name
-
-
-    def _fetch_chemical_database(self,
-                                chemical_name=None,
-                                suppress_print=False,
-                                language = 'NL'
-                                ):
-        ''' 
-        Fetch the pipe and chemical information corresponding to the given 
-        chemical choice and corresponding pipe material. 
-
-        Parameters
-        ----------
-        chemical_name: str
-            Name of the chemical for which to calculate the permeation
-        suppress_print: Boolean
-            Suppress printing the chemical name and matching name, e.g. in 
-            loop calculations
-        language: str
-            Language fo the chemical name to search for, default is Dutch ('NL'), 
-            English ('EN') also possible
-        '''
-        
-        database = list(self.ppc_database['chemical_name_'+language])
-        
-        matching_chemical_name = self._extract_matching_chemical_name(chemical_name=chemical_name, 
-                                             database=database)
-        
-        if suppress_print:
-            pass
-        else:
-            print("Input chemical name: ", str(chemical_name), "- Matched chemical name: ", str(matching_chemical_name))
-
-        df = self.ppc_database.loc[self.ppc_database['chemical_name_'+language] == matching_chemical_name]
-        pipe_permeability_dict = df.to_dict('records')[0]
-
-        #assign dict items as attribute of class
-        for k, v in pipe_permeability_dict.items():
-            setattr(self, k, v)
-
-    def _soil_to_groundwater(self):
-        ''' 
-        Calculate the concentration in soil given the concentration in 
-        groundwater
-        '''
-        
-        concentration_soil = (10 ** self.log_distribution_coefficient * self.concentration_groundwater * self.ASSESSMENT_FACTOR_SOIL / self.ASSESSMENT_FACTOR_GROUNDWATER)
-
-        return concentration_soil
-
-    def set_conditions(self,
-                    chemical_name,                                    
-                    concentration_groundwater=None,
-                    concentration_soil=None,
-                    flow_rate=None,
-                    concentration_drinking_water=None,
-                    temperature_groundwater= TEMPERATURE_GROUNDWATER_DEFAULT, 
-                    stagnation_time = STAGNATION_TIME_DEFAULT,
-                    suppress_print = False, 
-                    language = 'NL'
-                    ):
-        ''' 
-        Specifies the chemical of interest, concentration and temperature in the 
-        groundwater and returns the parameters as attributes of the class. 
-        If the concentration of groundwater is given, or the soil concentration 
-        and Kd are known, the diffusion and permeation parameters are calculated 
-        for the pipe segment(s). 
-
-        Parameters
-        ----------
-        chemical_name: string
-            Name of the chemical for which to calculate the permeation
-        concentration_groundwater: float
-            Concentration of the given chemical in groundwater, g/m3
-        concentration_soil: float
-            Concentration of the given chemical in soil, mg/kg.
-        flow_rate: float
-            Flow rate through pipe, m3/day.
-        concentration_drinking_water: float
-            Concentration of given chemical in drinking water pipe, g/m3. If no 
-            value given, concentration is assigned the drinking water norm value.
-        temperature_groundwater: float
-            Temperature of the groundwater, degrees Celcius
-        stagnation_time: float
-            Time in seconds which water in pipe is stagnant, unit of seconds. The 
-            stagnation factor is only valid for a stagnation time of 8 hours 
-            (28800 seconds), therefore using another other stagnation time is not advised.
-        suppress_print: Boolean
-            Suppress printing the chemical name and matching name, e.g. in loop calculations
-        language: str
-            Language fo the chemical name to search for, default is Dutch ('NL'), 
-            English ('EN') also possible
-
-        '''
-        self.chemical_name = chemical_name
-        self.temperature_groundwater = temperature_groundwater
-        self.stagnation_time = stagnation_time
-        self.language = language
-
-        #return to these checks...
-        self._conditions_set = True
-
-        self.flow_rate = flow_rate
-        if flow_rate is not None:
-            self._flow_rate_set = True
-
-        self._fetch_chemical_database(chemical_name=self.chemical_name, 
-                                        suppress_print=suppress_print, 
-                                        language=language)
-
-
-        #check if there is a known distribution coefficient
-        if np.isnan(self.log_distribution_coefficient):
-            self._Kd_known = False
-        else: self._Kd_known = True
-
-        self.concentration_groundwater = concentration_groundwater
-        self.concentration_soil = concentration_soil
-
-        # @alex I find this block of if statements a little confusing. I have the feeling it should be able to make it easier. Also if not neccesary remove all the commented out else statements
-        if (concentration_groundwater is None) and (concentration_soil is None):
-            pass #values already assigned, are None
-        if (concentration_groundwater is not None) and (concentration_soil is None): # @alex since there is no else it could also be if .... and .... and self.Kd_known:
-            if self._Kd_known: 
-                self.concentration_soil = self._soil_to_groundwater()
-            # else: self.concentration_soil = None
-        if (concentration_groundwater is None) and (concentration_soil is not None): # @alex same here
-            if self._Kd_known: 
-                self.concentration_groundwater = (self.concentration_soil * self.ASSESSMENT_FACTOR_GROUNDWATER) / ( 10 ** self.log_distribution_coefficient * self.ASSESSMENT_FACTOR_SOIL )
-            # else: self.concentration_soil = given value, self.concentration_groudnwater = None
-        if (concentration_groundwater is not None) and (concentration_soil is not None): # @alex and again same here
-            # @martin, take the gw concentration over the given soil concentration?
-            # or check the Kd? 
-            if self._Kd_known: 
-                self.concentration_soil = self._soil_to_groundwater()
-            # else: self.concentration_soil = given value
-
-        if self.concentration_groundwater is not None:
-            self._concentration_groundwater_set = True
-
-        # The default value for the concentration_drinking_water is the drinking water norm
-        if concentration_drinking_water is None:
-            self.concentration_drinking_water = self.Drinking_water_norm
-
-        else: 
-            self.concentration_drinking_water = concentration_drinking_water
-
-        if self.concentration_groundwater is not None: 
-            for segment in self.segment_list:          
-                segment._calculate_pipe_K_D(pipe = self, 
-                                            _conditions_set=self._conditions_set, )
-
-
-    def view_database_chemical_names(self, 
-                                     language='NL'):
-        '''
-        Function to view a list of the possible chemical names from the database.
-
-        Parameters
-        ----------
-        language: str
-            Language fo the chemical name to search for, default is Dutch ('NL'), 
-            English ('EN') also possible
-        '''
-
-        return list(self.ppc_database['chemical_name_'+language])
-
-
-    def calculate_mean_dw_concentration(self, 
-                                        tolerance = TOLERANCE_DEFAULT,
-                                        max_iterations = MAX_ITERATIONS_DEFAULT,):
-        '''
-        Calculates the mean concentration in drinking water for a 24 hour period
-        given a groundwater concentration. 
-        
-        Parameters
-        ----------
-        tolerance: float 
-            The allowable difference between the calculated and actual drinking 
-            water concentration, [-]
-        max_iterations: int
-            Maximum number of iterations allowed in the optimization scheme
-
-        Returns
-        -------
-        mean_concentration_pipe_drinking_water: float
-            Calculates the mean concentration in drinking water for a 24 hour period
-            given a groundwater concentration.
-
-        '''
-        self.max_iterations = int(max_iterations)
-        self.tolerance = tolerance
-        
-        # Check if the flow rate, conditions have been set and parameters 
-        # validated, if not raise error
-        if self._flow_rate_set is False: 
-            raise ValueError('Error, the flow rate in the pipe has not been set. Input the flow rate in .set_conditions()')
-
-        if self._concentration_groundwater_set is False: 
-            raise ValueError('Error, the groundwater concentration has not been set. Input the groundwater concentration in .set_conditions()')
-
-        elif self._conditions_set is False:
-            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
-
-        elif self._is_validated is False: 
-            raise ValueError('Error, the input parameters must first be validated. To set validate use .validate_input_parameters() ')
-
-        else: 
-            counter = 0
-            concentration_drinking_water_n_plus_1 = 0 #initial guess for drinking water 
-            lower_limit = 0 # initial value for the lower limit
-            upper_limit = self.concentration_groundwater # initial value for the upper limit
-            criteria_list = [0] # initial list of criteria values
-            min_criteria = 100 # initial value for minimum criteria value, high
-            while True: # @alex in my experience this loop could do with a little more comments    
-                concentration_drinking_water_n_min_1 = concentration_drinking_water_n_plus_1
-
-                sum_mass_segment = 0
-
-                for segment in self.segment_list:
-                    segment._calculate_mean_dw_mass_per_segment(pipe=self, 
-                                            concentration_drinking_water=concentration_drinking_water_n_min_1,
-                                            concentration_groundwater=self.concentration_groundwater,)
-
-                    sum_mass_segment += segment.mass_chemical_drinkwater
-
-                concentration_drinking_water_n = (sum_mass_segment / 
-                                                self.flow_rate ) 
-                counter +=1
-
-                criteria = abs(1 - concentration_drinking_water_n_min_1 
-                                    / concentration_drinking_water_n)
-
-                if criteria <= tolerance:
-                    break
-                elif counter > max_iterations:
-                    print('Max iterations exceeded')
-                    break
-                else:
-                    min_criteria = min(min_criteria, criteria)
-                    criteria_list.append(criteria)
-
-                    if counter == 1:
-                        concentration_drinking_water_n_plus_1 = self.concentration_groundwater * self.SCALE_FACTOR_UPPER_LIMIT 
-                    if counter == 2:
-                        concentration_drinking_water_n_plus_1 = self.concentration_groundwater * self.SCALE_FACTOR_LOWER_LIMIT
-                    if counter >2:
-                        if (criteria < criteria_list[counter-1]) or (concentration_drinking_water_n > self.concentration_groundwater):
-                            lower_limit = concentration_drinking_water_n_min_1
-                            concentration_drinking_water_n_plus_1 = lower_limit + (upper_limit -lower_limit)/2
-                        else:
-                            upper_limit = concentration_drinking_water_n_min_1
-                            concentration_drinking_water_n_plus_1 = lower_limit - (upper_limit -lower_limit)/2
-                            
-            self.concentration_drinking_water = concentration_drinking_water_n
-            if concentration_drinking_water_n > self.solubility:
-                print(f'Warning, the calculated drinking water concentration ({concentration_drinking_water_n}) is above the solubility limit, {self.solubility}.')
-
-        return concentration_drinking_water_n 
-
-
-    def calculate_peak_dw_concentration(self, 
-                                        tolerance = TOLERANCE_DEFAULT,
-                                        max_iterations = MAX_ITERATIONS_DEFAULT,):
-
-        '''
-        Calculates the peak (maximum) concentration in drinking water for a 
-        given a stagnation period given a groundwater concentration.
-        Stagnation period default of 8 hours. 
-        
-        Parameters
-        ----------
-        tolerance: float 
-            The allowable difference between the calculated and actual drinking water concentration, [-]
-        max_iterations: int
-            Maximum number of iterations allowed in the optimization scheme
-
-        Returns
-        -------
-        peak_concentration_pipe_drinking_water: float
-            Calculates the peak (maximum) concentration in drinking water for a 
-            given a stagnation period given a groundwater concentration.
-
-        '''
-
-        self.max_iterations = int(max_iterations)
-        self.tolerance = tolerance
-
-        if self.stagnation_time != self.STAGNATION_TIME_DEFAULT: 
-            print("Warning: the stagnation factor is only valid for a stagnation time of 8 hours. Using a different stagnation time is not advised.")
-
-        # Check if the conditions have been set and parameters 
-        # validated, if not raise error
-
-        if self._concentration_groundwater_set is False: 
-            raise ValueError('Error, the groundwater concentration has not been set. Input the groundwater concentration in .set_conditions()')
-
-        elif self._conditions_set is False:
-            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
-
-        elif self._is_validated is False: 
-            raise ValueError('Error, the input parameters must first be validated. To set validate use .validate_input_parameters() ')
-
-        else: 
-            counter = 0
-            concentration_drinking_water_n_plus_1 = 0
-            lower_limit = 0 # initial value for the lower limit
-            upper_limit = self.concentration_groundwater # initial value for the upper limit
-            criteria_list = [0] # initial list of criteria values
-            min_criteria = 100 # initial value for minimum criteria value, high
-
-            while True:  # @alex this loop could also do with a little more comments  
-
-                concentration_drinking_water_n_min_1 = concentration_drinking_water_n_plus_1
-
-                sum_mass_segment = 0
-
-                for segment in self.segment_list:
-                    segment._calculate_peak_dw_mass_per_segment(pipe=self, 
-                                            concentration_drinking_water=concentration_drinking_water_n_min_1,
-                                            concentration_groundwater=self.concentration_groundwater,)
-
-                    sum_mass_segment += segment.mass_chemical_drinkwater
-
-                concentration_drinking_water_n = (sum_mass_segment / 
-                                                self.total_volume ) # ah_todo @Martin, this is not correst??
-                counter +=1
-
-                criteria = abs(1 - concentration_drinking_water_n_min_1 / concentration_drinking_water_n)
-
-                if criteria <= tolerance:
-                    break
-                elif counter > max_iterations:
-                    print('Max iterations exceeded')
-                    break
-                else:
-                    min_criteria = min(min_criteria, criteria)
-                    criteria_list.append(criteria)
-
-                    if counter == 1:
-                        concentration_drinking_water_n_plus_1 = self.concentration_groundwater * self.SCALE_FACTOR_UPPER_LIMIT
-                    if counter == 2:
-                        concentration_drinking_water_n_plus_1 = self.concentration_groundwater * self.SCALE_FACTOR_LOWER_LIMIT
-                    if counter >2:
-                        if (criteria < criteria_list[counter-1]) or (concentration_drinking_water_n > self.concentration_groundwater):
-                            lower_limit = concentration_drinking_water_n_min_1
-                            concentration_drinking_water_n_plus_1 = lower_limit + (upper_limit -lower_limit)/2
-                        else:
-                            upper_limit = concentration_drinking_water_n_min_1
-                            concentration_drinking_water_n_plus_1 = lower_limit - (upper_limit -lower_limit)/2
-                
-            self.concentration_drinking_water = concentration_drinking_water_n
-            if concentration_drinking_water_n > self.solubility:
-                print(f'Warning, the calculated drinking water concentration ({concentration_drinking_water_n}) is above the solubility limit, {self.solubility}.')
-
-        return concentration_drinking_water_n
-
-
-    def calculate_mean_allowable_gw_concentration(self, 
-                                        tolerance = TOLERANCE_DEFAULT,
-                                        max_iterations = MAX_ITERATIONS_DEFAULT, 
-                                        debug=False,):
-        '''
-        Calculates the mean 24 hour concentration in groundwater which would not 
-        result in a drinking water concentration exceeding the drinking water
-        norm. If the distribution coefficient is known the soil concentration is
-        also calculated. 
-
-        Parameters
-        ----------
-        tolerance: float 
-            The allowable difference between the calculated and actual drinking water concentration, [-]
-        max_iterations: int
-            Maximum number of iterations allowed in the optimization scheme
-        debug: Boolean
-            If True, return the groundwater concentration, criteria and lower and 
-            upper limits every iteration.
- 
-        Returns
-        -------
-        concentration_mean_allowable_groundwater: float
-            Mean concentration in groundwater which would would not result in 
-            a mean daily (24 hours) concentration in drinking water exceeding 
-            the drinking water norm, g/m3.
-                    
-        '''
-        self.max_iterations = int(max_iterations)
-        self.tolerance = tolerance
-
-        # Check if the flow rate, conditions have been set and parameters 
-        # validated, if not raise error
-        if self._flow_rate_set is False: 
-            raise ValueError('Error, the flow rate in the pipe has not been set. To set flow rate use .set_flow_rate()')
-
-        elif self._conditions_set is False:
-            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
-
-        elif self._is_validated is False: 
-            raise ValueError('Error, the input parameters must first be validated. To set validate use .validate_input_parameters() ')
-        
-        if self.concentration_drinking_water is None:
-            raise ValueError('Error, no default drinking water norm, please input a drinking water concentration using .set_conditions()')
-
-        if self.concentration_drinking_water > self.solubility:
-            raise ValueError('Error, the drinking water concentration given or the default drinking water norm is higher than the solubility of the chemical. Input a lower drinking water concentration using .set_conditions()')
-
-        else: 
-            self._fetch_chemical_database(chemical_name=self.chemical_name, 
-                                          suppress_print = True,
-                                           language=self.language )
-
-            # calculate initial guess for gw concentration
-            sum_KDA_d = 0
-
-            for segment in self.segment_list:
-                # calculate the sum of the Kpw * DP * SA / d for all pipe segments
-                log_Dp_ref = segment._calculate_ref_logD(chemical_group_number=self.chemical_group_number,
-                            molecular_weight=self.molecular_weight)
-                log_Kpw_ref = segment._calculate_ref_logK(chemical_group_number=self.chemical_group_number,
-                            log_octanol_water_partitioning_coefficient=self.log_octanol_water_partitioning_coefficient)
-                
-                sum_KDA_d_segment = ( 10 ** log_Dp_ref * 10 ** log_Kpw_ref * segment.permeation_surface_area 
-                                    / segment.diffusion_path_length )
-
-                sum_KDA_d += sum_KDA_d_segment
-
-                # initial guess concentration in groundwater
-                concentration_groundwater_n_plus_1 = (self.concentration_drinking_water * (1
-                                         + self.flow_rate * self.ASSESSMENT_FACTOR_GROUNDWATER ) 
-                                            / sum_KDA_d ) * 24 * 60 * 60 #ah_todo is this correct??
-            
-            counter = 0
-            lower_limit = self.concentration_drinking_water # initial value for the lower limit
-            upper_limit = self.solubility # initial value for the upper limit
-            criteria_list = [0] # initial list of criteria values
-            min_criteria = 100 # initial value for minimum criteria value, high
-
-            while True: # @alex and this loop could also do with a little more comments
-                concentration_groundwater_n_min_1 = concentration_groundwater_n_plus_1
-
-                self.set_conditions(chemical_name=self.chemical_name,                                    
-                    concentration_groundwater=concentration_groundwater_n_min_1,
-                    flow_rate=self.flow_rate,
-                    concentration_drinking_water=self.concentration_drinking_water, 
-                    temperature_groundwater=self.temperature_groundwater, 
-                    stagnation_time = self.stagnation_time,
-                    suppress_print = True, 
-                    language = self.language)
-
-                sum_mass_segment = 0
-
-                # mass of chemical in pipe water to meet drinking water norm
-                mass_drinkingwater_norm = (self.concentration_drinking_water * self.flow_rate)
-
-                for segment in self.segment_list:
-                    segment._calculate_mean_dw_mass_per_segment(pipe=self, 
-                                            concentration_drinking_water=self.concentration_drinking_water,
-                                            concentration_groundwater=self.concentration_groundwater,)
-
-                    sum_mass_segment += segment.mass_chemical_drinkwater
-
-                counter +=1
-                criteria = abs(1 - mass_drinkingwater_norm / sum_mass_segment)
-                if criteria <= tolerance:
-                    if debug: #counter % 100 ==0 :
-                        print(concentration_groundwater_n_min_1, concentration_groundwater_n_plus_1, criteria, lower_limit, upper_limit) #for debugging
-                    break
-                elif counter > max_iterations:
-                    print('Max iterations exceeded')
-                    break
-                elif upper_limit == lower_limit:
-                    print('No solution found, lower_limit = upper_limit. Groundwater concentration necesary to satisfy the given drinking water concentration may be above the solubility limit.')
-                    break
-                else:
-                    min_criteria = min(min_criteria, criteria)
-                    criteria_list.append(criteria)
-                    # two initial guesses to compare the goodness of fit
-                    if counter == 1:
-                        concentration_groundwater_n_plus_1 = self.solubility * self.SCALE_FACTOR_UPPER_LIMIT
-                    if counter == 2:
-                        concentration_groundwater_n_plus_1 = 0
-                    if counter >2:
-                        if (criteria < criteria_list[counter-1]) or (concentration_groundwater_n_plus_1 < self.concentration_drinking_water):
-                            lower_limit = concentration_groundwater_n_min_1
-                            concentration_groundwater_n_plus_1 = lower_limit + (upper_limit -lower_limit)/2
-                        else:
-                            upper_limit = concentration_groundwater_n_min_1
-                            concentration_groundwater_n_plus_1 = lower_limit - (upper_limit -lower_limit)/2
-                    if debug: #counter % 100 ==0 :
-                        print(concentration_groundwater_n_min_1, concentration_groundwater_n_plus_1, criteria, lower_limit, upper_limit) #for debugging
-        
-        self.concentration_groundwater = concentration_groundwater_n_min_1
-        if concentration_groundwater_n_min_1 > self.solubility:
-            print(f'Warning, the calculated drinking water concentration ({concentration_groundwater_n_min_1}) is above the solubility limit, {self.solubility}.')
-
-        if self._Kd_known: 
-            self.concentration_soil = self._soil_to_groundwater()
-        else: 
-            self.concentration_soil = 'No known distribution coefficient to calculate soil concentration'
-
-        return concentration_groundwater_n_min_1 
-
-
-    def calculate_peak_allowable_gw_concentration(self, 
-                                    tolerance = TOLERANCE_DEFAULT,
-                                    max_iterations = MAX_ITERATIONS_DEFAULT,
-                                    debug=False,):
-        '''
-        Calculates the peak (maximum) concentration in groundwater water for a 
-        given a stagnation period that would not result in a peak concentration 
-        in drinking water exceeding the drinking water norm for each pipe segment.
-        Stagnation period default of 8 hours. If the distribution coefficient is 
-        known the soil concentration is also calculated. 
-
-        Parameters
-        ----------
-        tolerance: float 
-            The allowable difference between the calculated and actual drinking 
-            water concentration, [-]
-        max_iterations: int
-            Maximum number of iterations allowed in the optimization scheme
-        debug: Boolean
-            If True, return the groundwater concentration, criteria and lower and 
-            upper limits every iteration.
-
-            
-        Returns
-        -------
-        concentration_peak_allowable_groundwater: float
-            Concentration in groundwater which, after a stagnation period, 
-            would not result in a peak concentration in drinking water exceeding 
-            the drinking water norm, g/m3.
-            
-        '''
-        self.max_iterations = int(max_iterations)
-        self.tolerance = tolerance
-
-        if self.stagnation_time != self.STAGNATION_TIME_DEFAULT:
-            print("Warning: the stagnation factor is only valid for a stagnation time of 8 hours. Using a different stagnation time is not advised.")
-
-        # Check if the conditions have been set and parameters 
-        # validated, if not raise error
-        elif self._conditions_set is False:
-            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
-
-        elif self._is_validated is False: 
-            raise ValueError('Error, the input parameters must first be validated. To set validate use .validate_input_parameters() ')
-
-        if self.concentration_drinking_water > self.solubility:
-            raise ValueError('Error, the drinking water concentration given or the default drinking water norm is higher than the solubility of the chemical. Input a lower drinking water concentration using .set_conditions()')
-
-        else: 
-
-            self._fetch_chemical_database(chemical_name=self.chemical_name, 
-                                          suppress_print = True, 
-                                          language=self.language)
-
-            # calculate initial guess for gw concentration
-            sum_KDA_d = 0
-            for segment in self.segment_list:
-                # calculate the sum of the Kpw * DP * SA *f_stag / d for all pipe segments
-                log_Dp_ref = segment._calculate_ref_logD(chemical_group_number=self.chemical_group_number,
-                            molecular_weight=self.molecular_weight)
-                log_Kpw_ref = segment._calculate_ref_logK(chemical_group_number=self.chemical_group_number,
-                            log_octanol_water_partitioning_coefficient=self.log_octanol_water_partitioning_coefficient)
-                
-                #stagnation factor with reference values for LogDp and LogKpw
-                stagnation_factor = 10 ** max((((log_Dp_ref + 12.5) / 2 + 
-                                    log_Kpw_ref) * 0.73611 + 
-                                    -1.03574 ), 0)            
-
-                sum_KDA_d_segment = ( 10 ** log_Dp_ref * 10 ** log_Kpw_ref * segment.permeation_surface_area 
-                                    * stagnation_factor / segment.diffusion_path_length )
-
-                sum_KDA_d += sum_KDA_d_segment
-
-            # initial guess concentration in groundwater
-            concentration_groundwater_n_plus_1 = self.concentration_drinking_water * (1 
-                                        + self.total_volume * self.ASSESSMENT_FACTOR_GROUNDWATER 
-                                        / self.stagnation_time / sum_KDA_d) 
-            
-            counter = 0
-            lower_limit = self.concentration_drinking_water # initial value for the lower limit
-            upper_limit = self.solubility # initial value for the upper limit
-            criteria_list = [0] # initial list of criteria values
-            min_criteria = 100 # initial value for minimum criteria value, high
-
-            while True: # @alex this loop could also do with a little more comments.
-                concentration_groundwater_n_min_1 = concentration_groundwater_n_plus_1
-
-                self.set_conditions(chemical_name=self.chemical_name,                                    
-                    concentration_groundwater=concentration_groundwater_n_min_1,
-                    flow_rate=self.flow_rate,
-                    concentration_drinking_water=self.concentration_drinking_water, 
-                    temperature_groundwater=self.temperature_groundwater, 
-                    stagnation_time = self.stagnation_time,
-                    suppress_print = True, 
-                    language = self.language)
-
-                sum_mass_segment = 0
-
-                # mass of chemical in pipe water to meet drinking water norm
-                mass_drinkingwater_norm = (self.concentration_drinking_water * self.total_volume) 
-
-                for segment in self.segment_list:
-                    segment._calculate_peak_dw_mass_per_segment(pipe=self, 
-                                            concentration_drinking_water=self.concentration_drinking_water,
-                                            concentration_groundwater=self.concentration_groundwater,)
-
-                    sum_mass_segment += segment.mass_chemical_drinkwater
-
-                counter +=1
-                criteria = abs(1 - mass_drinkingwater_norm / sum_mass_segment)
-                
-                if criteria <= tolerance:
-                    break
-                elif counter > max_iterations:
-                    print('Max iterations exceeded')
-                    break
-                elif upper_limit == lower_limit:
-                    print('No solution found, lower_limit = upper_limit. Groundwater concentration necesary to satisfy the given drinking water concentration may be above the solubility limit.')
-                    break
-                else:
-                    min_criteria = min(min_criteria, criteria)
-                    criteria_list.append(criteria)
-
-                    # two initial guesses to compare the goodness of fit
-                    if counter == 1:
-                        concentration_groundwater_n_plus_1 = self.solubility * self.SCALE_FACTOR_UPPER_LIMIT
-                    if counter == 2:
-                        concentration_groundwater_n_plus_1 = 0
-                    if counter >2:
-                        if (criteria < criteria_list[counter-1]) or (concentration_groundwater_n_plus_1 < self.concentration_drinking_water):
-                            lower_limit = concentration_groundwater_n_min_1
-                            concentration_groundwater_n_plus_1 = lower_limit + (upper_limit -lower_limit)/2
-                        else:
-                            upper_limit = concentration_groundwater_n_min_1
-                            concentration_groundwater_n_plus_1 = lower_limit - (upper_limit -lower_limit)/2
-                    if debug: #counter % 100 ==0 :
-                        print(concentration_groundwater_n_min_1, concentration_groundwater_n_plus_1, criteria, lower_limit, upper_limit) #for debugging
-
-        self.concentration_groundwater = concentration_groundwater_n_min_1
-        if concentration_groundwater_n_min_1 > self.solubility:
-            print(f'Warning, the calculated drinking water concentration ({concentration_groundwater_n_min_1}) is above the solubility limit, {self.solubility}.')
-
-        if self._Kd_known: self.concentration_soil = self._soil_to_groundwater()
-        else: self.concentration_soil = 'No known distribution coefficient to calculate soil concentration'
-
-        return concentration_groundwater_n_min_1 
-
-
+#%% ----------------------------------------------------------------------------
+# A. Hockin, January 2023
+# KWR 403230-003
+# Pipe permeation calculator
+# With Martin vd Schans, Bram Hillebrand, Lennart Brokx
+#
+# ------------------------------------------------------------------------------
+
+import numpy as np
+import pandas as pd
+import fuzzywuzzy.fuzz as fwf
+import fuzzywuzzy.process as fwp
+
+from pipepermcalc.segment import *
+from pipepermcalc.database import DATA_DIR 
+
+class Pipe:
+    '''
+    Pipe object class to make segments of the pipe and calculate the peak and
+    mean concentration of a chemical in groundwater and soil.
+
+    Attributes
+    -------
+    segment_list: list
+        list of the pipe segment objects which make up the pipe
+    _conditions_set: Boolean
+        Default False, True when the groundwater conditions have been set.
+    _flow_rate_set: Boolean
+        Default False, True when the flow rate has been set.
+    _concentration_groundwater_set: Boolean
+        Default False, True when the flow rate has been set.
+    _is_validated: Boolean
+        Default False, True when the flow rate has been set.
+    total_volume: float
+        Total volume of the pipe, summed from the pipe segments, m3
+    total_length': float
+        Total length of the pipe, summed from the pipe segments, m
+    flow_rate: float
+        Flow rate through pipe, m3/day.
+    CAS_number: string
+        CAS is a unique identification number assigned by the Chemical 
+        Abstracts Service (CAS)
+    chemical_name_EN: string
+        Name of the chemical in English
+    chemical_name_NL: string
+        Name of the chemical in Dutch
+    molecular_weight: float
+        Mass of one mole of a given chemical, g/mol
+    solubility:	float
+        solubility of given chemical in water, g/m3
+    log_octanol_water_partitioning_coefficient:	float,
+        Partition coefficient for the two-phase system consisting of 
+        n-octanol and water, Log Kow, [-]
+    log_distribution_coefficient: float
+        Ratio of the amount of chemical  adsorbed onto soil per amount 
+        of water, m3/g
+    chemical_group: string
+        Grouping of chemicals (expert opinion) with similar properties
+        for permeation: Group 1: PAK, MAK, ClArom, ClAlk, Arom, Alk, 
+        Group 2: PCB, Group 3: overig, onbekend, O2, Cl, BDE. See KWR 2016.056
+    chemical_group_number: integer
+        Integer corresponding to the chemical group 
+    molecular_volume: float
+        Volume occupied by one mole of the substance at a given 
+        temperature and pressure, cm3/mol.
+    Drinking_water_norm: float
+        Concentration allowable in the Dutch Drinking water decree, g/m3.
+    _Kd_known: Boolean
+        True when a distribution coefficient (Kd) for the chemical is known. 
+        Kd is needed to convert from soil to groundwater concentration.
+    concentration_groundwater: float
+        Concentration of the given chemical in groundwater, g/m3.
+    tolerance: float 
+        The degree of acceptable error in the accuracy of the calculation, 
+        calculated as the difference between the calculated and actual drinking 
+        water concentration, default value of 0.01 (1%), [-].
+    max_iterations: int
+        Maximum number of iterations allowed in the optimization scheme. 
+    temperature_groundwater: float
+        Temperature of the groundwater, degrees Celcius.
+    stagnation_time: float
+        Time in seconds which water in pipe is stagnant, unit of seconds. The 
+        stagnation factor is only valid for a stagnation time of 8 hours 
+        (28800 seconds), therefore using another other stagnation time is not advised.
+    concentration_soil: float
+        Concentration of the given chemical in soil, mg/kg.
+    scale_factor_upper_limit: float
+        Scale factor used to set the upper limit of the bounds for calculating 
+        the mean concentration of drinking water or groundwater. Upper limit taken as the 
+        concentration of groundwater (solving for drinking water concentration) 
+        or solubility (solving for groundwater concentration) multiplied by the 
+        scale factor. Default value of 0.999 
+    scale_factor_lower_limit: float    
+        Scale factor used to set the upper limit of the bounds for calculating 
+        the mean concentration of drinking water or groundwater. Lower limit taken as the 
+        concentration of groundwater (solving for drinking water concentration) 
+        or solubility (solving for groundwater concentration) multiplied by the 
+        scale factor. Default value of 0.0001.  
+    ASSESSMENT_FACTOR_GROUNDWATER: float 
+        Factor used to correct calculations for observations in actual pipe 
+        permeation. Permeation of PE house connections in groundwater = 3, 
+        other pipe materials = 1. See section 7.2 in KWR 2016.056
+    ASSESSMENT_FACTOR_SOIL: float
+        Factor used to correct calculations for observations in actual pipe 
+        permeation. All pipe materials = 1.
+            
+    Note
+    ----
+    All parameters are in SI units: m, m2, g/m3 (equivalent to mg/L), seconds. 
+    Except for the flow rate, which is given in m3/day.
+
+    '''
+
+    #Constants for iterative calculations,
+    TOLERANCE_DEFAULT = 0.01
+    SCALE_FACTOR_UPPER_LIMIT = 0.999
+    SCALE_FACTOR_LOWER_LIMIT = 0.0001
+    MAX_ITERATIONS_DEFAULT = 1000
+    TEMPERATURE_GROUNDWATER_DEFAULT = 12 # degrees C
+    STAGNATION_TIME_DEFAULT = 8 * 60 * 60 # 8 hours in seconds
+    ASSESSMENT_FACTOR_GROUNDWATER = 3
+    ASSESSMENT_FACTOR_SOIL = 1
+    # FLOW_RATE_DEFAULT = 0.5/ 24 / 60 / 60 # 0.5 m3/day in seconds 
+    # @martin, do we want a default flow rate?
+
+    ppc_database = pd.read_csv(DATA_DIR + '/ppc_database.csv',  skiprows=[1, 2] ) 
+    
+    # drop chemicals for which the partitiong and/or diffusion ccoefficient cannot be calculated
+    ppc_database = ppc_database.dropna(subset=['molecular_weight', 'solubility'])
+
+    #dictionary to check input parameter value and dtype
+    parameter_validation_dictionary = \
+        {
+        'name':     {'value_dtype': [str]}, 
+        'material': {'str_options': ['PE40', 'PE80', 'SBR', 'EPDM', 'PVC'],
+                    'value_dtype': [str]}, 
+        'permeation_direction': {'str_options': ['perpendicular', 'parallel'],
+                    'value_dtype': [str]}, 
+        'length': {'min_value': 0, 
+                'value_dtype': [float, int]}, 
+        'inner_diameter': {'min_value': 0, 
+                        'value_dtype': [float, int]}, 
+        'wall_thickness': {'min_value': 0, 
+                        'value_dtype': [float, int]},  
+        'diffusion_path_length': {'min_value': 0, 
+                                'value_dtype': [float, int]},
+        'stagnation_time': {'min_value': 0, 
+                            'value_dtype': [float, int]},  
+        'flow_rate': {'min_value': 0, 
+                    'value_dtype': [float, int]},  
+        'concentration_soil': {'min_value': 0, 
+                                    'value_dtype': [float, int]},  
+        'concentration_groundwater': {'min_value': 0, 
+                                    'value_dtype': [float, int]},  
+        'temperature_groundwater': {'min_value': 0, 
+                                    'value_dtype': [float, int]},  
+        'concentration_drinking_water': {'min_value': 0, 
+                                        'value_dtype': [float, int]},  
+        'chemical_name': {'value_dtype': [str]},  
+        'language': {'str_options': ['NL', 'EN'],
+                    'value_dtype': [str]}, 
+        }
+
+    def __init__(self, 
+                 segment_list,
+                ):
+        '''
+        Attributes of the class added, default values of False added for the 
+        different conditions (flow rate, concentration groundwater, validation etc).
+
+        Attributes
+        ----------
+        segment_list: list
+            list of the segments objects
+        _conditions_set: Boolean
+            Default False, True when the groundwater conditions have been set.
+        _flow_rate_set: Boolean
+            Default False, True when the flow rate has been set.
+        _concentration_groundwater_set: Boolean
+            Default False, True when the flow rate has been set.
+        _is_validated: Boolean
+            Default False, True when the flow rate has been set.
+        total_volume: float
+            Total volume of the pipe, summed from the pipe segments, m3
+        total_length': float
+            Total length of the pipe, summed from the pipe segments, m
+                
+        ''' 
+
+        self.segment_list = segment_list
+        self._conditions_set = False
+        self._flow_rate_set = False
+        self._concentration_groundwater_set = False
+        self._is_validated = False
+        self._set_permeation_direction = False
+        self._check_not_all_PVC = False
+
+        sum_total_volume = 0
+        sum_total_length = 0
+        for segment in segment_list:
+            sum_total_length += segment.length
+            sum_total_volume += segment.volume
+
+        self.total_length = sum_total_length
+        self.total_volume = sum_total_volume
+    
+
+    def _validate_object(self, 
+                         check_object):
+        ''' Check that the input parameters are valid values and types for the 
+        input object, uses parameter_validation_dictionary to verify parameters.
+        
+        Parameters
+        ----------
+        check_object: object
+            Segment or Pipe object for which attributes must be validated.
+        '''
+
+        for k, v in self.parameter_validation_dictionary.items():
+            
+            if hasattr(check_object, k):
+                if (k == 'flow_rate' or k=='concentration_groundwater' or k=='concentration_soil') and getattr(check_object, k) is None:
+                    pass
+                else:
+                    if type(getattr(check_object, k)) not in v['value_dtype']:
+                        raise ValueError(f"Invalid value ~{getattr(check_object, k)}~ for parameter {k}. Input value should be a {v['value_dtype']}.")
+                    if 'min_value' in v.keys():
+                        if getattr(check_object, k) <= v['min_value']:
+                            raise ValueError(f"Invalid value {getattr(check_object, k)} for parameter {k}. Input value should be a > {v['min_value']}.")
+                    if 'max_value' in v.keys():
+                        if getattr(check_object, k) > v['max_value']:
+                            raise ValueError(f"Invalid value ~{getattr(check_object, k)}~ for parameter {k}. Input value should be a < {v['max_value']}.")
+                    if 'str_options' in v.keys():
+                        if getattr(check_object, k) not in v['str_options']:
+                            raise ValueError(f"Invalid value ~{getattr(check_object, k)}~ for parameter {k}. Input value should be one of {v['str_options']}.")        
+
+
+    def validate_input_parameters(self,):
+        ''' Check that the input parameters are valid values and types for the 
+        Pipe and Segment objects'''
+
+        #check if conditions are set
+        if self._conditions_set is False:
+            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
+        else: 
+            #validate the segment attributes
+            for segment in self.segment_list:
+                self._validate_object(segment)
+                if segment.permeation_direction == 'perpendicular':
+                    self._set_permeation_direction = True 
+        
+            #validate the pipe attributes
+            self._validate_object(self)
+
+            if self._set_permeation_direction is False:
+                raise ValueError('Error, there must be atlease one pipe segment with permeation perpendicular to the flow rate.')
+            else:
+                self._is_validated=True
+
+
+    def _fuzzy_min_score(self, 
+                         chemical_name): 
+        """
+        This function calculates the minimum score required for a valid
+        match in fuzzywuzzy's extractOne function. The minimum score depends
+        on the length of 's' and is calculated based on the string lengths and
+        scores in the DEFAULT_MINSCORES dictionary. 
+        From Vincent Post. 
+
+        Parameters
+        ----------
+        chemical_name : str
+            String for which the minimum score must be determined, in our case 
+            the chemical name
+
+        Returns
+        -------
+        result : float
+            The minimum score for 'chemical_name'.
+        """
+        DEFAULT_FUZZY_MINSCORES = {1: 100, 3: 100, 4: 90, 5: 85, 6: 80, 8: 75}
+
+        xp = list(DEFAULT_FUZZY_MINSCORES.keys()) 
+        fp = [v for v in DEFAULT_FUZZY_MINSCORES.values()]
+        # Use the interp function from NumPy. By default this function
+        # yields fp[0] for x < xp[0] and fp[-1] for x > xp[-1]
+        return np.interp(len(chemical_name), xp, fp)
+
+
+    def _extract_matching_chemical_name(self, 
+                                        chemical_name, 
+                                        database):
+        
+        ''' 
+        Search and extract the highest matching chemical name from the 
+        database for the given input.
+
+        Parameters
+        ----------
+        chemical_name: str
+            String for which the minimum score/highest matching chemical name 
+            must be determined.
+        database: pandas df
+            Dataframe of the database of chemical information, including chemical 
+            name, CAS number, molecular weight, solubility, LKow, Kd etc. 
+
+        Returns
+        -------
+        matching_chemical_name : str
+            Name with the highest match for the input chemical name from the 
+            database.
+        '''
+
+        # Exctract the highest scoring chemical name matching the 
+        minscore = self._fuzzy_min_score(chemical_name=chemical_name)
+
+        # Return only the highest scoring item
+        fuzzy_score = fwp.extractOne(
+            query=chemical_name,
+            choices=database,
+            scorer=fwf.token_sort_ratio,
+            score_cutoff=minscore,
+        )
+        
+        matching_chemical_name = fuzzy_score[0]
+
+        return matching_chemical_name
+
+
+    def _fetch_chemical_database(self,
+                                chemical_name=None,
+                                suppress_print=False,
+                                language = 'NL'
+                                ):
+        ''' 
+        Fetch the pipe and chemical information corresponding to the given 
+        chemical choice and corresponding pipe material. 
+
+        Parameters
+        ----------
+        chemical_name: str
+            Name of the chemical for which to calculate the permeation
+        suppress_print: Boolean
+            Suppress printing the chemical name and matching name, e.g. in 
+            loop calculations
+        language: str
+            Language fo the chemical name to search for, default is Dutch ('NL'), 
+            English ('EN') also possible
+        '''
+        
+        database = list(self.ppc_database['chemical_name_'+language])
+        
+        matching_chemical_name = self._extract_matching_chemical_name(chemical_name=chemical_name, 
+                                             database=database)
+        
+        if suppress_print:
+            pass
+        else:
+            print("Input chemical name: ", str(chemical_name), "- Matched chemical name: ", str(matching_chemical_name))
+
+        df = self.ppc_database.loc[self.ppc_database['chemical_name_'+language] == matching_chemical_name]
+        pipe_permeability_dict = df.to_dict('records')[0]
+
+        #assign dict items as attribute of class
+        for k, v in pipe_permeability_dict.items():
+            setattr(self, k, v)
+
+    def _soil_to_groundwater(self):
+        ''' 
+        Calculate the concentration in soil given the concentration in 
+        groundwater
+        '''
+        concentration_soil = (10 ** self.log_distribution_coefficient * self.concentration_groundwater 
+                              * self.ASSESSMENT_FACTOR_SOIL / self.ASSESSMENT_FACTOR_GROUNDWATER)
+
+        return concentration_soil
+
+    def set_conditions(self,
+                    chemical_name,                                    
+                    concentration_groundwater=None,
+                    concentration_soil=None,
+                    flow_rate=None,
+                    concentration_drinking_water=None,
+                    temperature_groundwater= TEMPERATURE_GROUNDWATER_DEFAULT, 
+                    stagnation_time = STAGNATION_TIME_DEFAULT,
+                    suppress_print = False, 
+                    language = 'NL'
+                    ):
+        ''' 
+        Specifies the chemical of interest, concentration and temperature in the 
+        groundwater and returns the parameters as attributes of the class. 
+        If the concentration of groundwater is given, or the soil concentration 
+        and Kd are known, the diffusion and permeation parameters are calculated 
+        for the pipe segment(s). 
+
+        Parameters
+        ----------
+        chemical_name: string
+            Name of the chemical for which to calculate the permeation
+        concentration_groundwater: float
+            Concentration of the given chemical in groundwater, g/m3
+        concentration_soil: float
+            Concentration of the given chemical in soil, mg/kg.
+        flow_rate: float
+            Flow rate through pipe, m3/day.
+        concentration_drinking_water: float
+            Concentration of given chemical in drinking water pipe, g/m3. If no 
+            value given, concentration is assigned the drinking water norm value.
+        temperature_groundwater: float
+            Temperature of the groundwater, degrees Celcius
+        stagnation_time: float
+            Time in seconds which water in pipe is stagnant, unit of seconds. The 
+            stagnation factor is only valid for a stagnation time of 8 hours 
+            (28800 seconds), therefore using another other stagnation time is not advised.
+        suppress_print: Boolean
+            Suppress printing the chemical name and matching name, e.g. in loop calculations
+        language: str
+            Language fo the chemical name to search for, default is Dutch ('NL'), 
+            English ('EN') also possible
+
+        '''
+
+        self.chemical_name = chemical_name
+        self.temperature_groundwater = temperature_groundwater
+        self.stagnation_time = stagnation_time
+
+        if (language == 'EN') or (language == 'NL'):
+            self.language = language
+        else: 
+            raise ValueError('Error, language must be one of "EN" or "NL" ')      
+
+        self._conditions_set = True
+
+        self.flow_rate = flow_rate
+        if flow_rate is not None:
+            self._flow_rate_set = True
+
+        self._fetch_chemical_database(chemical_name=self.chemical_name, 
+                                        suppress_print=suppress_print, 
+                                        language=language)
+
+
+        #check if there is a known distribution coefficient
+        if np.isnan(self.log_distribution_coefficient):
+            self._Kd_known = False
+        else: self._Kd_known = True
+
+        self.concentration_groundwater = concentration_groundwater
+        self.concentration_soil = concentration_soil
+
+        if (concentration_groundwater is None) and (concentration_soil is None):
+            pass #values already assigned, are None
+        if (concentration_groundwater is not None) and (concentration_soil is None) and (self._Kd_known): 
+            self.concentration_soil = self._soil_to_groundwater()
+        if (concentration_groundwater is None) and (concentration_soil is not None) and (self._Kd_known): 
+            self.concentration_groundwater = ((self.concentration_soil * self.ASSESSMENT_FACTOR_GROUNDWATER) 
+                                                / ( 10 ** self.log_distribution_coefficient * self.ASSESSMENT_FACTOR_SOIL ))
+        if (concentration_groundwater is not None) and (concentration_soil is not None) and (self._Kd_known):
+            # @martin, take the gw concentration over the given soil concentration?
+            # or check the Kd? 
+            print('Warning, both concentration_groundwater and concentration_soil given. Only using concentration_groundwater')
+            self.concentration_soil = self._soil_to_groundwater()
+
+        if self.concentration_groundwater is not None:
+            self._concentration_groundwater_set = True
+
+        # The default value for the concentration_drinking_water is the drinking water norm
+        if concentration_drinking_water is None:
+            self.concentration_drinking_water = self.Drinking_water_norm
+
+        else: 
+            self.concentration_drinking_water = concentration_drinking_water
+
+        if self.concentration_groundwater is not None: 
+            # self.validate_input_parameters()
+            for segment in self.segment_list:          
+                segment._calculate_pipe_K_D(pipe = self, 
+                                            _conditions_set=self._conditions_set, )
+
+
+    def view_database_chemical_names(self, 
+                                     language='NL'):
+        '''
+        Function to view a list of the possible chemical names from the database.
+
+        Parameters
+        ----------
+        language: str
+            Language fo the chemical name to search for, default is Dutch ('NL'), 
+            English ('EN') also possible
+        '''
+
+        return list(self.ppc_database['chemical_name_'+language])
+
+    def _check_max_terations_tolerance(self,
+                                       max_iterations, 
+                                       tolerance):
+        ''' 
+        Check the input values for max_iterations and the tolerance.
+
+        Parameters
+        ----------
+        tolerance: float 
+            The degree of acceptable error in the accuracy of the calculation, 
+            calculated as the difference between the calculated and actual drinking 
+            water concentration, default value of 0.01 (1%), [-].
+        max_iterations: int
+            Maximum number of iterations allowed in the optimization scheme
+        '''
+
+        if max_iterations <= 0:
+            raise ValueError('Error, max_iterations must be > 0')
+        else: 
+            self.max_iterations = int(max_iterations)
+
+        if (tolerance <= 0) or (tolerance > 1):
+            raise ValueError('Error, tolerance must be between 0 and 1')
+        else: 
+            self.tolerance = tolerance
+
+    def calculate_mean_dw_concentration(self, 
+                                        tolerance = TOLERANCE_DEFAULT,
+                                        max_iterations = MAX_ITERATIONS_DEFAULT,
+                                        debug=False,):
+        '''
+        Calculates the mean concentration in drinking water for a 24 hour period
+        given a groundwater concentration. 
+        
+        Parameters
+        ----------
+        tolerance: float 
+            The degree of acceptable error in the accuracy of the calculation, 
+            calculated as the difference between the calculated and actual drinking 
+            water concentration, default value of 0.01 (1%), [-].
+        max_iterations: int
+            Maximum number of iterations allowed in the optimization scheme
+
+        Returns
+        -------
+        mean_concentration_pipe_drinking_water: float
+            Calculates the mean concentration in drinking water for a 24 hour period
+            given a groundwater concentration.
+
+        '''
+        self._check_max_terations_tolerance(max_iterations=max_iterations, 
+                                       tolerance=tolerance)
+        
+        # Check if the flow rate, conditions have been set and parameters 
+        # validated, if not raise error
+        if self._flow_rate_set is False: 
+            raise ValueError('Error, the flow rate in the pipe has not been set. Input the flow rate in .set_conditions()')
+
+        if self._concentration_groundwater_set is False: 
+            raise ValueError('Error, the groundwater concentration has not been set. Input the groundwater concentration in .set_conditions()')
+
+        elif self._conditions_set is False:
+            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
+
+        elif self._is_validated is False: 
+            raise ValueError('Error, the input parameters must first be validated. To set validate use .validate_input_parameters() ')
+
+        else: 
+            counter = 0
+            concentration_drinking_water_n_plus_1 = 0 #initial guess for drinking water 
+            lower_limit = 0 # initial value for the lower limit
+            upper_limit = self.concentration_groundwater # initial value for the upper limit
+            goodness_fit_list = [0] # initial list of goodness_fit values
+            while True: 
+
+                # counter for the number of loops in the while statement, used to prevent infinite looping
+                counter +=1
+                # set the drinking water concentration to be the updated one from the last loop
+                concentration_drinking_water_n_min_1 = concentration_drinking_water_n_plus_1
+                # initalize summed mass of chemical in segments to 0
+                sum_mass_segment = 0
+                # calculate the mean dw mass per segment, and sum all segments for the pipe
+                for segment in self.segment_list:
+                    segment._calculate_mean_dw_mass_per_segment(pipe=self, 
+                                            concentration_drinking_water=concentration_drinking_water_n_min_1,
+                                            concentration_groundwater=self.concentration_groundwater,)
+                    sum_mass_segment += segment.mass_chemical_drinkwater
+
+                #calculate the dw concentration from the summed segments
+                concentration_drinking_water_n = (sum_mass_segment / 
+                                                self.flow_rate ) 
+                
+                # goodness_fit used to test if the calculated dw concentration is within the tolerance value for a correct solution
+                goodness_fit = abs(1 - concentration_drinking_water_n_min_1 
+                                    / concentration_drinking_water_n)
+                
+                # check if goodness_fit value meets the allowed tolerance value, 
+                # break loop is maximum iterations is exceeded
+                # if not calculate the new dw concentration
+                if goodness_fit <= tolerance:
+                    break
+                elif counter > max_iterations:
+                    print('Max iterations exceeded')
+                    break
+                else:
+                    goodness_fit_list.append(goodness_fit)
+                    
+                    # For the first two iterations use two set concentrations to begin the search for the solution, 
+                    # after the 2nd iteration, search for solution by half interval search
+                    if counter == 1: 
+                        concentration_drinking_water_n_plus_1 = self.concentration_groundwater * self.SCALE_FACTOR_UPPER_LIMIT 
+                    if counter == 2:
+                        concentration_drinking_water_n_plus_1 = self.concentration_groundwater * self.SCALE_FACTOR_LOWER_LIMIT
+                    if counter >2:
+                        if (goodness_fit < goodness_fit_list[counter-1]) or (concentration_drinking_water_n > self.concentration_groundwater):
+                            lower_limit = concentration_drinking_water_n_min_1
+                            concentration_drinking_water_n_plus_1 = lower_limit + (upper_limit -lower_limit)/2
+                        else:
+                            upper_limit = concentration_drinking_water_n_min_1
+                            concentration_drinking_water_n_plus_1 = lower_limit - (upper_limit -lower_limit)/2
+                    if debug: 
+                        print(concentration_drinking_water_n_min_1, concentration_drinking_water_n_plus_1, goodness_fit, lower_limit, upper_limit)
+
+            # assign the drinking water concentration to be the concentration calculated in the loop                            
+            self.concentration_drinking_water = concentration_drinking_water_n
+            if concentration_drinking_water_n > self.solubility:
+                print(f'Warning, the calculated drinking water concentration ({concentration_drinking_water_n}) is above the solubility limit, {self.solubility}.')
+
+        return concentration_drinking_water_n 
+
+
+    def calculate_peak_dw_concentration(self, 
+                                        tolerance = TOLERANCE_DEFAULT,
+                                        max_iterations = MAX_ITERATIONS_DEFAULT,
+                                        debug=False):
+
+        '''
+        Calculates the peak (maximum) concentration in drinking water for a 
+        given a stagnation period given a groundwater concentration.
+        Stagnation period default of 8 hours. 
+        
+        Parameters
+        ----------
+        tolerance: float 
+            The degree of acceptable error in the accuracy of the calculation, 
+            calculated as the difference between the calculated and actual drinking 
+            water concentration, default value of 0.01 (1%), [-].
+        max_iterations: int
+            Maximum number of iterations allowed in the optimization scheme
+
+        Returns
+        -------
+        peak_concentration_pipe_drinking_water: float
+            Calculates the peak (maximum) concentration in drinking water for a 
+            given a stagnation period given a groundwater concentration.
+
+        '''
+        self._check_max_terations_tolerance(max_iterations=max_iterations, 
+                                       tolerance=tolerance, )
+
+        if self.stagnation_time != self.STAGNATION_TIME_DEFAULT: 
+            print("Warning: the stagnation factor is only valid for a stagnation time of 8 hours. Using a different stagnation time is not advised.")
+
+        # Check if the conditions have been set and parameters 
+        # validated, if not raise error
+
+        if self._concentration_groundwater_set is False: 
+            raise ValueError('Error, the groundwater concentration has not been set. Input the groundwater concentration in .set_conditions()')
+
+        elif self._conditions_set is False:
+            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
+
+        elif self._is_validated is False: 
+            raise ValueError('Error, the input parameters must first be validated. To set validate use .validate_input_parameters() ')
+
+        else: 
+            counter = 0
+            concentration_drinking_water_n_plus_1 = 0
+            lower_limit = 0 # initial value for the lower limit
+            upper_limit = self.concentration_groundwater # initial value for the upper limit
+            goodness_fit_list = [0] # initial list of goodness_fit values
+
+            while True:                
+                # counter for the number of loops in the while statement, used to prevent infinite looping
+                counter +=1
+                # set the drinking water concentration to be the updated one from the last loop
+                concentration_drinking_water_n_min_1 = concentration_drinking_water_n_plus_1
+                # initalize summed mass of chemical in segments to 0
+                sum_mass_segment = 0
+                # calculate the mean dw mass per segment, and sum all segments for the pipe
+                for segment in self.segment_list:
+                    segment._calculate_peak_dw_mass_per_segment(pipe=self, 
+                                            concentration_drinking_water=concentration_drinking_water_n_min_1,
+                                            concentration_groundwater=self.concentration_groundwater,)
+
+                    sum_mass_segment += segment.mass_chemical_drinkwater
+                
+                #calculate the dw concentration from the summed segments
+                concentration_drinking_water_n = (sum_mass_segment / 
+                                                self.total_volume ) 
+                # goodness_fit used to test if the calculated dw concentration is within the tolerance value for a correct solution
+                goodness_fit = abs(1 - concentration_drinking_water_n_min_1 / concentration_drinking_water_n)
+                
+                # check if goodness_fit value meets the allowed tolerance value, 
+                # break loop is maximum iterations is exceeded
+                # if not calculate the new dw concentration
+                if goodness_fit <= tolerance:
+                    break
+                elif counter > max_iterations:
+                    print('Max iterations exceeded')
+                    break
+                else:
+                    goodness_fit_list.append(goodness_fit)
+                    
+                    # For the first two iterations use two set concentrations to begin the search for the solution, 
+                    # after the 2nd iteration, search for solution by half interval search
+                    if counter == 1:
+                        concentration_drinking_water_n_plus_1 = self.concentration_groundwater * self.SCALE_FACTOR_UPPER_LIMIT
+                    if counter == 2:
+                        concentration_drinking_water_n_plus_1 = self.concentration_groundwater * self.SCALE_FACTOR_LOWER_LIMIT
+                    if counter >2:
+                        if (goodness_fit < goodness_fit_list[counter-1]) or (concentration_drinking_water_n > self.concentration_groundwater):
+                            lower_limit = concentration_drinking_water_n_min_1
+                            concentration_drinking_water_n_plus_1 = lower_limit + (upper_limit -lower_limit)/2
+                        else:
+                            upper_limit = concentration_drinking_water_n_min_1
+                            concentration_drinking_water_n_plus_1 = lower_limit - (upper_limit -lower_limit)/2
+                    if debug: 
+                        print(concentration_drinking_water_n_min_1, concentration_drinking_water_n_plus_1, goodness_fit, lower_limit, upper_limit)
+
+            # assign the drinking water concentration to be the concentration calculated in the loop                            
+            self.concentration_drinking_water = concentration_drinking_water_n
+            if concentration_drinking_water_n > self.solubility:
+                print(f'Warning, the calculated drinking water concentration ({concentration_drinking_water_n}) is above the solubility limit, {self.solubility}.')
+
+        return concentration_drinking_water_n
+
+
+    def calculate_mean_allowable_gw_concentration(self, 
+                                        tolerance = TOLERANCE_DEFAULT,
+                                        max_iterations = MAX_ITERATIONS_DEFAULT, 
+                                        debug=False,):
+        '''
+        Calculates the mean 24 hour concentration in groundwater which would not 
+        result in a drinking water concentration exceeding the drinking water
+        norm. If the distribution coefficient is known the soil concentration is
+        also calculated. 
+
+        Parameters
+        ----------
+        tolerance: float 
+            The degree of acceptable error in the accuracy of the calculation, 
+            calculated as the difference between the calculated and actual drinking 
+            water concentration, default value of 0.01 (1%), [-].
+        max_iterations: int
+            Maximum number of iterations allowed in the optimization scheme
+        debug: Boolean
+            If True, return the groundwater concentration, goodness_fit and lower and 
+            upper limits every iteration.
+ 
+        Returns
+        -------
+        concentration_mean_allowable_groundwater: float
+            Mean concentration in groundwater which would would not result in 
+            a mean daily (24 hours) concentration in drinking water exceeding 
+            the drinking water norm, g/m3.
+                    
+        '''
+        self._check_max_terations_tolerance(max_iterations=max_iterations, 
+                                       tolerance=tolerance)
+
+        # Check if the flow rate, conditions have been set and parameters 
+        # validated, if not raise error
+        if self._flow_rate_set is False: 
+            raise ValueError('Error, the flow rate in the pipe has not been set. To set flow rate use .set_flow_rate()')
+
+        elif self._conditions_set is False:
+            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
+
+        elif self._is_validated is False: 
+            raise ValueError('Error, the input parameters must first be validated. To set validate use .validate_input_parameters() ')
+        
+        if self.concentration_drinking_water is None:
+            raise ValueError('Error, no default drinking water norm, please input a drinking water concentration using .set_conditions()')
+
+        if self.concentration_drinking_water > self.solubility:
+            raise ValueError('Error, the drinking water concentration given or the default drinking water norm is higher than the solubility of the chemical. Input a lower drinking water concentration using .set_conditions()')
+
+        else: 
+            self._fetch_chemical_database(chemical_name=self.chemical_name, 
+                                          suppress_print = True,
+                                           language=self.language )
+
+            # calculate initial guess for gw concentration
+            sum_KDA_d = 0
+
+            for segment in self.segment_list:
+                # calculate the sum of the Kpw * DP * SA / d for all pipe segments
+                log_Dp_ref = segment._calculate_ref_logD(chemical_group_number=self.chemical_group_number,
+                            molecular_weight=self.molecular_weight)
+                log_Kpw_ref = segment._calculate_ref_logK(chemical_group_number=self.chemical_group_number,
+                            log_octanol_water_partitioning_coefficient=self.log_octanol_water_partitioning_coefficient)
+                
+                sum_KDA_d_segment = ( 10 ** log_Dp_ref * 10 ** log_Kpw_ref * segment.permeation_surface_area 
+                                    / segment.diffusion_path_length )
+
+                sum_KDA_d += sum_KDA_d_segment
+
+                # initial guess concentration in groundwater
+                concentration_groundwater_n_plus_1 = (self.concentration_drinking_water * (1
+                                         + self.flow_rate * self.ASSESSMENT_FACTOR_GROUNDWATER ) 
+                                            / sum_KDA_d ) * 24 * 60 * 60 
+            
+            counter = 0
+            lower_limit = self.concentration_drinking_water # initial value for the lower limit
+            upper_limit = self.solubility # initial value for the upper limit
+            goodness_fit_list = [0] # initial list of goodness_fit values
+
+            while True:
+                # counter for the number of loops in the while statement, used to prevent infinite looping
+                counter +=1                
+                # set the groundwater concentration to be the updated one from the last loop
+                concentration_groundwater_n_min_1 = concentration_groundwater_n_plus_1
+
+                # set the conditions for the pipe with the updated groundwater concentration
+                self.set_conditions(chemical_name=self.chemical_name,                                    
+                    concentration_groundwater=concentration_groundwater_n_min_1,
+                    flow_rate=self.flow_rate,
+                    concentration_drinking_water=self.concentration_drinking_water, 
+                    temperature_groundwater=self.temperature_groundwater, 
+                    stagnation_time = self.stagnation_time,
+                    suppress_print = True, 
+                    language = self.language)
+
+                # initalize summed mass of chemical in segments to 0
+                sum_mass_segment = 0
+
+                # mass of chemical in pipe water to meet drinking water norm
+                mass_drinkingwater_norm = (self.concentration_drinking_water * self.flow_rate)
+
+                # calculate the mean dw mass per segment, and sum all segments for the pipe
+                for segment in self.segment_list:
+                    segment._calculate_mean_dw_mass_per_segment(pipe=self, 
+                                            concentration_drinking_water=self.concentration_drinking_water,
+                                            concentration_groundwater=self.concentration_groundwater,)
+
+                    sum_mass_segment += segment.mass_chemical_drinkwater
+                
+                # goodness_fit used to test if the calculated dw concentration is within the tolerance value for a correct solution
+                goodness_fit = abs(1 - mass_drinkingwater_norm / sum_mass_segment)
+
+                # check if goodness_fit value meets the allowed tolerance value, 
+                # break loop is maximum iterations is exceeded
+                # if not calculate the new gw concentration
+                if goodness_fit <= tolerance:
+                    if debug:
+                        print(concentration_groundwater_n_min_1, concentration_groundwater_n_plus_1, goodness_fit, lower_limit, upper_limit) #for debugging
+                    break
+                elif counter > max_iterations:
+                    print('Max iterations exceeded')
+                    break
+                elif upper_limit == lower_limit:
+                    print('No solution found, lower_limit = upper_limit. Groundwater concentration necesary to satisfy the given drinking water concentration may be above the solubility limit.')
+                    break
+                else:
+                    goodness_fit_list.append(goodness_fit)
+
+                    # For the first two iterations use two set concentrations to 
+                    # begin the search for the solution, after the 2nd iteration
+                    # search for solution by half interval search
+                    if counter == 1:
+                        concentration_groundwater_n_plus_1 = self.solubility * self.SCALE_FACTOR_UPPER_LIMIT
+                    if counter == 2:
+                        concentration_groundwater_n_plus_1 = 0
+                    if counter >2:
+                        if (goodness_fit < goodness_fit_list[counter-1]) or (concentration_groundwater_n_plus_1 < self.concentration_drinking_water):
+                            lower_limit = concentration_groundwater_n_min_1
+                            concentration_groundwater_n_plus_1 = lower_limit + (upper_limit -lower_limit)/2
+                        else:
+                            upper_limit = concentration_groundwater_n_min_1
+                            concentration_groundwater_n_plus_1 = lower_limit - (upper_limit -lower_limit)/2
+                    if debug: 
+                        print(concentration_groundwater_n_min_1, concentration_groundwater_n_plus_1, goodness_fit, lower_limit, upper_limit) #for debugging
+
+        # assign the groundwater concentration to be the concentration calculated in the loop                            
+        self.concentration_groundwater = concentration_groundwater_n_min_1
+
+        if concentration_groundwater_n_min_1 > self.solubility:
+            print(f'Warning, the calculated drinking water concentration ({concentration_groundwater_n_min_1}) is above the solubility limit, {self.solubility}.')
+
+        if self._Kd_known: 
+            self.concentration_soil = self._soil_to_groundwater()
+        else: 
+            self.concentration_soil = 'No known distribution coefficient to calculate soil concentration'
+
+        return concentration_groundwater_n_min_1 
+
+
+    def calculate_peak_allowable_gw_concentration(self, 
+                                    tolerance = TOLERANCE_DEFAULT,
+                                    max_iterations = MAX_ITERATIONS_DEFAULT,
+                                    debug=False,):
+        '''
+        Calculates the peak (maximum) concentration in groundwater water for a 
+        given a stagnation period that would not result in a peak concentration 
+        in drinking water exceeding the drinking water norm for each pipe segment.
+        Stagnation period default of 8 hours. If the distribution coefficient is 
+        known the soil concentration is also calculated. 
+
+        Parameters
+        ----------
+        tolerance: float 
+            The degree of acceptable error in the accuracy of the calculation, 
+            calculated as the difference between the calculated and actual drinking 
+            water concentration, default value of 0.01 (1%), [-].
+        max_iterations: int
+            Maximum number of iterations allowed in the optimization scheme
+        debug: Boolean
+            If True, return the groundwater concentration, goodness_fit and lower and 
+            upper limits every iteration.
+
+            
+        Returns
+        -------
+        concentration_peak_allowable_groundwater: float
+            Concentration in groundwater which, after a stagnation period, 
+            would not result in a peak concentration in drinking water exceeding 
+            the drinking water norm, g/m3.
+            
+        '''
+        self._check_max_terations_tolerance(max_iterations=max_iterations, 
+                                       tolerance=tolerance)
+
+        if self.stagnation_time != self.STAGNATION_TIME_DEFAULT:
+            print("Warning: the stagnation factor is only valid for a stagnation time of 8 hours. Using a different stagnation time is not advised.")
+
+        # Check if the conditions have been set and parameters validated, if not raise error
+        elif self._conditions_set is False:
+            raise ValueError('Error, the pipe conditions must first be set. To set pipe conditions use .set_conditions() ')
+
+        elif self._is_validated is False: 
+            raise ValueError('Error, the input parameters must first be validated. To set validate use .validate_input_parameters() ')
+
+        if self.concentration_drinking_water > self.solubility:
+            raise ValueError('Error, the drinking water concentration given or the default drinking water norm is higher than the solubility of the chemical. Input a lower drinking water concentration using .set_conditions()')
+
+        else: 
+
+            self._fetch_chemical_database(chemical_name=self.chemical_name, 
+                                          suppress_print = True, 
+                                          language=self.language)
+
+            # calculate initial guess for gw concentration
+            sum_KDA_d = 0
+            for segment in self.segment_list:
+                # calculate the sum of the Kpw * DP * SA *f_stag / d for all pipe segments
+                log_Dp_ref = segment._calculate_ref_logD(chemical_group_number=self.chemical_group_number,
+                            molecular_weight=self.molecular_weight)
+                log_Kpw_ref = segment._calculate_ref_logK(chemical_group_number=self.chemical_group_number,
+                            log_octanol_water_partitioning_coefficient=self.log_octanol_water_partitioning_coefficient)
+                
+                #stagnation factor with reference values for LogDp and LogKpw
+                stagnation_factor = 10 ** max((((log_Dp_ref + 12.5) / 2 + 
+                                    log_Kpw_ref) * 0.73611 + 
+                                    -1.03574 ), 0)            
+
+                sum_KDA_d_segment = ( 10 ** log_Dp_ref * 10 ** log_Kpw_ref * segment.permeation_surface_area 
+                                    * stagnation_factor / segment.diffusion_path_length )
+
+                sum_KDA_d += sum_KDA_d_segment
+
+            # initial guess concentration in groundwater
+            concentration_groundwater_n_plus_1 = self.concentration_drinking_water * (1 
+                                        + self.total_volume * self.ASSESSMENT_FACTOR_GROUNDWATER 
+                                        / self.stagnation_time / sum_KDA_d) 
+            
+            counter = 0
+            lower_limit = self.concentration_drinking_water # initial value for the lower limit
+            upper_limit = self.solubility # initial value for the upper limit
+            goodness_fit_list = [0] # initial list of goodness_fit values
+
+            while True: 
+                # counter for the number of loops in the while statement, used to prevent infinite looping
+                counter +=1                
+                # set the groundwater concentration to be the updated one from the last loop
+                concentration_groundwater_n_min_1 = concentration_groundwater_n_plus_1
+
+                # set the conditions for the pipe with the updated groundwater concentration
+                self.set_conditions(chemical_name=self.chemical_name,                                    
+                    concentration_groundwater=concentration_groundwater_n_min_1,
+                    flow_rate=self.flow_rate,
+                    concentration_drinking_water=self.concentration_drinking_water, 
+                    temperature_groundwater=self.temperature_groundwater, 
+                    stagnation_time = self.stagnation_time,
+                    suppress_print = True, 
+                    language = self.language)
+                
+                # initalize summed mass of chemical in segments to 0
+                sum_mass_segment = 0
+
+                # mass of chemical in pipe water to meet drinking water norm
+                mass_drinkingwater_norm = (self.concentration_drinking_water * self.total_volume) 
+
+                # calculate the mean dw mass per segment, and sum all segments for the pipe
+                for segment in self.segment_list:
+                    segment._calculate_peak_dw_mass_per_segment(pipe=self, 
+                                            concentration_drinking_water=self.concentration_drinking_water,
+                                            concentration_groundwater=self.concentration_groundwater,)
+
+                    sum_mass_segment += segment.mass_chemical_drinkwater
+
+                # goodness_fit used to test if the calculated dw concentration is within the tolerance value for a correct solution
+                goodness_fit = abs(1 - mass_drinkingwater_norm / sum_mass_segment)
+
+                # check if goodness_fit value meets the allowed tolerance value, 
+                # break loop is maximum iterations is exceeded
+                # if not calculate the new gw concentration
+                if goodness_fit <= tolerance:
+                    break
+                elif counter > max_iterations:
+                    print('Max iterations exceeded')
+                    break
+                elif upper_limit == lower_limit:
+                    print('No solution found, lower_limit = upper_limit. Groundwater concentration necesary to satisfy the given drinking water concentration may be above the solubility limit.')
+                    break
+                else:
+                    goodness_fit_list.append(goodness_fit)
+
+                    # two initial guesses to compare the goodness of fit
+                    if counter == 1:
+                        concentration_groundwater_n_plus_1 = self.solubility * self.SCALE_FACTOR_UPPER_LIMIT
+                    if counter == 2:
+                        concentration_groundwater_n_plus_1 = 0
+                    if counter >2:
+                        if (goodness_fit < goodness_fit_list[counter-1]) or (concentration_groundwater_n_plus_1 < self.concentration_drinking_water):
+                            lower_limit = concentration_groundwater_n_min_1
+                            concentration_groundwater_n_plus_1 = lower_limit + (upper_limit -lower_limit)/2
+                        else:
+                            upper_limit = concentration_groundwater_n_min_1
+                            concentration_groundwater_n_plus_1 = lower_limit - (upper_limit -lower_limit)/2
+                    if debug: 
+                        print(concentration_groundwater_n_min_1, concentration_groundwater_n_plus_1, goodness_fit, lower_limit, upper_limit) #for debugging
+        
+        # assign the groundwater concentration to be the concentration calculated in the loop
+        self.concentration_groundwater = concentration_groundwater_n_min_1
+        
+        if concentration_groundwater_n_min_1 > self.solubility:
+            print(f'Warning, the calculated drinking water concentration ({concentration_groundwater_n_min_1}) is above the solubility limit, {self.solubility}.')
+
+        if self._Kd_known: 
+            self.concentration_soil = self._soil_to_groundwater()
+        else: 
+            self.concentration_soil = 'No known distribution coefficient to calculate soil concentration'
+
+        return concentration_groundwater_n_min_1 
+
+
```

### Comparing `pipepermcalc-0.0.5/pipepermcalc/segment.py` & `pipepermcalc-0.8.6/pipepermcalc/segment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,688 +1,705 @@
-#%% ----------------------------------------------------------attributes------------------
-# A. Hockin, January 2023
-# KWR 403230-003
-# Pipe permeation calculator
-# With Martin vd Schans, Bram Hillebrand, Lennart Brokx
-#
-# ------------------------------------------------------------------------------
-import numpy as np
-import pandas as pd
-
-from pipepermcalc.pipe import * 
-
-class Segment:
-    ''' 
-    Segment object class to make segments of the pipe.
-
-    Attributes
-    ----------
-
-    PARTITIONING_A_DH: float
-        Coefficient for correcting the partitioning coefficient for temperature. 
-        From regression analysis, a is the slope, see table 5-6 in 
-        KWR 2016.056. Constant equal to 7.92169801506708. 
-    PARTITIONING_B_DH: float,
-        Coefficient for correcting the partitioning coefficient for temperature. 
-        From regression analysis, b is the intercept, see table 5-6 in 
-        KWR 2016.056. Constant equal to -17.1875608983359. 
-    DIFFUSION_A_DH: float 
-        Coefficient for correcting the diffusion coefficient for temperature. 
-        From regression analysis, a is the slope, see table 5-6 in 
-        KWR 2016.056. Constant equal to 61.8565740136974. 
-    DIFFUSION_B_DH: float
-        Coefficient for correcting the diffusion coefficient for temperature. 
-        From regression analysis, b is the intercept, see table 5-6 in 
-        KWR 2016.056. Constant equal to -78.9191401984509. 
-    PARTITIONING_A_C: float
-        Constant used in the correction for the partitioning coefficent due to 
-        the influence of temperature. See equation 5-20 in KWR 2016.056, for 
-        partitioning a_c = 0.103965019849463.
-    PARTITIONING_CREF_SW: float
-        Reference concentration used in the correction for the partitioning 
-        coefficent due to the influence of temperature. Ssee section 5.4.7 in 
-        KWR 2016.056. For partitioning, Cref_SW = 1.0.
-    DIFFUSION_A_C: float
-        Constant used in the correction for the diffusion coefficent due to 
-        the influence of temperature. See equation 5-18 in KWR 2016.056, for 
-        diffusion a_c = 0.784077209735583.
-    DIFFUSION_CREF_SW: float
-        Reference concentration used in the correction for the diffusion 
-        coefficent due to the influence of temperature. Ssee section 5.4.6 in 
-        KWR 2016.056. For partitioning, Cref_SW = 0.5.
-
-    name: string
-        name of the pipe segment
-    material: string
-        e.g. PE40, PE80, PVC, EPDM, rubber etc.
-    length: float
-        Length of the pipe segment, meters 
-    inner_diameter: float
-        Inner diameter of the pipe segment, meters
-    wall_thickness: float
-        wall_thickness of the pipe segment, meters
-    permeation_direction: string
-        Direction of permeation through the pipe segment. Options are 
-        'perpendicular' or 'parallel'. Default permeation is perpendicular 
-        to the flow direction. See schematic XX in read the docs. 
-    diffusion_path_length: float
-        In the case of permeation perpendicular to the flow direction, a 
-        diffusion path length is required to calculate the permeation through 
-        the pipe segment. For example in the case of a pipe coupling rings. 
-        Default permeation is perpendicular to the flow direction and the 
-        wall_thickness is used to calculate the diffusion through the pipe 
-        segment. Unit meters.
-    volume: float
-        Volume of the pipe segment, m3
-    permeation_surface_area: float
-        Surface area through which permeation takes place. If permeation is 
-        perpendicular to the flow, the permeation surface area is the inner 
-        surface area of the pipe. If diffusion is parallel to the flow, the 
-        permeation surface area is the annular area of the rubber. 
-    outer_diameter: float
-        Outer diameter of the pipe segment, unit m.
-    log_Kpw_ref: float
-        partitioning coefiicient under lab conditions, [-]
-    f_Ktemp: float
-        Temperature correction factor for partitioning coefficient, [-]
-    f_Kconc: float
-        Concentration correction factor for partitioning coefficient, [-]
-    log_Kpw: float
-        Calculated log partitioning coefficient for the given chemical and pipe material, [-]
-    log_Dp_ref: float
-        Diffusion coefficient under lab conditions, m2/s.
-    f_Dtemp:float
-        Temperature correction factor for diffusion coefficient, m2/s.
-    f_Dconc: float
-        Concentration correction factor for diffusion coefficient, [m2/s.
-    log_Dp: float
-        Calculated log diffusion coefficient for the given chemical and pipe material, m2/s.
-    stagnation_factor: float
-        Correction for the decrease in the concentratino gradient near the 
-        inner wall of the pipe during stagnation (e.g. no flow at at night)
-    mass_chemical_drinkwater: float
-        Mass of the given chemical in the pipe segment, g.
-    
-    Note
-    ----
-    All parameters are in SI units: m, m2, g/m3 (equivalent to mg/L), seconds.
-
-
-    '''
-
-    count = 0 # count of pipe segments
-
-    def __init__(self, 
-                name=None,
-                material=None,
-                length=None,
-                inner_diameter=None,
-                wall_thickness=None,
-                permeation_direction='perpendicular',
-                diffusion_path_length=None,
-                ):
-        '''
-        Creates a pipe segment with the attributes of the pipe (length, 
-        wall_thickness, diameter, material etc.). 
-        
-        Parameters
-        ----------
-        name: string
-            name of the pipe segment
-        material: string
-            e.g. PE40, PE80, PVC, EPDM, rubber etc.
-        length: float
-            Length of pipe segment, meters 
-        inner_diameter: float
-            Inner diameter of pipe segment, meters
-        wall_thickness: float
-            wall_thickness of pipe segment, meters
-        permeation_direction: string
-            Direction of permeation through the pipe segment. Options are 
-            'perpendicular' or 'parallel'. Default permeation is perpendicular 
-            to the flow direction. See schematic XX in read the docs.
-        diffusion_path_length: float
-            In the case of permeation perpendicular to the flow direction, a 
-            diffusion path length is required to calculate the permeation through 
-            the pipe segment. For example in the case of a pipe coupling rings. 
-            Default permeation is perpendicular to the flow direction and the 
-            wall_thickness is used to calculate the diffusion through the pipe 
-            segment. Unit meters.
-        '''  
-
-        #Constants for various LogK and Log D equations
-        self._PARTITIONING_A_DH = 7.92169801506708 #see table 5-6 in KWR 2016.056
-        self._PARTITIONING_B_DH = -17.1875608983359 #see table 5-6 in KWR 2016.056
-        self._DIFFUSION_A_DH = 61.8565740136974 #see table 5-6 in KWR 2016.056
-        self._DIFFUSION_B_DH = -78.9191401984509 #see table 5-6 in KWR 2016.056
-        self.PARTITIONING_A_C = 0.103965019849463 #see equation 5-20 in KWR 2016.056
-        self.PARTITIONING_CREF_SW = 1.000 #see section 5.4.7 in KWR 2016.056
-        self.DIFFUSION_A_C = 0.784077209735583 #see equation 5-18 in KWR 2016.056
-        self.DIFFUSION_CREF_SW = 0.5 #see section 5.4.6 in KWR 2016.056
-
-        self.name = name
-        self.material = material
-
-        self.length = float(length)
-        self.inner_diameter = float(inner_diameter)
-        self.wall_thickness = float(wall_thickness)
-        self.permeation_direction = permeation_direction
-
-        if diffusion_path_length is None:
-            self.diffusion_path_length = self.wall_thickness
-        else:
-            self.diffusion_path_length = float(diffusion_path_length)    
-
-        outer_diameter = inner_diameter + wall_thickness
-        volume = np.pi * (inner_diameter / 2) ** 2 * length
-        permeation_surface_area =(np.pi * inner_diameter * length)
-
-        if permeation_direction == 'parallel':
-            volume = 0 
-            permeation_surface_area = ((np.pi * ((inner_diameter + wall_thickness) ** 2 
-                                                - inner_diameter ** 2) ) / 4)
-                   
-        self.volume = volume
-        self.permeation_surface_area = permeation_surface_area
-        self.outer_diameter = outer_diameter
-        self.inner_diameter = inner_diameter
-
-    # @MartinK-> suggest to implement the "named tuple" method, leave for now do at the end
-    # #ah_todo SBR, EPDM refer to memo, ask m. meerkerk for memo number, include 
-    # project number for the memo
-
-    # reference_pipe_material_dict: dictionary 
-    #     Reference dictionary with regression values (slope=a-value, intercept=b-value)
-    #     for the partitioning (K) and diffusion (D) coefficient for the available 
-    #     plastics (PE40, PE80, SBR, EPDM) per chemical groups. 
-    #     Used to calculate the specifice partitioning or diffusion coefficient 
-    #     from the reference value. 
-    #     Chemical group numbers: Expert opinion (M. Meerkerk), @alex be aware of dutch in the comments (onbekend, overig)
-    #     see table 5-4 KWR 2016.056, Group 1: PAK, MAK, ClArom, ClAlk, Arom, Alk
-    #     Group 2: PCB, Group 3: overig, onbekend, O2, Cl, BDE
-    reference_pipe_material_dict = \
-        {
-        "PE40": {
-            "REF_LOG_D_A": {
-                1: -0.011,	
-                2: -0.00629,
-                3: -0.006,
-                },
-            "REF_LOG_D_B": {
-                1: -10.688,
-                2: -11.000,
-                3: -11.000
-                },
-            "REF_LOG_K_A": {
-                1: 1.097,
-                2: 1.059,
-                3: 0.979
-                },
-            "REF_LOG_K_B": {
-                1: -0.689,
-                2: -0.67,
-                3: -1.796,
-                },
-        },
-        "PE80": {
-            "REF_LOG_D_A": {
-                1: -0.011,	
-                2: -0.00629,
-                3: -0.00629,
-                },
-            "REF_LOG_D_B": {
-                1: -11.188,
-                2: -11.188,
-                3: -11.500,
-                },
-            "REF_LOG_K_A": {
-                1: 1.185,	
-                2: 1.185,
-                3: 1.231,
-                },
-            "REF_LOG_K_B": {
-                1: -1.437,	
-                2: -1.437,
-                3: -2.606,
-                },
-        },
-        "SBR": {
-            "REF_LOG_D_A": {
-                1: -0.011 * 0.950647410867427,	
-                2: -0.00629 * 0.950647410867427,
-                3: -0.006 * 0.950647410867427,
-                },
-            "REF_LOG_D_B": {
-                1: -10.688 * 0.950647410867427,
-                2: -11.000 * 0.950647410867427,
-                3: -11.000 * 0.950647410867427,
-                },
-            "REF_LOG_K_A": {
-                1: 1.0452,	
-                2: 1.0452,
-                3: 1.0452,
-                },
-            "REF_LOG_K_B": {
-                1: -0.3686,	
-                2: -0.3686,
-                3: -0.3686,
-                },
-        },  
-        "EPDM": {
-            "REF_LOG_D_A": {
-                1: -0.011* 0.920996123470591,	
-                2: -0.00629 * 0.920996123470591,
-                3: -0.006 * 0.920996123470591,
-                },
-            "REF_LOG_D_B": {
-                1: -10.688 * 0.920996123470591,
-                2: -11.000 * 0.920996123470591,
-                3: -11.000 * 0.920996123470591,
-                },
-            "REF_LOG_K_A": {
-                1: 1.0675,	
-                2: 1.0675,
-                3: 1.0675,
-                },
-            "REF_LOG_K_B": {
-                1: -0.3002,	
-                2: -0.3002,
-                3: -0.3002,
-                },
-        },  
-        "PVC": { #Diffusion through PVC is zero
-            "REF_LOG_D_A": {
-                1: 0,	
-                2: 0,
-                3: 0,
-                },
-            "REF_LOG_D_B": {
-                1: 0,	
-                2: 0,
-                3: 0,
-                },
-            "REF_LOG_K_A": {
-                1: 0,	
-                2: 0,
-                3: 0,
-                },
-            "REF_LOG_K_B": {
-                1: 0,	
-                2: 0,
-                3: 0,
-                },
-        },               
-        }
-
-    def _correct_for_temperature(self,
-                                temperature_groundwater,
-                                coefficient_name=None, 
-                                a_dh=None,
-                                b_dh=None,
-                                ):
-        '''
-        Temperature correction for the partitioning and diffusion coefficients. 
-        See table 5-3 in KWR 2016.056
-
-        Parameters
-        ----------
-        temperature_groundwater: float
-            Temperature of the groundwater, degrees Celcius
-        coefficient_name: string
-            Either 'solubility' or 'molecular_weight'
-        a_dh: string
-            Coefficient for correcting the partitioning or diffusion coefficient
-        b_dh: string
-            Coefficient for correcting the partitioning or diffusion coefficient
-
-        Returns
-        -------
-        f_temp: string
-            Temperature correction factor for the partitioning or diffusion 
-            coefficient.
-        '''
-
-        R = 0.008314 #universal gas constant
-        reference_temperature = 25 # deg. C
-        dh = a_dh * np.log10(coefficient_name) + b_dh
-        f_temp = dh / (R * np.log(10)) * (1 / (reference_temperature + 273) - 1 / (temperature_groundwater + 273))
-        return f_temp, dh
-
-
-    def _concentration_correction(self,
-                        solubility, 
-                        concentration_groundwater,
-                        a_c=None,
-                        Cref_Sw=None):
-        '''
-        Correction factor for the influence of concentration on the 
-        partitioning or diffusion coefficient. 
-        See table 5-3, equations 5-17 and 5-19 in KWR 2016.056
-
-        Parameters
-        ----------
-        solubility:	float
-            solubility of given chemical in water, g/m3
-        concentration_groundwater: float
-            Concentration of the given chemical in groundwater, g/m3.
-        a_c: float
-            Constant used in the correction for the partitioning or diffusion 
-            coefficent due to the influence of temperature. See equations 5-18 
-            and 5-20 in KWR 2016.056. 
-        Cref_Sw: float
-            Reference concentration used in the correction for the diffusion or 
-            partitioning coefficent due to the influence of temperature. See 
-            sections 5.4.6 and 5.4.7 in KWR 2016.056. 
-            
-        Returns
-        -------
-        f_conc: string
-            Concentration correction factor for the diffusion or partitioning
-            coefficient.
-        '''
-
-        Cg_Sw = min(concentration_groundwater / solubility, 1)
-        f_conc = a_c * (Cg_Sw - Cref_Sw)
-
-        return f_conc
-
-
-    def _correct_for_age(self,):
-        '''
-        Age correction, none implemented yet
-        
-        Returns
-        -------
-        f_age: float
-            Age correction for the partitioning or diffusion coefficient.
-        '''
-
-        f_age = 0.000
-        return f_age
-
-
-    def _calculate_ref_logK(self,
-                            chemical_group_number,
-                            log_octanol_water_partitioning_coefficient):
-        '''Calculate the reference partitioning coefficient for the pipe segment.
-        See tabel 5.3, equations 5-5, 5-6 in KWR 2016.056.  
-
-        Parameters
-        ----------
-        chemical_group_number: integer
-            Integer corresponding to the chemical group.
-        log_octanol_water_partitioning_coefficient:	float,
-            Partition coefficient for the two-phase system consisting of 
-            n-octanol and water, Log Kow, [-].
-
-        Returns
-        -------
-        log_Kpw_ref: float
-            partitioning coefiicient under lab conditions, [-].
-
-        '''
-
-        a_ref = self.reference_pipe_material_dict[self.material]['REF_LOG_K_A'][chemical_group_number]
-        b_ref = self.reference_pipe_material_dict[self.material]['REF_LOG_K_B'][chemical_group_number]
-        log_Kpw_ref = a_ref * log_octanol_water_partitioning_coefficient + b_ref
-
-        return log_Kpw_ref
-
-
-    def _calculate_ref_logD(self,
-                            chemical_group_number,
-                            molecular_weight):
-        '''
-        Calculate the reference diffusion (log D) based on the pipe material. A fixed 
-        ratio between the log of the diffusion coefficient of PE-40 (logD_p) 
-        and of SBR/EPDM (logD_s, logD_e) in m2/s is assumed for SBR and 
-        EPDM for the determination of the diffusion coefficient, see memo 2022 
-        "Permeatie door rubber afdichtingen van drinkwaterleidingen."  
-        #ah_todo find memo number
-
-        Parameters
-        ----------
-        chemical_group_number: integer
-            Integer corresponding to the chemical group.
-        molecular_weight: float
-            Mass of one mole of a given chemical, g/mol.
-
-        Returns
-        -------
-        log_Dp_ref: float
-            Diffusion coefficient under lab conditions, m2/s.
-        '''
-
-        if np.isnan(molecular_weight):
-            raise ValueError('Error, the molecular weight for this chemical is not known, therefore it is not possible to calculate the permeation.')
-
-
-        a_ref = self.reference_pipe_material_dict[self.material]['REF_LOG_D_A'][chemical_group_number]
-        b_ref = self.reference_pipe_material_dict[self.material]['REF_LOG_D_B'][chemical_group_number]
-        log_Dp_ref = a_ref * molecular_weight + b_ref
-
-        return log_Dp_ref    
-
-
-    def _calculate_logK(self, 
-                        pipe):
-        ''' 
-        Calculate the partitioning coefficient (Log K) value for the pipe material, 
-        corrected for temperature,concentration and age. 
-        
-        See table 5-3 in KWR 2016.056 for explanation of calculations. 
-
-        Parameters
-        ----------
-        pipe: object
-            Pipe object of the segment.
-
-        Returns
-        -------
-        log_Kpw: float
-            Calculated log partitioning coefficient for the given chemical and 
-            pipe material, [-]
-        '''
-
-        # calculate reference log K plastic-water (log kpw) 
-        log_Kpw_ref = self._calculate_ref_logK(chemical_group_number=pipe.chemical_group_number,
-                                               log_octanol_water_partitioning_coefficient= pipe.log_octanol_water_partitioning_coefficient)
-
-        # correct for temperature, concentration, age
-        f_Ktemp, K_dh = self._correct_for_temperature(coefficient_name = pipe.solubility,
-                            temperature_groundwater = pipe.temperature_groundwater, 
-                            a_dh = self._PARTITIONING_A_DH, 
-                            b_dh = self._PARTITIONING_B_DH, )
-
-        f_Kconc = self._concentration_correction(solubility=pipe.solubility, 
-                                concentration_groundwater = pipe.concentration_groundwater,
-                                a_c = self.PARTITIONING_A_C,
-                                Cref_Sw = self.PARTITIONING_CREF_SW) 
-        
-        f_Kage = self._correct_for_age()
-
-        if self.material == 'PVC':
-            f_Ktemp = 0
-            f_Kconc = 0
-            f_Kage = 0
-            log_Kpw_ref = 0
-
-        # sum corrections for final Log k
-        log_Kpw = log_Kpw_ref + f_Ktemp + f_Kconc + f_Kage
-        
-        self.log_Kpw_ref = log_Kpw_ref
-        self.f_Ktemp = f_Ktemp   
-        self.f_Kconc = f_Kconc
-        self.partitioning_enthalpie = K_dh
-        self.log_Kpw = log_Kpw
-
-        return log_Kpw
-
-
-    def _calculate_logD(self, 
-                        pipe):
-        ''' 
-        Calculate the LogK value for the pipe material, correct for temperature,
-        concentration and age. 
-
-        See table 5-3 in KWR 2016.056 for explanation of calculations
-
-        Parameters
-        ----------
-        pipe: object
-            Pipe object of the segment.
-
-        Returns
-        -------
-        log_Dp: float
-            Calculated log diffusion coefficient for the given chemical and pipe 
-            material, m2/s.
-        '''
-        
-        # calculate reference log D plastic (log Dp) 
-        log_Dp_ref = self._calculate_ref_logD(chemical_group_number=pipe.chemical_group_number,
-                            molecular_weight=pipe.molecular_weight)
-
-        # correct for temperature, concentration, age
-        f_Dtemp, D_dh = self._correct_for_temperature(coefficient_name =pipe.molecular_weight,
-                            temperature_groundwater = pipe.temperature_groundwater, 
-                            a_dh = self._DIFFUSION_A_DH, 
-                            b_dh = self._DIFFUSION_B_DH,)
-
-        f_Dconc = self._concentration_correction(
-                                solubility=pipe.solubility, 
-                                concentration_groundwater = pipe.concentration_groundwater,
-                                a_c = self.DIFFUSION_A_C , 
-                                Cref_Sw = self.DIFFUSION_CREF_SW) 
-        
-        f_Dage = self._correct_for_age()
-
-        if self.material == 'PVC':
-            f_Dtemp = 0
-            f_Dconc = 0
-            f_Dage = 0
-            log_Dp_ref = 0
-
-        # sum corrections for final Log D
-        log_Dp = log_Dp_ref + f_Dtemp + f_Dconc + f_Dage
-
-        self.log_Dp_ref = log_Dp_ref
-        self.f_Dtemp = f_Dtemp  
-        self.activattion_energy = D_dh
-        self.f_Dconc = f_Dconc
-        self.log_Dp = log_Dp #m2/s
-
-        return log_Dp
-
-
-    def _calculate_pipe_K_D(self,
-                            pipe,
-                            _conditions_set, ):
-        '''
-        Calculate the partitioning (Log Kpw) and diffusion (Log Dp) coefficients 
-        for the pipe segment(s), return as attributes of the segment.
-
-        See table 5-3 in KWR 2016.056 for explanation of calculations
-
-        Parameters
-        ----------
-        pipe: object
-            Pipe object of the segment.
-        _conditions_set: Boolean
-            Default False, True when the groundwater conditions have been set.
-        '''
-
-        # Check if the groundwater conditions have been set, if not raise error
-        if _conditions_set is None:
-            raise ValueError('Error, pipe conditions have not been set. To set pipe conditions use .set_conditions()')
-        else:           
-
-            # calculate log K plastic-water (log kpw) 
-            self.log_Kpw = self._calculate_logK(pipe = pipe)
-
-            # calculate log D plastic (log Dp) 
-            self.log_Dp = self._calculate_logD(pipe = pipe)
-            
-
-    def _calculate_stagnation_factor(self,):
-        ''' 
-        Calculates the stagnation factor given a pipe segment.
-        
-        Returns
-        -------
-        stagnation_factor: float
-            Correction for the decrease in the concentratino gradient near the 
-            inner wall of the pipe during stagnation (e.g. no flow at at night).
-
-        '''
-
-        stagnation_factor = 10 ** max((((self.log_Dp + 12.5) / 2 + 
-                                self.log_Kpw) * 0.73611 + 
-                                -1.03574 ), 0)
-        return stagnation_factor
-    
-
-    def _calculate_mean_dw_mass_per_segment(self, 
-                                            concentration_drinking_water,
-                                            concentration_groundwater,
-                                            pipe,): 
-        '''
-        Calculates the mean mass in drinking water for each pipe segment, for a 
-        24 hour period given a groundwater concentration. 
-        
-        Parameters
-        ----------
-        concentration_drinking_water: float
-            Concentration of given chemical in drinking water pipe, g/m3. 
-        concentration_groundwater: float
-            Concentration of the given chemical in groundwater, g/m3.
-        pipe: object
-            Pipe object of the segment.
-
-        '''
-         
-        # From equation 4-7 in KWR 2016.056, but not simplifying the mass flux 
-        # in equation 4-5 
-        delta_c = concentration_groundwater - concentration_drinking_water
-
-        self.mass_chemical_drinkwater = (((10 ** self.log_Dp * 10 ** self.log_Kpw)
-                                          * self.permeation_surface_area 
-                                          * delta_c / self.diffusion_path_length ) 
-                                            / pipe.ASSESSMENT_FACTOR_GROUNDWATER
-                                            * 24 * 60 * 60)
-        
-        if self.material == 'PVC':
-            self.mass_chemical_drinkwater = 0
-
-
-    def _calculate_peak_dw_mass_per_segment(self, 
-                                            concentration_drinking_water,
-                                            concentration_groundwater,
-                                            pipe,):
-        '''
-        Calculates the peak (maximum) mass in drinking water for a 
-        given a stagnation period given a groundwater concentration, for each pipe segment.
-        Stagnation period default of 8 hours. 
-        
-        Parameters
-        ----------
-        concentration_drinking_water: float
-            Concentration of given chemical in drinking water pipe, g/m3. 
-        concentration_groundwater: float
-            Concentration of the given chemical in groundwater, g/m3.
-        pipe: object
-            Pipe object of the segment.
-
-        '''
-
-        self.stagnation_factor = self._calculate_stagnation_factor()
-        delta_c = concentration_groundwater - concentration_drinking_water
-
-        # From equation 4-10 KWR 2016.056, but not simplifying the mass flux 
-        # in equation 4-5 and rearranging to remove C_dw from the equation       
-        self.mass_chemical_drinkwater = (((10 ** self.log_Dp * 10 ** self.log_Kpw)
-                                             * self.permeation_surface_area 
-                                             * delta_c / self.diffusion_path_length 
-                                             * pipe.stagnation_time ) 
-                                            / (pipe.ASSESSMENT_FACTOR_GROUNDWATER* self.stagnation_factor))
-        if self.material == 'PVC':
-            self.mass_chemical_drinkwater = 0
+#%% ----------------------------------------------------------attributes------------------
+# A. Hockin, January 2023
+# KWR 403230-003
+# Pipe permeation calculator
+# With Martin vd Schans, Bram Hillebrand, Lennart Brokx
+#
+# ------------------------------------------------------------------------------
+import numpy as np
+import pandas as pd
+
+from pipepermcalc.pipe import * 
+
+class Segment:
+    ''' 
+    Segment object class to make segments of the pipe.
+
+    Attributes
+    ----------
+
+    PARTITIONING_A_DH: float
+        Coefficient for correcting the partitioning coefficient for temperature. 
+        From regression analysis, a is the slope, see table 5-6 in 
+        KWR 2016.056. Constant equal to 7.92169801506708. 
+    PARTITIONING_B_DH: float,
+        Coefficient for correcting the partitioning coefficient for temperature. 
+        From regression analysis, b is the intercept, see table 5-6 in 
+        KWR 2016.056. Constant equal to -17.1875608983359. 
+    DIFFUSION_A_DH: float 
+        Coefficient for correcting the diffusion coefficient for temperature. 
+        From regression analysis, a is the slope, see table 5-6 in 
+        KWR 2016.056. Constant equal to 61.8565740136974. 
+    DIFFUSION_B_DH: float
+        Coefficient for correcting the diffusion coefficient for temperature. 
+        From regression analysis, b is the intercept, see table 5-6 in 
+        KWR 2016.056. Constant equal to -78.9191401984509. 
+    PARTITIONING_A_C: float
+        Constant used in the correction for the partitioning coefficent due to 
+        the influence of temperature. See equation 5-20 in KWR 2016.056, for 
+        partitioning a_c = 0.103965019849463.
+    PARTITIONING_CREF_SW: float
+        Reference concentration used in the correction for the partitioning 
+        coefficent due to the influence of temperature. Ssee section 5.4.7 in 
+        KWR 2016.056. For partitioning, Cref_SW = 1.0.
+    DIFFUSION_A_C: float
+        Constant used in the correction for the diffusion coefficent due to 
+        the influence of temperature. See equation 5-18 in KWR 2016.056, for 
+        diffusion a_c = 0.784077209735583.
+    DIFFUSION_CREF_SW: float
+        Reference concentration used in the correction for the diffusion 
+        coefficent due to the influence of temperature. Ssee section 5.4.6 in 
+        KWR 2016.056. For partitioning, Cref_SW = 0.5.
+    name: string
+        name of the pipe segment
+    material: string
+        Choice of pipe material: PE40, PE80, PVC, EPDM.
+    length: float
+        Length of the pipe segment in contact with the contaminated groundwater, meters. 
+    inner_diameter: float
+        Inner diameter of the pipe segment, meters
+    wall_thickness: float
+        wall_thickness of the pipe segment, meters
+    permeation_direction: string
+        Direction of permeation through the pipe segment. Options are 
+        'perpendicular' or 'parallel'. Default permeation is perpendicular 
+        to the flow direction. See schematic XX in read the docs. 
+    diffusion_path_length: float
+        In the case of permeation perpendicular to the flow direction, a 
+        diffusion path length is required to calculate the permeation through 
+        the pipe segment. For example in the case of a pipe coupling rings. 
+        Default permeation is perpendicular to the flow direction and the 
+        wall_thickness is used to calculate the diffusion through the pipe 
+        segment. Unit meters.
+    volume: float
+        Volume of the pipe segment, m3
+    permeation_surface_area: float
+        Surface area through which permeation takes place. If permeation is 
+        perpendicular to the flow, the permeation surface area is the inner 
+        surface area of the pipe. If diffusion is parallel to the flow, the 
+        permeation surface area is the annular area of the pipe segment. 
+    outer_diameter: float
+        Outer diameter of the pipe segment, unit m.
+    log_Kpw_ref: float
+        partitioning coefiicient under lab conditions, [-]
+    f_Ktemp: float
+        Temperature correction factor for partitioning coefficient, [-]
+    f_Kconc: float
+        Concentration correction factor for partitioning coefficient, [-]
+    log_Kpw: float
+        Calculated log partitioning coefficient for the given chemical and pipe material, [-]
+    log_Dp_ref: float
+        Diffusion coefficient under lab conditions, m2/s.
+    f_Dtemp:float
+        Temperature correction factor for diffusion coefficient, m2/s.
+    f_Dconc: float
+        Concentration correction factor for diffusion coefficient, [m2/s.
+    log_Dp: float
+        Calculated log diffusion coefficient for the given chemical and pipe material, m2/s.
+    stagnation_factor: float
+        Correction for the decrease in the concentration gradient near the 
+        inner wall of the pipe during stagnation (e.g. no flow at at night)
+    mass_chemical_drinkwater: float
+        Mass of the given chemical in the pipe segment, g.
+    
+    Note
+    ----
+    All parameters are in SI units: m, m2, g/m3 (equivalent to mg/L), seconds.
+
+
+    '''
+
+    def __init__(self, 
+                name=None,
+                material=None,
+                length=None,
+                inner_diameter=None,
+                wall_thickness=None,
+                permeation_direction='perpendicular',
+                diffusion_path_length=None,
+                ):
+        '''
+        Creates a pipe segment with the attributes of the pipe (length, 
+        wall_thickness, diameter, material etc.). 
+        
+        Parameters
+        ----------
+        name: string
+            name of the pipe segment
+        material: string
+            Choice of pipe material: PE40, PE80, PVC, EPDM.
+        length: float
+            Length of the pipe segment in contact with the contaminated groundwater, meters.         
+        inner_diameter: float
+            Inner diameter of pipe segment, meters
+        wall_thickness: float
+            wall_thickness of pipe segment, meters
+        permeation_direction: string
+            Direction of permeation through the pipe segment. Options are 
+            'perpendicular' or 'parallel'. Default permeation is perpendicular 
+            to the flow direction. See schematic XX in read the docs.
+        diffusion_path_length: float
+            In the case of permeation perpendicular to the flow direction, a 
+            diffusion path length is required to calculate the permeation through 
+            the pipe segment. For example in the case of a pipe coupling rings. 
+            Default permeation is perpendicular to the flow direction and the 
+            wall_thickness is used to calculate the diffusion through the pipe 
+            segment. Unit meters.
+        '''  
+
+        #Constants for various LogK and Log D equations
+        self._PARTITIONING_A_DH = 7.92169801506708 #see table 5-6 in KWR 2016.056
+        self._PARTITIONING_B_DH = -17.1875608983359 #see table 5-6 in KWR 2016.056
+        self._DIFFUSION_A_DH = 61.8565740136974 #see table 5-6 in KWR 2016.056
+        self._DIFFUSION_B_DH = -78.9191401984509 #see table 5-6 in KWR 2016.056
+        self.PARTITIONING_A_C = 0.103965019849463 #see equation 5-20 in KWR 2016.056
+        self.PARTITIONING_CREF_SW = 1.000 #see section 5.4.7 in KWR 2016.056
+        self.DIFFUSION_A_C = 0.784077209735583 #see equation 5-18 in KWR 2016.056
+        self.DIFFUSION_CREF_SW = 0.5 #see section 5.4.6 in KWR 2016.056
+
+        # check that segment values are defined (not None)
+        self.name = name
+
+        if material is None:
+            raise ValueError(f"material is not defined, choose one of 'PE40', 'PE80', 'SBR', 'EPDM', 'PVC'.")
+        else:
+            self.material = material
+
+        if length is None:
+            raise ValueError(f"length is not defined.")
+        else:
+            self.length = float(length)
+
+        if inner_diameter is None:
+            raise ValueError(f"inner_diameter is not defined.")
+        else:
+            self.inner_diameter = float(inner_diameter)
+
+        if wall_thickness is None:
+            raise ValueError(f"wall_thickness is not defined.")
+        else:
+            self.wall_thickness = float(wall_thickness)
+
+        self.permeation_direction = permeation_direction
+
+        if diffusion_path_length is None:
+            self.diffusion_path_length = self.wall_thickness
+        else:
+            self.diffusion_path_length = float(diffusion_path_length)    
+
+        outer_diameter = inner_diameter + wall_thickness
+        volume = np.pi * (inner_diameter / 2) ** 2 * length
+        permeation_surface_area =(np.pi * inner_diameter * length)
+
+        if permeation_direction == 'parallel':
+            volume = 0 
+            permeation_surface_area = ((np.pi * ((inner_diameter + wall_thickness) ** 2 
+                                                - inner_diameter ** 2) ) / 4)
+                   
+        self.volume = volume
+        self.permeation_surface_area = permeation_surface_area
+        self.outer_diameter = outer_diameter
+        self.inner_diameter = inner_diameter
+
+    # @MartinK-> suggest to implement the "named tuple" method, leave for now do at the end
+    # #ah_todo SBR, EPDM refer to memo, ask m. meerkerk for memo number, include 
+    # project number for the memo
+
+    # reference_pipe_material_dict: dictionary 
+    #     Reference dictionary with regression values (slope=a-value, intercept=b-value)
+    #     for the partitioning (K) and diffusion (D) coefficient for the available 
+    #     plastics (PE40, PE80, SBR, EPDM) per chemical groups. 
+    #     Used to calculate the specifice partitioning or diffusion coefficient 
+    #     from the reference value. 
+    #     Chemical group numbers: Expert opinion (M. Meerkerk)
+    #     see table 5-4 KWR 2016.056, Group 1: PAH, MAH, ClArom, ClAlk, Arom, Alk
+    #     Group 2: PCB, Group 3: other, unknown, O2, Cl, BDE
+    reference_pipe_material_dict = \
+        {
+        "PE40": {
+            "REF_LOG_D_A": {
+                1: -0.011,	
+                2: -0.00629,
+                3: -0.006,
+                },
+            "REF_LOG_D_B": {
+                1: -10.688,
+                2: -11.000,
+                3: -11.000
+                },
+            "REF_LOG_K_A": {
+                1: 1.097,
+                2: 1.059,
+                3: 0.979
+                },
+            "REF_LOG_K_B": {
+                1: -0.689,
+                2: -0.67,
+                3: -1.796,
+                },
+        },
+        "PE80": {
+            "REF_LOG_D_A": {
+                1: -0.011,	
+                2: -0.00629,
+                3: -0.00629,
+                },
+            "REF_LOG_D_B": {
+                1: -11.188,
+                2: -11.188,
+                3: -11.500,
+                },
+            "REF_LOG_K_A": {
+                1: 1.185,	
+                2: 1.185,
+                3: 1.231,
+                },
+            "REF_LOG_K_B": {
+                1: -1.437,	
+                2: -1.437,
+                3: -2.606,
+                },
+        },
+        "SBR": {
+            "REF_LOG_D_A": {
+                1: -0.011 * 0.950647410867427,	
+                2: -0.00629 * 0.950647410867427,
+                3: -0.006 * 0.950647410867427,
+                },
+            "REF_LOG_D_B": {
+                1: -10.688 * 0.950647410867427,
+                2: -11.000 * 0.950647410867427,
+                3: -11.000 * 0.950647410867427,
+                },
+            "REF_LOG_K_A": {
+                1: 1.0452,	
+                2: 1.0452,
+                3: 1.0452,
+                },
+            "REF_LOG_K_B": {
+                1: -0.3686,	
+                2: -0.3686,
+                3: -0.3686,
+                },
+        },  
+        "EPDM": {
+            "REF_LOG_D_A": {
+                1: -0.011* 0.920996123470591,	
+                2: -0.00629 * 0.920996123470591,
+                3: -0.006 * 0.920996123470591,
+                },
+            "REF_LOG_D_B": {
+                1: -10.688 * 0.920996123470591,
+                2: -11.000 * 0.920996123470591,
+                3: -11.000 * 0.920996123470591,
+                },
+            "REF_LOG_K_A": {
+                1: 1.0675,	
+                2: 1.0675,
+                3: 1.0675,
+                },
+            "REF_LOG_K_B": {
+                1: -0.3002,	
+                2: -0.3002,
+                3: -0.3002,
+                },
+        },  
+        "PVC": { #Diffusion through PVC is zero
+            "REF_LOG_D_A": {
+                1: 0,	
+                2: 0,
+                3: 0,
+                },
+            "REF_LOG_D_B": {
+                1: 0,	
+                2: 0,
+                3: 0,
+                },
+            "REF_LOG_K_A": {
+                1: 0,	
+                2: 0,
+                3: 0,
+                },
+            "REF_LOG_K_B": {
+                1: 0,	
+                2: 0,
+                3: 0,
+                },
+        },               
+        }
+
+    def _correct_for_temperature(self,
+                                temperature_groundwater,
+                                coefficient_name=None, 
+                                a_dh=None,
+                                b_dh=None,
+                                ):
+        '''
+        Temperature correction for the partitioning and diffusion coefficients. 
+        See table 5-3 in KWR 2016.056
+
+        Parameters
+        ----------
+        temperature_groundwater: float
+            Temperature of the groundwater, degrees Celcius
+        coefficient_name: string
+            Either 'solubility' or 'molecular_weight'
+        a_dh: string
+            Coefficient for correcting the partitioning or diffusion coefficient
+        b_dh: string
+            Coefficient for correcting the partitioning or diffusion coefficient
+
+        Returns
+        -------
+        f_temp: string
+            Temperature correction factor for the partitioning or diffusion 
+            coefficient.
+        '''
+
+        R = 0.008314 #universal gas constant [J/k/mol]
+        reference_temperature = 25 # deg. C
+        dh = a_dh * np.log10(coefficient_name) + b_dh
+        f_temp = dh / (R * np.log(10)) * (1 / (reference_temperature + 273) - 1 / (temperature_groundwater + 273))
+        return f_temp, dh
+
+
+    def _concentration_correction(self,
+                        solubility, 
+                        concentration_groundwater,
+                        a_c=None,
+                        Cref_Sw=None):
+        '''
+        Correction factor for the influence of concentration on the 
+        partitioning or diffusion coefficient. 
+        See table 5-3, equations 5-17 and 5-19 in KWR 2016.056
+
+        Parameters
+        ----------
+        solubility:	float
+            solubility of given chemical in water, g/m3
+        concentration_groundwater: float
+            Concentration of the given chemical in groundwater, g/m3.
+        a_c: float
+            Constant used in the correction for the partitioning or diffusion 
+            coefficent due to the influence of temperature. See equations 5-18 
+            and 5-20 in KWR 2016.056. 
+        Cref_Sw: float
+            Reference concentration used in the correction for the diffusion or 
+            partitioning coefficent due to the influence of temperature. See 
+            sections 5.4.6 and 5.4.7 in KWR 2016.056. 
+            
+        Returns
+        -------
+        f_conc: string
+            Concentration correction factor for the diffusion or partitioning
+            coefficient.
+        '''
+
+        Cg_Sw = min(concentration_groundwater / solubility, 1)
+        f_conc = a_c * (Cg_Sw - Cref_Sw)
+
+        return f_conc
+
+
+    def _correct_for_age(self,):
+        '''
+        Age correction, none implemented yet
+        
+        Returns
+        -------
+        f_age: float
+            Age correction for the partitioning or diffusion coefficient.
+        '''
+
+        f_age = 0.000
+        return f_age
+
+
+    def _calculate_ref_logK(self,
+                            chemical_group_number,
+                            log_octanol_water_partitioning_coefficient):
+        '''Calculate the reference partitioning coefficient for the pipe segment.
+        See tabel 5.3, equations 5-5, 5-6 in KWR 2016.056.  
+
+        Parameters
+        ----------
+        chemical_group_number: integer
+            Integer corresponding to the chemical group.
+        log_octanol_water_partitioning_coefficient:	float,
+            Partition coefficient for the two-phase system consisting of 
+            n-octanol and water, Log Kow, [-].
+
+        Returns
+        -------
+        log_Kpw_ref: float
+            partitioning coefiicient under lab conditions, [-].
+
+        '''
+
+        a_ref = self.reference_pipe_material_dict[self.material]['REF_LOG_K_A'][chemical_group_number]
+        b_ref = self.reference_pipe_material_dict[self.material]['REF_LOG_K_B'][chemical_group_number]
+        log_Kpw_ref = a_ref * log_octanol_water_partitioning_coefficient + b_ref
+
+        return log_Kpw_ref
+
+
+    def _calculate_ref_logD(self,
+                            chemical_group_number,
+                            molecular_weight):
+        '''
+        Calculate the reference diffusion (log D) based on the pipe material. A fixed 
+        ratio between the log of the diffusion coefficient of PE-40 (logD_p) 
+        and of SBR/EPDM (logD_s, logD_e) in m2/s is assumed for SBR and 
+        EPDM for the determination of the diffusion coefficient, see memo 2022 
+        "Permeatie door rubber afdichtingen van drinkwaterleidingen."  
+        #ah_todo find memo number
+
+        Parameters
+        ----------
+        chemical_group_number: integer
+            Integer corresponding to the chemical group.
+        molecular_weight: float
+            Mass of one mole of a given chemical, g/mol.
+
+        Returns
+        -------
+        log_Dp_ref: float
+            Diffusion coefficient under lab conditions, m2/s.
+        '''
+
+        if np.isnan(molecular_weight):
+            raise ValueError('Error, the molecular weight for this chemical is not known, therefore it is not possible to calculate the permeation.')
+
+
+        a_ref = self.reference_pipe_material_dict[self.material]['REF_LOG_D_A'][chemical_group_number]
+        b_ref = self.reference_pipe_material_dict[self.material]['REF_LOG_D_B'][chemical_group_number]
+        log_Dp_ref = a_ref * molecular_weight + b_ref
+
+        return log_Dp_ref    
+
+
+    def _calculate_logK(self, 
+                        pipe):
+        ''' 
+        Calculate the partitioning coefficient (Log K) value for the pipe material, 
+        corrected for temperature,concentration and age. 
+        
+        See table 5-3 in KWR 2016.056 for explanation of calculations. 
+
+        Parameters
+        ----------
+        pipe: object
+            Pipe object of the segment.
+
+        Returns
+        -------
+        log_Kpw: float
+            Calculated log partitioning coefficient for the given chemical and 
+            pipe material, [-]
+        '''
+
+        # calculate reference log K plastic-water (log kpw) 
+        log_Kpw_ref = self._calculate_ref_logK(chemical_group_number=pipe.chemical_group_number,
+                                               log_octanol_water_partitioning_coefficient= pipe.log_octanol_water_partitioning_coefficient)
+
+        # correct for temperature, concentration, age
+        f_Ktemp, K_dh = self._correct_for_temperature(coefficient_name = pipe.solubility,
+                            temperature_groundwater = pipe.temperature_groundwater, 
+                            a_dh = self._PARTITIONING_A_DH, 
+                            b_dh = self._PARTITIONING_B_DH, )
+
+        f_Kconc = self._concentration_correction(solubility=pipe.solubility, 
+                                concentration_groundwater = pipe.concentration_groundwater,
+                                a_c = self.PARTITIONING_A_C,
+                                Cref_Sw = self.PARTITIONING_CREF_SW) 
+        
+        f_Kage = self._correct_for_age()
+
+        # No diffusion though PVC, assign values to zero
+        if self.material == 'PVC':
+            f_Ktemp = 0
+            f_Kconc = 0
+            f_Kage = 0
+            log_Kpw_ref = 0
+
+        # sum corrections for final Log k
+        log_Kpw = log_Kpw_ref + f_Ktemp + f_Kconc + f_Kage
+        
+        self.log_Kpw_ref = log_Kpw_ref
+        self.f_Ktemp = f_Ktemp   
+        self.f_Kconc = f_Kconc
+        self.partitioning_enthalpie = K_dh
+        self.log_Kpw = log_Kpw
+
+        return log_Kpw
+
+
+    def _calculate_logD(self, 
+                        pipe):
+        ''' 
+        Calculate the LogK value for the pipe material, correct for temperature,
+        concentration and age. 
+
+        See table 5-3 in KWR 2016.056 for explanation of calculations
+
+        Parameters
+        ----------
+        pipe: object
+            Pipe object of the segment.
+
+        Returns
+        -------
+        log_Dp: float
+            Calculated log diffusion coefficient for the given chemical and pipe 
+            material, m2/s.
+        '''
+        
+        # calculate reference log D plastic (log Dp) 
+        log_Dp_ref = self._calculate_ref_logD(chemical_group_number=pipe.chemical_group_number,
+                            molecular_weight=pipe.molecular_weight)
+
+        # correct for temperature, concentration, age
+        f_Dtemp, D_dh = self._correct_for_temperature(coefficient_name =pipe.molecular_weight,
+                            temperature_groundwater = pipe.temperature_groundwater, 
+                            a_dh = self._DIFFUSION_A_DH, 
+                            b_dh = self._DIFFUSION_B_DH,)
+
+        f_Dconc = self._concentration_correction(
+                                solubility=pipe.solubility, 
+                                concentration_groundwater = pipe.concentration_groundwater,
+                                a_c = self.DIFFUSION_A_C , 
+                                Cref_Sw = self.DIFFUSION_CREF_SW) 
+        
+        f_Dage = self._correct_for_age()
+
+        # No diffusion though PVC, assign values to zero
+        if self.material == 'PVC':
+            f_Dtemp = 0
+            f_Dconc = 0
+            f_Dage = 0
+            log_Dp_ref = 0
+
+        # sum corrections for final Log D
+        log_Dp = log_Dp_ref + f_Dtemp + f_Dconc + f_Dage
+
+        self.log_Dp_ref = log_Dp_ref
+        self.f_Dtemp = f_Dtemp  
+        self.activattion_energy = D_dh
+        self.f_Dconc = f_Dconc
+        self.log_Dp = log_Dp #m2/s
+
+        return log_Dp
+
+
+    def _calculate_pipe_K_D(self,
+                            pipe,
+                            _conditions_set, ):
+        '''
+        Calculate the partitioning (Log Kpw) and diffusion (Log Dp) coefficients 
+        for the pipe segment(s), return as attributes of the segment.
+
+        See table 5-3 in KWR 2016.056 for explanation of calculations
+
+        Parameters
+        ----------
+        pipe: object
+            Pipe object of the segment.
+        _conditions_set: Boolean
+            Default False, True when the groundwater conditions have been set.
+        '''
+
+        # Check if the groundwater conditions have been set, if not raise error
+        if _conditions_set is None:
+            raise ValueError('Error, pipe conditions have not been set. To set pipe conditions use .set_conditions()')
+        else:           
+
+            # calculate log K plastic-water (log kpw) 
+            self.log_Kpw = self._calculate_logK(pipe = pipe)
+
+            # calculate log D plastic (log Dp) 
+            self.log_Dp = self._calculate_logD(pipe = pipe)
+            
+
+    def _calculate_stagnation_factor(self,):
+        ''' 
+        Calculates the stagnation factor given a pipe segment.
+        
+        Returns
+        -------
+        stagnation_factor: float
+            Correction for the decrease in the concentration gradient near the 
+            inner wall of the pipe during stagnation (e.g. no flow at at night).
+
+        '''
+
+        stagnation_factor = 10 ** max((((self.log_Dp + 12.5) / 2 + 
+                                self.log_Kpw) * 0.73611 + 
+                                -1.03574 ), 0)
+        
+        return stagnation_factor
+    
+
+    def _calculate_mean_dw_mass_per_segment(self, 
+                                            concentration_drinking_water,
+                                            concentration_groundwater,
+                                            pipe,): 
+        '''
+        Calculates the mean mass in drinking water for each pipe segment, for a 
+        24 hour period given a groundwater concentration. 
+        
+        Parameters
+        ----------
+        concentration_drinking_water: float
+            Concentration of given chemical in drinking water pipe, g/m3. 
+        concentration_groundwater: float
+            Concentration of the given chemical in groundwater, g/m3.
+        pipe: object
+            Pipe object of the segment.
+
+        '''
+         
+        # From equation 4-7 in KWR 2016.056, but not simplifying the mass flux 
+        # in equation 4-5 
+        delta_c = concentration_groundwater - concentration_drinking_water
+
+        self.mass_chemical_drinkwater = (((10 ** self.log_Dp * 10 ** self.log_Kpw)
+                                          * self.permeation_surface_area 
+                                          * delta_c / self.diffusion_path_length ) 
+                                            / pipe.ASSESSMENT_FACTOR_GROUNDWATER
+                                            * 24 * 60 * 60)
+        
+        if self.material == 'PVC':
+            self.mass_chemical_drinkwater = 0
+
+
+    def _calculate_peak_dw_mass_per_segment(self, 
+                                            concentration_drinking_water,
+                                            concentration_groundwater,
+                                            pipe,):
+        '''
+        Calculates the peak (maximum) mass in drinking water for a 
+        given a stagnation period given a groundwater concentration, for each pipe segment.
+        Stagnation period default of 8 hours. 
+        
+        Parameters
+        ----------
+        concentration_drinking_water: float
+            Concentration of given chemical in drinking water pipe, g/m3. 
+        concentration_groundwater: float
+            Concentration of the given chemical in groundwater, g/m3.
+        pipe: object
+            Pipe object of the segment.
+
+        '''
+
+        self.stagnation_factor = self._calculate_stagnation_factor()
+        delta_c = concentration_groundwater - concentration_drinking_water
+
+        # From equation 4-10 KWR 2016.056, but not simplifying the mass flux 
+        # in equation 4-5 and rearranging to remove C_dw from the equation       
+        self.mass_chemical_drinkwater = (((10 ** self.log_Dp * 10 ** self.log_Kpw)
+                                             * self.permeation_surface_area 
+                                             * delta_c / self.diffusion_path_length 
+                                             * pipe.stagnation_time ) 
+                                            / (pipe.ASSESSMENT_FACTOR_GROUNDWATER* self.stagnation_factor))
+        if self.material == 'PVC':
+            self.mass_chemical_drinkwater = 0
```

### Comparing `pipepermcalc-0.0.5/setup.py` & `pipepermcalc-0.8.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-import os
-from setuptools import setup, find_packages
-
-def read(fname):
-    with open(os.path.join(os.path.dirname(__file__), fname)) as f:
-        return f.read()
-
-package_name = 'pipepermcalc'
-setup(
-    name=package_name,
-    version='0.0.5',
-    packages=find_packages(exclude=['tests*', 'tests.*', 'research*',]),
-    license='All rights reserved',
-    description='A python package to ',
-    long_description=read('README.rst'),
-    long_description_content_type="text/x-rst",
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
-    ],
-    python_requires='>=3.7',
-    project_urls={
-    'Source': f'https://github.com/KWR-Water/{package_name}',
-    'Documentation': f'http://{package_name}.readthedocs.io/en/latest/',
-    'Tracker': f'https://github.com/KWR-Water/{package_name}/issues',
-    'Help': f'https://github.com/KWR-Water/{package_name}/issues',
-    },
-    install_requires=[
-        'pandas',
-        'openpyxl',
-        'pytest',
-        'fuzzywuzzy',
-        ],
-    url=f'https://github.com/KWR-Water/{package_name}',
-    author='KWR Water Research Institute',
-    author_email='alex.hockin@kwrwater.nl, bram.hillebrand@kwrwater.nl',
-    package_data={'': ['database/*.csv']},
-)
+import os
+from setuptools import setup, find_packages
+
+def read(fname):
+    with open(os.path.join(os.path.dirname(__file__), fname)) as f:
+        return f.read()
+
+package_name = 'pipepermcalc'
+setup(
+    name=package_name,
+    version='0.8.6',
+    packages=find_packages(exclude=['tests*', 'tests.*', 'research*',]),
+    license='All rights reserved',
+    description='A python package to ',
+    long_description=read('README.rst'),
+    long_description_content_type="text/x-rst",
+    
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.7',
+    ],
+    python_requires='>=3.7',
+    project_urls={
+    'Source': f'https://github.com/KWR-Water/{package_name}',
+    'Documentation': f'http://{package_name}.readthedocs.io/en/latest/',
+    'Tracker': f'https://github.com/KWR-Water/{package_name}/issues',
+    'Help': f'https://github.com/KWR-Water/{package_name}/issues',
+    },
+    install_requires=[
+        'pandas',
+        'openpyxl',
+        'pytest',
+        'fuzzywuzzy',
+        ],
+    url=f'https://github.com/KWR-Water/{package_name}',
+    author='KWR Water Research Institute',
+    author_email='alex.hockin@kwrwater.nl, bram.hillebrand@kwrwater.nl',
+    package_data={'': ['database/*.csv']},
+)
```

### Comparing `pipepermcalc-0.0.5/tests/test_pipepermcalc.py` & `pipepermcalc-0.8.6/tests/test_pipepermcalc.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,702 +1,702 @@
-#%% ----------------------------------------------------------------------------
-# A. Hockin, January 2023
-# KWR 403230-003
-# Pipe permeation calculator
-# With Martin vd Schans, Bram
-#
-# ------------------------------------------------------------------------------
-
-#%% ----------------------------------------------------------------------------
-# INITIALISATION OF PYTHON e.g. packages, etc.
-# ------------------------------------------------------------------------------
-
-# Plotting modules
-import matplotlib.pyplot as plt
-import matplotlib
-import matplotlib.colors as colors
-
-import numpy as np
-import pandas as pd
-import os
-import sys
-from pandas import read_csv
-from pandas import read_excel
-import math
-import datetime
-from datetime import timedelta
-
-from pathlib import Path
-
-from pipepermcalc.pipe import * 
-from pipepermcalc.segment import * 
-
-#%%
-
-def raise_exception_two_values(answer, ref_answer, round_values=None):
-    ''' Raise exception if two values are not equal.'''
-    if round_values is None:
-        assert answer == ref_answer
-    else:
-        answer_round = round(answer, round_values)
-        ref_answer = round(ref_answer, round_values)
-        assert answer_round == ref_answer
-
-
-def test_logKpw_ref():
-    '''test the calculatiion of the reference logK value against the excel'''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 0.112980124482, 
-                                    flow_rate=0.5)
-    raise_exception_two_values(answer=seg1.log_Kpw_ref, 
-                               ref_answer = 1.64761000, 
-                               round_values=5)
-
-def test_logDp_ref():
-    '''test the calculatiion of the reference logD value against the excel'''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 0.112980124482, 
-                                    flow_rate=0.5)
-  
-    raise_exception_two_values(answer=seg1.log_Dp_ref, 
-                               ref_answer = -11.54717, 
-                               round_values=5)
-
-def test_logKp_ref_temperature_correction():
-    '''test the calculatiion of the reference logK value, corrected for temperature
-      against the excel'''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 0.112980124482, 
-                                    flow_rate=0.5)
-    raise_exception_two_values(answer=seg1.f_Ktemp, 
-                               ref_answer = -0.071506, 
-                               round_values=6)
-
-
-def test_logDp_ref_temperature_correction():
-    '''test the calculatiion of the reference logD value, corrected for temperature
-      against the excel'''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 0.112980124482, 
-                                    flow_rate=0.5)
-    raise_exception_two_values(answer=seg1.f_Dtemp, 
-                               ref_answer = -0.305084,
-                               round_values=6)
-    
-
-def test_logKp_ref_concentration_correction():
-    '''test the calculation of the reference logK value, 
-    corrected for concentration against the excel'''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 1.8,
-                                    flow_rate=0.5)
-    
-    raise_exception_two_values(answer=seg1.f_Kconc,
-                               ref_answer = -0.103871,
-                               round_values=6)
-    
-
-def test_logDp_ref_concentration_correction():
-    '''test the calculatiion of the reference logD value, 
-    corrected for concentration '''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater =1.8,
-                                    flow_rate=0.5)
-    raise_exception_two_values(answer=seg1.f_Dconc,
-                               ref_answer =  -0.391329, 
-                               round_values=6)
-    
-
-def test_logKpw():
-    '''test the calculatiion of the logKpw'''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 1.8,
-                                    flow_rate=0.5)
-    raise_exception_two_values(answer=seg1.log_Kpw,
-                               ref_answer = 1.472233,
-                               round_values=6)
-    
-
-def test_logDpw():
-    '''test the calculatiion of the logDw'''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 1.8,
-                                    flow_rate=0.5)
-    raise_exception_two_values(answer=seg1.log_Dp, 
-                               ref_answer = -12.243587, 
-                               round_values=6)
-    
-
-def test_stagnation_factor():
-    '''test the calculatiion of the stagnation factor'''
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 1.8,
-                                    flow_rate=0.5)
-    
-    pipe1.validate_input_parameters()
-    pipe1.calculate_peak_dw_concentration()    
-
-    raise_exception_two_values(answer=seg1.stagnation_factor,
-                               ref_answer =  1.387905, 
-                               round_values=6)
-
-def test_updating_partitioning_coefficient():
-    ''' Test the update function for the partitioning coefficient '''
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 1.8,
-                                    flow_rate=0.5)
-    pipe1.validate_input_parameters()
-    seg1.log_Kpw= 0.9116730996845103
-
-    pipe1.calculate_peak_dw_concentration()    
-
-    raise_exception_two_values(answer=seg1.log_Kpw,
-                               ref_answer = 0.911673, 
-                               round_values=6)
-
-
-def test_updating_diffusion_coefficient():
-    ''' Test the update function for the diffusion coefficient '''
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 1.8,
-                                    flow_rate=0.5)
-    pipe1.validate_input_parameters()
-    seg1.log_Dp= -12.743586769549616
-    
-    pipe1.calculate_peak_dw_concentration()    
-   
-    raise_exception_two_values(answer=seg1.log_Dp, 
-                               ref_answer = -12.743586769549616, 
-                               round_values=None)
-
-
-
-def test_calculate_peak_dw_concentration():
-    ''' Test the calculation for the peak concentration in drinking water given 
-    a groundwater concentration '''
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 0.112980124482,
-                                    flow_rate=0.5)
-    pipe1.validate_input_parameters()
-    
-    pipe1.calculate_peak_dw_concentration()    
-
-    raise_exception_two_values(answer=pipe1.concentration_drinking_water, 
-                               ref_answer = 0.001, 
-                               round_values=3)
-    
-def test_calculate_peak_dw_mass():
-    ''' Test the calculation for the peak concentration in drinking water given 
-    a groundwater concentration '''
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 0.112980124482,
-                                    flow_rate=0.5)
-    pipe1.validate_input_parameters()
-    
-    pipe1.calculate_peak_dw_concentration()    
-
-    raise_exception_two_values(answer=seg1.mass_chemical_drinkwater, 
-                               ref_answer = 7.469113135415852e-06, 
-                               round_values=9)    
-
-def test_calculate_mean_dw_concentration():
-    ''' Test the calculation for the mean concentration in drinking water given 
-    a groundwater concentration '''
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 1.8,
-                                    flow_rate=0.5)
-    pipe1.validate_input_parameters()
-    
-    pipe1.calculate_mean_dw_concentration()    
-
-    raise_exception_two_values(answer=pipe1.concentration_drinking_water, 
-                               ref_answer = 0.001, 
-                               round_values=5)
-
-def test_calculate_mean_dw_mass():
-    ''' Test the calculation for the mean concentration in drinking water given 
-    a groundwater concentration '''
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=25,
-                    inner_diameter=0.0196,
-                    wall_thickness=0.0027,
-                    )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-
-    pipe1.set_conditions(chemical_name="Benzeen", 
-                                    temperature_groundwater=12, 
-                                    concentration_groundwater = 1.8,
-                                    flow_rate=0.5)
-    pipe1.validate_input_parameters()
-    
-    pipe1.calculate_mean_dw_concentration()    
-
-    raise_exception_two_values(answer=seg1.mass_chemical_drinkwater, 
-                               ref_answer = 0.0005000956341327644, 
-                               round_values=5)    
-
-def test_segment_surface_area_calculations():
-    ''' Test the calculation for the different surface area options '''
-    seg1 = Segment(name='seg1',
-                material='PE40',
-                length=7.5/1000,
-                inner_diameter=30.3/1000,
-                wall_thickness=1.5/1000,
-                permeation_direction='parallel',
-                diffusion_path_length=7.5/1000,
-                    )
-
-   
-    raise_exception_two_values(answer=seg1.permeation_surface_area, 
-                               ref_answer = 0.000073159839, 
-                               round_values=12)
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=1/1000,
-                    inner_diameter=28.5/1000,
-                    wall_thickness=10/1000,
-                    permeation_direction='perpendicular',
-                    diffusion_path_length=10/1000
-                    )
-
-    
-    raise_exception_two_values(answer=seg1.permeation_surface_area, 
-                               ref_answer = 0.000089535391, 
-                               round_values=12)
-
-    seg1 = Segment(name='seg1',
-                    material='PE40',
-                    length=33.3/1000,
-                    inner_diameter=25/1000,
-                    wall_thickness=2.7/1000,
-                    permeation_direction='perpendicular',)
-    
-    raise_exception_two_values(answer=seg1.permeation_surface_area, 
-                               ref_answer = 0.002615375884, 
-                               round_values=12)
-
-
-def test_return_matching_chemical_name():
-    seg1 = Segment(name='seg1',
-                material='PE40',
-                length=25,
-                inner_diameter=0.0196,
-                wall_thickness=0.0027,
-                )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.segment_list
-    chemical_name = 'Benzeen'
-    matching_name = pipe1._extract_matching_chemical_name(chemical_name=chemical_name, 
-                                          database=list(pipe1.ppc_database['chemical_name_NL']))
-    assert chemical_name == matching_name
-
-
-def test_calculate_mean_allowable_gw_concentration():
-    ''' Test the calculation for the mean concentration allowed in groundwater given 
-    a drinking water concentration '''
-    
-    seg1 = Segment(name='seg1',
-                material= 'PE40',
-                length=25,
-                inner_diameter=0.0196,
-                wall_thickness=0.0027,
-                )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.set_conditions(
-        chemical_name="Benzeen", 
-        temperature_groundwater=12, 
-        concentration_drinking_water=0.001,
-        flow_rate=0.5 )
-
-    pipe1.validate_input_parameters()
-
-    mean_conc = pipe1.calculate_mean_allowable_gw_concentration(tolerance = 0.001)
-
-    raise_exception_two_values(answer=mean_conc, 
-                               ref_answer = 1.8011, 
-                               round_values=4)
-
-def test_calculate_peak_allowable_gw_concentration():
-    ''' Test the calculation for the peak concentration allowed in groundwater given 
-    a drinking water concentration '''
-    seg1 = Segment(name='seg1',
-                material= 'PE40',
-                length=25,
-                inner_diameter=0.0196,
-                wall_thickness=0.0027,
-                )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    pipe1.set_conditions(
-        chemical_name="Benzeen", 
-        temperature_groundwater=12, 
-        concentration_drinking_water=0.001,
-        flow_rate=0.5 )
-
-    pipe1.validate_input_parameters()
-
-    peak_conc = pipe1.calculate_peak_allowable_gw_concentration(tolerance = 0.01)
-
-    raise_exception_two_values(answer=peak_conc, 
-                               ref_answer = 0.1138, 
-                               round_values=4)
-
-def test_groundwater_to_soil_conversion():
-    seg1 = Segment(name='seg1',
-                material= 'PE40',
-                length=25,
-                inner_diameter=0.0196,
-                wall_thickness=0.0027,
-                )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(
-        chemical_name="Benzeen", 
-        temperature_groundwater=12, 
-        concentration_groundwater=1.8,
-        flow_rate=0.5 )
-
-    pipe1.validate_input_parameters()
-
-    pipe1.calculate_mean_dw_concentration()
-
-    raise_exception_two_values(answer=pipe1.concentration_soil, 
-                               ref_answer =2.74, 
-                               round_values=3)
-    # Check that pipe summation is going correctly
-    seg1 = Segment(name='seg1',
-                material= 'PE40',
-                length=25,
-                inner_diameter=0.0196,
-                wall_thickness=0.0027,
-                )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(
-        chemical_name="ethylbenzene", 
-        temperature_groundwater=12, 
-        concentration_groundwater=0.277,
-        flow_rate=0.5 )
-
-    pipe1.validate_input_parameters()
-
-    pipe1.calculate_mean_dw_concentration()
-
-    raise_exception_two_values(answer=pipe1.concentration_soil, 
-                               ref_answer =1.842, 
-                               round_values=3)
-
-def test_soil_to_groundwater_conversion():
-    seg1 = Segment(name='seg1',
-                material= 'PE40',
-                length=25,
-                inner_diameter=0.0196,
-                wall_thickness=0.0027,
-                )
-
-    pipe1 = Pipe(segment_list=[seg1])
-
-    pipe1.set_conditions(
-        chemical_name="Benzeen",
-        temperature_groundwater=12, 
-        concentration_soil=2.7527429729399238,
-        flow_rate=0.5 )
-
-    pipe1.validate_input_parameters()
-
-    pipe1.calculate_mean_dw_concentration()
-
-    raise_exception_two_values(answer=pipe1.concentration_groundwater, 
-                               ref_answer = 1.8085521338873323, 
-                               round_values=5)
-
-def test_GW_to_DW_to_GW_peak():
-    '''Tests if the calculation from GW to DW gives the same result as DW to GW 
-    for the peak concentrations'''
-
-    seg1 = Segment(name='seg1',
-                material= 'PE40',
-                length=25,
-                inner_diameter=0.0196,
-                wall_thickness=0.0027,
-                )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    input_gw = 1
-
-    database = pipe1.view_database_chemical_names( language='NL')
-    database = pipe1.ppc_database.dropna(subset=['molecular_weight', 'solubility', 'Drinking_water_norm'])
-    database = database.loc[database['log_distribution_coefficient']>=0]
-    database = database.loc[database['Drinking_water_norm'] < database['solubility'] ]
-    database_chemicals = database['chemical_name_NL']
-    solubilities = database['solubility']
-
-    failed = []
-
-    for chemical_name, solubiliy in zip(database_chemicals, solubilities):
-        if input_gw > solubiliy:
-            input_gw = 0.01 * solubiliy
-
-        pipe1.set_conditions(
-            chemical_name=chemical_name, 
-                            concentration_groundwater =input_gw,
-                            temperature_groundwater=12, 
-                            flow_rate=0.5)
-
-        pipe1.validate_input_parameters()
-
-        peak_conc=pipe1.calculate_peak_dw_concentration()
-
-        pipe1.set_conditions(chemical_name=chemical_name, 
-                            temperature_groundwater=12, 
-                            concentration_drinking_water = peak_conc,
-                            flow_rate=0.5)
-
-        output_gw = pipe1.calculate_peak_allowable_gw_concentration()
-
-        if abs(1-(input_gw/output_gw)) < 0.02:
-            pass
-        else: 
-            failed.append(chemical_name)
-    
-    assert len(failed) == 0
-
-
-def test_GW_to_DW_to_GW_mean():
-    '''Tests if the calculation from GW to DW gives the same result as DW to GW 
-    for the mean concentrations'''
-
-    seg1 = Segment(name='seg1',
-                material= 'PE40',
-                length=25,
-                inner_diameter=0.0196,
-                wall_thickness=0.0027,
-                )
-
-    pipe1 = Pipe(segment_list=[seg1])
-    input_gw = 1
-
-    database = pipe1.view_database_chemical_names( language='NL')
-    database = pipe1.ppc_database.dropna(subset=['molecular_weight', 'solubility', 'Drinking_water_norm'])
-    database = database.loc[database['log_distribution_coefficient']>=0]
-    database = database.loc[database['Drinking_water_norm'] < database['solubility'] ]
-    database_chemicals = database['chemical_name_NL']
-    solubilities = database['solubility']
-
-    failed = []
-
-    for chemical_name, solubiliy in zip(database_chemicals, solubilities):
-        if input_gw > solubiliy:
-            input_gw = 0.01 * solubiliy
-
-        pipe1.set_conditions(
-            chemical_name=chemical_name, 
-                            concentration_groundwater =input_gw,
-                            temperature_groundwater=12, 
-                            flow_rate=0.5)
-
-        pipe1.validate_input_parameters()
-
-        mean_conc=pipe1.calculate_mean_dw_concentration()
-
-        pipe1.set_conditions(chemical_name=chemical_name, 
-                            temperature_groundwater=12, 
-                            concentration_drinking_water = mean_conc,
-                            flow_rate=0.5)
-
-        output_gw = pipe1.calculate_mean_allowable_gw_concentration()
-
-        if abs(1-(input_gw/output_gw)) < 0.02:
-            pass
-        else: 
-            failed.append(chemical_name)
-    
-    assert len(failed) == 0
-
-#%%
-# Pipe functions
-#  _validate_object
-# validate_input_parameters
-#? _fuzzy_min_score
-#* _extract_matching_chemical_name
-#? set_conditions
-#? _fetch_chemical_database
-#* calculate_mean_dw_concentration
-#* calculate_peak_dw_concentration
-#* calculate_mean_allowable_gw_concentration
-#* calculate_peak_allowable_gw_concentration
-
-#Segment functions
-#* _correct_for_temperature
-#* _concentration_correction
-# na _correct_for_age
-#* _calculate_ref_logK
-#* _calculate_ref_logD
-#* _calculate_logK
-#* _calculate_logD
-#* _calculate_pipe_K_D
-#* _calculate_stagnation_factor
-#* _calculate_mean_dw_mass_per_segment
-#* _calculate_peak_dw_mass_per_segment
+#%% ----------------------------------------------------------------------------
+# A. Hockin, January 2023
+# KWR 403230-003
+# Pipe permeation calculator
+# With Martin vd Schans, Bram
+#
+# ------------------------------------------------------------------------------
+
+#%% ----------------------------------------------------------------------------
+# INITIALISATION OF PYTHON e.g. packages, etc.
+# ------------------------------------------------------------------------------
+
+# Plotting modules
+import matplotlib.pyplot as plt
+import matplotlib
+import matplotlib.colors as colors
+
+import numpy as np
+import pandas as pd
+import os
+import sys
+from pandas import read_csv
+from pandas import read_excel
+import math
+import datetime
+from datetime import timedelta
+
+from pathlib import Path
+
+from pipepermcalc.pipe import * 
+from pipepermcalc.segment import * 
+
+#%%
+
+def raise_exception_two_values(answer, ref_answer, round_values=None):
+    ''' Raise exception if two values are not equal.'''
+    if round_values is None:
+        assert answer == ref_answer
+    else:
+        answer_round = round(answer, round_values)
+        ref_answer = round(ref_answer, round_values)
+        assert answer_round == ref_answer
+
+
+def test_logKpw_ref():
+    '''test the calculatiion of the reference logK value against the excel'''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 0.112980124482, 
+                                    flow_rate=0.5)
+    raise_exception_two_values(answer=seg1.log_Kpw_ref, 
+                               ref_answer = 1.64761000, 
+                               round_values=5)
+
+def test_logDp_ref():
+    '''test the calculatiion of the reference logD value against the excel'''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 0.112980124482, 
+                                    flow_rate=0.5)
+  
+    raise_exception_two_values(answer=seg1.log_Dp_ref, 
+                               ref_answer = -11.54717, 
+                               round_values=5)
+
+def test_logKp_ref_temperature_correction():
+    '''test the calculatiion of the reference logK value, corrected for temperature
+      against the excel'''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 0.112980124482, 
+                                    flow_rate=0.5)
+    raise_exception_two_values(answer=seg1.f_Ktemp, 
+                               ref_answer = -0.071506, 
+                               round_values=6)
+
+
+def test_logDp_ref_temperature_correction():
+    '''test the calculatiion of the reference logD value, corrected for temperature
+      against the excel'''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 0.112980124482, 
+                                    flow_rate=0.5)
+    raise_exception_two_values(answer=seg1.f_Dtemp, 
+                               ref_answer = -0.305084,
+                               round_values=6)
+    
+
+def test_logKp_ref_concentration_correction():
+    '''test the calculation of the reference logK value, 
+    corrected for concentration against the excel'''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 1.8,
+                                    flow_rate=0.5)
+    
+    raise_exception_two_values(answer=seg1.f_Kconc,
+                               ref_answer = -0.103871,
+                               round_values=6)
+    
+
+def test_logDp_ref_concentration_correction():
+    '''test the calculatiion of the reference logD value, 
+    corrected for concentration '''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater =1.8,
+                                    flow_rate=0.5)
+    raise_exception_two_values(answer=seg1.f_Dconc,
+                               ref_answer =  -0.391329, 
+                               round_values=6)
+    
+
+def test_logKpw():
+    '''test the calculatiion of the logKpw'''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 1.8,
+                                    flow_rate=0.5)
+    raise_exception_two_values(answer=seg1.log_Kpw,
+                               ref_answer = 1.472233,
+                               round_values=6)
+    
+
+def test_logDpw():
+    '''test the calculatiion of the logDw'''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 1.8,
+                                    flow_rate=0.5)
+    raise_exception_two_values(answer=seg1.log_Dp, 
+                               ref_answer = -12.243587, 
+                               round_values=6)
+    
+
+def test_stagnation_factor():
+    '''test the calculatiion of the stagnation factor'''
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 1.8,
+                                    flow_rate=0.5)
+    
+    pipe1.validate_input_parameters()
+    pipe1.calculate_peak_dw_concentration()    
+
+    raise_exception_two_values(answer=seg1.stagnation_factor,
+                               ref_answer =  1.387905, 
+                               round_values=6)
+
+def test_updating_partitioning_coefficient():
+    ''' Test the update function for the partitioning coefficient '''
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 1.8,
+                                    flow_rate=0.5)
+    pipe1.validate_input_parameters()
+    seg1.log_Kpw= 0.9116730996845103
+
+    pipe1.calculate_peak_dw_concentration()    
+
+    raise_exception_two_values(answer=seg1.log_Kpw,
+                               ref_answer = 0.911673, 
+                               round_values=6)
+
+
+def test_updating_diffusion_coefficient():
+    ''' Test the update function for the diffusion coefficient '''
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 1.8,
+                                    flow_rate=0.5)
+    pipe1.validate_input_parameters()
+    seg1.log_Dp= -12.743586769549616
+    
+    pipe1.calculate_peak_dw_concentration()    
+   
+    raise_exception_two_values(answer=seg1.log_Dp, 
+                               ref_answer = -12.743586769549616, 
+                               round_values=None)
+
+
+
+def test_calculate_peak_dw_concentration():
+    ''' Test the calculation for the peak concentration in drinking water given 
+    a groundwater concentration '''
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 0.112980124482,
+                                    flow_rate=0.5)
+    pipe1.validate_input_parameters()
+    
+    pipe1.calculate_peak_dw_concentration()    
+
+    raise_exception_two_values(answer=pipe1.concentration_drinking_water, 
+                               ref_answer = 0.001, 
+                               round_values=3)
+    
+def test_calculate_peak_dw_mass():
+    ''' Test the calculation for the peak concentration in drinking water given 
+    a groundwater concentration '''
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 0.112980124482,
+                                    flow_rate=0.5)
+    pipe1.validate_input_parameters()
+    
+    pipe1.calculate_peak_dw_concentration()    
+
+    raise_exception_two_values(answer=seg1.mass_chemical_drinkwater, 
+                               ref_answer = 7.469113135415852e-06, 
+                               round_values=9)    
+
+def test_calculate_mean_dw_concentration():
+    ''' Test the calculation for the mean concentration in drinking water given 
+    a groundwater concentration '''
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 1.8,
+                                    flow_rate=0.5)
+    pipe1.validate_input_parameters()
+    
+    pipe1.calculate_mean_dw_concentration()    
+
+    raise_exception_two_values(answer=pipe1.concentration_drinking_water, 
+                               ref_answer = 0.001, 
+                               round_values=5)
+
+def test_calculate_mean_dw_mass():
+    ''' Test the calculation for the mean concentration in drinking water given 
+    a groundwater concentration '''
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=25,
+                    inner_diameter=0.0196,
+                    wall_thickness=0.0027,
+                    )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+
+    pipe1.set_conditions(chemical_name="Benzeen", 
+                                    temperature_groundwater=12, 
+                                    concentration_groundwater = 1.8,
+                                    flow_rate=0.5)
+    pipe1.validate_input_parameters()
+    
+    pipe1.calculate_mean_dw_concentration()    
+
+    raise_exception_two_values(answer=seg1.mass_chemical_drinkwater, 
+                               ref_answer = 0.0005000956341327644, 
+                               round_values=5)    
+
+def test_segment_surface_area_calculations():
+    ''' Test the calculation for the different surface area options '''
+    seg1 = Segment(name='seg1',
+                material='PE40',
+                length=7.5/1000,
+                inner_diameter=30.3/1000,
+                wall_thickness=1.5/1000,
+                permeation_direction='parallel',
+                diffusion_path_length=7.5/1000,
+                    )
+
+   
+    raise_exception_two_values(answer=seg1.permeation_surface_area, 
+                               ref_answer = 0.000073159839, 
+                               round_values=12)
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=1/1000,
+                    inner_diameter=28.5/1000,
+                    wall_thickness=10/1000,
+                    permeation_direction='perpendicular',
+                    diffusion_path_length=10/1000
+                    )
+
+    
+    raise_exception_two_values(answer=seg1.permeation_surface_area, 
+                               ref_answer = 0.000089535391, 
+                               round_values=12)
+
+    seg1 = Segment(name='seg1',
+                    material='PE40',
+                    length=33.3/1000,
+                    inner_diameter=25/1000,
+                    wall_thickness=2.7/1000,
+                    permeation_direction='perpendicular',)
+    
+    raise_exception_two_values(answer=seg1.permeation_surface_area, 
+                               ref_answer = 0.002615375884, 
+                               round_values=12)
+
+
+def test_return_matching_chemical_name():
+    seg1 = Segment(name='seg1',
+                material='PE40',
+                length=25,
+                inner_diameter=0.0196,
+                wall_thickness=0.0027,
+                )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.segment_list
+    chemical_name = 'Benzeen'
+    matching_name = pipe1._extract_matching_chemical_name(chemical_name=chemical_name, 
+                                          database=list(pipe1.ppc_database['chemical_name_NL']))
+    assert chemical_name == matching_name
+
+
+def test_calculate_mean_allowable_gw_concentration():
+    ''' Test the calculation for the mean concentration allowed in groundwater given 
+    a drinking water concentration '''
+    
+    seg1 = Segment(name='seg1',
+                material= 'PE40',
+                length=25,
+                inner_diameter=0.0196,
+                wall_thickness=0.0027,
+                )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.set_conditions(
+        chemical_name="Benzeen", 
+        temperature_groundwater=12, 
+        concentration_drinking_water=0.001,
+        flow_rate=0.5 )
+
+    pipe1.validate_input_parameters()
+
+    mean_conc = pipe1.calculate_mean_allowable_gw_concentration(tolerance = 0.001)
+
+    raise_exception_two_values(answer=mean_conc, 
+                               ref_answer = 1.8011, 
+                               round_values=4)
+
+def test_calculate_peak_allowable_gw_concentration():
+    ''' Test the calculation for the peak concentration allowed in groundwater given 
+    a drinking water concentration '''
+    seg1 = Segment(name='seg1',
+                material= 'PE40',
+                length=25,
+                inner_diameter=0.0196,
+                wall_thickness=0.0027,
+                )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    pipe1.set_conditions(
+        chemical_name="Benzeen", 
+        temperature_groundwater=12, 
+        concentration_drinking_water=0.001,
+        flow_rate=0.5 )
+
+    pipe1.validate_input_parameters()
+
+    peak_conc = pipe1.calculate_peak_allowable_gw_concentration(tolerance = 0.01)
+
+    raise_exception_two_values(answer=peak_conc, 
+                               ref_answer = 0.1138, 
+                               round_values=4)
+
+def test_groundwater_to_soil_conversion():
+    seg1 = Segment(name='seg1',
+                material= 'PE40',
+                length=25,
+                inner_diameter=0.0196,
+                wall_thickness=0.0027,
+                )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(
+        chemical_name="Benzeen", 
+        temperature_groundwater=12, 
+        concentration_groundwater=1.8,
+        flow_rate=0.5 )
+
+    pipe1.validate_input_parameters()
+
+    pipe1.calculate_mean_dw_concentration()
+
+    raise_exception_two_values(answer=pipe1.concentration_soil, 
+                               ref_answer =2.74, 
+                               round_values=3)
+    # Check that pipe summation is going correctly
+    seg1 = Segment(name='seg1',
+                material= 'PE40',
+                length=25,
+                inner_diameter=0.0196,
+                wall_thickness=0.0027,
+                )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(
+        chemical_name="ethylbenzene", 
+        temperature_groundwater=12, 
+        concentration_groundwater=0.277,
+        flow_rate=0.5 )
+
+    pipe1.validate_input_parameters()
+
+    pipe1.calculate_mean_dw_concentration()
+
+    raise_exception_two_values(answer=pipe1.concentration_soil, 
+                               ref_answer =1.842, 
+                               round_values=3)
+
+def test_soil_to_groundwater_conversion():
+    seg1 = Segment(name='seg1',
+                material= 'PE40',
+                length=25,
+                inner_diameter=0.0196,
+                wall_thickness=0.0027,
+                )
+
+    pipe1 = Pipe(segment_list=[seg1])
+
+    pipe1.set_conditions(
+        chemical_name="Benzeen",
+        temperature_groundwater=12, 
+        concentration_soil=2.7527429729399238,
+        flow_rate=0.5 )
+
+    pipe1.validate_input_parameters()
+
+    pipe1.calculate_mean_dw_concentration()
+
+    raise_exception_two_values(answer=pipe1.concentration_groundwater, 
+                               ref_answer = 1.8085521338873323, 
+                               round_values=5)
+
+def test_GW_to_DW_to_GW_peak():
+    '''Tests if the calculation from GW to DW gives the same result as DW to GW 
+    for the peak concentrations'''
+
+    seg1 = Segment(name='seg1',
+                material= 'PE40',
+                length=25,
+                inner_diameter=0.0196,
+                wall_thickness=0.0027,
+                )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    input_gw = 1
+
+    database = pipe1.view_database_chemical_names( language='NL')
+    database = pipe1.ppc_database.dropna(subset=['molecular_weight', 'solubility', 'Drinking_water_norm'])
+    database = database.loc[database['log_distribution_coefficient']>=0]
+    database = database.loc[database['Drinking_water_norm'] < database['solubility'] ]
+    database_chemicals = database['chemical_name_NL']
+    solubilities = database['solubility']
+
+    failed = []
+
+    for chemical_name, solubiliy in zip(database_chemicals, solubilities):
+        if input_gw > solubiliy:
+            input_gw = 0.01 * solubiliy
+
+        pipe1.set_conditions(
+            chemical_name=chemical_name, 
+                            concentration_groundwater =input_gw,
+                            temperature_groundwater=12, 
+                            flow_rate=0.5)
+
+        pipe1.validate_input_parameters()
+
+        peak_conc=pipe1.calculate_peak_dw_concentration()
+
+        pipe1.set_conditions(chemical_name=chemical_name, 
+                            temperature_groundwater=12, 
+                            concentration_drinking_water = peak_conc,
+                            flow_rate=0.5)
+
+        output_gw = pipe1.calculate_peak_allowable_gw_concentration()
+
+        if abs(1-(input_gw/output_gw)) < 0.02:
+            pass
+        else: 
+            failed.append(chemical_name)
+    
+    assert len(failed) == 0
+
+
+def test_GW_to_DW_to_GW_mean():
+    '''Tests if the calculation from GW to DW gives the same result as DW to GW 
+    for the mean concentrations'''
+
+    seg1 = Segment(name='seg1',
+                material= 'PE40',
+                length=25,
+                inner_diameter=0.0196,
+                wall_thickness=0.0027,
+                )
+
+    pipe1 = Pipe(segment_list=[seg1])
+    input_gw = 1
+
+    database = pipe1.view_database_chemical_names( language='NL')
+    database = pipe1.ppc_database.dropna(subset=['molecular_weight', 'solubility', 'Drinking_water_norm'])
+    database = database.loc[database['log_distribution_coefficient']>=0]
+    database = database.loc[database['Drinking_water_norm'] < database['solubility'] ]
+    database_chemicals = database['chemical_name_NL']
+    solubilities = database['solubility']
+
+    failed = []
+
+    for chemical_name, solubiliy in zip(database_chemicals, solubilities):
+        if input_gw > solubiliy:
+            input_gw = 0.01 * solubiliy
+
+        pipe1.set_conditions(
+            chemical_name=chemical_name, 
+                            concentration_groundwater =input_gw,
+                            temperature_groundwater=12, 
+                            flow_rate=0.5)
+
+        pipe1.validate_input_parameters()
+
+        mean_conc=pipe1.calculate_mean_dw_concentration()
+
+        pipe1.set_conditions(chemical_name=chemical_name, 
+                            temperature_groundwater=12, 
+                            concentration_drinking_water = mean_conc,
+                            flow_rate=0.5)
+
+        output_gw = pipe1.calculate_mean_allowable_gw_concentration()
+
+        if abs(1-(input_gw/output_gw)) < 0.02:
+            pass
+        else: 
+            failed.append(chemical_name)
+    
+    assert len(failed) == 0
+
+#%%
+# Pipe functions
+#  _validate_object
+# validate_input_parameters
+#? _fuzzy_min_score
+#* _extract_matching_chemical_name
+#? set_conditions
+#? _fetch_chemical_database
+#* calculate_mean_dw_concentration
+#* calculate_peak_dw_concentration
+#* calculate_mean_allowable_gw_concentration
+#* calculate_peak_allowable_gw_concentration
+
+#Segment functions
+#* _correct_for_temperature
+#* _concentration_correction
+# na _correct_for_age
+#* _calculate_ref_logK
+#* _calculate_ref_logD
+#* _calculate_logK
+#* _calculate_logD
+#* _calculate_pipe_K_D
+#* _calculate_stagnation_factor
+#* _calculate_mean_dw_mass_per_segment
+#* _calculate_peak_dw_mass_per_segment
```

