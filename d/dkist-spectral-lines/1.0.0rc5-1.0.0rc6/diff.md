# Comparing `tmp/dkist-spectral-lines-1.0.0rc5.tar.gz` & `tmp/dkist-spectral-lines-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-spectral-lines-1.0.0rc5.tar", last modified: Wed Apr 12 18:55:05 2023, max compression
+gzip compressed data, was "dkist-spectral-lines-1.0.0rc6.tar", last modified: Thu Apr 13 16:08:11 2023, max compression
```

## Comparing `dkist-spectral-lines-1.0.0rc5.tar` & `dkist-spectral-lines-1.0.0rc6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2066 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.147088 dkist-spectral-lines-1.0.0rc5/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/changelog/1.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      643 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.147088 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5156 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/lines.py
--rw-rw-rw-   0 root         (0) root         (0)     1476 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/models.py
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/search.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.147088 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1416 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_lines.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3267 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_search.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.147088 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1136 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 16:08:11.627893 dkist-spectral-lines-1.0.0rc6/
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-04-13 16:08:11.627893 dkist-spectral-lines-1.0.0rc6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 16:08:11.623893 dkist-spectral-lines-1.0.0rc6/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/changelog/1.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      643 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 16:08:11.623893 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/search.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 16:08:11.623893 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/tests/test_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1912 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6114 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/tests/test_search.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 16:08:11.623893 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-04-13 16:08:11.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-13 16:08:11.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-13 16:08:11.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-04-13 16:08:11.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-13 16:08:11.000000 dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 16:08:11.627893 dkist-spectral-lines-1.0.0rc6/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 16:08:11.627893 dkist-spectral-lines-1.0.0rc6/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-04-13 16:08:11.627893 dkist-spectral-lines-1.0.0rc6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-13 16:08:06.000000 dkist-spectral-lines-1.0.0rc6/setup.py
```

### Comparing `dkist-spectral-lines-1.0.0rc5/.gitignore` & `dkist-spectral-lines-1.0.0rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/.pre-commit-config.yaml` & `dkist-spectral-lines-1.0.0rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/PKG-INFO` & `dkist-spectral-lines-1.0.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-spectral-lines
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Spectral line metadata for the DKIST suite of instruments
 Home-page: https://bitbucket.org/dkistdc/dkist-spectral-lines/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/spectral_lines
 Classifier: Programming Language :: Python
```

### Comparing `dkist-spectral-lines-1.0.0rc5/README.rst` & `dkist-spectral-lines-1.0.0rc6/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/bitbucket-pipelines.yml` & `dkist-spectral-lines-1.0.0rc6/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/check_changelog_updated.sh` & `dkist-spectral-lines-1.0.0rc6/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/lines.py` & `dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/lines.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,179 +1,185 @@
 """Spectral lines produced by DKIST instruments."""
+import astropy.units as u
+
 from dkist_spectral_lines.models import DiagnosticSpecies
 from dkist_spectral_lines.models import SpectralLine
 
 
