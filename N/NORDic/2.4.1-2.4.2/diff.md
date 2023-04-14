# Comparing `tmp/NORDic-2.4.1.tar.gz` & `tmp/NORDic-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NORDic-2.4.1.tar", last modified: Thu Mar  2 18:08:07 2023, max compression
+gzip compressed data, was "NORDic-2.4.2.tar", last modified: Fri Apr 14 18:05:27 2023, max compression
```

## Comparing `NORDic-2.4.1.tar` & `NORDic-2.4.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.110671 NORDic-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-02 18:08:07.110671 NORDic-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-03-02 18:07:58.000000 NORDic-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-02 18:07:58.000000 NORDic-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 18:08:07.110671 NORDic-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-02 18:07:58.000000 NORDic-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.106671 NORDic-2.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.106671 NORDic-2.4.1/src/NORDic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.106671 NORDic-2.4.1/src/NORDic/NORDic_DR/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_DR/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16854 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_DR/bandits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6023 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_DR/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14603 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_DR/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.106671 NORDic-2.4.1/src/NORDic/NORDic_DS/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_DS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13551 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_DS/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_DS/get_drug_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_DS/get_drug_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.106671 NORDic-2.4.1/src/NORDic/NORDic_NI/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_NI/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8840 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_NI/cytoscape_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    40173 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_NI/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.106671 NORDic-2.4.1/src/NORDic/NORDic_PMR/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_PMR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/NORDic_PMR/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.110671 NORDic-2.4.1/src/NORDic/UTILS/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7097 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/DISGENET_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28342 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/LINCS_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17756 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/STRING_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9247 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/utils_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14958 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/utils_exp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33766 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/utils_grn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/utils_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/utils_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/utils_sim.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7357 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/UTILS/utils_state.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 18:07:58.000000 NORDic-2.4.1/src/NORDic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 18:08:07.106671 NORDic-2.4.1/src/NORDic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-02 18:08:07.000000 NORDic-2.4.1/src/NORDic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-02 18:08:07.000000 NORDic-2.4.1/src/NORDic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 18:08:07.000000 NORDic-2.4.1/src/NORDic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-02 18:08:07.000000 NORDic-2.4.1/src/NORDic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-02 18:08:07.000000 NORDic-2.4.1/src/NORDic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.306291 NORDic-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-14 18:05:27.306291 NORDic-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-14 18:05:19.000000 NORDic-2.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 18:05:19.000000 NORDic-2.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:05:27.306291 NORDic-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-14 18:05:19.000000 NORDic-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.298291 NORDic-2.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.298291 NORDic-2.4.2/src/NORDic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.302291 NORDic-2.4.2/src/NORDic/NORDic_DR/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DR/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16854 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DR/bandits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6023 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DR/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14603 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DR/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.302291 NORDic-2.4.2/src/NORDic/NORDic_DS/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13551 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DS/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DS/get_drug_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DS/get_drug_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.302291 NORDic-2.4.2/src/NORDic/NORDic_NI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_NI/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8840 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_NI/cytoscape_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40173 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_NI/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.306291 NORDic-2.4.2/src/NORDic/NORDic_PMR/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_PMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_PMR/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.306291 NORDic-2.4.2/src/NORDic/UTILS/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7097 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/DISGENET_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28342 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/LINCS_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17756 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/STRING_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9247 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14958 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_exp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33766 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_grn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_sim.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7357 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.302291 NORDic-2.4.2/src/NORDic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/top_level.txt
```

### Comparing `NORDic-2.4.1/PKG-INFO` & `NORDic-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NORDic
-Version: 2.4.1
+Version: 2.4.2
 Summary: Network Oriented Repurposing of Drugs (NORDic): network identification / master regulator detection / drug effect simulator / drug repurposing
 Home-page: https://github.com/clreda/NORDic
 Author: Clémence Réda
 Author-email: clemence.reda@inserm.fr
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -62,29 +62,29 @@
 ```bash
 pip install -U colomoto-docker
 colomoto-docker
 ```
 
 ## Example usage
 
