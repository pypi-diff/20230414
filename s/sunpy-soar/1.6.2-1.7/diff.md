# Comparing `tmp/sunpy-soar-1.6.2.tar.gz` & `tmp/sunpy-soar-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunpy-soar-1.6.2.tar", last modified: Wed Feb  1 18:08:43 2023, max compression
+gzip compressed data, was "sunpy-soar-1.7.tar", last modified: Fri Apr 14 15:22:37 2023, max compression
```

## Comparing `sunpy-soar-1.6.2.tar` & `sunpy-soar-1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:43.347161 sunpy-soar-1.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/.github/workflows/python-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/sunpy_soar/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/sunpy_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/sunpy_soar/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/sunpy_soar/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/sunpy_soar/data/
--rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/sunpy_soar/data/attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/sunpy_soar/data/instrument_attrs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/sunpy_soar/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/sunpy_soar/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/sunpy_soar/tests/test_sunpy_soar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/sunpy_soar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-02-01 18:08:43.000000 sunpy-soar-1.6.2/sunpy_soar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-01 18:08:43.000000 sunpy-soar-1.6.2/sunpy_soar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 18:08:43.000000 sunpy-soar-1.6.2/sunpy_soar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 18:08:43.000000 sunpy-soar-1.6.2/sunpy_soar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-01 18:08:43.000000 sunpy-soar-1.6.2/sunpy_soar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-01 18:08:43.000000 sunpy-soar-1.6.2/sunpy_soar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:08:43.351161 sunpy-soar-1.6.2/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-02-01 18:08:27.000000 sunpy-soar-1.6.2/tools/update_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.397114 sunpy-soar-1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-14 15:22:16.000000 sunpy-soar-1.7/.github/workflows/python-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-14 15:22:16.000000 sunpy-soar-1.7/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 15:22:16.000000 sunpy-soar-1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 15:22:16.000000 sunpy-soar-1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-14 15:22:16.000000 sunpy-soar-1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-14 15:22:37.401114 sunpy-soar-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-14 15:22:16.000000 sunpy-soar-1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 15:22:16.000000 sunpy-soar-1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-14 15:22:37.405114 sunpy-soar-1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/sunpy_soar/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/sunpy_soar/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/data/attrs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/data/instrument_attrs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/sunpy_soar/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/tests/test_sunpy_soar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/sunpy_soar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-14 15:22:16.000000 sunpy-soar-1.7/tools/update_data.py
```

### Comparing `sunpy-soar-1.6.2/.github/workflows/python-release.yml` & `sunpy-soar-1.7/.github/workflows/python-release.yml`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.6.2/.github/workflows/python-test.yml` & `sunpy-soar-1.7/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.6.2/.pre-commit-config.yaml` & `sunpy-soar-1.7/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
           [
             "--count",
             "--select",
             "E901,E902,F822,F823",
           ]
         exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*|extern.*|.rst|.md|cm/__init__.py|sunpy/extern|sunpy/visualization/colormaps/color_tables.py)$"
   - repo: https://github.com/PyCQA/autoflake
-    rev: v2.0.0
+    rev: v2.0.2
     hooks:
       - id: autoflake
         args:
           [
             "--in-place",
             "--remove-all-unused-imports",
             "--remove-unused-variable",
@@ -29,15 +29,15 @@
         exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*|extern.*|.rst|.md|__init__.py|sunpy/extern|docs/conf.py)$"
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*|extern.*|.rst|.md|cm/__init__.py|sunpy/extern|docs/conf.py)$"
   - repo: https://github.com/pre-commit/mirrors-autopep8
-    rev: v2.0.1
+    rev: v2.0.2
     hooks:
     -   id: autopep8
         args: ["--in-place","--max-line-length", "200"]
         exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*|extern.*|.rst|.md|cm/__init__.py|sunpy/extern|sunpy/visualization/colormaps/color_tables.py)$"
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
```

