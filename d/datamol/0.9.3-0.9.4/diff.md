# Comparing `tmp/datamol-0.9.3.tar.gz` & `tmp/datamol-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamol-0.9.3.tar", last modified: Thu Apr 13 19:29:15 2023, max compression
+gzip compressed data, was "datamol-0.9.4.tar", last modified: Fri Apr 14 14:57:34 2023, max compression
```

## Comparing `datamol-0.9.3.tar` & `datamol-0.9.4.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.653833 datamol-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-13 19:27:46.000000 datamol-0.9.3/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.609833 datamol-0.9.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 19:27:46.000000 datamol-0.9.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 19:27:46.000000 datamol-0.9.3/.devcontainer/bashrc
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-13 19:27:46.000000 datamol-0.9.3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.613833 datamol-0.9.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.613833 datamol-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-13 19:27:46.000000 datamol-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-13 19:27:46.000000 datamol-0.9.3/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-13 19:27:46.000000 datamol-0.9.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25863 2023-04-13 19:27:46.000000 datamol-0.9.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-13 19:27:46.000000 datamol-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-13 19:29:15.649833 datamol-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-13 19:27:46.000000 datamol-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.613833 datamol-0.9.3/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 19:27:46.000000 datamol-0.9.3/binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 19:27:46.000000 datamol-0.9.3/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 19:27:46.000000 datamol-0.9.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.617833 datamol-0.9.3/datamol/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/_sanifix4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.617833 datamol-0.9.3/datamol/conformers/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/conformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/conformers/_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/conformers/_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.617833 datamol-0.9.3/datamol/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   160134 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/cdk2.sdf
--rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/freesolv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   124841 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/reactions.json
--rw-r--r--   0 runner    (1001) docker     (123)   245735 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/solubility.test.sdf
--rw-r--r--   0 runner    (1001) docker     (123)  1376487 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/solubility.train.sdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/descriptors/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/descriptors/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/fragment/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/fragment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/fragment/_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/fragment/_fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/isomers/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/isomers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/isomers/_enumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/isomers/_structural.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43876 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/molar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/predictors/esol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/reactions/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/reactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/reactions/_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/reactions/_reactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/scaffold/_fuzzy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_circle_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19122 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_lasso_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_substructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.617833 datamol-0.9.3/datamol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.625833 datamol-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.629833 datamol-0.9.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.align.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.cluster.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.conformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.convert.md
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.data.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.descriptors.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.fragment.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.io.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.isomers.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.log.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.mol.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.molar.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.reactions.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.scaffold.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.similarity.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.609833 datamol-0.9.3/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.629833 datamol-0.9.3/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/assets/css/custom-datamol.css
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.629833 datamol-0.9.3/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/contribute.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.633833 datamol-0.9.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.641833 datamol-0.9.3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   298565 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Aligning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   174933 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Clustering.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    94833 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Conformers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   180458 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Descriptors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Filesystem.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   297941 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Fragment.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   210862 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Fuzzy_Scaffolds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42846 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Preprocessing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    89360 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Reactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   151601 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Scaffolds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   521054 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/The_Basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   181122 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/Visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.645833 datamol-0.9.3/docs/tutorials/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1345316 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/data/ReactionBlock.rxn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.645833 datamol-0.9.3/docs/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (123)   141008 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Aligning_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    76455 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Aligning_2.png
--rw-r--r--   0 runner    (1001) docker     (123)   310889 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Conformers_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Descriptors_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   422734 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Fragment_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    67840 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Fragment_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    34879 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Fragment_3.png
--rw-r--r--   0 runner    (1001) docker     (123)   333241 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Preprocess_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   102167 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Scaffolds_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 19:27:47.000000 datamol-0.9.3/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-13 19:27:47.000000 datamol-0.9.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.645833 datamol-0.9.3/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 19:27:47.000000 datamol-0.9.3/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-13 19:27:47.000000 datamol-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-13 19:27:47.000000 datamol-0.9.3/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:29:15.653833 datamol-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.649833 datamol-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.649833 datamol-0.9.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/TUBB3-observations-last-broken.sdf
--rw-r--r--   0 runner    (1001) docker     (123)    30331 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/TUBB3-observations.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/TUBB3-observations.sdf.gz
--rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/freesolv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/freesolv.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/test.mol2
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_datamol_import_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_isomers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_molar.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_utils_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_utils_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_utils_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_viz_lasso_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_viz_substrcture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.922034 datamol-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-14 14:56:08.000000 datamol-0.9.4/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 14:56:08.000000 datamol-0.9.4/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 14:56:08.000000 datamol-0.9.4/.devcontainer/bashrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-14 14:56:08.000000 datamol-0.9.4/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 14:56:08.000000 datamol-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-14 14:56:08.000000 datamol-0.9.4/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-14 14:56:08.000000 datamol-0.9.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-04-14 14:56:08.000000 datamol-0.9.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-14 14:56:08.000000 datamol-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 14:57:34.922034 datamol-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-14 14:56:08.000000 datamol-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 14:56:08.000000 datamol-0.9.4/binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 14:56:08.000000 datamol-0.9.4/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 14:56:08.000000 datamol-0.9.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/datamol/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/_sanifix4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/conformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/conformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/conformers/_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/conformers/_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160134 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/cdk2.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/freesolv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   124841 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/reactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   245735 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/solubility.test.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)  1376487 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/solubility.train.sdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/descriptors/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/descriptors/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/fragment/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/fragment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/fragment/_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/fragment/_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/isomers/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/isomers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/isomers/_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/isomers/_structural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43876 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/molar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/predictors/esol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/reactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/reactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/reactions/_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/reactions/_reactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/scaffold/_fuzzy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_circle_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19046 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_lasso_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_substructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/datamol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.910033 datamol-0.9.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.align.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.cluster.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.conformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.convert.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.data.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.descriptors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.fragment.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.io.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.isomers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.log.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.mol.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.molar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.reactions.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.scaffold.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.similarity.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.894033 datamol-0.9.4/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.910033 datamol-0.9.4/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/assets/css/custom-datamol.css
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.910033 datamol-0.9.4/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/contribute.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.910033 datamol-0.9.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.914034 datamol-0.9.4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   298565 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Aligning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   174933 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Clustering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    94833 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Conformers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   180458 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Descriptors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Filesystem.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   297941 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Fragment.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   210862 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Fuzzy_Scaffolds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42846 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Preprocessing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    89360 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Reactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   151601 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Scaffolds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   521054 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/The_Basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   181122 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.914034 datamol-0.9.4/docs/tutorials/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1345316 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/data/ReactionBlock.rxn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.918034 datamol-0.9.4/docs/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   141008 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Aligning_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76455 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Aligning_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   310889 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Conformers_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Descriptors_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   422734 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Fragment_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67840 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Fragment_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34879 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Fragment_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   333241 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Preprocess_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102167 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Scaffolds_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 14:56:08.000000 datamol-0.9.4/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 14:56:08.000000 datamol-0.9.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.918034 datamol-0.9.4/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 14:56:08.000000 datamol-0.9.4/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-14 14:56:08.000000 datamol-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 14:56:08.000000 datamol-0.9.4/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:57:34.922034 datamol-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.922034 datamol-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.922034 datamol-0.9.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/TUBB3-observations-last-broken.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)    30331 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/TUBB3-observations.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/TUBB3-observations.sdf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/freesolv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/freesolv.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/test.mol2
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_datamol_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_isomers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_molar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_utils_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_utils_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_utils_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_viz_lasso_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_viz_substrcture.py
```

### Comparing `datamol-0.9.3/.authors.yml` & `datamol-0.9.4/.authors.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.devcontainer/Dockerfile` & `datamol-0.9.4/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.devcontainer/devcontainer.json` & `datamol-0.9.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.github/CODE_OF_CONDUCT.md` & `datamol-0.9.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.github/workflows/code-check.yml` & `datamol-0.9.4/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.github/workflows/doc.yml` & `datamol-0.9.4/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.github/workflows/release.yml` & `datamol-0.9.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.github/workflows/test.yml` & `datamol-0.9.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.gitignore` & `datamol-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/.mailmap` & `datamol-0.9.4/.mailmap`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/CHANGELOG.rst` & `datamol-0.9.4/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 ==================
 Datamol Changelogs
 ==================
 
 .. current developments
 
+v0.9.4
+====================
+
+**Fixed:**
+
+* Fix wrong image output for lasso viz function. Make it consistent with `dm.to_image()` and rdkit.
+* Avoid global `IPython` import so it's not an hard datamol dependency.
+* Add `importlib-resources` dep in the datamol pypi package.
+
+**Authors:**
+
+* Hadrien Mary
+
+
+
 v0.9.3
 ====================
 
 **Added:**
 
 * added a feature that highlights substructures of 2D molecular images
```