-Once installed, to import NORDic
+Once installed, to import **NORDic**
 
 ```python
 import NORDic 
 ```
 
 Please check out the associated Jupyter notebooks in folder [*notebooks/*](https://github.com/clreda/NORDic/tree/main/notebooks), starting with [this short notebook](https://github.com/clreda/NORDic/blob/main/notebooks/NORDic%20CoLoMoTo.ipynb). All functions are documented, so one can check out the inputs and outputs of a function *func* by typing
 
 ```python
 help(func)
 ```
 
 ## Cite
 
-If you use NORDic in published research, please cite the following preliminary work:
+If you use **NORDic** in academic research, please cite the following preliminary work (which relied on the same type of pipeline as **NORDic NI** and **NORDic PMR**, but with different implementations):
 
 + Formatted citation:
 
 > Réda, C., & Delahaye-Duriez, A. (2022, August). Prioritization of Candidate Genes Through Boolean Networks. In Computational Methods in Systems Biology: 20th International Conference, CMSB 2022, Bucharest, Romania, September 14–16, 2022, Proceedings (pp. 89-121). Cham: Springer International Publishing.
 
 + BibTeX citation:
```

### Comparing `NORDic-2.4.1/README.md` & `NORDic-2.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,29 +48,29 @@
 ```bash
 pip install -U colomoto-docker
 colomoto-docker
 ```
 
 ## Example usage
 
-Once installed, to import NORDic
+Once installed, to import **NORDic**
 
 ```python
 import NORDic 
 ```
 
 Please check out the associated Jupyter notebooks in folder [*notebooks/*](https://github.com/clreda/NORDic/tree/main/notebooks), starting with [this short notebook](https://github.com/clreda/NORDic/blob/main/notebooks/NORDic%20CoLoMoTo.ipynb). All functions are documented, so one can check out the inputs and outputs of a function *func* by typing
 
 ```python
 help(func)
 ```
 
 ## Cite
 
-If you use NORDic in published research, please cite the following preliminary work:
+If you use **NORDic** in academic research, please cite the following preliminary work (which relied on the same type of pipeline as **NORDic NI** and **NORDic PMR**, but with different implementations):
 
 + Formatted citation:
 
 > Réda, C., & Delahaye-Duriez, A. (2022, August). Prioritization of Candidate Genes Through Boolean Networks. In Computational Methods in Systems Biology: 20th International Conference, CMSB 2022, Bucharest, Romania, September 14–16, 2022, Proceedings (pp. 89-121). Cham: Springer International Publishing.
 
 + BibTeX citation:
```

### Comparing `NORDic-2.4.1/setup.py` & `NORDic-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "NORDic"
-VERSION = "2.4.1"
+VERSION = "2.4.2"
 
 setup(name=NAME,
     version=VERSION,
     author="Clémence Réda",
     author_email="clemence.reda@inserm.fr",
     url="https://github.com/clreda/NORDic",
     license_files = ('LICENSE'),
```

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_DR/bandits.py` & `NORDic-2.4.2/src/NORDic/NORDic_DR/bandits.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_DR/functions.py` & `NORDic-2.4.2/src/NORDic/NORDic_DR/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_DR/utils.py` & `NORDic-2.4.2/src/NORDic/NORDic_DR/utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_DS/functions.py` & `NORDic-2.4.2/src/NORDic/NORDic_DS/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_DS/get_drug_signatures.py` & `NORDic-2.4.2/src/NORDic/NORDic_DS/get_drug_signatures.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,21 +76,22 @@
         response = requests.get(request_url)
         assert response.status_code == 200
         data = json.loads(response.text)
         drug_name = data[0]["pert_iname"] if (len(data)>0) else np.nan
         pert_inames.setdefault(pubchem_cid, drug_name)
     return pert_inames
 
-def retrieve_drug_signature(pubchem_cid, cell_ids, gene_list, lincs_args, quiet=False):
+def retrieve_drug_signature(pubchem_cid, cell_ids, gene_list, lincs_args, binarize, quiet=False):
     '''
         Retrieve control & treated samples from LINCS L1000 and compute the corresponding drug signature
         @param\tpubchem_cid\tPython integer: drug PubChem CID
         @param\tcell_ids\tPython character string list: list of candidate cell lines in LINCS L1000
         @param\tgene_list\tPython integer list: list of EntrezID genes
         @param\tlincs_args\tPython dictionary: additional arguments for LINCS L1000 requests
+        @param\tbinarize\tPython bool: should the resulting signatures be binarized?
         @param\tquiet\tPython bool[default=False]
         @return\tsig\tPandas DataFrame: rows/[genes] x column/[drug PubChem]
     '''
     endpoint = "sigs"
     method = "filter"
     pert_iname = pubchem2drugname([pubchem_cid], lincs_args)[pubchem_cid]
     assert lincs_args and "credentials" in lincs_args
@@ -134,29 +135,30 @@
     nsamples = len(data_treated+data_control)
     if (not quiet):
         print("%d samples" % nsamples)
     sigs = create_restricted_drug_signatures(data_treated+data_control, gene_list, which_lvl=[3], strict=True, path_to_lincs=lincs_args["path_to_lincs"])
     if (sigs is None):
         return None
     assert sigs.shape[1] == nsamples
-    sig = binarize_via_CD(sigs, samples=[2]*len(data_treated)+[1]*len(data_control), binarize=0, nperm=10000)
+    sig = binarize_via_CD(sigs, samples=[2]*len(data_treated)+[1]*len(data_control), binarize=int(binarize), nperm=10000)
     sig.columns = [pubchem_cid]
     return sig
 
-def compute_drug_signatures_L1000(pubchem_cids, lincs_args, chunksize=10):
+def compute_drug_signatures_L1000(pubchem_cids, lincs_args, binarize=True, chunksize=10):
     '''
         Get drug signatures from LINCS L1000
         @param\tpubchem_cids\tPython integer list: list of drug PubChem CIDs
         @param\tlincs_args\tPython dictionary: additional arguments for LINCS L1000 requests
+        @param\tbinarize\tPython bool[default=True]: should the resulting signatures be binarized?
         @return\tsigs\tPandas DataFrame: rows/[genes] x columns/[drug names]
     '''
     assert lincs_args and "credentials" in lincs_args and "path_to_lincs" in lincs_args
     user_key = get_user_key(lincs_args["credentials"])
     path_to_lincs = lincs_args["path_to_lincs"]
     pert_inames = pubchem2drugname(pubchem_cids, lincs_args)
     gene_files, _, _, _ = download_lincs_files(path_to_lincs, which_lvl=[3])
     gene_df = pd.read_csv(path_to_lincs+gene_files[0], sep="\t", engine='python', index_col=0)
     gene_list, gene_name_list = list(gene_df.index), list(gene_df["pr_gene_symbol"])
-    sigs_list = [retrieve_drug_signature(pubchem_cid, get_all_celllines([pert_inames[pubchem_cid]], user_key) if (len(lincs_args.get("cell_lines", []))==0) else lincs_args["cell_lines"], gene_list, lincs_args) for pubchem_cid in pubchem_cids]
+    sigs_list = [retrieve_drug_signature(pubchem_cid, get_all_celllines([pert_inames[pubchem_cid]], user_key) if (len(lincs_args.get("cell_lines", []))==0) else lincs_args["cell_lines"], gene_list, lincs_args, binarize) for pubchem_cid in pubchem_cids]
     sigs = sigs_list[0].join(sigs_list[1:], how="outer")
     sigs.index = [gene_df.loc[i]["pr_gene_symbol"] for i in sigs.index]
     return sigs
```

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_DS/get_drug_targets.py` & `NORDic-2.4.2/src/NORDic/NORDic_DS/get_drug_targets.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_NI/cytoscape_style.py` & `NORDic-2.4.2/src/NORDic/NORDic_NI/cytoscape_style.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_NI/functions.py` & `NORDic-2.4.2/src/NORDic/NORDic_NI/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/NORDic_PMR/functions.py` & `NORDic-2.4.2/src/NORDic/NORDic_PMR/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/DISGENET_utils.py` & `NORDic-2.4.2/src/NORDic/UTILS/DISGENET_utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/LINCS_utils.py` & `NORDic-2.4.2/src/NORDic/UTILS/LINCS_utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/STRING_utils.py` & `NORDic-2.4.2/src/NORDic/UTILS/STRING_utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/utils_data.py` & `NORDic-2.4.2/src/NORDic/UTILS/utils_data.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/utils_exp.py` & `NORDic-2.4.2/src/NORDic/UTILS/utils_exp.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/utils_grn.py` & `NORDic-2.4.2/src/NORDic/UTILS/utils_grn.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/utils_network.py` & `NORDic-2.4.2/src/NORDic/UTILS/utils_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             x = network.iloc[idx,:]["score"]
             scores.append(x)
     final_network["score"] = scores
     return final_network
 
 ## https://workflows.omnipathdb.org/tissue-hpa.pdf
 ## https://workflows.omnipathdb.org/networks-r.html
-def get_network_from_OmniPath(gene_list=None, disease_name=None, species="human", sources_int=None, domains_int=None, types_int=None, min_curation_effort=-1, domains_annot='HPA_tissue', quiet=False):
+def get_network_from_OmniPath(gene_list=None, disease_name=None, species="human", sources_int="omnipath", domains_int=None, types_int=None, min_curation_effort=-1, domains_annot='HPA_tissue', quiet=False):
     '''
         Retrieve a network from OmniPath
         @param\tgene_list\tPython character string[default=None]: List of genes to consider (or do not filter the interactions from Omnipath if =None)
         @param\tdisease_name\tPython character string[default=None]: Disease name (in letters) to consider
         @param\tspecies\tPython character string[default=None]: Species to consider (either "human", "mouse", or "rat")
         @param\tsources_int\tPython character string[default=None]: Which databases for interactions to consider (if =None, consider them all)
         @param\tdomains_int\tPython character string[default=None]:
@@ -124,16 +124,16 @@
         @param\tdomain_annot\tPython integer[default='HPA_tissue']:
         @param\tquiet\tPython bool[default=None]:  
         @return\tfinal_network\tPandas DataFrame: rows/[interactions] x columns/[["preferredName_A", "preferredName_B", "sign", "directed", "score"]]
                 \tannot_wide\tPandas DataFrame: rows/[gene symbols] x columns/[annotations from the database @domains_annot]
     '''
     assert species in ['human', 'mouse', 'rat']
     assert types_int in [None, "post_translational", "transcriptional", "post_transcriptional", "mirna_transcriptional"]
-    assert sources_int in [None]+list(op.interactions.AllInteractions.resources())
-    assert domains_int in [None, "DOROTHEA", "KINASE_EXTRA", "LIGREC_EXTRA", "LNCRNA_MRNA", "MIRNA_TARGET","OMNIPATH",
+    assert sources_int in list(op.interactions.AllInteractions.resources())
+    assert domains_int in ["DOROTHEA", "KINASE_EXTRA", "LIGREC_EXTRA", "LNCRNA_MRNA", "MIRNA_TARGET","OMNIPATH",
         "PATHWAY_EXTRA", "SMALL_MOLECULE", "TF_MIRNA", "TF_REGULONS", "TF_TARGET"]
     assert domains_annot in [None]+list(op.requests.Annotations.resources())
     assert (gene_list is not None) or (disease_name is not None)
     params = {"organisms": species, "include": domains_int, "sources": sources_int, "fields": ['curation_effort'], #'references', 'sources', 'type'], 
               "genesymbols": True, "types": types_int, "directed": False, "signed": False} 
     with capture() as out:
         interactions = op.interactions.AllInteractions.get(**params).squeeze('columns')
```

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/utils_plot.py` & `NORDic-2.4.2/src/NORDic/UTILS/utils_plot.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/utils_sim.py` & `NORDic-2.4.2/src/NORDic/UTILS/utils_sim.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic/UTILS/utils_state.py` & `NORDic-2.4.2/src/NORDic/UTILS/utils_state.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.1/src/NORDic.egg-info/PKG-INFO` & `NORDic-2.4.2/src/NORDic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NORDic
-Version: 2.4.1
+Version: 2.4.2
 Summary: Network Oriented Repurposing of Drugs (NORDic): network identification / master regulator detection / drug effect simulator / drug repurposing
 Home-page: https://github.com/clreda/NORDic
 Author: Clémence Réda
 Author-email: clemence.reda@inserm.fr
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -62,29 +62,29 @@
 ```bash
 pip install -U colomoto-docker
 colomoto-docker
 ```
 
 ## Example usage
 
-Once installed, to import NORDic
+Once installed, to import **NORDic**
 
 ```python
 import NORDic 
 ```
 
 Please check out the associated Jupyter notebooks in folder [*notebooks/*](https://github.com/clreda/NORDic/tree/main/notebooks), starting with [this short notebook](https://github.com/clreda/NORDic/blob/main/notebooks/NORDic%20CoLoMoTo.ipynb). All functions are documented, so one can check out the inputs and outputs of a function *func* by typing
 
 ```python
 help(func)
 ```
 
 ## Cite
 
-If you use NORDic in published research, please cite the following preliminary work:
+If you use **NORDic** in academic research, please cite the following preliminary work (which relied on the same type of pipeline as **NORDic NI** and **NORDic PMR**, but with different implementations):
 
 + Formatted citation:
 
 > Réda, C., & Delahaye-Duriez, A. (2022, August). Prioritization of Candidate Genes Through Boolean Networks. In Computational Methods in Systems Biology: 20th International Conference, CMSB 2022, Bucharest, Romania, September 14–16, 2022, Proceedings (pp. 89-121). Cham: Springer International Publishing.
 
 + BibTeX citation:
```

### Comparing `NORDic-2.4.1/src/NORDic.egg-info/SOURCES.txt` & `NORDic-2.4.2/src/NORDic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

