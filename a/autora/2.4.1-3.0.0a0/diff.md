# Comparing `tmp/autora-2.4.1.tar.gz` & `tmp/autora-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-2.4.1.tar", max compression
+gzip compressed data, was "autora-3.0.0a0.tar", max compression
```

## Comparing `autora-2.4.1.tar` & `autora-3.0.0a0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1100 2023-04-07 16:00:32.253006 autora-2.4.1/LICENSE.md
--rw-r--r--   0        0        0    18724 2023-04-07 16:00:32.253006 autora-2.4.1/README.md
--rw-r--r--   0        0        0      173 2023-04-07 16:00:32.253006 autora-2.4.1/autora/__init__.py
--rw-r--r--   0        0        0      197 2023-04-07 16:00:32.253006 autora-2.4.1/autora/cycle/__init__.py
--rw-r--r--   0        0        0    20784 2023-04-07 16:00:32.253006 autora-2.4.1/autora/cycle/plot_utils.py
--rw-r--r--   0        0        0    21619 2023-04-07 16:00:32.253006 autora-2.4.1/autora/cycle/simple.py
--rw-r--r--   0        0        0        0 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/__init__.py
--rw-r--r--   0        0        0     5014 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/filter.py
--rw-r--r--   0        0        0    18310 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/pipeline.py
--rw-r--r--   0        0        0       87 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/pooler/__init__.py
--rw-r--r--   0        0        0     1800 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/pooler/general_pool.py
--rw-r--r--   0        0        0    13496 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/pooler/poppernet.py
--rw-r--r--   0        0        0      232 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/sampler/__init__.py
--rw-r--r--   0        0        0     2383 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/sampler/assumption.py
--rw-r--r--   0        0        0     2841 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/sampler/dissimilarity.py
--rw-r--r--   0        0        0     2216 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/sampler/model_disagreement.py
--rw-r--r--   0        0        0     1666 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/sampler/nearest_value.py
--rw-r--r--   0        0        0      497 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/sampler/random.py
--rw-r--r--   0        0        0     2052 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/sampler/uncertainty.py
--rw-r--r--   0        0        0     4586 2023-04-07 16:00:32.253006 autora-2.4.1/autora/experimentalist/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 16:00:32.253006 autora-2.4.1/autora/skl/__init__.py
--rw-r--r--   0        0        0     6087 2023-04-07 16:00:32.253006 autora-2.4.1/autora/skl/bms.py
--rw-r--r--   0        0        0    12781 2023-04-07 16:00:32.253006 autora-2.4.1/autora/skl/bsr.py
--rw-r--r--   0        0        0    31115 2023-04-07 16:00:32.253006 autora-2.4.1/autora/skl/darts.py
--rw-r--r--   0        0        0     2649 2023-04-07 16:00:32.253006 autora-2.4.1/autora/synthetic/__init__.py
--rw-r--r--   0        0        0       97 2023-04-07 16:00:32.253006 autora-2.4.1/autora/synthetic/data/__init__.py
--rw-r--r--   0        0        0     5123 2023-04-07 16:00:32.253006 autora-2.4.1/autora/synthetic/data/expected_value.py
--rw-r--r--   0        0        0     6631 2023-04-07 16:00:32.253006 autora-2.4.1/autora/synthetic/data/prospect_theory.py
--rw-r--r--   0        0        0     4587 2023-04-07 16:00:32.253006 autora-2.4.1/autora/synthetic/data/weber_fechner.py
--rw-r--r--   0        0        0     7338 2023-04-07 16:00:32.253006 autora-2.4.1/autora/synthetic/inventory.py
--rw-r--r--   0        0        0        0 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/__init__.py
--rw-r--r--   0        0        0      126 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/__init__.py
--rw-r--r--   0        0        0      164 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/data/named_equations.wiki.parsed__num_operations.dat
--rw-r--r--   0        0        0      130 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/data/named_equations.wiki.parsed__operation_type.dat
--rw-r--r--   0        0        0      133 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/data/named_equations.wiki.parsed__operation_type_sq.dat
--rw-r--r--   0        0        0     8599 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/fit_prior.py
--rw-r--r--   0        0        0    60372 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/mcmc.py
--rw-r--r--   0        0        0     5726 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/parallel.py
--rw-r--r--   0        0        0     2341 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/prior.py
--rwxr-xr-x   0        0        0     2860 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bms/utils.py
--rw-r--r--   0        0        0        0 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bsr/__init__.py
--rw-r--r--   0        0        0    32217 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bsr/funcs.py
--rw-r--r--   0        0        0     1430 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bsr/misc.py
--rw-r--r--   0        0        0     6521 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bsr/node.py
--rw-r--r--   0        0        0     2117 2023-04-07 16:00:32.253006 autora-2.4.1/autora/theorist/bsr/operation.py
--rw-r--r--   0        0        0     5114 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/bsr/prior.py
--rw-r--r--   0        0        0      347 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/__init__.py
--rwxr-xr-x   0        0        0    12774 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/architect.py
--rw-r--r--   0        0        0     1791 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/dataset.py
--rw-r--r--   0        0        0     1301 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/fan_out.py
--rwxr-xr-x   0        0        0    30660 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/model_search.py
--rwxr-xr-x   0        0        0    19820 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/operations.py
--rwxr-xr-x   0        0        0    41286 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/plot_utils.py
--rwxr-xr-x   0        0        0    13517 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/utils.py
--rwxr-xr-x   0        0        0     6645 2023-04-07 16:00:32.257007 autora-2.4.1/autora/theorist/darts/visualize.py
--rw-r--r--   0        0        0       25 2023-04-07 16:00:32.257007 autora-2.4.1/autora/utils/__init__.py
--rw-r--r--   0        0        0      441 2023-04-07 16:00:32.257007 autora-2.4.1/autora/utils/dictionary.py
--rw-r--r--   0        0        0     1866 2023-04-07 16:00:32.257007 autora-2.4.1/autora/variable/__init__.py
--rw-r--r--   0        0        0     2511 2023-04-07 16:00:32.257007 autora-2.4.1/autora/variable/time.py
--rw-r--r--   0        0        0     8899 2023-04-07 16:00:32.257007 autora-2.4.1/autora/variable/tinkerforge.py
--rw-r--r--   0        0        0     1810 2023-04-07 16:02:58.655477 autora-2.4.1/pyproject.toml
--rw-r--r--   0        0        0    20200 1970-01-01 00:00:00.000000 autora-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-04-14 15:50:00.492529 autora-3.0.0a0/LICENSE.md
+-rw-r--r--   0        0        0    18722 2023-04-14 15:50:00.492529 autora-3.0.0a0/README.md
+-rw-r--r--   0        0        0      173 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/cycle/__init__.py
+-rw-r--r--   0        0        0    20784 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/cycle/plot_utils.py
+-rw-r--r--   0        0        0    21619 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/cycle/simple.py
+-rw-r--r--   0        0        0        0 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/experimentalist/__init__.py
+-rw-r--r--   0        0        0     5014 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/experimentalist/filter.py
+-rw-r--r--   0        0        0    18310 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/experimentalist/pipeline.py
+-rw-r--r--   0        0        0       87 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/pooler/__init__.py
+-rw-r--r--   0        0        0     1800 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/pooler/general_pool.py
+-rw-r--r--   0        0        0    13496 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/pooler/poppernet.py
+-rw-r--r--   0        0        0      232 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/__init__.py
+-rw-r--r--   0        0        0     2383 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/assumption.py
+-rw-r--r--   0        0        0     2841 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/dissimilarity.py
+-rw-r--r--   0        0        0     2216 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/model_disagreement.py
+-rw-r--r--   0        0        0     1666 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/nearest_value.py
+-rw-r--r--   0        0        0      497 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/random.py
+-rw-r--r--   0        0        0     2052 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/uncertainty.py
+-rw-r--r--   0        0        0     4586 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/skl/__init__.py
+-rw-r--r--   0        0        0     6087 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/skl/bms.py
+-rw-r--r--   0        0        0    12781 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/skl/bsr.py
+-rw-r--r--   0        0        0    31115 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/skl/darts.py
+-rw-r--r--   0        0        0     2649 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/__init__.py
+-rw-r--r--   0        0        0       97 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/data/__init__.py
+-rw-r--r--   0        0        0     5123 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/data/expected_value.py
+-rw-r--r--   0        0        0     6631 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/data/prospect_theory.py
+-rw-r--r--   0        0        0     4587 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/data/weber_fechner.py
+-rw-r--r--   0        0        0     7338 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/inventory.py
+-rw-r--r--   0        0        0        0 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/__init__.py
+-rw-r--r--   0        0        0      126 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/data/named_equations.wiki.parsed__num_operations.dat
+-rw-r--r--   0        0        0      130 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/data/named_equations.wiki.parsed__operation_type.dat
+-rw-r--r--   0        0        0      133 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/data/named_equations.wiki.parsed__operation_type_sq.dat
+-rw-r--r--   0        0        0     8599 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/fit_prior.py
+-rw-r--r--   0        0        0    60372 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/mcmc.py
+-rw-r--r--   0        0        0     5726 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/parallel.py
+-rw-r--r--   0        0        0     2341 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/prior.py
+-rwxr-xr-x   0        0        0     2860 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/utils.py
+-rw-r--r--   0        0        0        0 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/__init__.py
+-rw-r--r--   0        0        0    32217 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/funcs.py
+-rw-r--r--   0        0        0     1430 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/misc.py
+-rw-r--r--   0        0        0     6521 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/node.py
+-rw-r--r--   0        0        0     2117 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/operation.py
+-rw-r--r--   0        0        0     5114 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/prior.py
+-rw-r--r--   0        0        0      347 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/__init__.py
+-rwxr-xr-x   0        0        0    12774 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/architect.py
+-rw-r--r--   0        0        0     1791 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/dataset.py
+-rw-r--r--   0        0        0     1301 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/fan_out.py
+-rwxr-xr-x   0        0        0    30660 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/model_search.py
+-rwxr-xr-x   0        0        0    19820 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/operations.py
+-rwxr-xr-x   0        0        0    41286 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/plot_utils.py
+-rwxr-xr-x   0        0        0    13517 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/utils.py
+-rwxr-xr-x   0        0        0     6645 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/visualize.py
+-rw-r--r--   0        0        0       25 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/utils/__init__.py
+-rw-r--r--   0        0        0      441 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/utils/dictionary.py
+-rw-r--r--   0        0        0     1866 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/variable/__init__.py
+-rw-r--r--   0        0        0     2511 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/variable/time.py
+-rw-r--r--   0        0        0     8899 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/variable/tinkerforge.py
+-rw-r--r--   0        0        0     1812 2023-04-14 15:52:10.495893 autora-3.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0    20200 1970-01-01 00:00:00.000000 autora-3.0.0a0/PKG-INFO
```

### Comparing `autora-2.4.1/LICENSE.md` & `autora-3.0.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/README.md` & `autora-3.0.0a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Autonomous Research Assistant
-Autonomous Research Assistant (AutoRA) is an open source AI-based system for automating each aspect of empirical research in the behavioral sciences, from the construction of a scientific hypothesis to conducting novel experiments. The documentation is here: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
+# Automated Research Assistant
+Automated Research Assistant (AutoRA) is an open source AI-based system for automating each aspect of empirical research in the behavioral sciences, from the construction of a scientific hypothesis to conducting novel experiments. The documentation is here: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 # Getting started
 
 You should be familiar with the command line for your operating system. The topics required are covered in:
 - **macOS**: Joe Kissell. [*Take Control of the Mac Command Line with Terminal, 3rd Edition*](https://bruknow.library.brown.edu/permalink/01BU_INST/528fgv/cdi_safari_books_v2_9781947282513). Take Control Books, 2022. Chapters *Read Me First* through *Bring the Command Line Into The Real World*.
 - **Linux**: William E. Shotts. [*The Linux Command Line: a Complete Introduction. 2nd edition.*](https://bruknow.library.brown.edu/permalink/01BU_INST/9mvq88/alma991043239704906966). No Starch Press, 2019. Parts *I: Learning the Shell* and *II: Configuration and the Environment*.
```

### Comparing `autora-2.4.1/autora/cycle/plot_utils.py` & `autora-3.0.0a0/autora/cycle/plot_utils.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/cycle/simple.py` & `autora-3.0.0a0/autora/cycle/simple.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/filter.py` & `autora-3.0.0a0/autora/experimentalist/filter.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/pipeline.py` & `autora-3.0.0a0/autora/experimentalist/pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/pooler/general_pool.py` & `autora-3.0.0a0/autora/experimentalist/pooler/general_pool.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/pooler/poppernet.py` & `autora-3.0.0a0/autora/experimentalist/pooler/poppernet.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/sampler/assumption.py` & `autora-3.0.0a0/autora/experimentalist/sampler/assumption.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/sampler/dissimilarity.py` & `autora-3.0.0a0/autora/experimentalist/sampler/dissimilarity.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/sampler/model_disagreement.py` & `autora-3.0.0a0/autora/experimentalist/sampler/model_disagreement.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/sampler/nearest_value.py` & `autora-3.0.0a0/autora/experimentalist/sampler/nearest_value.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/sampler/uncertainty.py` & `autora-3.0.0a0/autora/experimentalist/sampler/uncertainty.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/experimentalist/utils/__init__.py` & `autora-3.0.0a0/autora/experimentalist/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/skl/bms.py` & `autora-3.0.0a0/autora/skl/bms.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/skl/bsr.py` & `autora-3.0.0a0/autora/skl/bsr.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/skl/darts.py` & `autora-3.0.0a0/autora/skl/darts.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/synthetic/__init__.py` & `autora-3.0.0a0/autora/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/synthetic/data/expected_value.py` & `autora-3.0.0a0/autora/synthetic/data/expected_value.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/synthetic/data/prospect_theory.py` & `autora-3.0.0a0/autora/synthetic/data/prospect_theory.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/synthetic/data/weber_fechner.py` & `autora-3.0.0a0/autora/synthetic/data/weber_fechner.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/synthetic/inventory.py` & `autora-3.0.0a0/autora/synthetic/inventory.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bms/fit_prior.py` & `autora-3.0.0a0/autora/theorist/bms/fit_prior.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bms/mcmc.py` & `autora-3.0.0a0/autora/theorist/bms/mcmc.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bms/parallel.py` & `autora-3.0.0a0/autora/theorist/bms/parallel.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bms/prior.py` & `autora-3.0.0a0/autora/theorist/bms/prior.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bms/utils.py` & `autora-3.0.0a0/autora/theorist/bms/utils.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bsr/funcs.py` & `autora-3.0.0a0/autora/theorist/bsr/funcs.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bsr/misc.py` & `autora-3.0.0a0/autora/theorist/bsr/misc.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bsr/node.py` & `autora-3.0.0a0/autora/theorist/bsr/node.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bsr/operation.py` & `autora-3.0.0a0/autora/theorist/bsr/operation.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/bsr/prior.py` & `autora-3.0.0a0/autora/theorist/bsr/prior.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/darts/architect.py` & `autora-3.0.0a0/autora/theorist/darts/architect.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/darts/dataset.py` & `autora-3.0.0a0/autora/theorist/darts/dataset.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/darts/fan_out.py` & `autora-3.0.0a0/autora/theorist/darts/fan_out.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/darts/model_search.py` & `autora-3.0.0a0/autora/theorist/darts/model_search.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/darts/operations.py` & `autora-3.0.0a0/autora/theorist/darts/operations.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/darts/plot_utils.py` & `autora-3.0.0a0/autora/theorist/darts/plot_utils.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/darts/utils.py` & `autora-3.0.0a0/autora/theorist/darts/utils.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/theorist/darts/visualize.py` & `autora-3.0.0a0/autora/theorist/darts/visualize.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/variable/__init__.py` & `autora-3.0.0a0/autora/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/variable/time.py` & `autora-3.0.0a0/autora/variable/time.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/autora/variable/tinkerforge.py` & `autora-3.0.0a0/autora/variable/tinkerforge.py`

 * *Files identical despite different names*

### Comparing `autora-2.4.1/pyproject.toml` & `autora-3.0.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autora"
-version = "v2.4.1"
+version = "v3.0.0a0"
 description = "Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. This framework implements tools for autonomously and iteratively generating 1) new theories to describe real-world data, and 2) experiments to invalidate those theories and seed a new cycle of theory-making. The experiments will be run online via crowd-sourcing platforms (MTurk, Prolific)."
 authors = [
     "Sebastian Musslick <sebastian_musslick@brown.edu>",
     "John Gerrard Holland <john_holland1@brown.edu>",
 ]
 readme = "README.md"
 homepage = "https://musslick.github.io/AER_website/Research.html"
```

### Comparing `autora-2.4.1/PKG-INFO` & `autora-3.0.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 2.4.1
+Version: 3.0.0a0
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. This framework implements tools for autonomously and iteratively generating 1) new theories to describe real-world data, and 2) experiments to invalidate those theories and seed a new cycle of theory-making. The experiments will be run online via crowd-sourcing platforms (MTurk, Prolific).
 Home-page: https://musslick.github.io/AER_website/Research.html
 Author: Sebastian Musslick
 Author-email: sebastian_musslick@brown.edu
 Requires-Python: >=3.8.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -22,16 +22,16 @@
 Requires-Dist: tinkerforge (>=2.1.25,<3.0.0) ; extra == "tinkerforge"
 Requires-Dist: torch (==2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Project-URL: Documentation, https://autoresearch.github.io/autora/
 Project-URL: Repository, https://github.com/AutoResearch/autora
 Description-Content-Type: text/markdown
 
-# Autonomous Research Assistant
-Autonomous Research Assistant (AutoRA) is an open source AI-based system for automating each aspect of empirical research in the behavioral sciences, from the construction of a scientific hypothesis to conducting novel experiments. The documentation is here: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
+# Automated Research Assistant
+Automated Research Assistant (AutoRA) is an open source AI-based system for automating each aspect of empirical research in the behavioral sciences, from the construction of a scientific hypothesis to conducting novel experiments. The documentation is here: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 # Getting started
 
 You should be familiar with the command line for your operating system. The topics required are covered in:
 - **macOS**: Joe Kissell. [*Take Control of the Mac Command Line with Terminal, 3rd Edition*](https://bruknow.library.brown.edu/permalink/01BU_INST/528fgv/cdi_safari_books_v2_9781947282513). Take Control Books, 2022. Chapters *Read Me First* through *Bring the Command Line Into The Real World*.
 - **Linux**: William E. Shotts. [*The Linux Command Line: a Complete Introduction. 2nd edition.*](https://bruknow.library.brown.edu/permalink/01BU_INST/9mvq88/alma991043239704906966). No Starch Press, 2019. Parts *I: Learning the Shell* and *II: Configuration and the Environment*.
```