### Comparing `sunpy-soar-1.6.2/LICENSE` & `sunpy-soar-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.6.2/PKG-INFO` & `sunpy-soar-1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy-soar
-Version: 1.6.2
+Version: 1.7
 Summary: A sunpy plugin for accessing data in the Solar Orbiter Archive (SOAR).
 Home-page: 
 Author: David Stansby
 Author-email: d.stansby@ucl.ac.uk
 License: BSD-2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -39,32 +39,31 @@
 
 
 When interacting with the sunpy-soar project you are asked to follow the `SunPy Code of Conduct <https://sunpy.org/coc>`_ .
 
 Installation
 ------------
 
-sunpy-soar requires `python >= 3.7` and `sunpy >= 2.1`. Currently it can only be installed from
-PyPI using:
+sunpy-soar requires `python >= 3.7` and `sunpy >= 2.1`.
+Currently it can only be installed from PyPI using:
 
 .. code-block:: bash
 
    pip install sunpy-soar
 
 or conda using
 
 .. code-block:: bash
 
    conda install -c conda-forge sunpy-soar
 
 Example usage
 -------------
 
-The code below gives an example of how to search and download Solar Orbiter
-data using ``sunpy.net.Fido``:
+The code below gives an example of how to search and download Solar Orbiter data using ``sunpy.net.Fido``:
 
 .. code-block:: python
 
    # Importing sunpy_soar registers the client with sunpy
    import sunpy_soar
    from sunpy.net import Fido
    import sunpy.net.attrs as a
@@ -81,39 +80,42 @@
 
    # Download files
    files = Fido.fetch(result)
    print(files)
 
 Available search attributes
 ---------------------------
-The easiest way to access search attributes is using
-``import sunpy.net.attrs as a``. When constructing a search for SOAR ``a.Time`` must be
-provided. Other search attributes can be used too - ``sunpy-soar`` recognises the
-following:
+The easiest way to access search attributes is using ``import sunpy.net.attrs as a``.
+When constructing a search for SOAR ``a.Time`` must be provided.
+Other search attributes can be used too - ``sunpy-soar`` recognises the following:
 
 - ``a.Instrument``
 - ``a.Level`` - one of ``L0, L1, L2, L3, LL01, LL02, LL03``
 - ``a.soar.Product``
 
-The third ``near`` argument to ``a.Time`` is not currently supported - you will have to
-manually filter the results if you want to find the one closest to a given
-time.
+The third ``near`` argument to ``a.Time`` is not currently supported - you will have to manually filter the results if you want to find the one closest to a given time.
 
 ``sunpy-soar`` and the VSO
 ==========================
-``sunpy-soar`` queries the official repository of Solar Orbiter data, the SOAR. The Virtual Solar Observatory (VSO) as of writing (September 2022) mirrors a subset of the Solar Orbiter archive alongside many other solar physics data sources. The VSO allows data from multiple missions/observatories to be easily queried in one go, but users should be aware that the VSO is not the official repository for Solar Orbiter data and does not currently (as of September 2022) provide a comprehensive listing of all available Solar Orbiter data.
+``sunpy-soar`` queries the official repository of Solar Orbiter data, the SOAR.
+The Virtual Solar Observatory (VSO) as of writing (September 2022) mirrors a subset of the Solar Orbiter archive alongside many other solar physics data sources.
+The VSO allows data from multiple missions/observatories to be easily queried in one go, but users should be aware that the VSO is not the official repository for Solar Orbiter data and does not currently (as of September 2022) provide a comprehensive listing of all available Solar Orbiter data.
 
 Development
 ===========
 The SunPy developers maintain this package.
 Contributions for new features and bug fixes are welcome.
 
 Changelog
 =========
 
