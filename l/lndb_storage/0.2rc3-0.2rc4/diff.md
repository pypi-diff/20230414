# Comparing `tmp/lndb_storage-0.2rc3.tar.gz` & `tmp/lndb_storage-0.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb_storage-0.2rc3.tar", last modified: Sun Apr  9 22:17:27 2023, max compression
+gzip compressed data, was "lndb_storage-0.2rc4.tar", last modified: Fri Apr 14 10:46:22 2023, max compression
```

## Comparing `lndb_storage-0.2rc3.tar` & `lndb_storage-0.2rc4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2961 2023-03-29 20:45:21.388257 lndb_storage-0.2rc3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.2rc3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.2rc3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.2rc3/.gitignore
--rw-r--r--   0        0        0     1758 2023-03-29 20:45:21.388537 lndb_storage-0.2rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.2rc3/LICENSE
--rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.2rc3/README.md
--rw-r--r--   0        0        0     1884 2023-04-09 22:16:50.608709 lndb_storage-0.2rc3/docs/changelog.md
--rw-r--r--   0        0        0     3283 2023-04-09 22:15:42.448966 lndb_storage-0.2rc3/docs/guide/add-replace-stage.ipynb
--rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.2rc3/docs/guide/index.md
--rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.2rc3/docs/guide/iris.csv
--rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.2rc3/docs/guide/iris.data
--rw-r--r--   0        0        0     4615 2023-04-09 22:14:23.875491 lndb_storage-0.2rc3/docs/guide/serialize-cache.ipynb
--rw-r--r--   0        0        0     7035 2023-04-09 22:14:23.875871 lndb_storage-0.2rc3/docs/guide/stream.ipynb
--rw-r--r--   0        0        0     7566 2023-04-09 22:14:23.876185 lndb_storage-0.2rc3/docs/guide/upload.ipynb
--rw-r--r--   0        0        0      593 2023-04-09 20:42:44.949159 lndb_storage-0.2rc3/docs/index.md
--rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.2rc3/docs/reference.md
--rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.2rc3/lamin-project.yaml
--rw-r--r--   0        0        0      580 2023-04-09 22:16:33.330050 lndb_storage-0.2rc3/lndb_storage/__init__.py
--rw-r--r--   0        0        0     3300 2023-04-09 20:42:44.949890 lndb_storage-0.2rc3/lndb_storage/_file.py
--rw-r--r--   0        0        0      497 2023-04-09 20:42:44.950134 lndb_storage-0.2rc3/lndb_storage/_h5ad.py
--rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.2rc3/lndb_storage/_images.py
--rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.2rc3/lndb_storage/_subset.py
--rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.2rc3/lndb_storage/_zarr.py
--rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.2rc3/lndb_storage/object/__init__.py
--rw-r--r--   0        0        0      950 2023-03-29 20:45:21.391028 lndb_storage-0.2rc3/lndb_storage/object/_anndata.py
--rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.2rc3/lndb_storage/object/_anndata_sizes.py
--rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.2rc3/lndb_storage/object/_core.py
--rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.2rc3/lndb_storage/object/_lazy_field.py
--rw-r--r--   0        0        0     3507 2023-04-09 20:42:44.950762 lndb_storage-0.2rc3/lndb_storage/object/_subset_anndata.py
--rw-r--r--   0        0        0      913 2023-04-09 22:16:03.478614 lndb_storage-0.2rc3/noxfile.py
--rw-r--r--   0        0        0     1044 2023-04-09 20:42:44.951084 lndb_storage-0.2rc3/pyproject.toml
--rw-r--r--   0        0        0      490 2023-03-29 20:45:21.391918 lndb_storage-0.2rc3/tests/test_notebooks.py
--rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 lndb_storage-0.2rc3/PKG-INFO
+-rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.2rc4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.2rc4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.2rc4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.2rc4/.gitignore
+-rw-r--r--   0        0        0     1758 2023-03-29 20:45:21.388537 lndb_storage-0.2rc4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.2rc4/LICENSE
+-rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.2rc4/README.md
+-rw-r--r--   0        0        0     2039 2023-04-14 10:46:01.815237 lndb_storage-0.2rc4/docs/changelog.md
+-rw-r--r--   0        0        0     3283 2023-04-09 22:15:42.448966 lndb_storage-0.2rc4/docs/guide/add-replace-stage.ipynb
+-rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.2rc4/docs/guide/index.md
+-rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.2rc4/docs/guide/iris.csv
+-rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.2rc4/docs/guide/iris.data
+-rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.2rc4/docs/guide/serialize-cache.ipynb
+-rw-r--r--   0        0        0     7035 2023-04-09 22:14:23.875871 lndb_storage-0.2rc4/docs/guide/stream.ipynb
+-rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.2rc4/docs/guide/upload.ipynb
+-rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.2rc4/docs/index.md
+-rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.2rc4/docs/reference.md
+-rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.2rc4/lamin-project.yaml
+-rw-r--r--   0        0        0      580 2023-04-14 10:45:33.547174 lndb_storage-0.2rc4/lndb_storage/__init__.py
+-rw-r--r--   0        0        0     3317 2023-04-14 10:44:40.713660 lndb_storage-0.2rc4/lndb_storage/_file.py
+-rw-r--r--   0        0        0      497 2023-04-09 20:42:44.950134 lndb_storage-0.2rc4/lndb_storage/_h5ad.py
+-rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.2rc4/lndb_storage/_images.py
+-rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.2rc4/lndb_storage/_subset.py
+-rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.2rc4/lndb_storage/_zarr.py
+-rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.2rc4/lndb_storage/object/__init__.py
+-rw-r--r--   0        0        0      950 2023-03-29 20:45:21.391028 lndb_storage-0.2rc4/lndb_storage/object/_anndata.py
+-rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.2rc4/lndb_storage/object/_anndata_sizes.py
+-rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.2rc4/lndb_storage/object/_core.py
+-rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.2rc4/lndb_storage/object/_lazy_field.py
+-rw-r--r--   0        0        0     3507 2023-04-09 20:42:44.950762 lndb_storage-0.2rc4/lndb_storage/object/_subset_anndata.py
+-rw-r--r--   0        0        0      913 2023-04-09 22:16:03.478614 lndb_storage-0.2rc4/noxfile.py
+-rw-r--r--   0        0        0     1044 2023-04-09 20:42:44.951084 lndb_storage-0.2rc4/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-03-29 20:45:21.391918 lndb_storage-0.2rc4/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 lndb_storage-0.2rc4/PKG-INFO
```

### Comparing `lndb_storage-0.2rc3/.github/workflows/build.yml` & `lndb_storage-0.2rc4/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,19 @@
         uses: actions/checkout@v3
         with:
           repository: laminlabs/lndocs
           ssh-key: ${{ secrets.READ_LNDOCS }}
           path: lndocs
           ref: main
       - name: Setup Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml" # See dependencies below
       - name: Cache nox
         uses: actions/cache@v3
         with:
           path: .nox
           key: nox-${{ runner.os }}
       - name: Cache pre-commit
         uses: actions/cache@v3