### Comparing `datamol-0.9.3/LICENSE` & `datamol-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/PKG-INFO` & `datamol-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamol
-Version: 0.9.3
+Version: 0.9.4
 Summary: A python library to work with molecules. Built on top of RDKit.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol
 Project-URL: Bug Tracker, https://github.com/datamol-io/datamol/issues
 Project-URL: Documentation, https://docs.datamol.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datamol Version: 0.9.3 Summary: A python library to
+Metadata-Version: 2.1 Name: datamol Version: 0.9.4 Summary: A python library to
 work with molecules. Built on top of RDKit. Author-email: Hadrien Mary
 valencediscovery.com> License: Apache Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol Project-URL:
 Bug Tracker, https://github.com/datamol-io/datamol/issues Project-URL:
 Documentation, https://docs.datamol.io Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `datamol-0.9.3/README.md` & `datamol-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/binder/environment.yml` & `datamol-0.9.4/binder/environment.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/__init__.py` & `datamol-0.9.4/datamol/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/_sanifix4.py` & `datamol-0.9.4/datamol/_sanifix4.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/_version.py` & `datamol-0.9.4/datamol/_version.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/align.py` & `datamol-0.9.4/datamol/align.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/cluster.py` & `datamol-0.9.4/datamol/cluster.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/conformers/_conformers.py` & `datamol-0.9.4/datamol/conformers/_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/conformers/_features.py` & `datamol-0.9.4/datamol/conformers/_features.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/convert.py` & `datamol-0.9.4/datamol/convert.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/data/__init__.py` & `datamol-0.9.4/datamol/data/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/data/cdk2.sdf` & `datamol-0.9.4/datamol/data/cdk2.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/data/freesolv.csv` & `datamol-0.9.4/datamol/data/freesolv.csv`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/data/reactions.json` & `datamol-0.9.4/datamol/data/reactions.json`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/data/solubility.test.sdf` & `datamol-0.9.4/datamol/data/solubility.test.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/data/solubility.train.sdf` & `datamol-0.9.4/datamol/data/solubility.train.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/descriptors/__init__.py` & `datamol-0.9.4/datamol/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/descriptors/compute.py` & `datamol-0.9.4/datamol/descriptors/compute.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/descriptors/descriptors.py` & `datamol-0.9.4/datamol/descriptors/descriptors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/fp.py` & `datamol-0.9.4/datamol/fp.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/fragment/_assemble.py` & `datamol-0.9.4/datamol/fragment/_assemble.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/fragment/_fragment.py` & `datamol-0.9.4/datamol/fragment/_fragment.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/graph.py` & `datamol-0.9.4/datamol/graph.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/io.py` & `datamol-0.9.4/datamol/io.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/isomers/_enumerate.py` & `datamol-0.9.4/datamol/isomers/_enumerate.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/isomers/_structural.py` & `datamol-0.9.4/datamol/isomers/_structural.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/log.py` & `datamol-0.9.4/datamol/log.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/mcs.py` & `datamol-0.9.4/datamol/mcs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/mol.py` & `datamol-0.9.4/datamol/mol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/molar.py` & `datamol-0.9.4/datamol/molar.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/predictors/esol.py` & `datamol-0.9.4/datamol/predictors/esol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/reactions/__init__.py` & `datamol-0.9.4/datamol/reactions/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/reactions/_attachments.py` & `datamol-0.9.4/datamol/reactions/_attachments.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/reactions/_reactions.py` & `datamol-0.9.4/datamol/reactions/_reactions.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/scaffold/_fuzzy.py` & `datamol-0.9.4/datamol/scaffold/_fuzzy.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/similarity.py` & `datamol-0.9.4/datamol/similarity.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/utils/decorators.py` & `datamol-0.9.4/datamol/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/utils/fs.py` & `datamol-0.9.4/datamol/utils/fs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/utils/jobs.py` & `datamol-0.9.4/datamol/utils/jobs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/utils/perf.py` & `datamol-0.9.4/datamol/utils/perf.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/utils/testing.py` & `datamol-0.9.4/datamol/utils/testing.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/viz/_circle_grid.py` & `datamol-0.9.4/datamol/viz/_circle_grid.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/viz/_conformers.py` & `datamol-0.9.4/datamol/viz/_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/viz/_lasso_highlight.py` & `datamol-0.9.4/datamol/viz/_lasso_highlight.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,25 @@
 # - possibility to do this for multiple target molecules at once
 # - have the option to write to a file like to_image
 
 from typing import List, Iterator, Tuple, Union, Optional, Any
 
 from collections import defaultdict
 from collections import namedtuple