+1.7
+---
+- Added STIX data products to the list of valid data product identifiers.
+
 1.6
 ---
 - Registered a list of instruments available from the SOAR, with the ``a.Instrument`` attribute.
 - Registered the SOAR in the ``a.Provider`` attribute, meaning that a user can specifiy to the Fido search to only query the SOAR by use of ``a.Provider.soar``.
 - The ``_can_handle_query`` function within the SOARClient now checks to make sure if the SOAR supplies the queried data which fixes a bug which searched the SOAR for any data (e.g. AIA data).
 
 1.5
```

### Comparing `sunpy-soar-1.6.2/README.rst` & `sunpy-soar-1.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,31 @@
 
 
 When interacting with the sunpy-soar project you are asked to follow the `SunPy Code of Conduct <https://sunpy.org/coc>`_ .
 
 Installation
 ------------
 
-sunpy-soar requires `python >= 3.7` and `sunpy >= 2.1`. Currently it can only be installed from
-PyPI using:
+sunpy-soar requires `python >= 3.7` and `sunpy >= 2.1`.
+Currently it can only be installed from PyPI using:
 
 .. code-block:: bash
 
    pip install sunpy-soar
 
 or conda using
 
 .. code-block:: bash
 
    conda install -c conda-forge sunpy-soar
 
 Example usage
 -------------
 
-The code below gives an example of how to search and download Solar Orbiter
-data using ``sunpy.net.Fido``:
+The code below gives an example of how to search and download Solar Orbiter data using ``sunpy.net.Fido``:
 
 .. code-block:: python
 
    # Importing sunpy_soar registers the client with sunpy
    import sunpy_soar
    from sunpy.net import Fido
    import sunpy.net.attrs as a
@@ -57,39 +56,42 @@
 
    # Download files
    files = Fido.fetch(result)
    print(files)
 
 Available search attributes
 ---------------------------
-The easiest way to access search attributes is using
-``import sunpy.net.attrs as a``. When constructing a search for SOAR ``a.Time`` must be
-provided. Other search attributes can be used too - ``sunpy-soar`` recognises the
-following:
+The easiest way to access search attributes is using ``import sunpy.net.attrs as a``.
+When constructing a search for SOAR ``a.Time`` must be provided.
+Other search attributes can be used too - ``sunpy-soar`` recognises the following:
 
 - ``a.Instrument``
 - ``a.Level`` - one of ``L0, L1, L2, L3, LL01, LL02, LL03``
 - ``a.soar.Product``
 
-The third ``near`` argument to ``a.Time`` is not currently supported - you will have to
-manually filter the results if you want to find the one closest to a given
-time.
+The third ``near`` argument to ``a.Time`` is not currently supported - you will have to manually filter the results if you want to find the one closest to a given time.
 
 ``sunpy-soar`` and the VSO
 ==========================
-``sunpy-soar`` queries the official repository of Solar Orbiter data, the SOAR. The Virtual Solar Observatory (VSO) as of writing (September 2022) mirrors a subset of the Solar Orbiter archive alongside many other solar physics data sources. The VSO allows data from multiple missions/observatories to be easily queried in one go, but users should be aware that the VSO is not the official repository for Solar Orbiter data and does not currently (as of September 2022) provide a comprehensive listing of all available Solar Orbiter data.
+``sunpy-soar`` queries the official repository of Solar Orbiter data, the SOAR.
+The Virtual Solar Observatory (VSO) as of writing (September 2022) mirrors a subset of the Solar Orbiter archive alongside many other solar physics data sources.
+The VSO allows data from multiple missions/observatories to be easily queried in one go, but users should be aware that the VSO is not the official repository for Solar Orbiter data and does not currently (as of September 2022) provide a comprehensive listing of all available Solar Orbiter data.
 
 Development
 ===========
 The SunPy developers maintain this package.
 Contributions for new features and bug fixes are welcome.
 
 Changelog
 =========
 