@@ -51,21 +53,24 @@
           key: cache-postgres-0
       - name: Cache postgres miss
         if: steps.cache-postgres.outputs.cache-hit != 'true'
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
       - name: Cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
-      - name: Install dependencies
+      - name: Install Python dependencies
         run: |
           python -m pip install -U pip
           pip install -U laminci
-          pip install lamindb
+          pip install -U lamindb
+      - name: Install apt-get dependencies
+        run: |
           sudo apt-get -y install graphviz
           sudo apt-get install sqlite3-tools=3.37.2-2
+          sudo apt-get install libpq-dev
       - name: Configure AWS
         uses: aws-actions/configure-aws-credentials@v1
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       - name: Lint
```

### Comparing `lndb_storage-0.2rc3/.github/workflows/latest-changes.yml` & `lndb_storage-0.2rc4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/.gitignore` & `lndb_storage-0.2rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/.pre-commit-config.yaml` & `lndb_storage-0.2rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/LICENSE` & `lndb_storage-0.2rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/docs/changelog.md` & `lndb_storage-0.2rc4/docs/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Remove call to nbproject in progress bar | [18](https://github.com/laminlabs/lndb-storage/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-04-14 | 0.2rc4
 ✅ Introduce separate upload guide | [14](https://github.com/laminlabs/lndb-storage/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 | 0.2rc3
 💚 Attempt fix CI | [12](https://github.com/laminlabs/lndb-storage/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 |
 🚚 Move `UPath` back to `lndb` | [11](https://github.com/laminlabs/lndb-storage/pull/11) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 |
 ✅ Add test for replace and stage | [10](https://github.com/laminlabs/lndb-storage/pull/10) | [Koncopd](https://github.com/Koncopd) | 2023-04-04 |
 ➕ Add upath to deps | [9](https://github.com/laminlabs/lndb-storage/pull/9) | [Koncopd](https://github.com/Koncopd) | 2023-03-26 | 0.2rc2
 ➖ Remove lndb as explicit dependency | [7](https://github.com/laminlabs/lndb-storage/pull/7) | [Koncopd](https://github.com/Koncopd) | 2023-03-26 | 0.2rc1
 🚚 Rename `DObject` to `File` | [8](https://github.com/laminlabs/lndb-storage/pull/8) | [falexwolf](https://github.com/falexwolf) | 2023-03-24 |
 ✅ Test streaming here | [6](https://github.com/laminlabs/lndb-storage/pull/6) | [Koncopd](https://github.com/Koncopd) | 2023-03-17 |
 ♻️ Move the rest of storage code here | [4](https://github.com/laminlabs/lndb-storage/pull/4) | [Koncopd](https://github.com/Koncopd) | 2023-03-14 |
-:construction_worker: Update with latest cookiecutter | [5](https://github.com/laminlabs/lndb-storage/pull/5) | [falexwolf](https://github.com/falexwolf) | 2023-03-14 |
+👷 Update with latest cookiecutter | [5](https://github.com/laminlabs/lndb-storage/pull/5) | [falexwolf](https://github.com/falexwolf) | 2023-03-14 |
 🔨 Update storage code | [3](https://github.com/laminlabs/lndb-storage/pull/3) | [Koncopd](https://github.com/Koncopd) | 2023-03-11 |
 🎉 Start moving code from lamindb | [1](https://github.com/laminlabs/lndb-storage/pull/1) | [Koncopd](https://github.com/Koncopd) | 2022-11-20 |
```

### Comparing `lndb_storage-0.2rc3/docs/guide/add-replace-stage.ipynb` & `lndb_storage-0.2rc4/docs/guide/add-replace-stage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/docs/guide/iris.csv` & `lndb_storage-0.2rc4/docs/guide/iris.csv`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/docs/guide/iris.data` & `lndb_storage-0.2rc4/docs/guide/iris.data`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/docs/guide/serialize-cache.ipynb` & `lndb_storage-0.2rc4/docs/guide/serialize-cache.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/docs/guide/stream.ipynb` & `lndb_storage-0.2rc4/docs/guide/stream.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/docs/guide/upload.ipynb` & `lndb_storage-0.2rc4/docs/guide/upload.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/lndb_storage/__init__.py` & `lndb_storage-0.2rc4/lndb_storage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    :toctree: .
 
    store_object
    store_png
    delete_storage
 """
 
-__version__ = "0.2rc3"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.2rc4"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 from lndb.dev.upath import UPath
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 
 from ._file import delete_storage, load_to_memory, store_object
 from ._h5ad import h5ad_to_anndata
 from ._images import store_png
```

### Comparing `lndb_storage-0.2rc3/lndb_storage/_file.py` & `lndb_storage-0.2rc4/lndb_storage/_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import os
 import shutil
 from pathlib import Path
 from typing import Union
 
 import fsspec
-import nbproject
 import pandas as pd
 import readfcs
 from lndb.dev.upath import UPath
 
 from ._h5ad import read_adata_h5ad
 from ._zarr import read_adata_zarr
 
@@ -18,18 +18,18 @@
     ".fcs": readfcs.read,
     ".zarr": read_adata_zarr,
 }
 
 
 def print_hook(size, value, **kwargs):
     progress = value / size
-    out = f"Uploading {kwargs['filepath']}: {min(progress, 1.):4.2f}"
+    out = f"... uploading {Path(kwargs['filepath']).name}: {min(progress, 1.):4.2f}"
     if progress >= 1:
         out += "\n"
-    if nbproject.meta.env != "test":
+    if "NBPRJ_TEST_NBPATH" not in os.environ:
         print(out, end="\r")
 
 
 class ProgressCallback(fsspec.callbacks.Callback):
     def branch(self, path_1, path_2, kwargs):
         kwargs["callback"] = fsspec.callbacks.Callback(
             hooks=dict(print_hook=print_hook), filepath=path_1
```

### Comparing `lndb_storage-0.2rc3/lndb_storage/_subset.py` & `lndb_storage-0.2rc4/lndb_storage/_subset.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/lndb_storage/_zarr.py` & `lndb_storage-0.2rc4/lndb_storage/_zarr.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/lndb_storage/object/_anndata.py` & `lndb_storage-0.2rc4/lndb_storage/object/_anndata.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/lndb_storage/object/_anndata_sizes.py` & `lndb_storage-0.2rc4/lndb_storage/object/_anndata_sizes.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/lndb_storage/object/_core.py` & `lndb_storage-0.2rc4/lndb_storage/object/_core.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/lndb_storage/object/_lazy_field.py` & `lndb_storage-0.2rc4/lndb_storage/object/_lazy_field.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/lndb_storage/object/_subset_anndata.py` & `lndb_storage-0.2rc4/lndb_storage/object/_subset_anndata.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/noxfile.py` & `lndb_storage-0.2rc4/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/pyproject.toml` & `lndb_storage-0.2rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc3/PKG-INFO` & `lndb_storage-0.2rc4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lndb_storage
-Version: 0.2rc3
+Version: 0.2rc4
 Summary: Storage → object.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core
 Requires-Dist: lamin_logger>=0.3.0
 Requires-Dist: nbproject
 Requires-Dist: readfcs
```