-import io
-import sys
 
-from rdkit.Chem.Draw import rdMolDraw2D, IPythonConsole
+from rdkit.Chem.Draw import rdMolDraw2D
 from rdkit.Chem.rdmolops import Get3DDistanceMatrix
 from rdkit.Geometry.rdGeometry import Point2D
 
-from PIL import Image
-
 from loguru import logger
 
 import numpy as np
 import datamol as dm
 
+from .utils import drawer_to_image
 from .utils import prepare_mol_for_drawing
 
 
 def _angle_to_coord(center: np.ndarray, angle: float, radius: float) -> np.ndarray:
     """Determines a point relative to the center with distance (radius) at given angle.
     Angles are given in rad and 0 rad correspond to north of the center point.
 
@@ -371,16 +368,15 @@
     r_min: float = 0.3,
     r_dist: float = 0.13,
     relative_bond_width: float = 0.5,
     color_list: Optional[List[ColorTuple]] = None,
     line_width: int = 2,
     **kwargs: Any,
 ):
-    """A generalized interface to access both highlighting options whether the
-    input is as a smiles, smarts or mol
+    """Create an image of a molecule with substructure matches using lasso-based highlighting.
 
     args:
         target_molecule: The molecule to be highlighted
         search_molecules: The substructure to be identified
         mol_size: The size of the image to be returned
         use_svg: Whether to return an svg or png image
         r_min: Radius of the smallest circle around atoms. Length is relative to average bond length (1 = avg. bond len).
@@ -413,31 +409,31 @@
 
     mol = prepare_mol_for_drawing(target_molecule, kekulize=True)
 
     if mol is None:
         raise ValueError("The molecule has failed to be prepared by `prepare_mol_for_drawing`.")
 
     if use_svg:
-        d = rdMolDraw2D.MolDraw2DSVG(mol_size[0], mol_size[1])
+        drawer = rdMolDraw2D.MolDraw2DSVG(mol_size[0], mol_size[1])
     else:
-        d = rdMolDraw2D.MolDraw2DCairo(mol_size[0], mol_size[1])
+        drawer = rdMolDraw2D.MolDraw2DCairo(mol_size[0], mol_size[1])
 
     # Setting the drawing options
-    draw_options = d.drawOptions()
+    draw_options = drawer.drawOptions()
     for k, v in kwargs.items():
         if not hasattr(draw_options, k):
             raise ValueError(
                 f"Invalid drawing option: {k}={v}. Check `rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions` for valid ones."
             )
         else:
             setattr(draw_options, k, v)
 
     # Setting up the coordinate system by drawing and erasing molecule
-    d.DrawMolecule(mol)
-    d.ClearDrawing()
+    drawer.DrawMolecule(mol)
+    drawer.ClearDrawing()
 
     # get the atom indices for the search molecules
     atom_idx_list = []
     if isinstance(search_molecules, str):
         smart_obj = dm.to_mol(search_molecules)
         matches = mol.GetSubstructMatches(smart_obj)
         if not matches:
@@ -476,27 +472,22 @@
     if color_list is None:
         color_list = DEFAULT_LASSO_COLORS
 
     if len(atom_idx_list) == 0:
         logger.warning("No matches found for the given search molecules")
     else:
         _draw_multi_matches(
-            d,
+            drawer,
             mol,
             atom_idx_list,
             r_min=r_min,
             r_dist=r_dist,
             relative_bond_width=relative_bond_width,
             line_width=line_width,
             color_list=color_list,
         )
 
-    d.DrawMolecule(mol)
-    d.FinishDrawing()
+    drawer.DrawMolecule(mol)
+    drawer.FinishDrawing()
 
-    if "ipykernel" in sys.modules:
-        if use_svg:
-            return IPythonConsole.SVG(d.GetDrawingText())
-        else:
-            return Image.open(io.BytesIO(d.GetDrawingText()))
-    else:
-        return d.GetDrawingText()
+    # NOTE(hadim): process the drawer object to return the image type matching the same behavior as RDkit and `datamol.to_image()`
+    return drawer_to_image(drawer)
```

### Comparing `datamol-0.9.3/datamol/viz/_substructure.py` & `datamol-0.9.4/datamol/viz/_substructure.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol/viz/_viz.py` & `datamol-0.9.4/datamol/viz/_viz.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/datamol.egg-info/PKG-INFO` & `datamol-0.9.4/datamol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamol
-Version: 0.9.3
+Version: 0.9.4
 Summary: A python library to work with molecules. Built on top of RDKit.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol
 Project-URL: Bug Tracker, https://github.com/datamol-io/datamol/issues
 Project-URL: Documentation, https://docs.datamol.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datamol Version: 0.9.3 Summary: A python library to
+Metadata-Version: 2.1 Name: datamol Version: 0.9.4 Summary: A python library to
 work with molecules. Built on top of RDKit. Author-email: Hadrien Mary
 valencediscovery.com> License: Apache Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol Project-URL:
 Bug Tracker, https://github.com/datamol-io/datamol/issues Project-URL:
 Documentation, https://docs.datamol.io Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `datamol-0.9.3/datamol.egg-info/SOURCES.txt` & `datamol-0.9.4/datamol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/assets/css/custom-datamol.css` & `datamol-0.9.4/docs/assets/css/custom-datamol.css`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/assets/css/custom.css` & `datamol-0.9.4/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/contribute.md` & `datamol-0.9.4/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/images/logo-black.png` & `datamol-0.9.4/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/images/logo-black.svg` & `datamol-0.9.4/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/images/logo-title.svg` & `datamol-0.9.4/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/images/logo.png` & `datamol-0.9.4/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/images/logo.svg` & `datamol-0.9.4/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/index.md` & `datamol-0.9.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Aligning.ipynb` & `datamol-0.9.4/docs/tutorials/Aligning.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Clustering.ipynb` & `datamol-0.9.4/docs/tutorials/Clustering.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Conformers.ipynb` & `datamol-0.9.4/docs/tutorials/Conformers.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Descriptors.ipynb` & `datamol-0.9.4/docs/tutorials/Descriptors.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Filesystem.ipynb` & `datamol-0.9.4/docs/tutorials/Filesystem.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Fragment.ipynb` & `datamol-0.9.4/docs/tutorials/Fragment.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Fuzzy_Scaffolds.ipynb` & `datamol-0.9.4/docs/tutorials/Fuzzy_Scaffolds.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Preprocessing.ipynb` & `datamol-0.9.4/docs/tutorials/Preprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Reactions.ipynb` & `datamol-0.9.4/docs/tutorials/Reactions.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Scaffolds.ipynb` & `datamol-0.9.4/docs/tutorials/Scaffolds.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/The_Basics.ipynb` & `datamol-0.9.4/docs/tutorials/The_Basics.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/Visualization.ipynb` & `datamol-0.9.4/docs/tutorials/Visualization.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf` & `datamol-0.9.4/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/data/ReactionBlock.rxn` & `datamol-0.9.4/docs/tutorials/data/ReactionBlock.rxn`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Aligning_1.png` & `datamol-0.9.4/docs/tutorials/images/Aligning_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Aligning_2.png` & `datamol-0.9.4/docs/tutorials/images/Aligning_2.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Conformers_1.png` & `datamol-0.9.4/docs/tutorials/images/Conformers_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Descriptors_1.png` & `datamol-0.9.4/docs/tutorials/images/Descriptors_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Fragment_1.png` & `datamol-0.9.4/docs/tutorials/images/Fragment_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Fragment_2.png` & `datamol-0.9.4/docs/tutorials/images/Fragment_2.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Fragment_3.png` & `datamol-0.9.4/docs/tutorials/images/Fragment_3.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Preprocess_1.png` & `datamol-0.9.4/docs/tutorials/images/Preprocess_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/tutorials/images/Scaffolds_1.png` & `datamol-0.9.4/docs/tutorials/images/Scaffolds_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/docs/usage.md` & `datamol-0.9.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/env.yml` & `datamol-0.9.4/env.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/mkdocs.yml` & `datamol-0.9.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/pyproject.toml` & `datamol-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "matplotlib",
     "pillow",
     "selfies",
     "platformdirs",
     "scikit-learn",
     "packaging",
     "typing-extensions",
+    "importlib-resources",
     # NOTE(hadim): can't add rdkit because of `pip` will always override
     # the conda package at the moment.
     # See:
     # - https://github.com/rdkit/rdkit/issues/5378
     # - https://github.com/conda-forge/rdkit-feedstock/issues/104
     # "rdkit",
 ]
```

### Comparing `datamol-0.9.3/tests/conftest.py` & `datamol-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/data/TUBB3-observations-last-broken.sdf` & `datamol-0.9.4/tests/data/TUBB3-observations-last-broken.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/data/TUBB3-observations.sdf` & `datamol-0.9.4/tests/data/TUBB3-observations.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/data/TUBB3-observations.sdf.gz` & `datamol-0.9.4/tests/data/TUBB3-observations.sdf.gz`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/data/freesolv.csv` & `datamol-0.9.4/tests/data/freesolv.csv`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/data/freesolv.xlsx` & `datamol-0.9.4/tests/data/freesolv.xlsx`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/data/test.mol2` & `datamol-0.9.4/tests/data/test.mol2`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_align.py` & `datamol-0.9.4/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_cluster.py` & `datamol-0.9.4/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_conformers.py` & `datamol-0.9.4/tests/test_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_convert.py` & `datamol-0.9.4/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_data.py` & `datamol-0.9.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_datamol_import_time.py` & `datamol-0.9.4/tests/test_datamol_import_time.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_descriptors.py` & `datamol-0.9.4/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_fp.py` & `datamol-0.9.4/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_fragment.py` & `datamol-0.9.4/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_graph.py` & `datamol-0.9.4/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_io.py` & `datamol-0.9.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_isomers.py` & `datamol-0.9.4/tests/test_isomers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import pytest
-import time
-
-from rdkit import Chem
 
 import datamol as dm
 
 
 def test_enumerate_tautomers():
     mol = dm.to_mol("OC1=CC2CCCCC2[N:1]=C1")
 
@@ -49,22 +46,22 @@
 
 
 def test_enumerate_structural():
     mol = dm.to_mol("CCCCC")  # pentane has only three structural isomers
 
     mols_iso = dm.enumerate_structisomers(
         mol,
-        n_variants=5,
+        n_variants=2,
         allow_cycle=False,
-        depth=2,
+        depth=1,
         allow_double_bond=False,
         allow_triple_bond=False,
     )
 
-    assert {dm.to_smiles(m) for m in mols_iso} == {"CCC(C)C", "CC(C)(C)C"}
+    assert {dm.to_smiles(m) for m in mols_iso} == {"CCC(C)C"}
 
     # NOTE(hadim): disable to reduce testing time
     # mols_cyclo_iso = dm.enumerate_structisomers(mol, n_variants=5, depth=2, allow_cycle=True)
 
     # # expect 3 molecules with cycles
     # assert sum([Chem.rdMolDescriptors.CalcNumRings(x) == 1 for x in mols_cyclo_iso]) == 3  # type: ignore
```

### Comparing `datamol-0.9.3/tests/test_log.py` & `datamol-0.9.4/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_mcs.py` & `datamol-0.9.4/tests/test_mcs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_mol.py` & `datamol-0.9.4/tests/test_mol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_molar.py` & `datamol-0.9.4/tests/test_molar.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_notebooks.py` & `datamol-0.9.4/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_predictors.py` & `datamol-0.9.4/tests/test_predictors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_reactions.py` & `datamol-0.9.4/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_scaffold.py` & `datamol-0.9.4/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_similarity.py` & `datamol-0.9.4/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_utils_fs.py` & `datamol-0.9.4/tests/test_utils_fs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_utils_jobs.py` & `datamol-0.9.4/tests/test_utils_jobs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_viz.py` & `datamol-0.9.4/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.3/tests/test_viz_lasso_highlight.py` & `datamol-0.9.4/tests/test_viz_lasso_highlight.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,23 +126,25 @@
 
 # testing using <class 'IPython.core.display.SVG'>" == str(type(img)) so to not bring in IPython
 # as a dependency for the tests
 def test_SVG_is_returned_explicit():
     smi = "CO[C@@H](O)C1=C(O[C@H](F)Cl)C(C#N)=C1ONNC[NH3+]"
     smarts_list = ["CC"]
     img = dm.lasso_highlight_image(smi, smarts_list, use_svg=True)
-    assert "<class 'IPython.core.display.SVG'>" == str(type(img))
+    assert isinstance(img, str)
 
 
 def test_SVG_is_returned_implict():
     smi = "CO[C@@H](O)C1=C(O[C@H](F)Cl)C(C#N)=C1ONNC[NH3+]"
     smarts_list = ["CC"]
     img = dm.lasso_highlight_image(smi, smarts_list)
-    assert "<class 'IPython.core.display.SVG'>" == str(type(img))
+    assert isinstance(img, str)
 
 
 def test_PNG_is_returned():
     smi = "CO[C@@H](O)C1=C(O[C@H](F)Cl)C(C#N)=C1ONNC[NH3+]"
     smarts_list = ["CC"]
     img = dm.lasso_highlight_image(smi, smarts_list, use_svg=False)
-    image_format = img.format.lower()
-    assert image_format == "png"
+
+    from PIL import Image
+
+    assert isinstance(img, Image.Image)
```

### Comparing `datamol-0.9.3/tests/test_viz_substrcture.py` & `datamol-0.9.4/tests/test_viz_substrcture.py`

 * *Files identical despite different names*