+1.7
+---
+- Added STIX data products to the list of valid data product identifiers.
+
 1.6
 ---
 - Registered a list of instruments available from the SOAR, with the ``a.Instrument`` attribute.
 - Registered the SOAR in the ``a.Provider`` attribute, meaning that a user can specifiy to the Fido search to only query the SOAR by use of ``a.Provider.soar``.
 - The ``_can_handle_query`` function within the SOARClient now checks to make sure if the SOAR supplies the queried data which fixes a bug which searched the SOAR for any data (e.g. AIA data).
 
 1.5
```

### Comparing `sunpy-soar-1.6.2/setup.cfg` & `sunpy-soar-1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.6.2/sunpy_soar/attrs.py` & `sunpy-soar-1.7/sunpy_soar/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.6.2/sunpy_soar/client.py` & `sunpy-soar-1.7/sunpy_soar/client.py`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.6.2/sunpy_soar/data/attrs.json` & `sunpy-soar-1.7/sunpy_soar/data/attrs.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8026315789473685%*

 * *Differences: {"'EUI-FSI174-IMAGE-DARK'": "''",*

 * * "'EUI-FSI174-IMAGE-OCCULTER'": "''",*

 * * "'EUI-FSI174-IMAGE-SHORT'": "''",*

 * * "'EUI-FSI304-IMAGE-DARK'": "''",*

 * * "'EUI-FSI304-IMAGE-LED'": "''",*

 * * "'EUI-FSI304-IMAGE-OCCULTER'": "''",*

 * * "'EUI-FSI304-IMAGE-SHORT'": "''",*

 * * "'EUI-FSIBLK-IMAGE-DARK'": "''",*

 * * "'EUI-FSIBLK-IMAGE-LED'": "''",*

 * * "'EUI-HRIEUV174-IMAGE-DARK'": "''",*

 * * "'EUI-HRIEUV174-IMAGE-LED'": "''",*

 * * "'EUI-HRIEUV174-IMAGE-SHORT'": "''",*

 * * "'EUI-HRIEUVBLK-IMAGE-DARK'": "''",*

 * * "'EUI-HRIEUVBLK-IMAGE-LED'": "''",*

 * * "'EUI-HRIEUVO […]*

```diff
@@ -55,21 +55,43 @@
     "EPD-STEP-MAIN-CLOSE": "Solar Orbiter, Level 1 Data, Energetic Particle Detector, SupraThermal Electrons and Protons, Main product close mode",
     "EPD-STEP-MAIN-FAR": "Solar Orbiter, Level 1 Data, Energetic Particle Detector, SupraThermal Electrons and Protons, Main product far mode",
     "EPD-STEP-NOM-CLOSE": "Solar Orbiter, Level 1 Data, Energetic Particle Detector, SupraThermal Electrons and Protons, Nominal product close mode",
     "EPD-STEP-NOM-FAR": "Solar Orbiter, Level 1 Data, Energetic Particle Detector, SupraThermal Electrons and Protons, Nominal product far mode",
     "EPD-STEP-QUICKLOOK": "Solar Orbiter, Level 1 Data, Energetic Particle Detector, SupraThermal Electrons and Protons, Quicklook product",
     "EPD-STEP-RATES": "Solar Orbiter, Level 2 Data, Energetic Particle Detector, SupraThermal Electrons and Protons, Rates",
     "EUI-FSI174-IMAGE": "",
+    "EUI-FSI174-IMAGE-DARK": "",
+    "EUI-FSI174-IMAGE-OCCULTER": "",
+    "EUI-FSI174-IMAGE-SHORT": "",
     "EUI-FSI304-IMAGE": "",
+    "EUI-FSI304-IMAGE-DARK": "",
+    "EUI-FSI304-IMAGE-LED": "",
+    "EUI-FSI304-IMAGE-OCCULTER": "",
+    "EUI-FSI304-IMAGE-SHORT": "",
     "EUI-FSIBLK-IMAGE": "",