-SPECTRAL_LINES = (
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.CA_II_K,
-        rest_wavelength_in_air=393.37,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.CA_II_H,
-        rest_wavelength_in_air=396.85,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.H_EPSILON,
-        rest_wavelength_in_air=397,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=404.58,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.H_DELTA,
-        rest_wavelength_in_air=410.17,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.CA_I,
-        rest_wavelength_in_air=422.67,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.H_GAMMA,
-        rest_wavelength_in_air=434.05,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.TI_I,
-        rest_wavelength_in_air=453.6,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.BA_II,
-        rest_wavelength_in_air=455.4,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.SR_I,
-        rest_wavelength_in_air=460.73,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.H_BETA,
-        rest_wavelength_in_air=486.13,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.MG_I_B1,
-        rest_wavelength_in_air=517.27,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.MG_I_B2,
-        rest_wavelength_in_air=518.36,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=525.04,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_XIV,
-        rest_wavelength_in_air=530.3,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.MN_I,
-        rest_wavelength_in_air=553.78,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=557.6,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.HE_I,
-        rest_wavelength_in_air=587.59,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.HE_I_D3,
-        rest_wavelength_in_air=587.6,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.NA_I_D2,
-        rest_wavelength_in_air=589,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.NA_I_D1,
-        rest_wavelength_in_air=589.59,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=617.33,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=630.15,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=630.25,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.H_ALPHA,
-        rest_wavelength_in_air=656.28,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.NI_I,
-        rest_wavelength_in_air=676.78,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=709,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.CA_I,
-        rest_wavelength_in_air=714.82,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=751.15,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.K_I,
-        rest_wavelength_in_air=769.9,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_XI,
-        rest_wavelength_in_air=789.2,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.NA_I,
-        rest_wavelength_in_air=818.33,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.NA_I,
-        rest_wavelength_in_air=819.48,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.CA_II,
-        rest_wavelength_in_air=849.81,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.CA_II,
-        rest_wavelength_in_air=854.21,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.CA_II,
-        rest_wavelength_in_air=866.22,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.MN_I,
-        rest_wavelength_in_air=874.1,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_XIII,
-        rest_wavelength_in_air=1074.7,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_XIII,
-        rest_wavelength_in_air=1079.8,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.HE_I,
-        rest_wavelength_in_air=1083,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.SI_X,
-        rest_wavelength_in_air=1430,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.FE_I,
-        rest_wavelength_in_air=1565,
-    ),
-    SpectralLine(
-        diagnostic_species=DiagnosticSpecies.SI_IX,
-        rest_wavelength_in_air=3934,
-    ),
+_SPECTRAL_LINES = sorted(
+    [
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.CA_II_K,
+            rest_wavelength_in_air=393.37 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.CA_II_H,
+            rest_wavelength_in_air=396.85 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.H_EPSILON,
+            rest_wavelength_in_air=397 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=404.58 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.H_DELTA,
+            rest_wavelength_in_air=410.17 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.CA_I,
+            rest_wavelength_in_air=422.67 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.H_GAMMA,
+            rest_wavelength_in_air=434.05 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.TI_I,
+            rest_wavelength_in_air=453.6 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.BA_II,
+            rest_wavelength_in_air=455.4 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.SR_I,
+            rest_wavelength_in_air=460.73 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.H_BETA,
+            rest_wavelength_in_air=486.13 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.MG_I_B1,
+            rest_wavelength_in_air=517.27 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.MG_I_B2,
+            rest_wavelength_in_air=518.36 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=525.04 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_XIV,
+            rest_wavelength_in_air=530.3 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.MN_I,
+            rest_wavelength_in_air=553.78 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=557.6 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.HE_I,
+            rest_wavelength_in_air=587.59 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.HE_I_D3,
+            rest_wavelength_in_air=587.6 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.NA_I_D2,
+            rest_wavelength_in_air=589 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.NA_I_D1,
+            rest_wavelength_in_air=589.59 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=617.33 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=630.15 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=630.25 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.H_ALPHA,
+            rest_wavelength_in_air=656.28 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.NI_I,
+            rest_wavelength_in_air=676.78 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=709 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.CA_I,
+            rest_wavelength_in_air=714.82 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=751.15 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.K_I,
+            rest_wavelength_in_air=769.9 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_XI,
+            rest_wavelength_in_air=789.2 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.NA_I,
+            rest_wavelength_in_air=818.33 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.NA_I,
+            rest_wavelength_in_air=819.48 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.CA_II,
+            rest_wavelength_in_air=849.81 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.CA_II,
+            rest_wavelength_in_air=854.21 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.CA_II,
+            rest_wavelength_in_air=866.22 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.MN_I,
+            rest_wavelength_in_air=874.1 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_XIII,
+            rest_wavelength_in_air=1074.7 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_XIII,
+            rest_wavelength_in_air=1079.8 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.HE_I,
+            rest_wavelength_in_air=1083 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.SI_X,
+            rest_wavelength_in_air=1430 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.FE_I,
+            rest_wavelength_in_air=1565 * u.nm,
+        ),
+        SpectralLine(
+            diagnostic_species=DiagnosticSpecies.SI_IX,
+            rest_wavelength_in_air=3934 * u.nm,
+        ),
+    ]
 )
+
+SPECTRAL_LINES = tuple(_SPECTRAL_LINES)
```

### Comparing `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/search.py` & `dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 """Search for spectral lines."""
+import astropy.units as u
+
 from dkist_spectral_lines.lines import SPECTRAL_LINES
 from dkist_spectral_lines.models import SpectralLine
 
 
-def get_spectral_lines(wavelength_min: float, wavelength_max: float) -> list[SpectralLine]:
-    """Get all spectral lines found in the wavelength range inclusive of the extremes."""
+def _to_nanometers(wavelength: float | u.Quantity) -> u.Quantity:
+    if not isinstance(wavelength, u.Quantity):
+        return wavelength * u.nm
+    return wavelength.to(u.nm)
+
+
+def get_spectral_lines(
+    wavelength_min: float | u.Quantity, wavelength_max: float | u.Quantity
+) -> list[SpectralLine]:
+    """Get all spectral lines found in the wavelength range inclusive of the extremes.  Wavelengths are assumed to be in nm unless specified otherwise as a astropy.units.Quantity."""
+    wavelength_min = _to_nanometers(wavelength_min)
+    wavelength_max = _to_nanometers(wavelength_max)
+
     result = [
         line
         for line in SPECTRAL_LINES
         if wavelength_min <= line.rest_wavelength_in_air <= wavelength_max
     ]
     return result
 
 
-def get_closest_spectral_line(wavelength: float) -> SpectralLine:
+def get_closest_spectral_line(wavelength: float | u.Quantity) -> SpectralLine:
     """Get the spectral line that is closest to reference wavelength."""
+    wavelength = _to_nanometers(wavelength)
     return min(SPECTRAL_LINES, key=lambda x: abs(x.rest_wavelength_in_air - wavelength))
```

### Comparing `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_lines.py` & `dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_models.py` & `dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines/tests/test_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 """Tests for the SpectralLine data structure and validation"""
 import random
 
+import astropy.units as u
 import pytest
+from astropy.units import Unit
 from pydantic import ValidationError
 
 from dkist_spectral_lines.lines import DiagnosticSpecies
 from dkist_spectral_lines.models import SpectralLine
 
 
+@pytest.mark.parametrize("unit", [u.nm, u.angstrom])
 @pytest.mark.parametrize("diagnostic_species", [l for l in DiagnosticSpecies])
-def test_spectral_line_valid(diagnostic_species):
+def test_spectral_line_valid(diagnostic_species, unit):
     """
     :Given: Diagnostic species and wavelength
     :When: Instantiating a SpectralLine
     :Then: Instance created and name property renders
     """
     # Given
-    wavelength = random.random() * 100
+    wavelength = random.random() * 100 * unit
     # When
     spectral_line = SpectralLine(
         diagnostic_species=diagnostic_species, rest_wavelength_in_air=wavelength
     )
     # Then
     assert spectral_line.name
+    assert spectral_line.rest_wavelength_in_air.unit == Unit("nm")
 
 
 @pytest.mark.parametrize(
     "diagnostic_species, wavelength",
     [
-        pytest.param("bad line", 1.1, id="diagnostic_species"),
+        pytest.param("bad line", 1.1 * u.nm, id="diagnostic_species"),
         pytest.param(DiagnosticSpecies.CA_I, "a", id="wavelength"),
+        pytest.param(DiagnosticSpecies.CA_I, 1.1, id="wavelength_no_units"),
         pytest.param("bad line", "a", id="diagnostic_species_and_wavelength"),
-        pytest.param(None, 1.1, id="diagnostic_species_required"),
+        pytest.param(None, 1.1 * u.nm, id="diagnostic_species_required"),
         pytest.param(DiagnosticSpecies.CA_I, None, id="wavelength_required"),
+        pytest.param(DiagnosticSpecies.CA_I, 1.1 * u.s, id="wavelength_wrong_units"),
     ],
 )
 def test_spectral_line_invalid(diagnostic_species, wavelength):
     """
     :Given: Invalid diagnostic species and/or wavelength
     :When: Instantiating a SpectralLine
     :Then: Pydantic Validation error raised
```

### Comparing `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/PKG-INFO` & `dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-spectral-lines
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Spectral line metadata for the DKIST suite of instruments
 Home-page: https://bitbucket.org/dkistdc/dkist-spectral-lines/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/spectral_lines
 Classifier: Programming Language :: Python
```

### Comparing `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/SOURCES.txt` & `dkist-spectral-lines-1.0.0rc6/dkist_spectral_lines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/docs/Makefile` & `dkist-spectral-lines-1.0.0rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/docs/conf.py` & `dkist-spectral-lines-1.0.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/docs/make.bat` & `dkist-spectral-lines-1.0.0rc6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/licenses/LICENSE.rst` & `dkist-spectral-lines-1.0.0rc6/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/pyproject.toml` & `dkist-spectral-lines-1.0.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc5/setup.cfg` & `dkist-spectral-lines-1.0.0rc6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
 	pydantic
+	astropy
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	pytest-mock
 	towncrier
```