+    "EUI-FSIBLK-IMAGE-DARK": "",
+    "EUI-FSIBLK-IMAGE-LED": "",
     "EUI-HRIEUV174-IMAGE": "",
+    "EUI-HRIEUV174-IMAGE-DARK": "",
+    "EUI-HRIEUV174-IMAGE-LED": "",
+    "EUI-HRIEUV174-IMAGE-SHORT": "",
     "EUI-HRIEUVBLK-IMAGE": "",
+    "EUI-HRIEUVBLK-IMAGE-DARK": "",
+    "EUI-HRIEUVBLK-IMAGE-LED": "",
     "EUI-HRIEUVNON-IMAGE": "",
+    "EUI-HRIEUVOPN-IMAGE": "",
+    "EUI-HRIEUVOPN-IMAGE-DARK": "",
+    "EUI-HRIEUVOPN-IMAGE-LED": "",
     "EUI-HRIEUVZER-IMAGE": "",
+    "EUI-HRIEUVZER-IMAGE-DARK": "",
+    "EUI-HRIEUVZER-IMAGE-LED": "",
+    "EUI-HRIEUVZER-IMAGE-SHORT": "",
     "EUI-HRILYA1216-IMAGE": "",
+    "EUI-HRILYA1216-IMAGE-DARK": "",
+    "EUI-HRILYA1216-IMAGE-LED": "",
     "MAG": "Solar Orbiter Level 2 Low Latency Magnetometer Data",
     "MAG-IBS": "Solar Orbiter Magnetometer L1 Data",
     "MAG-OBS": "Solar Orbiter Magnetometer L1 Data",
     "MAG-RTN": "Solar Orbiter Magnetometer L2 Data",
     "MAG-RTN DERIVED FROM LL DATA": "Solar Orbiter Magnetometer L2 Data derived from LL data",
     "MAG-RTN-BURST": "Solar Orbiter Magnetometer Level 2 Burst Mode Data in RTN coordinates",
     "MAG-RTN-NORMAL": "Solar Orbiter Magnetometer Level 2 Normal Mode Data in RTN coordinates",
@@ -91,14 +113,16 @@
     "PHI-HRT-BLOS": "",
     "PHI-HRT-BMAG": "",
     "PHI-HRT-ICNT": "",
     "PHI-HRT-STOKES": "",
     "PHI-HRT-VLOS": "",
     "RPW-BIA-DENSITY-10-SECONDS-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the spacecraft potential, downsampled",
     "RPW-BIA-DENSITY-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the spacecraft potential",
+    "RPW-BIA-EFIELD": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector",
+    "RPW-BIA-EFIELD-10-SECONDS": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector, downsampled",
     "RPW-BIA-EFIELD-10-SECONDS-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector, downsampled",
     "RPW-BIA-EFIELD-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector",
     "RPW-BIA-SCPOT-10-SECONDS-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential, downsampled",
     "RPW-BIA-SCPOT-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential",
     "RPW-HFR-SURV": "Solar Orbiter Radio/Plasma Wave, HFR L2 parameters",
     "RPW-LFR-SURV-ASM": "Solar Orbiter Radio/Plasma Wave, LFR L2 parameters",
     "RPW-LFR-SURV-BP1": "Solar Orbiter Radio/Plasma Wave, LFR L2 parameters",
@@ -143,18 +167,39 @@
     "SOLOHI-MAP1-3": "",
     "SOLOHI-MAP2-0": "",
     "SOLOHI-MAP3-0": "",
     "SOLOHI-MAP3-3": "",
     "SOLOHI-MAP4-0": "",
     "SPICE-N-EXP": "",
     "SPICE-N-RAS": "",
+    "SPICE-N-RAS-INT": "",
     "SPICE-N-SIT": "",
     "SPICE-W-EXP": "",
     "SPICE-W-RAS": "",
     "SPICE-W-SIT": "",
+    "STIX-CAL-ENERGY": "",
+    "STIX-HK-MAXI": "",
+    "STIX-HK-MINI": "",
+    "STIX-QL-BACKGROUND": "",
+    "STIX-QL-FLAREFLAG": "",
+    "STIX-QL-LIGHTCURVE": "",
+    "STIX-QL-SPECTRA": "",
+    "STIX-QL-VARIANCE": "",
+    "STIX-SCI-ASPECT-BURST": "",
+    "STIX-SCI-XRAY-CPD": "",
+    "STIX-SCI-XRAY-CPD-SUP1": "",
+    "STIX-SCI-XRAY-RPD": "",
+    "STIX-SCI-XRAY-RPD-SUP1": "",
+    "STIX-SCI-XRAY-SCPD": "",
+    "STIX-SCI-XRAY-SCPD-SUP1": "",
+    "STIX-SCI-XRAY-SPEC": "",
+    "STIX-SCI-XRAY-SPEC-SUP1": "",
+    "STIX-SCI-XRAY-SPEC-SUP2": "",
+    "STIX-SCI-XRAY-VIS": "",
+    "STIX-SCI-XRAY-VIS-SUP1": "",
     "SWA-EAS-PAD-DEF": "SWA-EAS 2D Burst Mode data",
     "SWA-EAS-PAD-DNF": "SWA-EAS 2D Burst Mode data",
     "SWA-EAS-PAD-PSD": "SWA-EAS 2D Burst Mode data",
     "SWA-EAS-PADC": "SWA-EAS Pitch Angle Counts data",
     "SWA-EAS-PARTMOMS": "SWA-EAS Partial Moments data",
     "SWA-EAS-SS": "SWA-EAS Low Latency LL02 Data",
     "SWA-EAS1-NM3D": "SWA-EAS1 Nominal Mode 3D data",
```

### Comparing `sunpy-soar-1.6.2/sunpy_soar/tests/test_sunpy_soar.py` & `sunpy-soar-1.7/sunpy_soar/tests/test_sunpy_soar.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     time = a.Time('2021-02-11', '2021-02-12')
     level = a.Level(1)
     product = a.soar.Product('EUI-FSI174-IMAGE')
 
     res = Fido.search(id, time, level, product)
     assert len(res) == 1
     assert len(res[0]) == 37
-    assert u.allclose(res[0, 0]['Filesize'], 3.574*u.Mbyte)
+    assert u.allclose(res[0, 0]['Filesize'], 3.47*u.Mbyte)
 
     files = Fido.fetch(res[0, 0])
     assert len(files) == 1
     fname = files[0]
     assert u.allclose(os.path.getsize(fname) * u.byte,
                       res[0, 0]['Filesize'], atol=1e-3*u.Mbyte)
     # Smoke test that we can read this into a map
@@ -78,15 +78,15 @@
     assert len(res) == 0
 
 
 def test_no_instrument():
     # Check that a time only search returns results
     time = a.Time('2020-04-16', '2020-04-17')
     res = SOARClient().search(time)
-    assert len(res) == 50
+    assert len(res) == 63
 
 
 def test_download_path(tmp_path):
     # Check that we can download things to a custom path using
     # the search parameters
     id = a.Instrument('EUI')
     time = a.Time('2021-02-01', '2021-02-02')
```

### Comparing `sunpy-soar-1.6.2/sunpy_soar.egg-info/PKG-INFO` & `sunpy-soar-1.7/sunpy_soar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy-soar
-Version: 1.6.2
+Version: 1.7
 Summary: A sunpy plugin for accessing data in the Solar Orbiter Archive (SOAR).
 Home-page: 
 Author: David Stansby
 Author-email: d.stansby@ucl.ac.uk
 License: BSD-2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -39,32 +39,31 @@
 
 
 When interacting with the sunpy-soar project you are asked to follow the `SunPy Code of Conduct <https://sunpy.org/coc>`_ .
 
 Installation
 ------------
 
-sunpy-soar requires `python >= 3.7` and `sunpy >= 2.1`. Currently it can only be installed from
-PyPI using:
+sunpy-soar requires `python >= 3.7` and `sunpy >= 2.1`.
+Currently it can only be installed from PyPI using:
 
 .. code-block:: bash
 
    pip install sunpy-soar
 
 or conda using
 
 .. code-block:: bash
 
    conda install -c conda-forge sunpy-soar
 
 Example usage
 -------------
 
-The code below gives an example of how to search and download Solar Orbiter
-data using ``sunpy.net.Fido``:
+The code below gives an example of how to search and download Solar Orbiter data using ``sunpy.net.Fido``:
 
 .. code-block:: python
 
    # Importing sunpy_soar registers the client with sunpy
    import sunpy_soar
    from sunpy.net import Fido
    import sunpy.net.attrs as a
@@ -81,39 +80,42 @@
 
    # Download files
    files = Fido.fetch(result)
    print(files)
 
 Available search attributes
 ---------------------------
-The easiest way to access search attributes is using
-``import sunpy.net.attrs as a``. When constructing a search for SOAR ``a.Time`` must be
-provided. Other search attributes can be used too - ``sunpy-soar`` recognises the
-following:
+The easiest way to access search attributes is using ``import sunpy.net.attrs as a``.
+When constructing a search for SOAR ``a.Time`` must be provided.
+Other search attributes can be used too - ``sunpy-soar`` recognises the following:
 
 - ``a.Instrument``
 - ``a.Level`` - one of ``L0, L1, L2, L3, LL01, LL02, LL03``
 - ``a.soar.Product``
 
-The third ``near`` argument to ``a.Time`` is not currently supported - you will have to
-manually filter the results if you want to find the one closest to a given
-time.
+The third ``near`` argument to ``a.Time`` is not currently supported - you will have to manually filter the results if you want to find the one closest to a given time.
 
 ``sunpy-soar`` and the VSO
 ==========================
-``sunpy-soar`` queries the official repository of Solar Orbiter data, the SOAR. The Virtual Solar Observatory (VSO) as of writing (September 2022) mirrors a subset of the Solar Orbiter archive alongside many other solar physics data sources. The VSO allows data from multiple missions/observatories to be easily queried in one go, but users should be aware that the VSO is not the official repository for Solar Orbiter data and does not currently (as of September 2022) provide a comprehensive listing of all available Solar Orbiter data.
+``sunpy-soar`` queries the official repository of Solar Orbiter data, the SOAR.
+The Virtual Solar Observatory (VSO) as of writing (September 2022) mirrors a subset of the Solar Orbiter archive alongside many other solar physics data sources.
+The VSO allows data from multiple missions/observatories to be easily queried in one go, but users should be aware that the VSO is not the official repository for Solar Orbiter data and does not currently (as of September 2022) provide a comprehensive listing of all available Solar Orbiter data.
 
 Development
 ===========
 The SunPy developers maintain this package.
 Contributions for new features and bug fixes are welcome.
 
 Changelog
 =========
 
+1.7
+---
+- Added STIX data products to the list of valid data product identifiers.
+
 1.6
 ---
 - Registered a list of instruments available from the SOAR, with the ``a.Instrument`` attribute.
 - Registered the SOAR in the ``a.Provider`` attribute, meaning that a user can specifiy to the Fido search to only query the SOAR by use of ``a.Provider.soar``.
 - The ``_can_handle_query`` function within the SOARClient now checks to make sure if the SOAR supplies the queried data which fixes a bug which searched the SOAR for any data (e.g. AIA data).
 
 1.5
```

### Comparing `sunpy-soar-1.6.2/sunpy_soar.egg-info/SOURCES.txt` & `sunpy-soar-1.7/sunpy_soar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.6.2/tools/update_data.py` & `sunpy-soar-1.7/tools/update_data.py`

 * *Files identical despite different names*

