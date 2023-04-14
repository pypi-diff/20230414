# Comparing `tmp/boilercv-0.0.0.tar.gz` & `tmp/boilercv-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boilercv-0.0.0.tar", last modified: Thu Apr 13 19:02:06 2023, max compression
+gzip compressed data, was "boilercv-0.0.1.tar", last modified: Fri Apr 14 20:47:11 2023, max compression
```

## Comparing `boilercv-0.0.0.tar` & `boilercv-0.0.1.tar`

### file list

```diff
@@ -1,140 +1,2440 @@
--rw-r--r--   0        0        0      392 2023-04-10 18:29:43.384898 boilercv-0.0.0/.copier-answers.yml
--rw-r--r--   0        0        0      512 2023-04-10 18:29:42.797895 boilercv-0.0.0/.coveragerc
--rw-r--r--   0        0        0       29 2023-03-02 22:38:55.010265 boilercv-0.0.0/.dvc/.gitignore
--rw-r--r--   0        0        0       97 2023-03-04 01:07:15.968362 boilercv-0.0.0/.dvc/config
--rw-r--r--   0        0        0     3028 2023-04-10 23:14:59.824066 boilercv-0.0.0/.env
--rw-r--r--   0        0        0     1105 2023-04-10 18:29:42.806896 boilercv-0.0.0/.gitattributes
--rw-r--r--   0        0        0      319 2023-04-10 18:29:42.816895 boilercv-0.0.0/.github/workflows/changerelease.yml
--rw-r--r--   0        0        0      676 2023-04-12 01:11:50.291878 boilercv-0.0.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     2182 2023-04-10 18:29:43.861900 boilercv-0.0.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      920 2023-04-10 18:29:43.862895 boilercv-0.0.0/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0     5229 2023-04-10 18:29:43.863898 boilercv-0.0.0/.gitignore
--rw-r--r--   0        0        0      528 2023-04-10 18:29:42.890896 boilercv-0.0.0/.gitmodules
--rw-r--r--   0        0        0       47 2023-04-10 18:29:42.895897 boilercv-0.0.0/.markdownlint.yaml
--rw-r--r--   0        0        0       96 2023-04-10 18:29:42.921895 boilercv-0.0.0/.nest_md
--rw-r--r--   0        0        0       94 2023-04-10 18:29:42.936901 boilercv-0.0.0/.nest_tools_config
--rw-r--r--   0        0        0     2655 2023-04-13 18:24:46.284921 boilercv-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      389 2023-04-10 18:29:43.865896 boilercv-0.0.0/.sourcery.yaml
--rw-r--r--   0        0        0     5510 2023-04-13 18:27:09.907806 boilercv-0.0.0/.tools/pyproject.toml
--rw-r--r--   0        0        0      579 2023-04-10 18:29:43.867898 boilercv-0.0.0/.tools/requirements/requirements_both.txt
--rw-r--r--   0        0        0       26 2023-04-10 18:29:43.031898 boilercv-0.0.0/.tools/requirements/requirements_ci.txt
--rw-r--r--   0        0        0      713 2023-04-10 18:29:43.039897 boilercv-0.0.0/.tools/requirements/requirements_dev.txt
--rw-r--r--   0        0        0      445 2023-04-04 19:44:49.183504 boilercv-0.0.0/.tools/requirements/requirements_docs.txt
--rw-r--r--   0        0        0      103 2023-04-04 22:12:56.250123 boilercv-0.0.0/.tools/requirements/requirements_nodeps.txt
--rw-r--r--   0        0        0      241 2023-04-10 18:29:43.067895 boilercv-0.0.0/.tools/scripts/Copy-Template.ps1
--rw-r--r--   0        0        0      431 2023-04-10 18:29:43.080897 boilercv-0.0.0/.tools/scripts/Update-Template.ps1
--rw-r--r--   0        0        0      632 2023-04-10 18:29:43.869900 boilercv-0.0.0/.tools/scripts/compose_pyproject.py
--rw-r--r--   0        0        0      238 2023-04-10 18:29:43.074899 boilercv-0.0.0/.tools/scripts/template_common.ps1
--rw-r--r--   0        0        0      715 2022-07-07 19:02:36.085788 boilercv-0.0.0/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1078 2023-04-10 18:29:43.120896 boilercv-0.0.0/.vscode/extensions.json
--rw-r--r--   0        0        0     4109 2023-04-11 18:35:33.782938 boilercv-0.0.0/.vscode/launch.json
--rw-r--r--   0        0        0     8275 2023-04-13 18:04:32.884897 boilercv-0.0.0/.vscode/settings.json
--rw-r--r--   0        0        0    11605 2023-04-13 18:40:41.756366 boilercv-0.0.0/.vscode/tasks.json
--rw-r--r--   0        0        0      532 2023-04-13 18:56:37.638600 boilercv-0.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      447 2023-04-13 19:00:38.498201 boilercv-0.0.0/CITATION.cff
--rw-r--r--   0        0        0     6281 2023-04-10 18:29:43.203894 boilercv-0.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1072 2022-06-14 23:28:29.368988 boilercv-0.0.0/LICENSE
--rw-r--r--   0        0        0      185 2023-04-13 18:59:53.642334 boilercv-0.0.0/README.md
--rw-r--r--   0        0        0     8165 2023-03-02 23:10:23.966020 boilercv-0.0.0/build.txt
--rw-r--r--   0        0        0       56 2023-04-10 18:29:43.161897 boilercv-0.0.0/codecov.yml
--rw-r--r--   0        0        0        7 2023-04-04 06:27:10.419011 boilercv-0.0.0/data/.dvcignore
--rw-r--r--   0        0        0       50 2023-03-14 22:08:59.910344 boilercv-0.0.0/data/.gitignore
--rw-r--r--   0        0        0      103 2023-04-11 19:16:23.057334 boilercv-0.0.0/data/examples.dvc
--rw-r--r--   0        0        0      100 2023-04-11 19:16:26.155859 boilercv-0.0.0/data/rois.dvc
--rw-r--r--   0        0        0      102 2023-04-11 19:16:27.099860 boilercv-0.0.0/data/samples.dvc
--rw-r--r--   0        0        0      104 2023-04-11 19:17:01.290534 boilercv-0.0.0/data/sources.dvc
--rw-r--r--   0        0        0       16 2023-03-02 17:32:24.265449 boilercv-0.0.0/docs/.gitignore
--rw-r--r--   0        0        0   234596 2023-04-12 00:29:26.844000 boilercv-0.0.0/docs/_static/multicolor.png
--rw-r--r--   0        0        0       77 2023-04-13 18:22:43.066888 boilercv-0.0.0/docs/changelog.md
--rw-r--r--   0        0        0      389 2023-04-13 18:22:59.643786 boilercv-0.0.0/docs/conf.py
--rw-r--r--   0        0        0      443 2023-04-10 18:19:56.011597 boilercv-0.0.0/docs/dag.md
--rw-r--r--   0        0        0      574 2023-04-13 18:23:33.988025 boilercv-0.0.0/docs/index.md
--rw-r--r--   0        0        0     4562 2023-04-11 19:16:14.748914 boilercv-0.0.0/dvc.lock
--rw-r--r--   0        0        0     1469 2023-04-07 03:13:23.218269 boilercv-0.0.0/dvc.yaml
--rw-r--r--   0        0        0     1059 2023-04-13 18:42:02.828609 boilercv-0.0.0/dvc_repro.ps1
--rw-r--r--   0        0        0     1056 2023-04-13 18:52:06.802638 boilercv-0.0.0/params.yaml
--rw-r--r--   0        0        0     2174 2023-04-13 18:46:37.057754 boilercv-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1977 2023-04-10 18:29:43.875896 boilercv-0.0.0/pyrightconfig.json
--rw-r--r--   0        0        0     3052 2023-04-10 23:15:09.401627 boilercv-0.0.0/pytest.ini
--rw-r--r--   0        0        0      701 2023-04-10 18:29:43.255894 boilercv-0.0.0/pythonrc.py
--rw-r--r--   0        0        0     2901 2023-04-11 17:41:19.321385 boilercv-0.0.0/renovate.json
--rw-r--r--   0        0        0     6461 2023-04-13 18:48:37.626536 boilercv-0.0.0/repro.txt
--rw-r--r--   0        0        0     1241 2023-04-12 17:20:48.645471 boilercv-0.0.0/requirements.txt
--rw-r--r--   0        0        0      776 2023-04-10 18:29:43.308901 boilercv-0.0.0/setup.ps1
--rw-r--r--   0        0        0     2278 2023-04-13 18:29:18.015199 boilercv-0.0.0/src/boilercv/__init__.py
--rw-r--r--   0        0        0       62 2023-04-11 18:08:31.942096 boilercv-0.0.0/src/boilercv/captivate/__init__.py
--rw-r--r--   0        0        0     2349 2023-04-11 22:41:59.640256 boilercv-0.0.0/src/boilercv/captivate/captures.py
--rw-r--r--   0        0        0    12311 2023-04-11 22:28:02.251077 boilercv-0.0.0/src/boilercv/captivate/previews.py
--rw-r--r--   0        0        0      356 2023-04-04 01:49:21.900581 boilercv-0.0.0/src/boilercv/colors.py
--rw-r--r--   0        0        0     4205 2023-04-12 00:31:13.466205 boilercv-0.0.0/src/boilercv/data/__init__.py
--rw-r--r--   0        0        0      927 2023-04-11 23:00:35.152310 boilercv-0.0.0/src/boilercv/data/frames.py
--rw-r--r--   0        0        0     2781 2023-04-03 02:57:06.896496 boilercv-0.0.0/src/boilercv/data/models.py
--rw-r--r--   0        0        0     1209 2023-04-04 23:06:47.512265 boilercv-0.0.0/src/boilercv/data/packing.py
--rw-r--r--   0        0        0     3987 2023-04-12 00:00:59.318587 boilercv-0.0.0/src/boilercv/data/sets.py
--rw-r--r--   0        0        0     3235 2023-04-11 18:11:38.846010 boilercv-0.0.0/src/boilercv/data/video.py
--rw-r--r--   0        0        0      706 2023-04-06 19:39:58.755755 boilercv-0.0.0/src/boilercv/examples/__init__.py
--rw-r--r--   0        0        0     1060 2023-03-18 00:53:23.636346 boilercv-0.0.0/src/boilercv/examples/blobs/__init__.py
--rw-r--r--   0        0        0     1407 2023-04-11 23:55:12.495971 boilercv-0.0.0/src/boilercv/examples/blobs/bubbles.py
--rw-r--r--   0        0        0     1043 2023-04-11 18:11:27.793770 boilercv-0.0.0/src/boilercv/examples/blobs/galaxy.py
--rw-r--r--   0        0        0     1179 2023-04-12 00:33:44.412725 boilercv-0.0.0/src/boilercv/examples/contours.py
--rw-r--r--   0        0        0     1095 2023-04-11 18:22:38.989558 boilercv-0.0.0/src/boilercv/examples/cv/__init__.py
--rw-r--r--   0        0        0      443 2023-04-11 19:42:21.192138 boilercv-0.0.0/src/boilercv/examples/cv/__main__.py
--rw-r--r--   0        0        0      611 2023-04-11 19:41:02.814927 boilercv-0.0.0/src/boilercv/examples/cv/basic_test.py
--rw-r--r--   0        0        0      432 2023-04-11 19:45:36.561751 boilercv-0.0.0/src/boilercv/examples/cv/starry.py
--rw-r--r--   0        0        0     4623 2023-04-11 18:11:36.348005 boilercv-0.0.0/src/boilercv/examples/detect_surface.py
--rw-r--r--   0        0        0     1867 2023-04-12 00:33:44.412725 boilercv-0.0.0/src/boilercv/examples/fill.py
--rw-r--r--   0        0        0     1624 2023-04-11 18:11:25.683734 boilercv-0.0.0/src/boilercv/examples/large/__init__.py
--rw-r--r--   0        0        0      387 2023-03-31 02:33:40.367171 boilercv-0.0.0/src/boilercv/examples/large/binarize.py
--rw-r--r--   0        0        0     1273 2023-04-11 18:11:24.239706 boilercv-0.0.0/src/boilercv/examples/large/combined.py
--rw-r--r--   0        0        0      401 2023-04-04 23:37:38.810350 boilercv-0.0.0/src/boilercv/examples/large/compare.py
--rw-r--r--   0        0        0      454 2023-04-04 23:37:53.865115 boilercv-0.0.0/src/boilercv/examples/large/compress.py
--rw-r--r--   0        0        0      491 2023-04-04 23:37:47.999817 boilercv-0.0.0/src/boilercv/examples/large/compress_packed.py
--rw-r--r--   0        0        0      498 2023-04-10 18:19:56.030598 boilercv-0.0.0/src/boilercv/examples/large/convert.py
--rw-r--r--   0        0        0      340 2023-03-31 03:03:00.716140 boilercv-0.0.0/src/boilercv/examples/large/pack.py
--rw-r--r--   0        0        0      358 2023-03-31 03:03:37.579928 boilercv-0.0.0/src/boilercv/examples/large/unpack.py
--rw-r--r--   0        0        0       99 2023-04-11 22:18:16.195865 boilercv-0.0.0/src/boilercv/examples/previews/__init__.py
--rw-r--r--   0        0        0     1194 2023-04-11 18:11:21.278676 boilercv-0.0.0/src/boilercv/examples/previews/binarized_composite.py
--rw-r--r--   0        0        0     1134 2023-04-11 22:45:36.578539 boilercv-0.0.0/src/boilercv/examples/previews/gray_composite.py
--rw-r--r--   0        0        0     1891 2023-04-12 00:43:25.336351 boilercv-0.0.0/src/boilercv/examples/previews/multicolor_composite.py
--rw-r--r--   0        0        0     1544 2023-04-11 18:11:18.015677 boilercv-0.0.0/src/boilercv/examples/previews/triple_composite.py
--rw-r--r--   0        0        0      815 2023-04-11 18:11:31.607781 boilercv-0.0.0/src/boilercv/examples/save_roi.py
--rw-r--r--   0        0        0     3479 2023-04-12 00:13:44.329614 boilercv-0.0.0/src/boilercv/images/__init__.py
--rw-r--r--   0        0        0     5076 2023-04-11 23:55:22.965109 boilercv-0.0.0/src/boilercv/images/cv.py
--rw-r--r--   0        0        0       38 2023-04-03 05:15:06.758223 boilercv-0.0.0/src/boilercv/manual/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-10 18:19:56.035598 boilercv-0.0.0/src/boilercv/manual/binarize.py
--rw-r--r--   0        0        0      700 2023-04-10 18:19:56.036598 boilercv-0.0.0/src/boilercv/manual/convert.py
--rw-r--r--   0        0        0      735 2023-04-10 18:19:56.038600 boilercv-0.0.0/src/boilercv/manual/decompress.py
--rw-r--r--   0        0        0     1476 2023-04-10 18:19:56.039600 boilercv-0.0.0/src/boilercv/manual/rename.py
--rw-r--r--   0        0        0     3109 2023-04-10 18:19:56.040599 boilercv-0.0.0/src/boilercv/models/__init__.py
--rw-r--r--   0        0        0      508 2023-04-10 18:19:56.041600 boilercv-0.0.0/src/boilercv/models/params.py
--rw-r--r--   0        0        0     5163 2023-04-10 23:10:48.281240 boilercv-0.0.0/src/boilercv/models/paths.py
--rw-r--r--   0        0        0       51 2023-04-05 23:01:30.675827 boilercv-0.0.0/src/boilercv/old/__init__.py
--rw-r--r--   0        0        0      201 2023-04-05 23:01:30.675827 boilercv-0.0.0/src/boilercv/old/_build.py
--rw-r--r--   0        0        0     1016 2023-04-10 18:39:05.118023 boilercv-0.0.0/src/boilercv/old/_contours.ipynb
--rw-r--r--   0        0        0     2958 2023-04-11 18:11:16.419679 boilercv-0.0.0/src/boilercv/old/_contours.py
--rw-r--r--   0        0        0     3227 2023-04-06 19:33:19.085431 boilercv-0.0.0/src/boilercv/old/_contours_mp4.py
--rw-r--r--   0        0        0     1422 2023-04-10 18:19:56.043597 boilercv-0.0.0/src/boilercv/old/_convert_2021_06.py
--rw-r--r--   0        0        0     3847 2023-04-11 18:11:14.931676 boilercv-0.0.0/src/boilercv/old/_detect_surface.py
--rw-r--r--   0        0        0      349 2023-04-05 23:01:30.682828 boilercv-0.0.0/src/boilercv/old/_remove_prefix.py
--rw-r--r--   0        0        0     1801 2023-04-10 23:42:14.231543 boilercv-0.0.0/src/boilercv/previews/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-11 19:41:44.490001 boilercv-0.0.0/src/boilercv/previews/__main__.py
--rw-r--r--   0        0        0      642 2023-04-11 19:17:46.279788 boilercv-0.0.0/src/boilercv/previews/binarized.py
--rw-r--r--   0        0        0     1035 2023-04-11 19:17:48.631213 boilercv-0.0.0/src/boilercv/previews/composite.py
--rw-r--r--   0        0        0      642 2023-04-11 19:17:28.036255 boilercv-0.0.0/src/boilercv/previews/filled.py
--rw-r--r--   0        0        0      582 2023-04-11 19:17:44.214788 boilercv-0.0.0/src/boilercv/previews/gray.py
--rw-r--r--   0        0        0       40 2023-03-22 20:29:54.936164 boilercv-0.0.0/src/boilercv/stages/__init__.py
--rw-r--r--   0        0        0       97 2023-04-06 19:28:58.069346 boilercv-0.0.0/src/boilercv/stages/check_cv.py
--rw-r--r--   0        0        0     1889 2023-04-05 23:02:31.490152 boilercv-0.0.0/src/boilercv/stages/contours.py
--rw-r--r--   0        0        0     1550 2023-04-12 00:33:44.414721 boilercv-0.0.0/src/boilercv/stages/fill.py
--rw-r--r--   0        0        0      641 2023-03-31 22:31:44.277170 boilercv-0.0.0/src/boilercv/stages/schema.py
--rw-r--r--   0        0        0     3167 2023-04-11 18:11:05.902444 boilercv-0.0.0/src/boilercv/stages/update_previews/__init__.py
--rw-r--r--   0        0        0      835 2023-04-07 00:33:11.765355 boilercv-0.0.0/src/boilercv/stages/update_previews/binarized.py
--rw-r--r--   0        0        0      767 2023-04-07 00:32:17.581476 boilercv-0.0.0/src/boilercv/stages/update_previews/filled.py
--rw-r--r--   0        0        0      768 2023-04-11 19:15:22.361642 boilercv-0.0.0/src/boilercv/stages/update_previews/gray.py
--rw-r--r--   0        0        0     1654 2023-04-10 23:10:56.256243 boilercv-0.0.0/src/boilercv/types.py
-drwxr-xr-x   0        0        0        0 2023-04-10 18:29:15.924636 boilercv-0.0.0/template/
--rw-r--r--   0        0        0        0 2023-03-08 22:27:34.144876 boilercv-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0       79 2023-04-10 18:19:56.135600 boilercv-0.0.0/tests/test_boilercv.py
-drwxr-xr-x   0        0        0        0 2023-03-06 21:38:04.898133 boilercv-0.0.0/typings/
--rw-r--r--   0        0        0     1568 2023-04-10 18:29:43.882896 boilercv-0.0.0/update.ps1
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 boilercv-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-04-14 20:46:11.637535 boilercv-0.0.1/.copier-answers.yml
+-rw-r--r--   0        0        0      512 2023-04-14 20:46:11.633535 boilercv-0.0.1/.coveragerc
+-rw-r--r--   0        0        0       26 2023-04-14 20:45:31.609519 boilercv-0.0.1/.dvc/.gitignore
+-rw-r--r--   0        0        0       92 2023-04-14 20:45:31.609519 boilercv-0.0.1/.dvc/config
+-rw-r--r--   0        0        0     3014 2023-04-14 20:46:11.693535 boilercv-0.0.1/.env
+-rw-r--r--   0        0        0     1032 2023-04-14 20:46:11.633535 boilercv-0.0.1/.gitattributes
+-rw-r--r--   0        0        0      319 2023-04-14 20:46:11.669535 boilercv-0.0.1/.github/workflows/changerelease.yml
+-rw-r--r--   0        0        0      676 2023-04-14 20:45:31.609519 boilercv-0.0.1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     2127 2023-04-14 20:46:11.693535 boilercv-0.0.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      409 2023-04-14 20:46:11.677535 boilercv-0.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      883 2023-04-14 20:46:11.693535 boilercv-0.0.1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0     5015 2023-04-14 20:46:11.693535 boilercv-0.0.1/.gitignore
+-rw-r--r--   0        0        0      516 2023-04-14 20:46:11.641535 boilercv-0.0.1/.gitmodules
+-rw-r--r--   0        0        0       45 2023-04-14 20:46:11.665535 boilercv-0.0.1/.markdownlint.yaml
+-rw-r--r--   0        0        0       95 2023-04-14 20:46:11.637535 boilercv-0.0.1/.nest_md
+-rw-r--r--   0        0        0       93 2023-04-14 20:46:11.681535 boilercv-0.0.1/.nest_tools_config
+-rw-r--r--   0        0        0     2189 2023-04-14 20:46:11.697535 boilercv-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      368 2023-04-14 20:46:11.697535 boilercv-0.0.1/.sourcery.yaml
+-rw-r--r--   0        0        0     5385 2023-04-14 20:46:11.697535 boilercv-0.0.1/.tools/pyproject.toml
+-rw-r--r--   0        0        0      552 2023-04-14 20:46:11.697535 boilercv-0.0.1/.tools/requirements/requirements_both.txt
+-rw-r--r--   0        0        0       25 2023-04-14 20:46:11.649535 boilercv-0.0.1/.tools/requirements/requirements_ci.txt
+-rw-r--r--   0        0        0      678 2023-04-14 20:46:11.645535 boilercv-0.0.1/.tools/requirements/requirements_dev.txt
+-rw-r--r--   0        0        0      433 2023-04-14 20:45:31.613519 boilercv-0.0.1/.tools/requirements/requirements_docs.txt
+-rw-r--r--   0        0        0      101 2023-04-14 20:45:31.613519 boilercv-0.0.1/.tools/requirements/requirements_nodeps.txt
+-rw-r--r--   0        0        0      234 2023-04-14 20:46:11.657535 boilercv-0.0.1/.tools/scripts/Copy-Template.ps1
+-rw-r--r--   0        0        0      416 2023-04-14 20:46:11.657535 boilercv-0.0.1/.tools/scripts/Update-Template.ps1
+-rw-r--r--   0        0        0      613 2023-04-14 20:46:11.697535 boilercv-0.0.1/.tools/scripts/compose_pyproject.py
+-rw-r--r--   0        0        0      230 2023-04-14 20:46:11.657535 boilercv-0.0.1/.tools/scripts/template_common.ps1
+-rw-r--r--   0        0        0      692 2023-04-14 20:45:31.613519 boilercv-0.0.1/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0     1046 2023-04-14 20:46:11.685535 boilercv-0.0.1/.vscode/extensions.json
+-rw-r--r--   0        0        0     3953 2023-04-14 20:46:11.697535 boilercv-0.0.1/.vscode/launch.json
+-rw-r--r--   0        0        0     7913 2023-04-14 20:46:11.697535 boilercv-0.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0    11204 2023-04-14 20:46:11.697535 boilercv-0.0.1/.vscode/tasks.json
+-rw-r--r--   0        0        0      801 2023-04-14 20:45:31.613519 boilercv-0.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      439 2023-04-14 20:45:31.613519 boilercv-0.0.1/CITATION.cff
+-rw-r--r--   0        0        0     6281 2023-04-14 20:46:11.645535 boilercv-0.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1072 2023-04-14 20:45:31.613519 boilercv-0.0.1/LICENSE
+-rw-r--r--   0        0        0     1206 2023-04-14 20:45:31.613519 boilercv-0.0.1/README.md
+-rw-r--r--   0        0        0     8047 2023-04-14 20:45:31.613519 boilercv-0.0.1/build.txt
+-rw-r--r--   0        0        0       52 2023-04-14 20:46:11.637535 boilercv-0.0.1/codecov.yml
+-rw-r--r--   0        0        0        6 2023-04-14 20:45:31.613519 boilercv-0.0.1/data/.dvcignore
+-rw-r--r--   0        0        0       45 2023-04-14 20:45:31.613519 boilercv-0.0.1/data/.gitignore
+-rw-r--r--   0        0        0       98 2023-04-14 20:45:31.613519 boilercv-0.0.1/data/examples.dvc
+-rw-r--r--   0        0        0       95 2023-04-14 20:45:31.613519 boilercv-0.0.1/data/rois.dvc
+-rw-r--r--   0        0        0       97 2023-04-14 20:45:31.613519 boilercv-0.0.1/data/samples.dvc
+-rw-r--r--   0        0        0       99 2023-04-14 20:45:31.613519 boilercv-0.0.1/data/sources.dvc
+-rw-r--r--   0        0        0       14 2023-04-14 20:45:31.613519 boilercv-0.0.1/docs/.gitignore
+-rw-r--r--   0        0        0   234596 2023-04-14 20:45:31.613519 boilercv-0.0.1/docs/_static/multicolor.png
+-rw-r--r--   0        0        0       73 2023-04-14 20:45:31.613519 boilercv-0.0.1/docs/changelog.md
+-rw-r--r--   0        0        0      360 2023-04-14 20:45:31.613519 boilercv-0.0.1/docs/conf.py
+-rw-r--r--   0        0        0      384 2023-04-14 20:45:31.613519 boilercv-0.0.1/docs/dag.md
+-rw-r--r--   0        0        0      926 2023-04-14 20:45:31.613519 boilercv-0.0.1/docs/index.md
+-rw-r--r--   0        0        0     4411 2023-04-14 20:45:31.613519 boilercv-0.0.1/dvc.lock
+-rw-r--r--   0        0        0     1307 2023-04-14 20:45:31.613519 boilercv-0.0.1/dvc.yaml
+-rw-r--r--   0        0        0     1029 2023-04-14 20:45:31.613519 boilercv-0.0.1/dvc_repro.ps1
+-rw-r--r--   0        0        0      978 2023-04-14 20:45:31.613519 boilercv-0.0.1/params.yaml
+-rw-r--r--   0        0        0     2121 2023-04-14 20:46:11.789535 boilercv-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1968 2023-04-14 20:46:11.697535 boilercv-0.0.1/pyrightconfig.json
+-rw-r--r--   0        0        0     3016 2023-04-14 20:46:11.665535 boilercv-0.0.1/pytest.ini
+-rw-r--r--   0        0        0      673 2023-04-14 20:46:11.633535 boilercv-0.0.1/pythonrc.py
+-rw-r--r--   0        0        0     2805 2023-04-14 20:46:11.697535 boilercv-0.0.1/renovate.json
+-rw-r--r--   0        0        0     6161 2023-04-14 20:45:31.613519 boilercv-0.0.1/repro.txt
+-rw-r--r--   0        0        0     1199 2023-04-14 20:45:31.613519 boilercv-0.0.1/requirements.txt
+-rw-r--r--   0        0        0      776 2023-04-14 20:46:11.681535 boilercv-0.0.1/setup.ps1
+-rw-r--r--   0        0        0     2209 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/captivate/__init__.py
+-rw-r--r--   0        0        0     2263 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/captivate/captures.py
+-rw-r--r--   0        0        0    11946 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/captivate/previews.py
+-rw-r--r--   0        0        0      339 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/colors.py
+-rw-r--r--   0        0        0     4037 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/data/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/data/frames.py
+-rw-r--r--   0        0        0     2702 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/data/models.py
+-rw-r--r--   0        0        0     1159 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/data/packing.py
+-rw-r--r--   0        0        0     5787 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/data/sets.py
+-rw-r--r--   0        0        0     3117 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/data/video.py
+-rw-r--r--   0        0        0      684 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/examples/__init__.py
+-rw-r--r--   0        0        0     1008 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/examples/blobs/__init__.py
+-rw-r--r--   0        0        0     1364 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/examples/blobs/bubbles.py
+-rw-r--r--   0        0        0     1008 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/examples/blobs/galaxy.py
+-rw-r--r--   0        0        0     1145 2023-04-14 20:45:31.613519 boilercv-0.0.1/src/boilercv/examples/contours.py
+-rw-r--r--   0        0        0     1054 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/cv/__init__.py
+-rw-r--r--   0        0        0      426 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/cv/__main__.py
+-rw-r--r--   0        0        0      587 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/cv/basic_test.py
+-rw-r--r--   0        0        0      412 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/cv/starry.py
+-rw-r--r--   0        0        0     4510 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/detect_surface.py
+-rw-r--r--   0        0        0     1811 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/fill.py
+-rw-r--r--   0        0        0     1576 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/__init__.py
+-rw-r--r--   0        0        0      373 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/binarize.py
+-rw-r--r--   0        0        0     1236 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/combined.py
+-rw-r--r--   0        0        0      386 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/compare.py
+-rw-r--r--   0        0        0      440 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/compress.py
+-rw-r--r--   0        0        0      475 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/compress_packed.py
+-rw-r--r--   0        0        0      481 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/convert.py
+-rw-r--r--   0        0        0      326 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/pack.py
+-rw-r--r--   0        0        0      343 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/large/unpack.py
+-rw-r--r--   0        0        0       95 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/previews/__init__.py
+-rw-r--r--   0        0        0     1164 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/previews/binarized_composite.py
+-rw-r--r--   0        0        0     1105 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/previews/gray_composite.py
+-rw-r--r--   0        0        0     1850 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/previews/multicolor_composite.py
+-rw-r--r--   0        0        0     1495 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/previews/triple_composite.py
+-rw-r--r--   0        0        0      792 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/examples/save_roi.py
+-rw-r--r--   0        0        0     3403 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/images/__init__.py
+-rw-r--r--   0        0        0     4936 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/images/cv.py
+-rw-r--r--   0        0        0       37 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/manual/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/manual/binarize.py
+-rw-r--r--   0        0        0      675 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/manual/convert.py
+-rw-r--r--   0        0        0      710 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/manual/decompress.py
+-rw-r--r--   0        0        0     1422 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/manual/rename.py
+-rw-r--r--   0        0        0     3023 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/models/__init__.py
+-rw-r--r--   0        0        0      486 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/models/params.py
+-rw-r--r--   0        0        0     4985 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/models/paths.py
+-rw-r--r--   0        0        0       50 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/old/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/old/_build.py
+-rw-r--r--   0        0        0      970 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/old/_contours.ipynb
+-rw-r--r--   0        0        0     2815 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/old/_contours.py
+-rw-r--r--   0        0        0     3127 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/old/_contours_mp4.py
+-rw-r--r--   0        0        0     1377 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/old/_convert_2021_06.py
+-rw-r--r--   0        0        0     3744 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/old/_detect_surface.py
+-rw-r--r--   0        0        0      334 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/old/_remove_prefix.py
+-rw-r--r--   0        0        0     1734 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/previews/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/previews/__main__.py
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/previews/binarized.py
+-rw-r--r--   0        0        0     1004 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/previews/composite.py
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/previews/filled.py
+-rw-r--r--   0        0        0      560 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/previews/gray.py
+-rw-r--r--   0        0        0       39 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/stages/__init__.py
+-rw-r--r--   0        0        0     2966 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/stages/contours.py
+-rw-r--r--   0        0        0     1388 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/stages/fill.py
+-rw-r--r--   0        0        0      617 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/stages/schema.py
+-rw-r--r--   0        0        0     3164 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/stages/update_previews/__init__.py
+-rw-r--r--   0        0        0      811 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/stages/update_previews/binarized.py
+-rw-r--r--   0        0        0      744 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/stages/update_previews/filled.py
+-rw-r--r--   0        0        0      745 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/stages/update_previews/gray.py
+-rw-r--r--   0        0        0     1589 2023-04-14 20:45:31.617519 boilercv-0.0.1/src/boilercv/types.py
+-rw-r--r--   0        0        0      463 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.copier-answers.yml
+-rw-r--r--   0        0        0      517 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.coveragerc
+-rw-r--r--   0        0        0     2976 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.env
+-rw-r--r--   0        0        0     1032 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.gitattributes
+-rw-r--r--   0        0        0     1945 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.github/workflows/main.yml
+-rw-r--r--   0        0        0     4307 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.gitignore
+-rw-r--r--   0        0        0       45 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.markdownlint.yaml
+-rw-r--r--   0        0        0       95 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.nest_md_top
+-rw-r--r--   0        0        0       93 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.nest_tools_config_top
+-rw-r--r--   0        0        0     2058 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      430 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.sourcery.yaml
+-rw-r--r--   0        0        0      443 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/requirements/requirements_both.txt
+-rw-r--r--   0        0        0       25 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/requirements/requirements_ci.txt
+-rw-r--r--   0        0        0      587 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/requirements/requirements_dev.txt
+-rw-r--r--   0        0        0      370 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/requirements/requirements_docs.txt
+-rw-r--r--   0        0        0      234 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/scripts/Copy-Template.ps1
+-rw-r--r--   0        0        0      416 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/scripts/Update-Template.ps1
+-rw-r--r--   0        0        0     1968 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/scripts/bump_requirements.py
+-rw-r--r--   0        0        0      621 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/scripts/compose_pyproject.py
+-rw-r--r--   0        0        0      230 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.tools/scripts/template_common.ps1
+-rw-r--r--   0        0        0     1046 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.vscode/extensions.json
+-rw-r--r--   0        0        0      744 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.vscode/launch.json
+-rw-r--r--   0        0        0     7479 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.vscode/settings.json
+-rw-r--r--   0        0        0     4999 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/.vscode/tasks.json
+-rw-r--r--   0        0        0      485 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/CHANGELOG.md
+-rw-r--r--   0        0        0     6301 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1072 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/LICENSE
+-rw-r--r--   0        0        0      597 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/README.md
+-rw-r--r--   0        0        0       52 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/codecov.yml
+-rw-r--r--   0        0        0     1380 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/copier.yml
+-rw-r--r--   0        0        0     2995 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/pyproject.toml
+-rw-r--r--   0        0        0      942 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/pyrightconfig.json
+-rw-r--r--   0        0        0     3018 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/pytest.ini
+-rw-r--r--   0        0        0      673 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/pythonrc.py
+-rw-r--r--   0        0        0     1118 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/renovate.json
+-rw-r--r--   0        0        0      776 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/setup.ps1
+-rw-r--r--   0        0        0      522 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.coveragerc.jinja
+-rw-r--r--   0        0        0     2976 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.env
+-rw-r--r--   0        0        0     1032 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.gitattributes
+-rw-r--r--   0        0        0      347 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.github/workflows/changerelease.yml.jinja
+-rw-r--r--   0        0        0      637 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.github/workflows/codeql-analysis.yml.jinja
+-rw-r--r--   0        0        0     1265 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.github/workflows/main.yml.jinja
+-rw-r--r--   0        0        0      453 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.github/workflows/publish.yml.jinja
+-rw-r--r--   0        0        0      993 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.github/workflows/sphinx.yml.jinja
+-rw-r--r--   0        0        0     4661 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.gitignore
+-rw-r--r--   0        0        0      516 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.gitmodules
+-rw-r--r--   0        0        0       45 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.markdownlint.yaml
+-rw-r--r--   0        0        0       95 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.nest_md
+-rw-r--r--   0        0        0       93 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.nest_tools_config
+-rw-r--r--   0        0        0     1962 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      334 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.sourcery.yaml.jinja
+-rw-r--r--   0        0        0     4807 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.tools/pyproject.toml.jinja
+-rw-r--r--   0        0        0      497 2023-04-14 20:45:32.473519 boilercv-0.0.1/template/template/.tools/requirements/requirements_both.txt
+-rw-r--r--   0        0        0       25 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.tools/requirements/requirements_ci.txt
+-rw-r--r--   0        0        0      678 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.tools/requirements/requirements_dev.txt
+-rw-r--r--   0        0        0      471 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.tools/requirements/{% if docs_engine == 'Jupyter Book' %}requirements_docs.txt{% endif %}
+-rw-r--r--   0        0        0      403 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.tools/requirements/{% if docs_engine == 'MyST' %}requirements_docs.txt{% endif %}
+-rw-r--r--   0        0        0      234 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.tools/scripts/Copy-Template.ps1
+-rw-r--r--   0        0        0      416 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.tools/scripts/Update-Template.ps1
+-rw-r--r--   0        0        0      621 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.tools/scripts/compose_pyproject.py
+-rw-r--r--   0        0        0      230 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.tools/scripts/template_common.ps1
+-rw-r--r--   0        0        0     1046 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.vscode/extensions.json
+-rw-r--r--   0        0        0      821 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.vscode/launch.json
+-rw-r--r--   0        0        0     7323 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.vscode/settings.json
+-rw-r--r--   0        0        0     5254 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/.vscode/tasks.json
+-rw-r--r--   0        0        0     6305 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/CODE_OF_CONDUCT.md.jinja
+-rw-r--r--   0        0        0       52 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/codecov.yml
+-rw-r--r--   0        0        0     1854 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/pyrightconfig.json
+-rw-r--r--   0        0        0     3016 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/pytest.ini
+-rw-r--r--   0        0        0      673 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/pythonrc.py
+-rw-r--r--   0        0        0     2681 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/renovate.json
+-rw-r--r--   0        0        0      808 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/setup.ps1.jinja
+-rw-r--r--   0        0        0     1366 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/update.ps1
+-rw-r--r--   0        0        0      100 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/template/{{ _copier_conf.answers_file }}.jinja
+-rw-r--r--   0        0        0     1366 2023-04-14 20:45:32.477519 boilercv-0.0.1/template/update.ps1
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:31.617519 boilercv-0.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       76 2023-04-14 20:45:31.617519 boilercv-0.0.1/tests/test_boilercv.py
+-rw-r--r--   0        0        0      389 2023-04-14 20:45:33.045518 boilercv-0.0.1/typings/.vscode/tasks.json
+-rw-r--r--   0        0        0     5971 2023-04-14 20:45:33.045518 boilercv-0.0.1/typings/README.md
+-rw-r--r--   0        0        0   564004 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/cv2-stubs/__init__.pyi
+-rw-r--r--   0        0        0        8 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/cv2-stubs/py.typed
+-rw-r--r--   0        0        0      157 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/__init__.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/apps/__init__.pyi
+-rw-r--r--   0        0        0      848 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/apps/config.pyi
+-rw-r--r--   0        0        0     2137 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/apps/registry.pyi
+-rw-r--r--   0        0        0      716 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/conf/__init__.pyi
+-rw-r--r--   0        0        0    17494 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/conf/global_settings.pyi
+-rw-r--r--   0        0        0       62 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/conf/locale/__init__.pyi
+-rw-r--r--   0        0        0     1064 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/conf/urls/__init__.pyi
+-rw-r--r--   0        0        0      313 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/conf/urls/i18n.pyi
+-rw-r--r--   0        0        0      188 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/conf/urls/static.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/__init__.pyi
+-rw-r--r--   0        0        0     1157 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/__init__.pyi
+-rw-r--r--   0        0        0      372 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/actions.pyi
+-rw-r--r--   0        0        0      142 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/apps.pyi
+-rw-r--r--   0        0        0      921 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/checks.pyi
+-rw-r--r--   0        0        0      977 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/decorators.pyi
+-rw-r--r--   0        0        0      198 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/exceptions.pyi
+-rw-r--r--   0        0        0     3842 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/filters.pyi
+-rw-r--r--   0        0        0      249 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/forms.pyi
+-rw-r--r--   0        0        0     4885 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/helpers.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/migrations/__init__.pyi
+-rw-r--r--   0        0        0     1142 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/models.pyi
+-rw-r--r--   0        0        0    15335 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/options.pyi
+-rw-r--r--   0        0        0     3536 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/sites.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/templatetags/__init__.pyi
+-rw-r--r--   0        0        0     2066 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/templatetags/admin_list.pyi
+-rw-r--r--   0        0        0      696 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/templatetags/admin_modify.pyi
+-rw-r--r--   0        0        0       73 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/templatetags/admin_static.pyi
+-rw-r--r--   0        0        0      557 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/templatetags/admin_urls.pyi
+-rw-r--r--   0        0        0      653 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/templatetags/base.pyi
+-rw-r--r--   0        0        0      454 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/templatetags/log.pyi
+-rw-r--r--   0        0        0     1469 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/tests.pyi
+-rw-r--r--   0        0        0     3351 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/utils.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/views/__init__.pyi
+-rw-r--r--   0        0        0      354 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/views/autocomplete.pyi
+-rw-r--r--   0        0        0      412 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/views/decorators.pyi
+-rw-r--r--   0        0        0     3708 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/views/main.pyi
+-rw-r--r--   0        0        0     3516 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admin/widgets.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admindocs/__init__.pyi
+-rw-r--r--   0        0        0      154 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admindocs/apps.pyi
+-rw-r--r--   0        0        0      462 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admindocs/middleware.pyi
+-rw-r--r--   0        0        0       59 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admindocs/urls.pyi
+-rw-r--r--   0        0        0      776 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admindocs/utils.pyi
+-rw-r--r--   0        0        0      882 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/admindocs/views.pyi
+-rw-r--r--   0        0        0     1339 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/__init__.pyi
+-rw-r--r--   0        0        0      655 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/admin.pyi
+-rw-r--r--   0        0        0       68 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/apps.pyi
+-rw-r--r--   0        0        0     1773 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/backends.pyi
+-rw-r--r--   0        0        0     1614 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/base_user.pyi
+-rw-r--r--   0        0        0      382 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/checks.pyi
+-rw-r--r--   0        0        0      617 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/context_processors.pyi
+-rw-r--r--   0        0        0     1011 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/decorators.pyi
+-rw-r--r--   0        0        0     3156 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/forms.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/handlers/__init__.pyi
+-rw-r--r--   0        0        0      204 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/handlers/modwsgi.pyi
+-rw-r--r--   0        0        0     2012 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/hashers.pyi
+-rw-r--r--   0        0        0      384 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/management/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/management/commands/__init__.pyi
+-rw-r--r--   0        0        0      125 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/management/commands/changepassword.pyi
+-rw-r--r--   0        0        0      208 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
+-rw-r--r--   0        0        0      774 2023-04-14 20:45:33.049518 boilercv-0.0.1/typings/django-stubs/contrib/auth/middleware.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/migrations/__init__.pyi
+-rw-r--r--   0        0        0     1202 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/mixins.pyi
+-rw-r--r--   0        0        0     4878 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/models.pyi
+-rw-r--r--   0        0        0     2118 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/password_validation.pyi
+-rw-r--r--   0        0        0      120 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/signals.pyi
+-rw-r--r--   0        0        0      673 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/tokens.pyi
+-rw-r--r--   0        0        0       59 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/urls.pyi
+-rw-r--r--   0        0        0      160 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/validators.pyi
+-rw-r--r--   0        0        0     2597 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/auth/views.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/__init__.pyi
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/admin.pyi
+-rw-r--r--   0        0        0       76 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/apps.pyi
+-rw-r--r--   0        0        0      330 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/checks.pyi
+-rw-r--r--   0        0        0     4413 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/fields.pyi
+-rw-r--r--   0        0        0     1187 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/forms.pyi
+-rw-r--r--   0        0        0     1380 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/management/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
+-rw-r--r--   0        0        0      410 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/migrations/__init__.pyi
+-rw-r--r--   0        0        0     1174 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/models.pyi
+-rw-r--r--   0        0        0      257 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/contenttypes/views.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/__init__.pyi
+-rw-r--r--   0        0        0      240 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/admin.pyi
+-rw-r--r--   0        0        0      154 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/apps.pyi
+-rw-r--r--   0        0        0      142 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/forms.pyi
+-rw-r--r--   0        0        0      313 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/middleware.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/migrations/__init__.pyi
+-rw-r--r--   0        0        0      451 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/models.pyi
+-rw-r--r--   0        0        0       81 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/sitemaps.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/templatetags/__init__.pyi
+-rw-r--r--   0        0        0      557 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
+-rw-r--r--   0        0        0       59 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/urls.pyi
+-rw-r--r--   0        0        0      315 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/flatpages/views.pyi
+-rw-r--r--   0        0        0       24 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/__init__.pyi
+-rw-r--r--   0        0        0      842 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/admin/__init__.pyi
+-rw-r--r--   0        0        0     1547 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/admin/options.pyi
+-rw-r--r--   0        0        0      254 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/admin/widgets.pyi
+-rw-r--r--   0        0        0      181 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/apps.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/base/__init__.pyi
+-rw-r--r--   0        0        0      208 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/base/adapter.pyi
+-rw-r--r--   0        0        0     1539 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/base/features.pyi
+-rw-r--r--   0        0        0      836 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/base/models.pyi
+-rw-r--r--   0        0        0     1421 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/base/operations.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
+-rw-r--r--   0        0        0      275 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/mysql/base.pyi
+-rw-r--r--   0        0        0      760 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/mysql/features.pyi
+-rw-r--r--   0        0        0      373 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
+-rw-r--r--   0        0        0      829 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
+-rw-r--r--   0        0        0      725 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
+-rw-r--r--   0        0        0      244 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
+-rw-r--r--   0        0        0      278 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/oracle/base.pyi
+-rw-r--r--   0        0        0      515 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/oracle/features.pyi
+-rw-r--r--   0        0        0      307 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
+-rw-r--r--   0        0        0      860 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/oracle/models.pyi
+-rw-r--r--   0        0        0     1724 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
+-rw-r--r--   0        0        0      876 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
+-rw-r--r--   0        0        0      419 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
+-rw-r--r--   0        0        0      384 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/base.pyi
+-rw-r--r--   0        0        0      189 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/const.pyi
+-rw-r--r--   0        0        0      478 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/features.pyi
+-rw-r--r--   0        0        0      406 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
+-rw-r--r--   0        0        0      947 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/models.pyi
+-rw-r--r--   0        0        0     2313 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
+-rw-r--r--   0        0        0      247 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
+-rw-r--r--   0        0        0      370 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
+-rw-r--r--   0        0        0      196 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
+-rw-r--r--   0        0        0      513 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
+-rw-r--r--   0        0        0      151 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
+-rw-r--r--   0        0        0      415 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
+-rw-r--r--   0        0        0      585 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
+-rw-r--r--   0        0        0      957 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
+-rw-r--r--   0        0        0     1425 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
+-rw-r--r--   0        0        0     1237 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
+-rw-r--r--   0        0        0      384 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/backends/utils.pyi
+-rw-r--r--   0        0        0      982 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/models/__init__.pyi
+-rw-r--r--   0        0        0     1173 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/models/aggregates.pyi
+-rw-r--r--   0        0        0     5066 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/models/fields.pyi
+-rw-r--r--   0        0        0     6356 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/models/functions.pyi
+-rw-r--r--   0        0        0     3356 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/models/lookups.pyi
+-rw-r--r--   0        0        0      375 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/models/proxy.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/models/sql/__init__.pyi
+-rw-r--r--   0        0        0      889 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/db/models/sql/conversion.pyi
+-rw-r--r--   0        0        0     1249 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/feeds.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/forms/__init__.pyi
+-rw-r--r--   0        0        0      977 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/forms/fields.pyi
+-rw-r--r--   0        0        0     1043 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/forms/widgets.pyi
+-rw-r--r--   0        0        0      651 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/__init__.pyi
+-rw-r--r--   0        0        0      159 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/base.pyi
+-rw-r--r--   0        0        0      548 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/datasource.pyi
+-rw-r--r--   0        0        0      342 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/driver.pyi
+-rw-r--r--   0        0        0      613 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/envelope.pyi
+-rw-r--r--   0        0        0      200 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/error.pyi
+-rw-r--r--   0        0        0      773 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/feature.pyi
+-rw-r--r--   0        0        0     1433 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/field.pyi
+-rw-r--r--   0        0        0     3907 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/geometries.pyi
+-rw-r--r--   0        0        0      312 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/geomtype.pyi
+-rw-r--r--   0        0        0      952 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/layer.pyi
+-rw-r--r--   0        0        0      436 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/libgdal.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
+-rw-r--r--   0        0        0     1036 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
+-rw-r--r--   0        0        0      986 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
+-rw-r--r--   0        0        0     1151 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
+-rw-r--r--   0        0        0      970 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
+-rw-r--r--   0        0        0     1053 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
+-rw-r--r--   0        0        0      614 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/raster/__init__.pyi
+-rw-r--r--   0        0        0     1386 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/raster/band.pyi
+-rw-r--r--   0        0        0      237 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/raster/base.pyi
+-rw-r--r--   0        0        0      236 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/raster/const.pyi
+-rw-r--r--   0        0        0     1787 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/raster/source.pyi
+-rw-r--r--   0        0        0     2057 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/gdal/srs.pyi
+-rw-r--r--   0        0        0      106 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geoip2/__init__.pyi
+-rw-r--r--   0        0        0     1000 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geoip2/base.pyi
+-rw-r--r--   0        0        0       99 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geoip2/resources.pyi
+-rw-r--r--   0        0        0       70 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geometry.pyi
+-rw-r--r--   0        0        0      781 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/__init__.pyi
+-rw-r--r--   0        0        0      159 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/base.pyi
+-rw-r--r--   0        0        0      626 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/collections.pyi
+-rw-r--r--   0        0        0     1143 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/coordseq.pyi
+-rw-r--r--   0        0        0       36 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/error.pyi
+-rw-r--r--   0        0        0      114 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/factory.pyi
+-rw-r--r--   0        0        0     4652 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/geometry.pyi
+-rw-r--r--   0        0        0      399 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/io.pyi
+-rw-r--r--   0        0        0      921 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/libgeos.pyi
+-rw-r--r--   0        0        0      726 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/linestring.pyi
+-rw-r--r--   0        0        0     1069 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/mutable_list.pyi
+-rw-r--r--   0        0        0      830 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/point.pyi
+-rw-r--r--   0        0        0      544 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/polygon.pyi
+-rw-r--r--   0        0        0      642 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prepared.pyi
+-rw-r--r--   0        0        0     4312 2023-04-14 20:45:33.053518 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
+-rw-r--r--   0        0        0      858 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
+-rw-r--r--   0        0        0      474 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
+-rw-r--r--   0        0        0      859 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/geom.pyi
+-rw-r--r--   0        0        0     3186 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/io.pyi
+-rw-r--r--   0        0        0      244 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/misc.pyi
+-rw-r--r--   0        0        0      596 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
+-rw-r--r--   0        0        0      471 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
+-rw-r--r--   0        0        0      562 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
+-rw-r--r--   0        0        0      646 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/geos/prototypes/topology.pyi
+-rw-r--r--   0        0        0     1341 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/measure.pyi
+-rw-r--r--   0        0        0      270 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/ptr.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/serializers/__init__.pyi
+-rw-r--r--   0        0        0      499 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/serializers/geojson.pyi
+-rw-r--r--   0        0        0      177 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/shortcuts.pyi
+-rw-r--r--   0        0        0      138 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/sitemaps/__init__.pyi
+-rw-r--r--   0        0        0      370 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/sitemaps/kml.pyi
+-rw-r--r--   0        0        0      324 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/sitemaps/views.pyi
+-rw-r--r--   0        0        0      300 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/utils/__init__.pyi
+-rw-r--r--   0        0        0     1991 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/utils/layermapping.pyi
+-rw-r--r--   0        0        0       92 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/utils/ogrinfo.pyi
+-rw-r--r--   0        0        0      194 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/utils/ogrinspect.pyi
+-rw-r--r--   0        0        0      218 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/utils/srs.pyi
+-rw-r--r--   0        0        0      111 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/gis/views.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/humanize/__init__.pyi
+-rw-r--r--   0        0        0      153 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/humanize/apps.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/humanize/templatetags/__init__.pyi
+-rw-r--r--   0        0        0      973 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/humanize/templatetags/humanize.pyi
+-rw-r--r--   0        0        0      721 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/__init__.pyi
+-rw-r--r--   0        0        0     1252 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/api.pyi
+-rw-r--r--   0        0        0      153 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/apps.pyi
+-rw-r--r--   0        0        0      187 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/constants.pyi
+-rw-r--r--   0        0        0      256 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/context_processors.pyi
+-rw-r--r--   0        0        0      363 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/middleware.pyi
+-rw-r--r--   0        0        0      168 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/storage/__init__.pyi
+-rw-r--r--   0        0        0      949 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/storage/base.pyi
+-rw-r--r--   0        0        0      487 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/storage/cookie.pyi
+-rw-r--r--   0        0        0      240 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/storage/fallback.pyi
+-rw-r--r--   0        0        0      496 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/storage/session.pyi
+-rw-r--r--   0        0        0       69 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/utils.pyi
+-rw-r--r--   0        0        0      308 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/messages/views.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/__init__.pyi
+-rw-r--r--   0        0        0      826 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/aggregates/__init__.pyi
+-rw-r--r--   0        0        0      338 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/aggregates/general.pyi
+-rw-r--r--   0        0        0       29 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/aggregates/mixins.pyi
+-rw-r--r--   0        0        0      470 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/aggregates/statistics.pyi
+-rw-r--r--   0        0        0      301 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/apps.pyi
+-rw-r--r--   0        0        0      584 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/constraints.pyi
+-rw-r--r--   0        0        0       86 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/expressions.pyi
+-rw-r--r--   0        0        0      860 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/fields/__init__.pyi
+-rw-r--r--   0        0        0     3072 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/fields/array.pyi
+-rw-r--r--   0        0        0     6791 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/fields/citext.pyi
+-rw-r--r--   0        0        0     3084 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/fields/hstore.pyi
+-rw-r--r--   0        0        0     1050 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/fields/jsonb.pyi
+-rw-r--r--   0        0        0      113 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/fields/mixins.pyi
+-rw-r--r--   0        0        0     1600 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/fields/ranges.pyi
+-rw-r--r--   0        0        0      106 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/fields/utils.pyi
+-rw-r--r--   0        0        0       95 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/functions.pyi
+-rw-r--r--   0        0        0     2519 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/indexes.pyi
+-rw-r--r--   0        0        0      608 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/lookups.pyi
+-rw-r--r--   0        0        0      964 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/operations.pyi
+-rw-r--r--   0        0        0     4274 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/search.pyi
+-rw-r--r--   0        0        0      177 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/serializers.pyi
+-rw-r--r--   0        0        0      237 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/signals.pyi
+-rw-r--r--   0        0        0      113 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/utils.pyi
+-rw-r--r--   0        0        0      699 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/postgres/validators.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/redirects/__init__.pyi
+-rw-r--r--   0        0        0      223 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/redirects/admin.pyi
+-rw-r--r--   0        0        0      154 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/redirects/apps.pyi
+-rw-r--r--   0        0        0      405 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/redirects/middleware.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/redirects/migrations/__init__.pyi
+-rw-r--r--   0        0        0      207 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/redirects/models.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/__init__.pyi
+-rw-r--r--   0        0        0      153 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/apps.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/backends/__init__.pyi
+-rw-r--r--   0        0        0     1570 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/backends/base.pyi
+-rw-r--r--   0        0        0      299 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/backends/cache.pyi
+-rw-r--r--   0        0        0      305 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/backends/cached_db.pyi
+-rw-r--r--   0        0        0      577 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/backends/db.pyi
+-rw-r--r--   0        0        0      283 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/backends/file.pyi
+-rw-r--r--   0        0        0      100 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/backends/signed_cookies.pyi
+-rw-r--r--   0        0        0      683 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/base_session.pyi
+-rw-r--r--   0        0        0      156 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/exceptions.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/management/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/management/commands/__init__.pyi
+-rw-r--r--   0        0        0       85 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
+-rw-r--r--   0        0        0      492 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/middleware.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/migrations/__init__.pyi
+-rw-r--r--   0        0        0      176 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/models.pyi
+-rw-r--r--   0        0        0      311 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sessions/serializers.pyi
+-rw-r--r--   0        0        0     1594 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sitemaps/__init__.pyi
+-rw-r--r--   0        0        0      153 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sitemaps/apps.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sitemaps/management/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
+-rw-r--r--   0        0        0       85 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
+-rw-r--r--   0        0        0      810 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sitemaps/views.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/__init__.pyi
+-rw-r--r--   0        0        0      164 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/admin.pyi
+-rw-r--r--   0        0        0       69 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/apps.pyi
+-rw-r--r--   0        0        0      288 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/management.pyi
+-rw-r--r--   0        0        0      180 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/managers.pyi
+-rw-r--r--   0        0        0      209 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/middleware.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/migrations/__init__.pyi
+-rw-r--r--   0        0        0      613 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/models.pyi
+-rw-r--r--   0        0        0      298 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/requests.pyi
+-rw-r--r--   0        0        0      266 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/sites/shortcuts.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/__init__.pyi
+-rw-r--r--   0        0        0      126 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/apps.pyi
+-rw-r--r--   0        0        0      247 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/checks.pyi
+-rw-r--r--   0        0        0     1764 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/finders.pyi
+-rw-r--r--   0        0        0      417 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/handlers.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/management/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
+-rw-r--r--   0        0        0     1167 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
+-rw-r--r--   0        0        0       87 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
+-rw-r--r--   0        0        0      120 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
+-rw-r--r--   0        0        0     2390 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/storage.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/templatetags/__init__.pyi
+-rw-r--r--   0        0        0      234 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/templatetags/staticfiles.pyi
+-rw-r--r--   0        0        0      100 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/testing.pyi
+-rw-r--r--   0        0        0      198 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/urls.pyi
+-rw-r--r--   0        0        0      465 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/utils.pyi
+-rw-r--r--   0        0        0      228 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/staticfiles/views.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/syndication/__init__.pyi
+-rw-r--r--   0        0        0      156 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/syndication/apps.pyi
+-rw-r--r--   0        0        0     1265 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/contrib/syndication/views.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/__init__.pyi
+-rw-r--r--   0        0        0       98 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/asgi.pyi
+-rw-r--r--   0        0        0      816 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/backends/__init__.pyi
+-rw-r--r--   0        0        0     3438 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/backends/base.pyi
+-rw-r--r--   0        0        0      595 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/backends/db.pyi
+-rw-r--r--   0        0        0      182 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/backends/dummy.pyi
+-rw-r--r--   0        0        0      216 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/backends/filebased.pyi
+-rw-r--r--   0        0        0      186 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/backends/locmem.pyi
+-rw-r--r--   0        0        0      446 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/backends/memcached.pyi
+-rw-r--r--   0        0        0      190 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/cache/utils.pyi
+-rw-r--r--   0        0        0      652 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/__init__.pyi
+-rw-r--r--   0        0        0      203 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/async_checks.pyi
+-rw-r--r--   0        0        0      278 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/caches.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/compatibility/__init__.pyi
+-rw-r--r--   0        0        0      103 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/database.pyi
+-rw-r--r--   0        0        0      966 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/messages.pyi
+-rw-r--r--   0        0        0      369 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/model_checks.pyi
+-rw-r--r--   0        0        0     1333 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/registry.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/security/__init__.pyi
+-rw-r--r--   0        0        0     1735 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/security/base.pyi
+-rw-r--r--   0        0        0      402 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/security/csrf.pyi
+-rw-r--r--   0        0        0      564 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/security/sessions.pyi
+-rw-r--r--   0        0        0      414 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/templates.pyi
+-rw-r--r--   0        0        0      255 2023-04-14 20:45:33.057519 boilercv-0.0.1/typings/django-stubs/core/checks/translation.pyi
+-rw-r--r--   0        0        0      831 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/checks/urls.pyi
+-rw-r--r--   0        0        0     1699 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/exceptions.pyi
+-rw-r--r--   0        0        0       68 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/__init__.pyi
+-rw-r--r--   0        0        0     1449 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/base.pyi
+-rw-r--r--   0        0        0      315 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/images.pyi
+-rw-r--r--   0        0        0      308 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/locks.pyi
+-rw-r--r--   0        0        0      143 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/move.pyi
+-rw-r--r--   0        0        0     1783 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/storage.pyi
+-rw-r--r--   0        0        0      100 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/temp.pyi
+-rw-r--r--   0        0        0     1510 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/uploadedfile.pyi
+-rw-r--r--   0        0        0     3172 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/uploadhandler.pyi
+-rw-r--r--   0        0        0      554 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/files/utils.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/handlers/__init__.pyi
+-rw-r--r--   0        0        0     1229 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/handlers/asgi.pyi
+-rw-r--r--   0        0        0      627 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/handlers/base.pyi
+-rw-r--r--   0        0        0      620 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/handlers/exception.pyi
+-rw-r--r--   0        0        0     1349 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/handlers/wsgi.pyi
+-rw-r--r--   0        0        0     1615 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/backends/__init__.pyi
+-rw-r--r--   0        0        0      629 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/backends/base.pyi
+-rw-r--r--   0        0        0      103 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/backends/console.pyi
+-rw-r--r--   0        0        0      103 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/backends/dummy.pyi
+-rw-r--r--   0        0        0      103 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/backends/filebased.pyi
+-rw-r--r--   0        0        0      103 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/backends/locmem.pyi
+-rw-r--r--   0        0        0      510 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/backends/smtp.pyi
+-rw-r--r--   0        0        0     4365 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/message.pyi
+-rw-r--r--   0        0        0       95 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/mail/utils.pyi
+-rw-r--r--   0        0        0      871 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/__init__.pyi
+-rw-r--r--   0        0        0     3030 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/base.pyi
+-rw-r--r--   0        0        0     1075 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/color.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/__init__.pyi
+-rw-r--r--   0        0        0      408 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/check.pyi
+-rw-r--r--   0        0        0      784 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/compilemessages.pyi
+-rw-r--r--   0        0        0      841 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/createcachetable.pyi
+-rw-r--r--   0        0        0      348 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/dbshell.pyi
+-rw-r--r--   0        0        0      573 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/diffsettings.pyi
+-rw-r--r--   0        0        0      123 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/dumpdata.pyi
+-rw-r--r--   0        0        0      669 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/flush.pyi
+-rw-r--r--   0        0        0     1013 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/inspectdb.pyi
+-rw-r--r--   0        0        0      625 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/loaddata.pyi
+-rw-r--r--   0        0        0     1167 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/makemessages.pyi
+-rw-r--r--   0        0        0     1734 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/makemigrations.pyi
+-rw-r--r--   0        0        0     1630 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/migrate.pyi
+-rw-r--r--   0        0        0      194 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/runserver.pyi
+-rw-r--r--   0        0        0      346 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/sendtestemail.pyi
+-rw-r--r--   0        0        0      424 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/shell.pyi
+-rw-r--r--   0        0        0      593 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/showmigrations.pyi
+-rw-r--r--   0        0        0      301 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/sqlflush.pyi
+-rw-r--r--   0        0        0      579 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/sqlmigrate.pyi
+-rw-r--r--   0        0        0      205 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/sqlsequencereset.pyi
+-rw-r--r--   0        0        0     1074 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/squashmigrations.pyi
+-rw-r--r--   0        0        0      149 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/startapp.pyi
+-rw-r--r--   0        0        0      217 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/startproject.pyi
+-rw-r--r--   0        0        0      454 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/test.pyi
+-rw-r--r--   0        0        0       85 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/commands/testserver.pyi
+-rw-r--r--   0        0        0      458 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/sql.pyi
+-rw-r--r--   0        0        0      659 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/templates.pyi
+-rw-r--r--   0        0        0      622 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/management/utils.pyi
+-rw-r--r--   0        0        0     1986 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/paginator.pyi
+-rw-r--r--   0        0        0     1468 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/serializers/__init__.pyi
+-rw-r--r--   0        0        0     3531 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/serializers/base.pyi
+-rw-r--r--   0        0        0      422 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/serializers/json.pyi
+-rw-r--r--   0        0        0      560 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/serializers/python.pyi
+-rw-r--r--   0        0        0      576 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/serializers/pyyaml.pyi
+-rw-r--r--   0        0        0     2600 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/serializers/xml_serializer.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/servers/__init__.pyi
+-rw-r--r--   0        0        0     1376 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/servers/basehttp.pyi
+-rw-r--r--   0        0        0      163 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/signals.pyi
+-rw-r--r--   0        0        0     1592 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/signing.pyi
+-rw-r--r--   0        0        0     4093 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/validators.pyi
+-rw-r--r--   0        0        0       98 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/core/wsgi.pyi
+-rw-r--r--   0        0        0     1236 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/__init__.pyi
+-rw-r--r--   0        0        0     4442 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/base.pyi
+-rw-r--r--   0        0        0      274 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/client.pyi
+-rw-r--r--   0        0        0     1239 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/creation.pyi
+-rw-r--r--   0        0        0     4258 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/features.pyi
+-rw-r--r--   0        0        0     1581 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/introspection.pyi
+-rw-r--r--   0        0        0     6530 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/operations.pyi
+-rw-r--r--   0        0        0     3550 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/schema.pyi
+-rw-r--r--   0        0        0      395 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/base/validation.pyi
+-rw-r--r--   0        0        0     3143 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/ddl_references.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/dummy/__init__.pyi
+-rw-r--r--   0        0        0     1029 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/dummy/base.pyi
+-rw-r--r--   0        0        0      250 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/dummy/features.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/__init__.pyi
+-rw-r--r--   0        0        0     1764 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/base.pyi
+-rw-r--r--   0        0        0      392 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/client.pyi
+-rw-r--r--   0        0        0      554 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/compiler.pyi
+-rw-r--r--   0        0        0      222 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/creation.pyi
+-rw-r--r--   0        0        0     2955 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/features.pyi
+-rw-r--r--   0        0        0     1042 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/introspection.pyi
+-rw-r--r--   0        0        0     2841 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/operations.pyi
+-rw-r--r--   0        0        0      922 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/schema.pyi
+-rw-r--r--   0        0        0      299 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/mysql/validation.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/__init__.pyi
+-rw-r--r--   0        0        0     2151 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/base.pyi
+-rw-r--r--   0        0        0      186 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/client.pyi
+-rw-r--r--   0        0        0      315 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/creation.pyi
+-rw-r--r--   0        0        0     2158 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/features.pyi
+-rw-r--r--   0        0        0      474 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/functions.pyi
+-rw-r--r--   0        0        0      957 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/introspection.pyi
+-rw-r--r--   0        0        0     3978 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/operations.pyi
+-rw-r--r--   0        0        0      944 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/schema.pyi
+-rw-r--r--   0        0        0      577 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/utils.pyi
+-rw-r--r--   0        0        0      252 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/oracle/validation.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/postgresql/__init__.pyi
+-rw-r--r--   0        0        0      459 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/postgresql/base.pyi
+-rw-r--r--   0        0        0      281 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/postgresql/client.pyi
+-rw-r--r--   0        0        0      117 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/postgresql/creation.pyi
+-rw-r--r--   0        0        0     2336 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/postgresql/features.pyi
+-rw-r--r--   0        0        0      789 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/postgresql/introspection.pyi
+-rw-r--r--   0        0        0      125 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/postgresql/operations.pyi
+-rw-r--r--   0        0        0      831 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/postgresql/schema.pyi
+-rw-r--r--   0        0        0       69 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/signals.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/sqlite3/__init__.pyi
+-rw-r--r--   0        0        0      369 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/sqlite3/base.pyi
+-rw-r--r--   0        0        0      158 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/sqlite3/client.pyi
+-rw-r--r--   0        0        0      117 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/sqlite3/creation.pyi
+-rw-r--r--   0        0        0      117 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/sqlite3/features.pyi
+-rw-r--r--   0        0        0      363 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/sqlite3/introspection.pyi
+-rw-r--r--   0        0        0      125 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/sqlite3/operations.pyi
+-rw-r--r--   0        0        0      127 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/sqlite3/schema.pyi
+-rw-r--r--   0        0        0     4249 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/backends/utils.pyi
+-rw-r--r--   0        0        0      312 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/__init__.pyi
+-rw-r--r--   0        0        0     3134 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/autodetector.pyi
+-rw-r--r--   0        0        0      723 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/exceptions.pyi
+-rw-r--r--   0        0        0     1763 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/executor.pyi
+-rw-r--r--   0        0        0     2647 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/graph.pyi
+-rw-r--r--   0        0        0     1903 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/loader.pyi
+-rw-r--r--   0        0        0     1245 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/migration.pyi
+-rw-r--r--   0        0        0     1043 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/operations/__init__.pyi
+-rw-r--r--   0        0        0      980 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/operations/base.pyi
+-rw-r--r--   0        0        0     1322 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/operations/fields.pyi
+-rw-r--r--   0        0        0     3226 2023-04-14 20:45:33.061519 boilercv-0.0.1/typings/django-stubs/db/migrations/operations/models.pyi
+-rw-r--r--   0        0        0     1397 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/operations/special.pyi
+-rw-r--r--   0        0        0      256 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/operations/utils.pyi
+-rw-r--r--   0        0        0      371 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/optimizer.pyi
+-rw-r--r--   0        0        0     1233 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/questioner.pyi
+-rw-r--r--   0        0        0      810 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/recorder.pyi
+-rw-r--r--   0        0        0     1855 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/serializer.pyi
+-rw-r--r--   0        0        0     2785 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/state.pyi
+-rw-r--r--   0        0        0      367 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/topological_sort.pyi
+-rw-r--r--   0        0        0      207 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/utils.pyi
+-rw-r--r--   0        0        0     1469 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/migrations/writer.pyi
+-rw-r--r--   0        0        0     4927 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/__init__.pyi
+-rw-r--r--   0        0        0      547 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/aggregates.pyi
+-rw-r--r--   0        0        0     3043 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/base.pyi
+-rw-r--r--   0        0        0       22 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/constants.pyi
+-rw-r--r--   0        0        0     1190 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/constraints.pyi
+-rw-r--r--   0        0        0     2050 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/deletion.pyi
+-rw-r--r--   0        0        0      997 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/enums.pyi
+-rw-r--r--   0        0        0     9344 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/expressions.pyi
+-rw-r--r--   0        0        0    58021 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/__init__.pyi
+-rw-r--r--   0        0        0     4945 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/files.pyi
+-rw-r--r--   0        0        0     7167 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/json.pyi
+-rw-r--r--   0        0        0      545 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/mixins.pyi
+-rw-r--r--   0        0        0      166 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/proxy.pyi
+-rw-r--r--   0        0        0    15632 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/related.pyi
+-rw-r--r--   0        0        0     3401 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/related_descriptors.pyi
+-rw-r--r--   0        0        0     1667 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/related_lookups.pyi
+-rw-r--r--   0        0        0     4208 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/fields/reverse_related.pyi
+-rw-r--r--   0        0        0     3225 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/functions/__init__.pyi
+-rw-r--r--   0        0        0      336 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/functions/comparison.pyi
+-rw-r--r--   0        0        0      972 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/functions/datetime.pyi
+-rw-r--r--   0        0        0     1235 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/functions/math.pyi
+-rw-r--r--   0        0        0      100 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/functions/mixins.pyi
+-rw-r--r--   0        0        0     2357 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/functions/text.pyi
+-rw-r--r--   0        0        0      748 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/functions/window.pyi
+-rw-r--r--   0        0        0     1557 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/indexes.pyi
+-rw-r--r--   0        0        0     5334 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/lookups.pyi
+-rw-r--r--   0        0        0     3188 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/manager.pyi
+-rw-r--r--   0        0        0     5311 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/options.pyi
+-rw-r--r--   0        0        0    12244 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/query.pyi
+-rw-r--r--   0        0        0     3178 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/query_utils.pyi
+-rw-r--r--   0        0        0      953 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/signals.pyi
+-rw-r--r--   0        0        0      284 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/sql/__init__.pyi
+-rw-r--r--   0        0        0     5780 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/sql/compiler.pyi
+-rw-r--r--   0        0        0      267 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/sql/constants.pyi
+-rw-r--r--   0        0        0     2009 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/sql/datastructures.pyi
+-rw-r--r--   0        0        0     9783 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/sql/query.pyi
+-rw-r--r--   0        0        0     1978 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/sql/subqueries.pyi
+-rw-r--r--   0        0        0     2046 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/sql/where.pyi
+-rw-r--r--   0        0        0      157 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/models/utils.pyi
+-rw-r--r--   0        0        0     2036 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/transaction.pyi
+-rw-r--r--   0        0        0     1330 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/db/utils.pyi
+-rw-r--r--   0        0        0      116 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/dispatch/__init__.pyi
+-rw-r--r--   0        0        0     1150 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/dispatch/dispatcher.pyi
+-rw-r--r--   0        0        0     4112 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/__init__.pyi
+-rw-r--r--   0        0        0     2407 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/boundfield.pyi
+-rw-r--r--   0        0        0    13708 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/fields.pyi
+-rw-r--r--   0        0        0     3178 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/forms.pyi
+-rw-r--r--   0        0        0     2600 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/formsets.pyi
+-rw-r--r--   0        0        0    10478 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/models.pyi
+-rw-r--r--   0        0        0      737 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/renderers.pyi
+-rw-r--r--   0        0        0     1272 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/utils.pyi
+-rw-r--r--   0        0        0     6446 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/forms/widgets.pyi
+-rw-r--r--   0        0        0     1273 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/http/__init__.pyi
+-rw-r--r--   0        0        0      132 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/http/cookie.pyi
+-rw-r--r--   0        0        0     2079 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/http/multipartparser.pyi
+-rw-r--r--   0        0        0     3900 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/http/request.pyi
+-rw-r--r--   0        0        0     5173 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/http/response.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/__init__.pyi
+-rw-r--r--   0        0        0     1128 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/cache.pyi
+-rw-r--r--   0        0        0      415 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/clickjacking.pyi
+-rw-r--r--   0        0        0     1043 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/common.pyi
+-rw-r--r--   0        0        0     1317 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/csrf.pyi
+-rw-r--r--   0        0        0      353 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/gzip.pyi
+-rw-r--r--   0        0        0      383 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/http.pyi
+-rw-r--r--   0        0        0      437 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/locale.pyi
+-rw-r--r--   0        0        0      743 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/middleware/security.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/py.typed
+-rw-r--r--   0        0        0     2170 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/shortcuts.pyi
+-rw-r--r--   0        0        0      756 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/backends/__init__.pyi
+-rw-r--r--   0        0        0      601 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/backends/base.pyi
+-rw-r--r--   0        0        0      726 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/backends/django.pyi
+-rw-r--r--   0        0        0      523 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/backends/dummy.pyi
+-rw-r--r--   0        0        0      591 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/backends/jinja2.pyi
+-rw-r--r--   0        0        0      211 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/backends/utils.pyi
+-rw-r--r--   0        0        0     6290 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/base.pyi
+-rw-r--r--   0        0        0     3313 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/context.pyi
+-rw-r--r--   0        0        0      664 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/context_processors.pyi
+-rw-r--r--   0        0        0     3741 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/defaultfilters.pyi
+-rw-r--r--   0        0        0     7308 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/defaulttags.pyi
+-rw-r--r--   0        0        0     2210 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/engine.pyi
+-rw-r--r--   0        0        0      596 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/exceptions.pyi
+-rw-r--r--   0        0        0     3349 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/library.pyi
+-rw-r--r--   0        0        0      636 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/loader.pyi
+-rw-r--r--   0        0        0     2386 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/loader_tags.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/loaders/__init__.pyi
+-rw-r--r--   0        0        0       88 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/loaders/app_directories.pyi
+-rw-r--r--   0        0        0      512 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/loaders/base.pyi
+-rw-r--r--   0        0        0      578 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/loaders/cached.pyi
+-rw-r--r--   0        0        0      433 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/loaders/filesystem.pyi
+-rw-r--r--   0        0        0      354 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/loaders/locmem.pyi
+-rw-r--r--   0        0        0     2396 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/response.pyi
+-rw-r--r--   0        0        0     1295 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/smartif.pyi
+-rw-r--r--   0        0        0      578 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/template/utils.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/templatetags/__init__.pyi
+-rw-r--r--   0        0        0      681 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/templatetags/cache.pyi
+-rw-r--r--   0        0        0     3200 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/templatetags/i18n.pyi
+-rw-r--r--   0        0        0      428 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/templatetags/l10n.pyi
+-rw-r--r--   0        0        0     1183 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/templatetags/static.pyi
+-rw-r--r--   0        0        0     1177 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/templatetags/tz.pyi
+-rw-r--r--   0        0        0      848 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/test/__init__.pyi
+-rw-r--r--   0        0        0     7064 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/test/client.pyi
+-rw-r--r--   0        0        0     1217 2023-04-14 20:45:33.065518 boilercv-0.0.1/typings/django-stubs/test/html.pyi
+-rw-r--r--   0        0        0     5424 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/test/runner.pyi
+-rw-r--r--   0        0        0      382 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/test/selenium.pyi
+-rw-r--r--   0        0        0      987 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/test/signals.pyi
+-rw-r--r--   0        0        0     8519 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/test/testcases.pyi
+-rw-r--r--   0        0        0     5636 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/test/utils.pyi
+-rw-r--r--   0        0        0     1474 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/urls/__init__.pyi
+-rw-r--r--   0        0        0      897 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/urls/base.pyi
+-rw-r--r--   0        0        0     1399 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/urls/conf.pyi
+-rw-r--r--   0        0        0      827 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/urls/converters.pyi
+-rw-r--r--   0        0        0      102 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/urls/exceptions.pyi
+-rw-r--r--   0        0        0     4359 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/urls/resolvers.pyi
+-rw-r--r--   0        0        0      193 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/urls/utils.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/__init__.pyi
+-rw-r--r--   0        0        0      321 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/_os.pyi
+-rw-r--r--   0        0        0     1043 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/archive.pyi
+-rw-r--r--   0        0        0       67 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/asyncio.pyi
+-rw-r--r--   0        0        0     2833 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/autoreload.pyi
+-rw-r--r--   0        0        0      607 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/baseconv.pyi
+-rw-r--r--   0        0        0     1357 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/cache.pyi
+-rw-r--r--   0        0        0      564 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/crypto.pyi
+-rw-r--r--   0        0        0     2843 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/datastructures.pyi
+-rw-r--r--   0        0        0     1878 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/dateformat.pyi
+-rw-r--r--   0        0        0      425 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/dateparse.pyi
+-rw-r--r--   0        0        0      181 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/dates.pyi
+-rw-r--r--   0        0        0      381 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/datetime_safe.pyi
+-rw-r--r--   0        0        0      105 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/deconstruct.pyi
+-rw-r--r--   0        0        0     1227 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/decorators.pyi
+-rw-r--r--   0        0        0     1412 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/deprecation.pyi
+-rw-r--r--   0        0        0      198 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/duration.pyi
+-rw-r--r--   0        0        0     1118 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/encoding.pyi
+-rw-r--r--   0        0        0     2888 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/feedgenerator.pyi
+-rw-r--r--   0        0        0     1307 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/formats.pyi
+-rw-r--r--   0        0        0     2202 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/functional.pyi
+-rw-r--r--   0        0        0       66 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/hashable.pyi
+-rw-r--r--   0        0        0     1399 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/html.pyi
+-rw-r--r--   0        0        0     1579 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/http.pyi
+-rw-r--r--   0        0        0      456 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/inspect.pyi
+-rw-r--r--   0        0        0      157 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/ipv6.pyi
+-rw-r--r--   0        0        0       61 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/itercompat.pyi
+-rw-r--r--   0        0        0      748 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/jslex.pyi
+-rw-r--r--   0        0        0     1548 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/log.pyi
+-rw-r--r--   0        0        0      248 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/lorem_ipsum.pyi
+-rw-r--r--   0        0        0      247 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/module_loading.pyi
+-rw-r--r--   0        0        0      344 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/numberformat.pyi
+-rw-r--r--   0        0        0      673 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/regex_helper.pyi
+-rw-r--r--   0        0        0      488 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/safestring.pyi
+-rw-r--r--   0        0        0     3491 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/six.pyi
+-rw-r--r--   0        0        0      550 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/termcolors.pyi
+-rw-r--r--   0        0        0     1625 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/text.pyi
+-rw-r--r--   0        0        0      381 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/timesince.pyi
+-rw-r--r--   0        0        0     2871 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/timezone.pyi
+-rw-r--r--   0        0        0      322 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/topological_sort.pyi
+-rw-r--r--   0        0        0     2546 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/translation/__init__.pyi
+-rw-r--r--   0        0        0      305 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/translation/reloader.pyi
+-rw-r--r--   0        0        0      235 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/translation/template.pyi
+-rw-r--r--   0        0        0      771 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/translation/trans_null.pyi
+-rw-r--r--   0        0        0     1910 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/translation/trans_real.pyi
+-rw-r--r--   0        0        0      824 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/tree.pyi
+-rw-r--r--   0        0        0      529 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/version.pyi
+-rw-r--r--   0        0        0      458 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/utils/xmlutils.pyi
+-rw-r--r--   0        0        0       39 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/__init__.pyi
+-rw-r--r--   0        0        0      280 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/csrf.pyi
+-rw-r--r--   0        0        0     2901 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/debug.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/decorators/__init__.pyi
+-rw-r--r--   0        0        0      329 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/decorators/cache.pyi
+-rw-r--r--   0        0        0      247 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/decorators/clickjacking.pyi
+-rw-r--r--   0        0        0      563 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/decorators/csrf.pyi
+-rw-r--r--   0        0        0      232 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/decorators/debug.pyi
+-rw-r--r--   0        0        0      129 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/decorators/gzip.pyi
+-rw-r--r--   0        0        0      651 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/decorators/http.pyi
+-rw-r--r--   0        0        0      191 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/decorators/vary.pyi
+-rw-r--r--   0        0        0      826 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/defaults.pyi
+-rw-r--r--   0        0        0      797 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/generic/__init__.pyi
+-rw-r--r--   0        0        0     2393 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/generic/base.pyi
+-rw-r--r--   0        0        0     3856 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/generic/dates.pyi
+-rw-r--r--   0        0        0     1118 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/generic/detail.pyi
+-rw-r--r--   0        0        0     2792 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/generic/edit.pyi
+-rw-r--r--   0        0        0     1727 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/generic/list.pyi
+-rw-r--r--   0        0        0     1306 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/i18n.pyi
+-rw-r--r--   0        0        0      480 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/django-stubs/views/static.pyi
+-rw-r--r--   0        0        0     1704 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/core.pyi
+-rw-r--r--   0        0        0      848 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/envs/registration.pyi
+-rw-r--r--   0        0        0      350 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/logger.pyi
+-rw-r--r--   0        0        0        8 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/py.typed
+-rw-r--r--   0        0        0      376 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/spaces/box.pyi
+-rw-r--r--   0        0        0      201 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/spaces/dict.pyi
+-rw-r--r--   0        0        0       93 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/spaces/discrete.pyi
+-rw-r--r--   0        0        0      154 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/spaces/multi_binary.pyi
+-rw-r--r--   0        0        0      139 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/spaces/multi_discrete.pyi
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/spaces/space.pyi
+-rw-r--r--   0        0        0      148 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/spaces/tuple.pyi
+-rw-r--r--   0        0        0      249 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/spaces/utils.pyi
+-rw-r--r--   0        0        0      491 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/vector/__init__.pyi
+-rw-r--r--   0        0        0      709 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/vector/async_vector_env.pyi
+-rw-r--r--   0        0        0      439 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/vector/sync_vector_env.pyi
+-rw-r--r--   0        0        0      965 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/vector/vector_env.pyi
+-rw-r--r--   0        0        0      174 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/gym-stubs/wrappers/time_limit.pyi
+-rw-r--r--   0        0        0     1154 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/__init__.pyi
+-rw-r--r--   0        0        0    47015 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/basic.pyi
+-rw-r--r--   0        0        0     4741 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/callback.pyi
+-rw-r--r--   0        0        0     2296 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/compat.pyi
+-rw-r--r--   0        0        0     7903 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/dask.pyi
+-rw-r--r--   0        0        0    16327 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/engine.pyi
+-rw-r--r--   0        0        0      337 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/libpath.pyi
+-rw-r--r--   0        0        0    13386 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/plotting.pyi
+-rw-r--r--   0        0        0        8 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/py.typed
+-rw-r--r--   0        0        0    19673 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/lightgbm-stubs/sklearn.pyi
+-rw-r--r--   0        0        0     1021 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/README.md
+-rw-r--r--   0        0        0     1645 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/__init__.pyi
+-rw-r--r--   0        0        0     1360 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_afm.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_api.pyi
+-rw-r--r--   0        0        0     1069 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_api/__init__.pyi
+-rw-r--r--   0        0        0     1361 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_api/deprecation.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_c_internal_utils.pyi
+-rw-r--r--   0        0        0      238 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_cm.pyi
+-rw-r--r--   0        0        0      162 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_color_data.pyi
+-rw-r--r--   0        0        0     1584 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_constrained_layout.pyi
+-rw-r--r--   0        0        0      576 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_docstring.pyi
+-rw-r--r--   0        0        0      401 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_enums.pyi
+-rw-r--r--   0        0        0      386 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_fontconfig_pattern.pyi
+-rw-r--r--   0        0        0     2258 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_layoutgrid.pyi
+-rw-r--r--   0        0        0     8347 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_mathtext.pyi
+-rw-r--r--   0        0        0      233 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_mathtext_data.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_preprocess_data.pyi
+-rw-r--r--   0        0        0      876 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_pylab_helpers.pyi
+-rw-r--r--   0        0        0      176 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_text_helpers.pyi
+-rw-r--r--   0        0        0      316 2023-04-14 20:45:33.069518 boilercv-0.0.1/typings/matplotlib/_tight_bbox.pyi
+-rw-r--r--   0        0        0      951 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/_tight_layout.pyi
+-rw-r--r--   0        0        0      459 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/_typing.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/_version.pyi
+-rw-r--r--   0        0        0     2550 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/afm.pyi
+-rw-r--r--   0        0        0     5670 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/animation.pyi
+-rw-r--r--   0        0        0     5055 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/artist.pyi
+-rw-r--r--   0        0        0       46 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/axes/__init__.pyi
+-rw-r--r--   0        0        0    20910 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/axes/_axes.pyi
+-rw-r--r--   0        0        0    11341 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/axes/_base.pyi
+-rw-r--r--   0        0        0     1009 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/axes/_secondary_axes.pyi
+-rw-r--r--   0        0        0      421 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/axes/_subplots.pyi
+-rw-r--r--   0        0        0     9447 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/axis.pyi
+-rw-r--r--   0        0        0    14651 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backend_bases.pyi
+-rw-r--r--   0        0        0     1704 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backend_managers.pyi
+-rw-r--r--   0        0        0     5926 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backend_tools.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/__init__.pyi
+-rw-r--r--   0        0        0     1584 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/_backend_gtk.pyi
+-rw-r--r--   0        0        0      809 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/_backend_pdf_ps.pyi
+-rw-r--r--   0        0        0     4010 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/_backend_tk.pyi
+-rw-r--r--   0        0        0     3134 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_agg.pyi
+-rw-r--r--   0        0        0     2430 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_cairo.pyi
+-rw-r--r--   0        0        0     2813 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_gtk3.pyi
+-rw-r--r--   0        0        0      481 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_gtk3agg.pyi
+-rw-r--r--   0        0        0      554 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_mixed.pyi
+-rw-r--r--   0        0        0     9185 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_pdf.pyi
+-rw-r--r--   0        0        0     3276 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_pgf.pyi
+-rw-r--r--   0        0        0     3838 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_ps.pyi
+-rw-r--r--   0        0        0     4547 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_qt.pyi
+-rw-r--r--   0        0        0      370 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_qtagg.pyi
+-rw-r--r--   0        0        0     3773 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_svg.pyi
+-rw-r--r--   0        0        0      389 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/backend_tkagg.pyi
+-rw-r--r--   0        0        0      122 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/backends/qt_compat.pyi
+-rw-r--r--   0        0        0     1817 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/bezier.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/blocking_input.pyi
+-rw-r--r--   0        0        0      978 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/category.pyi
+-rw-r--r--   0        0        0     4315 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/cbook/__init__.pyi
+-rw-r--r--   0        0        0     1659 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/cm.pyi
+-rw-r--r--   0        0        0     8459 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/collections.pyi
+-rw-r--r--   0        0        0     3748 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/colorbar.pyi
+-rw-r--r--   0        0        0     7748 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/colors.pyi
+-rw-r--r--   0        0        0     1684 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/container.pyi
+-rw-r--r--   0        0        0     2794 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/contour.pyi
+-rw-r--r--   0        0        0     6836 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/dates.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/docstring.pyi
+-rw-r--r--   0        0        0     1329 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/dviread.pyi
+-rw-r--r--   0        0        0    10343 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/figure.pyi
+-rw-r--r--   0        0        0     6043 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/font_manager.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/fontconfig_pattern.pyi
+-rw-r--r--   0        0        0    12512 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/ft2font.pyi
+-rw-r--r--   0        0        0     3268 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/gridspec.pyi
+-rw-r--r--   0        0        0     1474 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/hatch.pyi
+-rw-r--r--   0        0        0     6373 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/image.pyi
+-rw-r--r--   0        0        0     1506 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/layout_engine.pyi
+-rw-r--r--   0        0        0     3046 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/legend.pyi
+-rw-r--r--   0        0        0     6007 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/legend_handler.pyi
+-rw-r--r--   0        0        0     5143 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/lines.pyi
+-rw-r--r--   0        0        0     1235 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/markers.pyi
+-rw-r--r--   0        0        0     1611 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/mathtext.pyi
+-rw-r--r--   0        0        0     2368 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/mlab.pyi
+-rw-r--r--   0        0        0     8259 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/offsetbox.pyi
+-rw-r--r--   0        0        0    19257 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/patches.pyi
+-rw-r--r--   0        0        0     4064 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/path.pyi
+-rw-r--r--   0        0        0     3017 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/patheffects.pyi
+-rw-r--r--   0        0        0      407 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/projections/__init__.pyi
+-rw-r--r--   0        0        0     3698 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/projections/geo.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/projections/plot_directive.pyi
+-rw-r--r--   0        0        0     5651 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/projections/polar.pyi
+-rw-r--r--   0        0        0    25517 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/pyplot.pyi
+-rw-r--r--   0        0        0     2091 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/quiver.pyi
+-rw-r--r--   0        0        0     1901 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/rcsetup.pyi
+-rw-r--r--   0        0        0      964 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/sankey.pyi
+-rw-r--r--   0        0        0     4989 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/scale.pyi
+-rw-r--r--   0        0        0     2481 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/spines.pyi
+-rw-r--r--   0        0        0      365 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/stackplot.pyi
+-rw-r--r--   0        0        0     1766 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/streamplot.pyi
+-rw-r--r--   0        0        0      164 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/streamploy.pyi
+-rw-r--r--   0        0        0      373 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/style/__init__.pyi
+-rw-r--r--   0        0        0      732 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/style/core.pyi
+-rw-r--r--   0        0        0     3114 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/table.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/testing/__init__.pyi
+-rw-r--r--   0        0        0     1068 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/texmanager.pyi
+-rw-r--r--   0        0        0     7860 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/text.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/textmanager.pyi
+-rw-r--r--   0        0        0     1328 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/textpath.pyi
+-rw-r--r--   0        0        0    10842 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/ticker.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tight_layout.pyi
+-rw-r--r--   0        0        0    14107 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/transforms.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/__init__.pyi
+-rw-r--r--   0        0        0      834 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/triangulation.pyi
+-rw-r--r--   0        0        0      302 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/tricontour.pyi
+-rw-r--r--   0        0        0      354 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/trifinder.pyi
+-rw-r--r--   0        0        0     3544 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/triinterpolate.pyi
+-rw-r--r--   0        0        0      308 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/tripcolor.pyi
+-rw-r--r--   0        0        0      139 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/triplot.pyi
+-rw-r--r--   0        0        0      643 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/trirefine.pyi
+-rw-r--r--   0        0        0      390 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/tri/tritools.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.073518 boilercv-0.0.1/typings/matplotlib/type1font.pyi
+-rw-r--r--   0        0        0      982 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/matplotlib/units.pyi
+-rw-r--r--   0        0        0    12333 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/matplotlib/widgets.pyi
+-rw-r--r--   0        0        0       71 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/README.md
+-rw-r--r--   0        0        0     1659 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/__init__.pyi
+-rw-r--r--   0        0        0      459 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/_typing.pyi
+-rw-r--r--   0        0        0     9465 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/__init__.pyi
+-rw-r--r--   0        0        0     1587 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/__init__.pyi
+-rw-r--r--   0        0        0      346 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/clique.pyi
+-rw-r--r--   0        0        0      219 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/clustering_coefficient.pyi
+-rw-r--r--   0        0        0      427 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/connectivity.pyi
+-rw-r--r--   0        0        0      167 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/distance_measures.pyi
+-rw-r--r--   0        0        0      379 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/dominating_set.pyi
+-rw-r--r--   0        0        0      825 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/kcomponents.pyi
+-rw-r--r--   0        0        0      119 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/matching.pyi
+-rw-r--r--   0        0        0      451 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/maxcut.pyi
+-rw-r--r--   0        0        0      170 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/ramsey.pyi
+-rw-r--r--   0        0        0      323 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/steinertree.pyi
+-rw-r--r--   0        0        0     1462 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/traveling_salesman.pyi
+-rw-r--r--   0        0        0      480 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/treewidth.pyi
+-rw-r--r--   0        0        0      141 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/approximation/vertex_cover.pyi
+-rw-r--r--   0        0        0      984 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/assortativity/__init__.pyi
+-rw-r--r--   0        0        0      453 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/assortativity/connectivity.pyi
+-rw-r--r--   0        0        0      777 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/assortativity/correlation.pyi
+-rw-r--r--   0        0        0     1053 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/assortativity/mixing.pyi
+-rw-r--r--   0        0        0      216 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/assortativity/neighbor_degree.pyi
+-rw-r--r--   0        0        0      223 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/assortativity/pairs.pyi
+-rw-r--r--   0        0        0      306 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/asteroidal.pyi
+-rw-r--r--   0        0        0     2184 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/__init__.pyi
+-rw-r--r--   0        0        0      555 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/basic.pyi
+-rw-r--r--   0        0        0      345 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/centrality.pyi
+-rw-r--r--   0        0        0      634 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/cluster.pyi
+-rw-r--r--   0        0        0      287 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/covering.pyi
+-rw-r--r--   0        0        0      807 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/edgelist.pyi
+-rw-r--r--   0        0        0     1200 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/generators.pyi
+-rw-r--r--   0        0        0     1425 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/matching.pyi
+-rw-r--r--   0        0        0      395 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/matrix.pyi
+-rw-r--r--   0        0        0      843 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/projection.pyi
+-rw-r--r--   0        0        0      223 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/redundancy.pyi
+-rw-r--r--   0        0        0      157 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bipartite/spectral.pyi
+-rw-r--r--   0        0        0      446 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/boundary.pyi
+-rw-r--r--   0        0        0      317 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/bridges.pyi
+-rw-r--r--   0        0        0     3149 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/__init__.pyi
+-rw-r--r--   0        0        0      777 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/betweenness.pyi
+-rw-r--r--   0        0        0      578 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/betweenness_subset.pyi
+-rw-r--r--   0        0        0      515 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/closeness.pyi
+-rw-r--r--   0        0        0      962 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/current_flow_betweenness.pyi
+-rw-r--r--   0        0        0      604 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/current_flow_betweenness_subset.pyi
+-rw-r--r--   0        0        0      456 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/current_flow_closeness.pyi
+-rw-r--r--   0        0        0      348 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/degree_alg.pyi
+-rw-r--r--   0        0        0      238 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/dispersion.pyi
+-rw-r--r--   0        0        0      396 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/eigenvector.pyi
+-rw-r--r--   0        0        0     1115 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/flow_matrix.pyi
+-rw-r--r--   0        0        0      943 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/group.pyi
+-rw-r--r--   0        0        0      227 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/harmonic.pyi
+-rw-r--r--   0        0        0      529 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/katz.pyi
+-rw-r--r--   0        0        0      346 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/load.pyi
+-rw-r--r--   0        0        0      212 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/percolation.pyi
+-rw-r--r--   0        0        0      371 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/reaching.pyi
+-rw-r--r--   0        0        0      258 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/second_order.pyi
+-rw-r--r--   0        0        0      459 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/subgraph_alg.pyi
+-rw-r--r--   0        0        0      437 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/trophic.pyi
+-rw-r--r--   0        0        0      158 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/centrality/voterank_alg.pyi
+-rw-r--r--   0        0        0      160 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/chains.pyi
+-rw-r--r--   0        0        0      726 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/chordal.pyi
+-rw-r--r--   0        0        0     1688 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/clique.pyi
+-rw-r--r--   0        0        0      702 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/cluster.pyi
+-rw-r--r--   0        0        0      181 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/coloring/__init__.pyi
+-rw-r--r--   0        0        0      568 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/coloring/equitable_coloring.pyi
+-rw-r--r--   0        0        0     1595 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/coloring/greedy_coloring.pyi
+-rw-r--r--   0        0        0      270 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/communicability_alg.pyi
+-rw-r--r--   0        0        0      979 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/__init__.pyi
+-rw-r--r--   0        0        0      380 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/asyn_fluid.pyi
+-rw-r--r--   0        0        0      123 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/centrality.pyi
+-rw-r--r--   0        0        0      109 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/community_utils.pyi
+-rw-r--r--   0        0        0      171 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/kclique.pyi
+-rw-r--r--   0        0        0      391 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/kernighan_lin.pyi
+-rw-r--r--   0        0        0      466 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/label_propagation.pyi
+-rw-r--r--   0        0        0      488 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/louvain.pyi
+-rw-r--r--   0        0        0      482 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/lukes.pyi
+-rw-r--r--   0        0        0      661 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/modularity_max.pyi
+-rw-r--r--   0        0        0      921 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/community/quality.pyi
+-rw-r--r--   0        0        0     1402 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/components/__init__.pyi
+-rw-r--r--   0        0        0      450 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/components/attracting.pyi
+-rw-r--r--   0        0        0      415 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/components/biconnected.pyi
+-rw-r--r--   0        0        0      439 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/components/connected.pyi
+-rw-r--r--   0        0        0      243 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/components/semiconnected.pyi
+-rw-r--r--   0        0        0      652 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/components/strongly_connected.pyi
+-rw-r--r--   0        0        0      355 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/components/weakly_connected.pyi
+-rw-r--r--   0        0        0     1431 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/__init__.pyi
+-rw-r--r--   0        0        0     1202 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/connectivity.pyi
+-rw-r--r--   0        0        0      800 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/cuts.pyi
+-rw-r--r--   0        0        0      844 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/disjoint_paths.pyi
+-rw-r--r--   0        0        0     1320 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/edge_augmentation.pyi
+-rw-r--r--   0        0        0      630 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/edge_kcomponents.pyi
+-rw-r--r--   0        0        0      446 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/kcomponents.pyi
+-rw-r--r--   0        0        0      428 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/kcutsets.pyi
+-rw-r--r--   0        0        0      233 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/stoerwagner.pyi
+-rw-r--r--   0        0        0      228 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/connectivity/utils.pyi
+-rw-r--r--   0        0        0      763 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/core.pyi
+-rw-r--r--   0        0        0      319 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/covering.pyi
+-rw-r--r--   0        0        0     1005 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/cuts.pyi
+-rw-r--r--   0        0        0      498 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/cycles.pyi
+-rw-r--r--   0        0        0      207 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/d_separation.pyi
+-rw-r--r--   0        0        0     1731 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/dag.pyi
+-rw-r--r--   0        0        0      831 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/distance_measures.pyi
+-rw-r--r--   0        0        0      577 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/distance_regular.pyi
+-rw-r--r--   0        0        0      257 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/dominance.pyi
+-rw-r--r--   0        0        0      303 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/dominating.pyi
+-rw-r--r--   0        0        0      318 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/efficiency_measures.pyi
+-rw-r--r--   0        0        0      545 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/euler.pyi
+-rw-r--r--   0        0        0      975 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/__init__.pyi
+-rw-r--r--   0        0        0      424 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/boykovkolmogorov.pyi
+-rw-r--r--   0        0        0      336 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/capacityscaling.pyi
+-rw-r--r--   0        0        0      389 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/dinitz_alg.pyi
+-rw-r--r--   0        0        0      390 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/edmondskarp.pyi
+-rw-r--r--   0        0        0      291 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/gomory_hu.pyi
+-rw-r--r--   0        0        0      978 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/maxflow.pyi
+-rw-r--r--   0        0        0      584 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/mincost.pyi
+-rw-r--r--   0        0        0     1054 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/networksimplex.pyi
+-rw-r--r--   0        0        0      560 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/preflowpush.pyi
+-rw-r--r--   0        0        0      498 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/shortestaugmentingpath.pyi
+-rw-r--r--   0        0        0      742 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/flow/utils.pyi
+-rw-r--r--   0        0        0      590 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/graph_hashing.pyi
+-rw-r--r--   0        0        0      656 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/graphical.pyi
+-rw-r--r--   0        0        0      190 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/hierarchy.pyi
+-rw-r--r--   0        0        0      287 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/hybrid.pyi
+-rw-r--r--   0        0        0      209 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isolate.pyi
+-rw-r--r--   0        0        0     1390 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isomorphism/__init__.pyi
+-rw-r--r--   0        0        0     2933 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isomorphism/ismags.pyi
+-rw-r--r--   0        0        0      647 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isomorphism/isomorph.pyi
+-rw-r--r--   0        0        0     1498 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isomorphism/isomorphvf2.pyi
+-rw-r--r--   0        0        0     1788 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isomorphism/matchhelpers.pyi
+-rw-r--r--   0        0        0     1168 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isomorphism/temporalisomorphvf2.pyi
+-rw-r--r--   0        0        0      623 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isomorphism/tree_isomorphism.pyi
+-rw-r--r--   0        0        0     1015 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/isomorphism/vf2userfunc.pyi
+-rw-r--r--   0        0        0      398 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/link_analysis/__init__.pyi
+-rw-r--r--   0        0        0      554 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/link_analysis/hits_alg.pyi
+-rw-r--r--   0        0        0     1095 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/link_analysis/pagerank_alg.pyi
+-rw-r--r--   0        0        0      897 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/link_prediction.pyi
+-rw-r--r--   0        0        0      609 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/lowest_common_ancestors.pyi
+-rw-r--r--   0        0        0      825 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/matching.pyi
+-rw-r--r--   0        0        0      394 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/minors/__init__.pyi
+-rw-r--r--   0        0        0      807 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/minors/contraction.pyi
+-rw-r--r--   0        0        0      339 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/mis.pyi
+-rw-r--r--   0        0        0      151 2023-04-14 20:45:33.077519 boilercv-0.0.1/typings/networkx/algorithms/moral.pyi
+-rw-r--r--   0        0        0      134 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/node_classification/__init__.pyi
+-rw-r--r--   0        0        0      259 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/node_classification/hmn.pyi
+-rw-r--r--   0        0        0      302 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/node_classification/lgc.pyi
+-rw-r--r--   0        0        0       35 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/node_classification/utils.pyi
+-rw-r--r--   0        0        0      191 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/non_randomness.pyi
+-rw-r--r--   0        0        0      406 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/operators/__init__.pyi
+-rw-r--r--   0        0        0      331 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/operators/all.pyi
+-rw-r--r--   0        0        0      489 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/operators/binary.pyi
+-rw-r--r--   0        0        0      529 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/operators/product.pyi
+-rw-r--r--   0        0        0      149 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/operators/unary.pyi
+-rw-r--r--   0        0        0      667 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/planar_drawing.pyi
+-rw-r--r--   0        0        0     1966 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/planarity.pyi
+-rw-r--r--   0        0        0      238 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/polynomials.pyi
+-rw-r--r--   0        0        0      281 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/reciprocity.pyi
+-rw-r--r--   0        0        0      267 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/regular.pyi
+-rw-r--r--   0        0        0      261 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/richclub.pyi
+-rw-r--r--   0        0        0     2616 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/shortest_paths/__init__.pyi
+-rw-r--r--   0        0        0      313 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/shortest_paths/astar.pyi
+-rw-r--r--   0        0        0      530 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/shortest_paths/dense.pyi
+-rw-r--r--   0        0        0      598 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/shortest_paths/generic.pyi
+-rw-r--r--   0        0        0     1015 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/shortest_paths/unweighted.pyi
+-rw-r--r--   0        0        0     3191 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/shortest_paths/weighted.pyi
+-rw-r--r--   0        0        0     2803 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/similarity.pyi
+-rw-r--r--   0        0        0      702 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/simple_paths.pyi
+-rw-r--r--   0        0        0      532 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/smallworld.pyi
+-rw-r--r--   0        0        0      113 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/smetric.pyi
+-rw-r--r--   0        0        0      245 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/sparsifiers.pyi
+-rw-r--r--   0        0        0      494 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/structuralholes.pyi
+-rw-r--r--   0        0        0      445 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/summarization.pyi
+-rw-r--r--   0        0        0      357 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/swap.pyi
+-rw-r--r--   0        0        0     1830 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/threshold.pyi
+-rw-r--r--   0        0        0      833 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/tournament.pyi
+-rw-r--r--   0        0        0      707 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/traversal/__init__.pyi
+-rw-r--r--   0        0        0      179 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/traversal/beamsearch.pyi
+-rw-r--r--   0        0        0      789 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/traversal/breadth_first_search.pyi
+-rw-r--r--   0        0        0      752 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/traversal/depth_first_search.pyi
+-rw-r--r--   0        0        0      189 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/traversal/edgebfs.pyi
+-rw-r--r--   0        0        0      158 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/traversal/edgedfs.pyi
+-rw-r--r--   0        0        0     1315 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/tree/__init__.pyi
+-rw-r--r--   0        0        0     3846 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/tree/branchings.pyi
+-rw-r--r--   0        0        0      642 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/tree/coding.pyi
+-rw-r--r--   0        0        0      294 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/tree/decomposition.pyi
+-rw-r--r--   0        0        0     2389 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/tree/mst.pyi
+-rw-r--r--   0        0        0      237 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/tree/operations.pyi
+-rw-r--r--   0        0        0      262 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/tree/recognition.pyi
+-rw-r--r--   0        0        0     1302 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/triads.pyi
+-rw-r--r--   0        0        0      247 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/vitality.pyi
+-rw-r--r--   0        0        0      198 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/voronoi.pyi
+-rw-r--r--   0        0        0      386 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/algorithms/wiener.pyi
+-rw-r--r--   0        0        0     1142 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/__init__.pyi
+-rw-r--r--   0        0        0     3074 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/coreviews.pyi
+-rw-r--r--   0        0        0     2208 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/digraph.pyi
+-rw-r--r--   0        0        0      685 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/filters.pyi
+-rw-r--r--   0        0        0     2936 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/function.pyi
+-rw-r--r--   0        0        0     2883 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/graph.pyi
+-rw-r--r--   0        0        0      637 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/graphviews.pyi
+-rw-r--r--   0        0        0     1845 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/multidigraph.pyi
+-rw-r--r--   0        0        0     1767 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/multigraph.pyi
+-rw-r--r--   0        0        0     1195 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/ordered.pyi
+-rw-r--r--   0        0        0     5711 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/classes/reportviews.pyi
+-rw-r--r--   0        0        0      677 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/conftest.pyi
+-rw-r--r--   0        0        0      915 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/convert.pyi
+-rw-r--r--   0        0        0     2470 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/convert_matrix.pyi
+-rw-r--r--   0        0        0      715 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/drawing/__init__.pyi
+-rw-r--r--   0        0        0     2120 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/drawing/layout.pyi
+-rw-r--r--   0        0        0      916 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/drawing/nx_agraph.pyi
+-rw-r--r--   0        0        0      660 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/drawing/nx_pydot.pyi
+-rw-r--r--   0        0        0     2700 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/drawing/nx_pylab.pyi
+-rw-r--r--   0        0        0     1204 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/exception.pyi
+-rw-r--r--   0        0        0     3964 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/__init__.pyi
+-rw-r--r--   0        0        0     1672 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/atlas.pyi
+-rw-r--r--   0        0        0     1920 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/classic.pyi
+-rw-r--r--   0        0        0      164 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/cographs.pyi
+-rw-r--r--   0        0        0     1682 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/community.pyi
+-rw-r--r--   0        0        0     1784 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/degree_seq.pyi
+-rw-r--r--   0        0        0     1146 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/directed.pyi
+-rw-r--r--   0        0        0      414 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/duplication.pyi
+-rw-r--r--   0        0        0      170 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/ego.pyi
+-rw-r--r--   0        0        0     1073 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/expanders.pyi
+-rw-r--r--   0        0        0     1898 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/geometric.pyi
+-rw-r--r--   0        0        0      227 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/harary_graph.pyi
+-rw-r--r--   0        0        0      969 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/internet_as_graphs.pyi
+-rw-r--r--   0        0        0      490 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/intersection.pyi
+-rw-r--r--   0        0        0      138 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/interval_graph.pyi
+-rw-r--r--   0        0        0      571 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/joint_degree_seq.pyi
+-rw-r--r--   0        0        0      879 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/lattice.pyi
+-rw-r--r--   0        0        0      361 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/line.pyi
+-rw-r--r--   0        0        0      206 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/mycielski.pyi
+-rw-r--r--   0        0        0      211 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/nonisomorphic_trees.pyi
+-rw-r--r--   0        0        0      278 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/random_clustered.pyi
+-rw-r--r--   0        0        0     2650 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/random_graphs.pyi
+-rw-r--r--   0        0        0     2145 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/small.pyi
+-rw-r--r--   0        0        0      306 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/social.pyi
+-rw-r--r--   0        0        0      276 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/spectral_graph_forge.pyi
+-rw-r--r--   0        0        0      223 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/stochastic.pyi
+-rw-r--r--   0        0        0      128 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/sudoku.pyi
+-rw-r--r--   0        0        0      642 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/trees.pyi
+-rw-r--r--   0        0        0      537 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/generators/triads.pyi
+-rw-r--r--   0        0        0      388 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/lazy_imports.pyi
+-rw-r--r--   0        0        0      977 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/linalg/__init__.pyi
+-rw-r--r--   0        0        0      956 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/linalg/algebraicconnectivity.pyi
+-rw-r--r--   0        0        0      525 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/linalg/attrmatrix.pyi
+-rw-r--r--   0        0        0      285 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/linalg/bethehessianmatrix.pyi
+-rw-r--r--   0        0        0      361 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/linalg/graphmatrix.pyi
+-rw-r--r--   0        0        0     1062 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/linalg/laplacianmatrix.pyi
+-rw-r--r--   0        0        0      432 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/linalg/modularitymatrix.pyi
+-rw-r--r--   0        0        0      511 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/linalg/spectrum.pyi
+-rw-r--r--   0        0        0     1164 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/__init__.pyi
+-rw-r--r--   0        0        0      621 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/adjlist.pyi
+-rw-r--r--   0        0        0     1162 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/edgelist.pyi
+-rw-r--r--   0        0        0     2524 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/gexf.pyi
+-rw-r--r--   0        0        0     1294 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/gml.pyi
+-rw-r--r--   0        0        0      222 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/gpickle.pyi
+-rw-r--r--   0        0        0      932 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/graph6.pyi
+-rw-r--r--   0        0        0     3462 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/graphml.pyi
+-rw-r--r--   0        0        0      242 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/json_graph/__init__.pyi
+-rw-r--r--   0        0        0      339 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/json_graph/adjacency.pyi
+-rw-r--r--   0        0        0      311 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/json_graph/cytoscape.pyi
+-rw-r--r--   0        0        0      253 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/json_graph/jit.pyi
+-rw-r--r--   0        0        0      650 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/json_graph/node_link.pyi
+-rw-r--r--   0        0        0      451 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/json_graph/tree.pyi
+-rw-r--r--   0        0        0      407 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/leda.pyi
+-rw-r--r--   0        0        0      758 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/multiline_adjlist.pyi
+-rw-r--r--   0        0        0      295 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/nx_shp.pyi
+-rw-r--r--   0        0        0        2 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/nx_yaml.pyi
+-rw-r--r--   0        0        0      282 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/p2g.pyi
+-rw-r--r--   0        0        0      393 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/pajek.pyi
+-rw-r--r--   0        0        0      804 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/sparse6.pyi
+-rw-r--r--   0        0        0      257 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/readwrite/text.pyi
+-rw-r--r--   0        0        0      308 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/relabel.pyi
+-rw-r--r--   0        0        0      143 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/testing/__init__.pyi
+-rw-r--r--   0        0        0       66 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/testing/test.pyi
+-rw-r--r--   0        0        0      362 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/testing/utils.pyi
+-rw-r--r--   0        0        0     1054 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/__init__.pyi
+-rw-r--r--   0        0        0      157 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/contextmanagers.pyi
+-rw-r--r--   0        0        0     1706 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/decorators.pyi
+-rw-r--r--   0        0        0     1149 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/heaps.pyi
+-rw-r--r--   0        0        0      694 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/mapped_queue.pyi
+-rw-r--r--   0        0        0     2936 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/misc.pyi
+-rw-r--r--   0        0        0      828 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/random_sequence.pyi
+-rw-r--r--   0        0        0      443 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/rcm.pyi
+-rw-r--r--   0        0        0      217 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/networkx/utils/union_find.pyi
+-rw-r--r--   0        0        0     3687 2023-04-14 20:45:33.081519 boilercv-0.0.1/typings/pandas/__init__.pyi
+-rw-r--r--   0        0        0      220 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_config/__init__.pyi
+-rw-r--r--   0        0        0     3961 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_config/config.pyi
+-rw-r--r--   0        0        0      251 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/__init__.pyi
+-rw-r--r--   0        0        0      132 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/indexing.pyi
+-rw-r--r--   0        0        0     8083 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/interval.pyi
+-rw-r--r--   0        0        0      130 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/json.pyi
+-rw-r--r--   0        0        0      838 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/lib.pyi
+-rw-r--r--   0        0        0     1847 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/missing.pyi
+-rw-r--r--   0        0        0      126 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/ops_dispatch.pyi
+-rw-r--r--   0        0        0      408 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/properties.pyi
+-rw-r--r--   0        0        0       91 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/sparse.pyi
+-rw-r--r--   0        0        0      543 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/__init__.pyi
+-rw-r--r--   0        0        0       65 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/base.pyi
+-rw-r--r--   0        0        0      567 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/ccalendar.pyi
+-rw-r--r--   0        0        0      143 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/conversion.pyi
+-rw-r--r--   0        0        0     1143 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/dtypes.pyi
+-rw-r--r--   0        0        0     3421 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/nattype.pyi
+-rw-r--r--   0        0        0       87 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/np_datetime.pyi
+-rw-r--r--   0        0        0     7957 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/offsets.pyi
+-rw-r--r--   0        0        0      163 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/parsing.pyi
+-rw-r--r--   0        0        0     6317 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/period.pyi
+-rw-r--r--   0        0        0       72 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/strptime.pyi
+-rw-r--r--   0        0        0    13598 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/timedeltas.pyi
+-rw-r--r--   0        0        0    10432 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/timestamps.pyi
+-rw-r--r--   0        0        0       62 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/tzconversion.pyi
+-rw-r--r--   0        0        0      596 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/tslibs/vectorized.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_libs/window/__init__.pyi
+-rw-r--r--   0        0        0     6588 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_testing.pyi
+-rw-r--r--   0        0        0     3985 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_testing/__init__.pyi
+-rw-r--r--   0        0        0    14623 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_typing.pyi
+-rw-r--r--   0        0        0      117 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/_version.pyi
+-rw-r--r--   0        0        0       94 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/api/__init__.pyi
+-rw-r--r--   0        0        0      586 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/api/extensions/__init__.pyi
+-rw-r--r--   0        0        0      241 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/api/indexers/__init__.pyi
+-rw-r--r--   0        0        0      162 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/api/interchange/__init__.pyi
+-rw-r--r--   0        0        0     1909 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/api/types/__init__.pyi
+-rw-r--r--   0        0        0      373 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/arrays/__init__.pyi
+-rw-r--r--   0        0        0      268 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/compat/__init__.pyi
+-rw-r--r--   0        0        0      140 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/compat/_optional.pyi
+-rw-r--r--   0        0        0      137 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/compat/numpy/__init__.pyi
+-rw-r--r--   0        0        0      200 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/compat/pickle_compat.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/__init__.pyi
+-rw-r--r--   0        0        0      471 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/accessor.pyi
+-rw-r--r--   0        0        0     6314 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/algorithms.pyi
+-rw-r--r--   0        0        0     2698 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/api.pyi
+-rw-r--r--   0        0        0     2630 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/apply.pyi
+-rw-r--r--   0        0        0     1805 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arraylike.pyi
+-rw-r--r--   0        0        0      708 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/_arrow_utils.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/_ranges.pyi
+-rw-r--r--   0        0        0      310 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/arrow/dtype.pyi
+-rw-r--r--   0        0        0     2100 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/base.pyi
+-rw-r--r--   0        0        0      925 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/boolean.pyi
+-rw-r--r--   0        0        0     7190 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/categorical.pyi
+-rw-r--r--   0        0        0     2753 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/datetimelike.pyi
+-rw-r--r--   0        0        0     2136 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/datetimes.pyi
+-rw-r--r--   0        0        0      129 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/floating.pyi
+-rw-r--r--   0        0        0      980 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/integer.pyi
+-rw-r--r--   0        0        0     2354 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/interval.pyi
+-rw-r--r--   0        0        0      930 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/masked.pyi
+-rw-r--r--   0        0        0       96 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/numeric.pyi
+-rw-r--r--   0        0        0      496 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/numpy_.pyi
+-rw-r--r--   0        0        0     1608 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/period.pyi
+-rw-r--r--   0        0        0      204 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/sparse/__init__.pyi
+-rw-r--r--   0        0        0      595 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/sparse/accessor.pyi
+-rw-r--r--   0        0        0     2239 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/sparse/array.pyi
+-rw-r--r--   0        0        0      431 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/sparse/dtype.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/sparse/scipy_sparse.pyi
+-rw-r--r--   0        0        0      695 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/string_.pyi
+-rw-r--r--   0        0        0     1894 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/arrays/timedeltas.pyi
+-rw-r--r--   0        0        0     2593 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/base.pyi
+-rw-r--r--   0        0        0      925 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/common.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/__init__.pyi
+-rw-r--r--   0        0        0       79 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/align.pyi
+-rw-r--r--   0        0        0       54 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/api.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/check.pyi
+-rw-r--r--   0        0        0       46 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/common.pyi
+-rw-r--r--   0        0        0      421 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/engines.pyi
+-rw-r--r--   0        0        0      640 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/eval.pyi
+-rw-r--r--   0        0        0     2265 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/expr.pyi
+-rw-r--r--   0        0        0      270 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/expressions.pyi
+-rw-r--r--   0        0        0     2324 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/ops.pyi
+-rw-r--r--   0        0        0      475 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/parsing.pyi
+-rw-r--r--   0        0        0     3061 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/pytables.pyi
+-rw-r--r--   0        0        0      645 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/computation/scope.pyi
+-rw-r--r--   0        0        0     1621 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/config_init.pyi
+-rw-r--r--   0        0        0      893 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/construction.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/__init__.pyi
+-rw-r--r--   0        0        0     1584 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/api.pyi
+-rw-r--r--   0        0        0      804 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/base.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/cast.pyi
+-rw-r--r--   0        0        0     2321 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/common.pyi
+-rw-r--r--   0        0        0      295 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/concat.pyi
+-rw-r--r--   0        0        0     1627 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/dtypes.pyi
+-rw-r--r--   0        0        0      201 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/generic.pyi
+-rw-r--r--   0        0        0      591 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/inference.pyi
+-rw-r--r--   0        0        0      982 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/dtypes/missing.pyi
+-rw-r--r--   0        0        0   112087 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/frame.pyi
+-rw-r--r--   0        0        0    14519 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/generic.pyi
+-rw-r--r--   0        0        0      120 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/groupby/__init__.pyi
+-rw-r--r--   0        0        0      253 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/groupby/base.pyi
+-rw-r--r--   0        0        0      240 2023-04-14 20:45:33.085518 boilercv-0.0.1/typings/pandas/core/groupby/categorical.pyi
+-rw-r--r--   0        0        0    32672 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/groupby/generic.pyi
+-rw-r--r--   0        0        0     4021 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/groupby/groupby.pyi
+-rw-r--r--   0        0        0     1574 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/groupby/grouper.pyi
+-rw-r--r--   0        0        0     2623 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/groupby/ops.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/index.pyi
+-rw-r--r--   0        0        0     1621 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexers.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/__init__.pyi
+-rw-r--r--   0        0        0    12500 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/accessors.pyi
+-rw-r--r--   0        0        0      908 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/api.pyi
+-rw-r--r--   0        0        0     9701 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/base.pyi
+-rw-r--r--   0        0        0     1692 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/category.pyi
+-rw-r--r--   0        0        0      793 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/datetimelike.pyi
+-rw-r--r--   0        0        0     4275 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/datetimes.pyi
+-rw-r--r--   0        0        0       77 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/extension.pyi
+-rw-r--r--   0        0        0      429 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/frozen.pyi
+-rw-r--r--   0        0        0    12555 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/interval.pyi
+-rw-r--r--   0        0        0     5194 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/multi.pyi
+-rw-r--r--   0        0        0     1717 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/numeric.pyi
+-rw-r--r--   0        0        0     2841 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/period.pyi
+-rw-r--r--   0        0        0     2771 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/range.pyi
+-rw-r--r--   0        0        0     2635 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexes/timedeltas.pyi
+-rw-r--r--   0        0        0     1786 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/indexing.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/interchange/__init__.pyi
+-rw-r--r--   0        0        0     3047 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/interchange/dataframe_protocol.pyi
+-rw-r--r--   0        0        0       89 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/interchange/from_dataframe.pyi
+-rw-r--r--   0        0        0      606 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/internals/__init__.pyi
+-rw-r--r--   0        0        0     8221 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/internals/blocks.pyi
+-rw-r--r--   0        0        0      489 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/internals/concat.pyi
+-rw-r--r--   0        0        0      583 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/internals/construction.pyi
+-rw-r--r--   0        0        0     4342 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/internals/managers.pyi
+-rw-r--r--   0        0        0      338 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/missing.pyi
+-rw-r--r--   0        0        0     1631 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/nanops.pyi
+-rw-r--r--   0        0        0      204 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/__init__.pyi
+-rw-r--r--   0        0        0      504 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/array_ops.pyi
+-rw-r--r--   0        0        0       45 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/common.pyi
+-rw-r--r--   0        0        0      117 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/dispatch.pyi
+-rw-r--r--   0        0        0       17 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/docstrings.pyi
+-rw-r--r--   0        0        0       81 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/invalid.pyi
+-rw-r--r--   0        0        0      606 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/mask_ops.pyi
+-rw-r--r--   0        0        0       95 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/methods.pyi
+-rw-r--r--   0        0        0      130 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/missing.pyi
+-rw-r--r--   0        0        0      337 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/ops/roperator.pyi
+-rw-r--r--   0        0        0     6057 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/resample.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/__init__.pyi
+-rw-r--r--   0        0        0      609 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/api.pyi
+-rw-r--r--   0        0        0     2756 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/concat.pyi
+-rw-r--r--   0        0        0      684 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/encoding.pyi
+-rw-r--r--   0        0        0     3886 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/melt.pyi
+-rw-r--r--   0        0        0     9749 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/merge.pyi
+-rw-r--r--   0        0        0     7951 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/pivot.pyi
+-rw-r--r--   0        0        0      392 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/reshape.pyi
+-rw-r--r--   0        0        0     7458 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/tile.pyi
+-rw-r--r--   0        0        0       30 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/reshape/util.pyi
+-rw-r--r--   0        0        0   105999 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/series.pyi
+-rw-r--r--   0        0        0     1221 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/sorting.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/sparse/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/sparse/api.pyi
+-rw-r--r--   0        0        0     6483 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/strings.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/tools/__init__.pyi
+-rw-r--r--   0        0        0     2679 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/tools/datetimes.pyi
+-rw-r--r--   0        0        0      832 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/tools/numeric.pyi
+-rw-r--r--   0        0        0     1033 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/tools/timedeltas.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/util/__init__.pyi
+-rw-r--r--   0        0        0      458 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/util/hashing.pyi
+-rw-r--r--   0        0        0      274 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/window/__init__.pyi
+-rw-r--r--   0        0        0      503 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/window/common.pyi
+-rw-r--r--   0        0        0     2394 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/window/ewm.pyi
+-rw-r--r--   0        0        0     3695 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/window/expanding.pyi
+-rw-r--r--   0        0        0     2495 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/window/indexers.pyi
+-rw-r--r--   0        0        0      379 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/window/numba_.pyi
+-rw-r--r--   0        0        0     5593 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/core/window/rolling.pyi
+-rw-r--r--   0        0        0     1760 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/errors/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/__init__.pyi
+-rw-r--r--   0        0        0     1132 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/api.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/clipboard/__init__.pyi
+-rw-r--r--   0        0        0     7035 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/clipboards.pyi
+-rw-r--r--   0        0        0      470 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/common.pyi
+-rw-r--r--   0        0        0      241 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/date_converters.pyi
+-rw-r--r--   0        0        0      128 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/excel/__init__.pyi
+-rw-r--r--   0        0        0    20297 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/excel/_base.pyi
+-rw-r--r--   0        0        0       73 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/excel/_util.pyi
+-rw-r--r--   0        0        0      320 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/feather_format.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/__init__.pyi
+-rw-r--r--   0        0        0       93 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/console.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/css.pyi
+-rw-r--r--   0        0        0     1389 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/csvs.pyi
+-rw-r--r--   0        0        0     2075 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/excel.pyi
+-rw-r--r--   0        0        0      328 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/format.pyi
+-rw-r--r--   0        0        0     1626 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/html.pyi
+-rw-r--r--   0        0        0      814 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/latex.pyi
+-rw-r--r--   0        0        0      927 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/printing.pyi
+-rw-r--r--   0        0        0    11047 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/style.pyi
+-rw-r--r--   0        0        0     2352 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/formats/style_render.pyi
+-rw-r--r--   0        0        0      662 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/gbq.pyi
+-rw-r--r--   0        0        0      175 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/gcs.pyi
+-rw-r--r--   0        0        0     1330 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/html.pyi
+-rw-r--r--   0        0        0      167 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/json/__init__.pyi
+-rw-r--r--   0        0        0     3982 2023-04-14 20:45:33.089518 boilercv-0.0.1/typings/pandas/io/json/_json.pyi
+-rw-r--r--   0        0        0      389 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/json/_normalize.pyi
+-rw-r--r--   0        0        0      272 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/json/_table_schema.pyi
+-rw-r--r--   0        0        0      267 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/orc.pyi
+-rw-r--r--   0        0        0      402 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/parquet.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/parsers.pyi
+-rw-r--r--   0        0        0      162 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/parsers/__init__.pyi
+-rw-r--r--   0        0        0    15855 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/parsers/readers.pyi
+-rw-r--r--   0        0        0      536 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/pickle.pyi
+-rw-r--r--   0        0        0     6494 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/pytables.pyi
+-rw-r--r--   0        0        0      432 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/s3.pyi
+-rw-r--r--   0        0        0       57 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/sas/__init__.pyi
+-rw-r--r--   0        0        0      248 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/sas/sas7bdat.pyi
+-rw-r--r--   0        0        0     3457 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/sas/sas_constants.pyi
+-rw-r--r--   0        0        0      242 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/sas/sas_xport.pyi
+-rw-r--r--   0        0        0     2869 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/sas/sasreader.pyi
+-rw-r--r--   0        0        0      238 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/spss.pyi
+-rw-r--r--   0        0        0     4717 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/sql.pyi
+-rw-r--r--   0        0        0     8815 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/stata.pyi
+-rw-r--r--   0        0        0      981 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/io/xml.pyi
+-rw-r--r--   0        0        0      567 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/__init__.pyi
+-rw-r--r--   0        0        0    12425 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_core.pyi
+-rw-r--r--   0        0        0      659 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/__init__.pyi
+-rw-r--r--   0        0        0     1173 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/boxplot.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/compat.pyi
+-rw-r--r--   0        0        0     2746 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/converter.pyi
+-rw-r--r--   0        0        0     2494 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/core.pyi
+-rw-r--r--   0        0        0      897 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/hist.pyi
+-rw-r--r--   0        0        0      890 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/misc.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/style.pyi
+-rw-r--r--   0        0        0       55 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/timeseries.pyi
+-rw-r--r--   0        0        0      110 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_matplotlib/tools.pyi
+-rw-r--r--   0        0        0     2273 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/plotting/_misc.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/py.typed
+-rw-r--r--   0        0        0      368 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/testing.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/tseries/__init__.pyi
+-rw-r--r--   0        0        0       64 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/tseries/api.pyi
+-rw-r--r--   0        0        0      366 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/tseries/frequencies.pyi
+-rw-r--r--   0        0        0      115 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/tseries/holiday.pyi
+-rw-r--r--   0        0        0     1312 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/tseries/offsets.pyi
+-rw-r--r--   0        0        0      245 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/__init__.pyi
+-rw-r--r--   0        0        0     1187 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/_decorators.pyi
+-rw-r--r--   0        0        0      317 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/_depr_module.pyi
+-rw-r--r--   0        0        0      279 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/_doctools.pyi
+-rw-r--r--   0        0        0       57 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/_exceptions.pyi
+-rw-r--r--   0        0        0       52 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/_print_versions.pyi
+-rw-r--r--   0        0        0      607 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/_test_decorators.pyi
+-rw-r--r--   0        0        0       38 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/_tester.pyi
+-rw-r--r--   0        0        0      581 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/_validators.pyi
+-rw-r--r--   0        0        0     1834 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/pandas/util/version/__init__.pyi
+-rw-r--r--   0        0        0     1560 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/_lib/_ccallback_c.pyi
+-rw-r--r--   0        0        0      520 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/_lib/_fpumode.pyi
+-rw-r--r--   0        0        0      697 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/_lib/_test_ccallback.pyi
+-rw-r--r--   0        0        0      397 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/_lib/_test_deprecation_call.pyi
+-rw-r--r--   0        0        0      380 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/_lib/_test_deprecation_def.pyi
+-rw-r--r--   0        0        0      766 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/_lib/_uarray/_uarray.pyi
+-rw-r--r--   0        0        0     1860 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/_lib/messagestream.pyi
+-rw-r--r--   0        0        0    12481 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/cluster/_hierarchy.pyi
+-rw-r--r--   0        0        0     5220 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/cluster/_optimal_leaf_ordering.pyi
+-rw-r--r--   0        0        0     1652 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/cluster/_vq.pyi
+-rw-r--r--   0        0        0    12136 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/fft/_pocketfft/pypocketfft.pyi
+-rw-r--r--   0        0        0     3923 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/fftpack/convolve.pyi
+-rw-r--r--   0        0        0     3702 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/integrate/_dop.pyi
+-rw-r--r--   0        0        0      873 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/integrate/_odepack.pyi
+-rw-r--r--   0        0        0     1875 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/integrate/_quadpack.pyi
+-rw-r--r--   0        0        0      476 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/integrate/_test_multivariate.pyi
+-rw-r--r--   0        0        0     2208 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/integrate/_test_odeint_banded.pyi
+-rw-r--r--   0        0        0     1824 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/integrate/lsoda.pyi
+-rw-r--r--   0        0        0     3308 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/integrate/vode.pyi
+-rw-r--r--   0        0        0     6666 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/interpolate/_bspl.pyi
+-rw-r--r--   0        0        0     2841 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/interpolate/_fitpack.pyi
+-rw-r--r--   0        0        0     6091 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/interpolate/_ppoly.pyi
+-rw-r--r--   0        0        0    17762 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/interpolate/dfitpack.pyi
+-rw-r--r--   0        0        0    16912 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/interpolate/interpnd.pyi
+-rw-r--r--   0        0        0     1384 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/io/_test_fortran.pyi
+-rw-r--r--   0        0        0     9064 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/io/matlab/mio5_utils.pyi
+-rw-r--r--   0        0        0      902 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/io/matlab/mio_utils.pyi
+-rw-r--r--   0        0        0     4248 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/io/matlab/streams.pyi
+-rw-r--r--   0        0        0    15070 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/linalg/_decomp_update.pyi
+-rw-r--r--   0        0        0   102616 2023-04-14 20:45:33.093518 boilercv-0.0.1/typings/scipy-stubs/linalg/_fblas.pyi
+-rw-r--r--   0        0        0   349604 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/linalg/_flapack.pyi
+-rw-r--r--   0        0        0     5080 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/linalg/_flinalg.pyi
+-rw-r--r--   0        0        0    41556 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/linalg/_interpolative.pyi
+-rw-r--r--   0        0        0      622 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/linalg/_matfuncs_sqrtm_triu.pyi
+-rw-r--r--   0        0        0     6784 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/linalg/_solve_toeplitz.pyi
+-rw-r--r--   0        0        0     1219 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/linalg/cython_blas.pyi
+-rw-r--r--   0        0        0      453 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/linalg/cython_lapack.pyi
+-rw-r--r--   0        0        0      452 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/ndimage/_ctest.pyi
+-rw-r--r--   0        0        0      629 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/ndimage/_cytest.pyi
+-rw-r--r--   0        0        0     1264 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/ndimage/_nd_image.pyi
+-rw-r--r--   0        0        0      656 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/ndimage/_ni_label.pyi
+-rw-r--r--   0        0        0     1656 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/odr/__odrpack.pyi
+-rw-r--r--   0        0        0     1168 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/__nnls.pyi
+-rw-r--r--   0        0        0    14840 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_bglu_dense.pyi
+-rw-r--r--   0        0        0     1323 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_cobyla.pyi
+-rw-r--r--   0        0        0      486 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_group_columns.pyi
+-rw-r--r--   0        0        0     1538 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_highs/_highs_constants.pyi
+-rw-r--r--   0        0        0    12578 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_highs/_highs_wrapper.pyi
+-rw-r--r--   0        0        0     1481 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_highs/_mpswriter.pyi
+-rw-r--r--   0        0        0     1533 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_lbfgsb.pyi
+-rw-r--r--   0        0        0      445 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_lsap_module.pyi
+-rw-r--r--   0        0        0     1228 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_lsq/givens_elimination.pyi
+-rw-r--r--   0        0        0     1434 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_minpack.pyi
+-rw-r--r--   0        0        0     2271 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_slsqp.pyi
+-rw-r--r--   0        0        0     2812 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_trlib/_trlib.pyi
+-rw-r--r--   0        0        0      519 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/_zeros.pyi
+-rw-r--r--   0        0        0     2155 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/cython_optimize/_zeros.pyi
+-rw-r--r--   0        0        0     1560 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/minpack2.pyi
+-rw-r--r--   0        0        0      377 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/optimize/moduleTNC.pyi
+-rw-r--r--   0        0        0        8 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/py.typed
+-rw-r--r--   0        0        0      459 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/signal/_max_len_seq_inner.pyi
+-rw-r--r--   0        0        0     5966 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/signal/_peak_finding_utils.pyi
+-rw-r--r--   0        0        0      495 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/signal/_sosfilt.pyi
+-rw-r--r--   0        0        0      993 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/signal/_spectral.pyi
+-rw-r--r--   0        0        0      806 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/signal/_upfirdn_apply.pyi
+-rw-r--r--   0        0        0     1518 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/signal/sigtools.pyi
+-rw-r--r--   0        0        0     4958 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/signal/spline.pyi
+-rw-r--r--   0        0        0     5523 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/_csparsetools.pyi
+-rw-r--r--   0        0        0     3762 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/_sparsetools.pyi
+-rw-r--r--   0        0        0    10443 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/csgraph/_flow.pyi
+-rw-r--r--   0        0        0    14110 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/csgraph/_matching.pyi
+-rw-r--r--   0        0        0     4705 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/csgraph/_min_spanning_tree.pyi
+-rw-r--r--   0        0        0    11442 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/csgraph/_reordering.pyi
+-rw-r--r--   0        0        0    22971 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/csgraph/_shortest_path.pyi
+-rw-r--r--   0        0        0    15343 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/csgraph/_tools.pyi
+-rw-r--r--   0        0        0    16485 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/csgraph/_traversal.pyi
+-rw-r--r--   0        0        0     7071 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/linalg/_eigen/lobpcg/lobpcg.pyi
+-rw-r--r--   0        0        0     1513 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/linalg/dsolve/_superlu.pyi
+-rw-r--r--   0        0        0    17296 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/linalg/eigen/arpack/_arpack.pyi
+-rw-r--r--   0        0        0    17308 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/sparse/linalg/isolve/_iterative.pyi
+-rw-r--r--   0        0        0     3545 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/spatial/_distance_wrap.pyi
+-rw-r--r--   0        0        0      459 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/spatial/_hausdorff.pyi
+-rw-r--r--   0        0        0      463 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/spatial/_voronoi.pyi
+-rw-r--r--   0        0        0    38821 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/spatial/ckdtree.pyi
+-rw-r--r--   0        0        0    63956 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/spatial/qhull.pyi
+-rw-r--r--   0        0        0    65293 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/spatial/transform/rotation.pyi
+-rw-r--r--   0        0        0      388 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/special/_comb.pyi
+-rw-r--r--   0        0        0      595 2023-04-14 20:45:33.097519 boilercv-0.0.1/typings/scipy-stubs/special/_ellip_harm_2.pyi
+-rw-r--r--   0        0        0      924 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/scipy-stubs/special/_test_round.pyi
+-rw-r--r--   0        0        0   290997 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/scipy-stubs/special/_ufuncs.pyi
+-rw-r--r--   0        0        0      373 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/scipy-stubs/special/_ufuncs_cxx.pyi
+-rw-r--r--   0        0        0    21038 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/scipy-stubs/special/cython_special.pyi
+-rw-r--r--   0        0        0     7170 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/scipy-stubs/special/specfun.pyi
+-rw-r--r--   0        0        0     1727 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/scipy-stubs/stats/_stats.pyi
+-rw-r--r--   0        0        0     2529 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/scipy-stubs/stats/mvn.pyi
+-rw-r--r--   0        0        0     1287 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/scipy-stubs/stats/statlib.pyi
+-rw-r--r--   0        0        0     1888 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/seaborn-stubs/palettes.pyi
+-rw-r--r--   0        0        0        8 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/seaborn-stubs/py.typed
+-rw-r--r--   0        0        0      199 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/README.md
+-rw-r--r--   0        0        0       39 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/__check_build/__init__.pyi
+-rw-r--r--   0        0        0       32 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/__check_build/_check_build.pyi
+-rw-r--r--   0        0        0      253 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/__check_build/setup.pyi
+-rw-r--r--   0        0        0      873 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/__init__.pyi
+-rw-r--r--   0        0        0      609 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_build_utils/__init__.pyi
+-rw-r--r--   0        0        0      411 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_build_utils/openmp_helpers.pyi
+-rw-r--r--   0        0        0      339 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_build_utils/pre_build_helpers.pyi
+-rw-r--r--   0        0        0     1081 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_config.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_distributor_init.pyi
+-rw-r--r--   0        0        0      623 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_loss/__init__.pyi
+-rw-r--r--   0        0        0     2900 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_loss/_loss.pyi
+-rw-r--r--   0        0        0     1732 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_loss/glm_distribution.pyi
+-rw-r--r--   0        0        0     2415 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_loss/link.pyi
+-rw-r--r--   0        0        0     7882 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_loss/loss.pyi
+-rw-r--r--   0        0        0      220 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_loss/setup.pyi
+-rw-r--r--   0        0        0      521 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_min_dependencies.pyi
+-rw-r--r--   0        0        0      895 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/_typing.pyi
+-rw-r--r--   0        0        0     3343 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/base.pyi
+-rw-r--r--   0        0        0     5345 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/calibration.pyi
+-rw-r--r--   0        0        0     1846 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/__init__.pyi
+-rw-r--r--   0        0        0     2446 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_affinity_propagation.pyi
+-rw-r--r--   0        0        0     4649 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_agglomerative.pyi
+-rw-r--r--   0        0        0     3344 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_bicluster.pyi
+-rw-r--r--   0        0        0     3497 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_birch.pyi
+-rw-r--r--   0        0        0     2086 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_bisect_k_means.pyi
+-rw-r--r--   0        0        0     2091 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_dbscan.pyi
+-rw-r--r--   0        0        0      120 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_dbscan_inner.pyi
+-rw-r--r--   0        0        0      618 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_feature_agglomeration.pyi
+-rw-r--r--   0        0        0       23 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_k_means_common.pyi
+-rw-r--r--   0        0        0     9566 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_k_means_elkan.pyi
+-rw-r--r--   0        0        0     4121 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_k_means_lloyd.pyi
+-rw-r--r--   0        0        0     6231 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_kmeans.pyi
+-rw-r--r--   0        0        0     2475 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_mean_shift.pyi
+-rw-r--r--   0        0        0     2894 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_optics.pyi
+-rw-r--r--   0        0        0     2988 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/_spectral.pyi
+-rw-r--r--   0        0        0      269 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cluster/setup.pyi
+-rw-r--r--   0        0        0      399 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/compose/__init__.pyi
+-rw-r--r--   0        0        0     3057 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/compose/_column_transformer.pyi
+-rw-r--r--   0        0        0     1711 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/compose/_target.pyi
+-rw-r--r--   0        0        0     1328 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/conftest.pyi
+-rw-r--r--   0        0        0     1095 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/covariance/__init__.pyi
+-rw-r--r--   0        0        0     1828 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/covariance/_elliptic_envelope.pyi
+-rw-r--r--   0        0        0     1885 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/covariance/_empirical_covariance.pyi
+-rw-r--r--   0        0        0     4364 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/covariance/_graph_lasso.pyi
+-rw-r--r--   0        0        0     3059 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/covariance/_robust_covariance.pyi
+-rw-r--r--   0        0        0     2838 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/covariance/_shrunk_covariance.pyi
+-rw-r--r--   0        0        0      192 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cross_decomposition/__init__.pyi
+-rw-r--r--   0        0        0     6208 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/cross_decomposition/_pls.pyi
+-rw-r--r--   0        0        0     3385 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/__init__.pyi
+-rw-r--r--   0        0        0     1003 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_arff_parser.pyi
+-rw-r--r--   0        0        0     3083 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_base.pyi
+-rw-r--r--   0        0        0      644 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_california_housing.pyi
+-rw-r--r--   0        0        0     1138 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_covtype.pyi
+-rw-r--r--   0        0        0     1191 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_kddcup99.pyi
+-rw-r--r--   0        0        0     1518 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_lfw.pyi
+-rw-r--r--   0        0        0      861 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_olivetti_faces.pyi
+-rw-r--r--   0        0        0     1880 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_openml.pyi
+-rw-r--r--   0        0        0     1901 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_rcv1.pyi
+-rw-r--r--   0        0        0     6168 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_samples_generator.pyi
+-rw-r--r--   0        0        0      814 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_species_distributions.pyi
+-rw-r--r--   0        0        0     1235 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_svmlight_format_io.pyi
+-rw-r--r--   0        0        0     1869 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/_twenty_newsgroups.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/data/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/descr/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/images/__init__.pyi
+-rw-r--r--   0        0        0      200 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/datasets/setup.pyi
+-rw-r--r--   0        0        0     1439 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/decomposition/__init__.pyi
+-rw-r--r--   0        0        0     1148 2023-04-14 20:45:33.101518 boilercv-0.0.1/typings/sklearn/decomposition/_base.pyi
+-rw-r--r--   0        0        0     8532 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_dict_learning.pyi
+-rw-r--r--   0        0        0     2366 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_factor_analysis.pyi
+-rw-r--r--   0        0        0     2946 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_fastica.pyi
+-rw-r--r--   0        0        0     1557 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_incremental_pca.pyi
+-rw-r--r--   0        0        0     2594 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_kernel_pca.pyi
+-rw-r--r--   0        0        0     2869 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_lda.pyi
+-rw-r--r--   0        0        0     5781 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_nmf.pyi
+-rw-r--r--   0        0        0      240 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_online_lda_fast.pyi
+-rw-r--r--   0        0        0     2526 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_pca.pyi
+-rw-r--r--   0        0        0     3362 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_sparse_pca.pyi
+-rw-r--r--   0        0        0     2110 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/_truncated_svd.pyi
+-rw-r--r--   0        0        0      184 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/decomposition/setup.pyi
+-rw-r--r--   0        0        0     3948 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/discriminant_analysis.pyi
+-rw-r--r--   0        0        0     3234 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/dummy.pyi
+-rw-r--r--   0        0        0     1724 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/__init__.pyi
+-rw-r--r--   0        0        0     4752 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_bagging.pyi
+-rw-r--r--   0        0        0     2396 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_base.pyi
+-rw-r--r--   0        0        0    11569 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_forest.pyi
+-rw-r--r--   0        0        0     7058 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_gb.pyi
+-rw-r--r--   0        0        0     5500 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_gb_losses.pyi
+-rw-r--r--   0        0        0      582 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_gradient_boosting.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/__init__.pyi
+-rw-r--r--   0        0        0      344 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/_bitset.pyi
+-rw-r--r--   0        0        0     1569 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/binning.pyi
+-rw-r--r--   0        0        0      673 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/common.pyi
+-rw-r--r--   0        0        0     6263 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/gradient_boosting.pyi
+-rw-r--r--   0        0        0     3684 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/grower.pyi
+-rw-r--r--   0        0        0     3813 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/histogram.pyi
+-rw-r--r--   0        0        0      885 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/predictor.pyi
+-rw-r--r--   0        0        0     8719 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/splitting.pyi
+-rw-r--r--   0        0        0       88 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_hist_gradient_boosting/utils.pyi
+-rw-r--r--   0        0        0     2405 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_iforest.pyi
+-rw-r--r--   0        0        0     5020 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_stacking.pyi
+-rw-r--r--   0        0        0     3498 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_voting.pyi
+-rw-r--r--   0        0        0     4413 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/_weight_boosting.pyi
+-rw-r--r--   0        0        0      174 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/ensemble/setup.pyi
+-rw-r--r--   0        0        0      725 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/exceptions.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/experimental/__init__.pyi
+-rw-r--r--   0        0        0      211 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/experimental/enable_halving_search_cv.pyi
+-rw-r--r--   0        0        0      133 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/experimental/enable_hist_gradient_boosting.pyi
+-rw-r--r--   0        0        0      101 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/experimental/enable_iterative_imputer.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/externals/__init__.pyi
+-rw-r--r--   0        0        0     5897 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/externals/_arff.pyi
+-rw-r--r--   0        0        0     1077 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/externals/_lobpcg.pyi
+-rw-r--r--   0        0        0     1992 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/externals/_numpy_compiler_patch.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/externals/_packaging/__init__.pyi
+-rw-r--r--   0        0        0     2476 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/externals/_packaging/_structures.pyi
+-rw-r--r--   0        0        0     4490 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/externals/_packaging/version.pyi
+-rw-r--r--   0        0        0      293 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/externals/conftest.pyi
+-rw-r--r--   0        0        0      344 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_extraction/__init__.pyi
+-rw-r--r--   0        0        0     1784 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_extraction/_dict_vectorizer.pyi
+-rw-r--r--   0        0        0     1098 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_extraction/_hash.pyi
+-rw-r--r--   0        0        0      343 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_extraction/_hashing_fast.pyi
+-rw-r--r--   0        0        0      216 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_extraction/_stop_words.pyi
+-rw-r--r--   0        0        0     2073 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_extraction/image.pyi
+-rw-r--r--   0        0        0      132 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_extraction/setup.pyi
+-rw-r--r--   0        0        0     8237 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_extraction/text.pyi
+-rw-r--r--   0        0        0     1241 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_selection/__init__.pyi
+-rw-r--r--   0        0        0      941 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_selection/_base.pyi
+-rw-r--r--   0        0        0     1902 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_selection/_from_model.pyi
+-rw-r--r--   0        0        0     1296 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_selection/_mutual_info.pyi
+-rw-r--r--   0        0        0     3296 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_selection/_rfe.pyi
+-rw-r--r--   0        0        0     1788 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_selection/_sequential.pyi
+-rw-r--r--   0        0        0     4832 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_selection/_univariate_selection.pyi
+-rw-r--r--   0        0        0     1003 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/feature_selection/_variance_threshold.pyi
+-rw-r--r--   0        0        0      456 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/gaussian_process/__init__.pyi
+-rw-r--r--   0        0        0     4407 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/gaussian_process/_gpc.pyi
+-rw-r--r--   0        0        0     2710 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/gaussian_process/_gpr.pyi
+-rw-r--r--   0        0        0    11388 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/gaussian_process/kernels.pyi
+-rw-r--r--   0        0        0      279 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/impute/__init__.pyi
+-rw-r--r--   0        0        0     3083 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/impute/_base.pyi
+-rw-r--r--   0        0        0     2787 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/impute/_iterative.pyi
+-rw-r--r--   0        0        0     1765 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/impute/_knn.pyi
+-rw-r--r--   0        0        0      483 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/inspection/__init__.pyi
+-rw-r--r--   0        0        0     1694 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/inspection/_partial_dependence.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/inspection/_pd_utils.pyi
+-rw-r--r--   0        0        0      819 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/inspection/_permutation_importance.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/inspection/_plot/__init__.pyi
+-rw-r--r--   0        0        0     1785 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/inspection/_plot/decision_boundary.pyi
+-rw-r--r--   0        0        0     3467 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/inspection/_plot/partial_dependence.pyi
+-rw-r--r--   0        0        0      161 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/inspection/setup.pyi
+-rw-r--r--   0        0        0     2553 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/isotonic.pyi
+-rw-r--r--   0        0        0     5116 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/kernel_approximation.pyi
+-rw-r--r--   0        0        0     1471 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/kernel_ridge.pyi
+-rw-r--r--   0        0        0     3248 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/__init__.pyi
+-rw-r--r--   0        0        0     3221 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_base.pyi
+-rw-r--r--   0        0        0     3203 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_bayes.pyi
+-rw-r--r--   0        0        0    12488 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_coordinate_descent.pyi
+-rw-r--r--   0        0        0      353 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_glm/__init__.pyi
+-rw-r--r--   0        0        0     2271 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_glm/_newton_solver.pyi
+-rw-r--r--   0        0        0     4324 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_glm/glm.pyi
+-rw-r--r--   0        0        0     1391 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_huber.pyi
+-rw-r--r--   0        0        0     7612 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_least_angle.pyi
+-rw-r--r--   0        0        0     2760 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_linear_loss.pyi
+-rw-r--r--   0        0        0     5512 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_logistic.pyi
+-rw-r--r--   0        0        0     3508 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_omp.pyi
+-rw-r--r--   0        0        0     3425 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_passive_aggressive.pyi
+-rw-r--r--   0        0        0     1400 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_perceptron.pyi
+-rw-r--r--   0        0        0     1705 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_quantile.pyi
+-rw-r--r--   0        0        0     2551 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_ransac.pyi
+-rw-r--r--   0        0        0     8792 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_ridge.pyi
+-rw-r--r--   0        0        0     1373 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_sag.pyi
+-rw-r--r--   0        0        0     1226 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_sag_fast.pyi
+-rw-r--r--   0        0        0     3227 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_sgd_fast.pyi
+-rw-r--r--   0        0        0    10787 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_stochastic_gradient.pyi
+-rw-r--r--   0        0        0     1830 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/_theil_sen.pyi
+-rw-r--r--   0        0        0      230 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/linear_model/setup.pyi
+-rw-r--r--   0        0        0      628 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/manifold/__init__.pyi
+-rw-r--r--   0        0        0     2536 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/manifold/_isomap.pyi
+-rw-r--r--   0        0        0     3554 2023-04-14 20:45:33.105518 boilercv-0.0.1/typings/sklearn/manifold/_locally_linear.pyi
+-rw-r--r--   0        0        0     2335 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/manifold/_mds.pyi
+-rw-r--r--   0        0        0     2624 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/manifold/_spectral_embedding.pyi
+-rw-r--r--   0        0        0     2972 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/manifold/_t_sne.pyi
+-rw-r--r--   0        0        0      185 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/manifold/setup.pyi
+-rw-r--r--   0        0        0     6097 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/__init__.pyi
+-rw-r--r--   0        0        0      247 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_base.pyi
+-rw-r--r--   0        0        0     6946 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_classification.pyi
+-rw-r--r--   0        0        0     3944 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_dist_metrics.pyi
+-rw-r--r--   0        0        0      251 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_pairwise_distances_reduction/__init__.pyi
+-rw-r--r--   0        0        0    11416 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_pairwise_distances_reduction/_dispatcher.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_plot/__init__.pyi
+-rw-r--r--   0        0        0       51 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_plot/base.pyi
+-rw-r--r--   0        0        0     2772 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_plot/confusion_matrix.pyi
+-rw-r--r--   0        0        0     1597 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_plot/det_curve.pyi
+-rw-r--r--   0        0        0     1874 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_plot/precision_recall_curve.pyi
+-rw-r--r--   0        0        0     2109 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_plot/regression.pyi
+-rw-r--r--   0        0        0     1715 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_plot/roc_curve.pyi
+-rw-r--r--   0        0        0     3727 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_ranking.pyi
+-rw-r--r--   0        0        0     5248 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_regression.pyi
+-rw-r--r--   0        0        0     4676 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/_scorer.pyi
+-rw-r--r--   0        0        0     1546 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/cluster/__init__.pyi
+-rw-r--r--   0        0        0      559 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/cluster/_bicluster.pyi
+-rw-r--r--   0        0        0       78 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/cluster/_expected_mutual_info_fast.pyi
+-rw-r--r--   0        0        0     2715 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/cluster/_supervised.pyi
+-rw-r--r--   0        0        0     1233 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/cluster/_unsupervised.pyi
+-rw-r--r--   0        0        0      185 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/cluster/setup.pyi
+-rw-r--r--   0        0        0     5964 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/pairwise.pyi
+-rw-r--r--   0        0        0      190 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/metrics/setup.pyi
+-rw-r--r--   0        0        0      207 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/mixture/__init__.pyi
+-rw-r--r--   0        0        0     1992 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/mixture/_base.pyi
+-rw-r--r--   0        0        0     2338 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/mixture/_bayesian_mixture.pyi
+-rw-r--r--   0        0        0     1771 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/mixture/_gaussian_mixture.pyi
+-rw-r--r--   0        0        0     2175 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/model_selection/__init__.pyi
+-rw-r--r--   0        0        0     2543 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/model_selection/_plot.pyi
+-rw-r--r--   0        0        0     5663 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/model_selection/_search.pyi
+-rw-r--r--   0        0        0     5201 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/model_selection/_search_successive_halving.pyi
+-rw-r--r--   0        0        0     7970 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/model_selection/_split.pyi
+-rw-r--r--   0        0        0     4792 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/model_selection/_validation.pyi
+-rw-r--r--   0        0        0     4691 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/multiclass.pyi
+-rw-r--r--   0        0        0     5320 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/multioutput.pyi
+-rw-r--r--   0        0        0     6230 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/naive_bayes.pyi
+-rw-r--r--   0        0        0     1664 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/__init__.pyi
+-rw-r--r--   0        0        0      107 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_ball_tree.pyi
+-rw-r--r--   0        0        0     3622 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_base.pyi
+-rw-r--r--   0        0        0     1884 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_binary_tree.pyi
+-rw-r--r--   0        0        0     2997 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_classification.pyi
+-rw-r--r--   0        0        0      218 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_distance_metric.pyi
+-rw-r--r--   0        0        0     3579 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_graph.pyi
+-rw-r--r--   0        0        0       68 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_kd_tree.pyi
+-rw-r--r--   0        0        0     2359 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_kde.pyi
+-rw-r--r--   0        0        0     2132 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_lof.pyi
+-rw-r--r--   0        0        0     2168 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_nca.pyi
+-rw-r--r--   0        0        0     1554 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_nearest_centroid.pyi
+-rw-r--r--   0        0        0     2998 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_regression.pyi
+-rw-r--r--   0        0        0     1044 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/_unsupervised.pyi
+-rw-r--r--   0        0        0      132 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neighbors/setup.pyi
+-rw-r--r--   0        0        0      218 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neural_network/__init__.pyi
+-rw-r--r--   0        0        0     1148 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neural_network/_base.pyi
+-rw-r--r--   0        0        0     6623 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neural_network/_multilayer_perceptron.pyi
+-rw-r--r--   0        0        0     2127 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neural_network/_rbm.pyi
+-rw-r--r--   0        0        0     1538 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/neural_network/_stochastic_optimizers.pyi
+-rw-r--r--   0        0        0     5337 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/pipeline.pyi
+-rw-r--r--   0        0        0     1810 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/preprocessing/__init__.pyi
+-rw-r--r--   0        0        0    11635 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/preprocessing/_data.pyi
+-rw-r--r--   0        0        0     1977 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/preprocessing/_discretization.pyi
+-rw-r--r--   0        0        0     3154 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/preprocessing/_encoders.pyi
+-rw-r--r--   0        0        0     1777 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/preprocessing/_function_transformer.pyi
+-rw-r--r--   0        0        0     3471 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/preprocessing/_label.pyi
+-rw-r--r--   0        0        0     2994 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/preprocessing/_polynomial.pyi
+-rw-r--r--   0        0        0      132 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/preprocessing/setup.pyi
+-rw-r--r--   0        0        0        1 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/py.typed
+-rw-r--r--   0        0        0     3362 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/random_projection.pyi
+-rw-r--r--   0        0        0      269 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/semi_supervised/__init__.pyi
+-rw-r--r--   0        0        0     3227 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/semi_supervised/_label_propagation.pyi
+-rw-r--r--   0        0        0     2091 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/semi_supervised/_self_training.pyi
+-rw-r--r--   0        0        0      229 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/setup.pyi
+-rw-r--r--   0        0        0      360 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/svm/__init__.pyi
+-rw-r--r--   0        0        0     3517 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/svm/_base.pyi
+-rw-r--r--   0        0        0      753 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/svm/_bounds.pyi
+-rw-r--r--   0        0        0     9620 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/svm/_classes.pyi
+-rw-r--r--   0        0        0      209 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/svm/setup.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tests/__init__.pyi
+-rw-r--r--   0        0        0      241 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tests/random_seed.pyi
+-rw-r--r--   0        0        0      603 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tree/__init__.pyi
+-rw-r--r--   0        0        0     8943 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tree/_classes.pyi
+-rw-r--r--   0        0        0     1460 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tree/_criterion.pyi
+-rw-r--r--   0        0        0     4043 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tree/_export.pyi
+-rw-r--r--   0        0        0     1444 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tree/_reingold_tilford.pyi
+-rw-r--r--   0        0        0     1874 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tree/_splitter.pyi
+-rw-r--r--   0        0        0     2259 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tree/_tree.pyi
+-rw-r--r--   0        0        0      185 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/tree/setup.pyi
+-rw-r--r--   0        0        0     3870 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/__init__.pyi
+-rw-r--r--   0        0        0       65 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_arpack.pyi
+-rw-r--r--   0        0        0     1116 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_array_api.pyi
+-rw-r--r--   0        0        0      392 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_available_if.pyi
+-rw-r--r--   0        0        0      340 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_bunch.pyi
+-rw-r--r--   0        0        0      702 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_encode.pyi
+-rw-r--r--   0        0        0      916 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_estimator_html_repr.pyi
+-rw-r--r--   0        0        0       39 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_fast_dict.pyi
+-rw-r--r--   0        0        0      154 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_isfinite.pyi
+-rw-r--r--   0        0        0      482 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_joblib.pyi
+-rw-r--r--   0        0        0      139 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_mask.pyi
+-rw-r--r--   0        0        0     2274 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_mocking.pyi
+-rw-r--r--   0        0        0     4556 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_param_validation.pyi
+-rw-r--r--   0        0        0     4327 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_pprint.pyi
+-rw-r--r--   0        0        0      297 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_random.pyi
+-rw-r--r--   0        0        0      107 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_readonly_array_wrapper.pyi
+-rw-r--r--   0        0        0     1199 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_seq_dataset.pyi
+-rw-r--r--   0        0        0      582 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_set_output.pyi
+-rw-r--r--   0        0        0      145 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_show_versions.pyi
+-rw-r--r--   0        0        0       46 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_tags.pyi
+-rw-r--r--   0        0        0     5436 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/_testing.pyi
+-rw-r--r--   0        0        0      305 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/arrayfuncs.pyi
+-rw-r--r--   0        0        0      617 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/class_weight.pyi
+-rw-r--r--   0        0        0      347 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/deprecation.pyi
+-rw-r--r--   0        0        0      858 2023-04-14 20:45:33.109518 boilercv-0.0.1/typings/sklearn/utils/discovery.pyi
+-rw-r--r--   0        0        0     9774 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/estimator_checks.pyi
+-rw-r--r--   0        0        0     2753 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/extmath.pyi
+-rw-r--r--   0        0        0     1225 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/fixes.pyi
+-rw-r--r--   0        0        0      628 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/graph.pyi
+-rw-r--r--   0        0        0      810 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/metaestimators.pyi
+-rw-r--r--   0        0        0      924 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/multiclass.pyi
+-rw-r--r--   0        0        0      119 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/murmurhash.pyi
+-rw-r--r--   0        0        0      448 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/optimize.pyi
+-rw-r--r--   0        0        0      746 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/parallel.pyi
+-rw-r--r--   0        0        0      275 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/random.pyi
+-rw-r--r--   0        0        0      242 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/setup.pyi
+-rw-r--r--   0        0        0     1722 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/sparsefuncs.pyi
+-rw-r--r--   0        0        0     4425 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/sparsefuncs_fast.pyi
+-rw-r--r--   0        0        0       71 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/stats.pyi
+-rw-r--r--   0        0        0     3973 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/utils/validation.pyi
+-rw-r--r--   0        0        0       73 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/README.md
+-rw-r--r--   0        0        0      487 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/__init__.pyi
+-rw-r--r--   0        0        0      459 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/_typing.pyi
+-rw-r--r--   0        0        0      608 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/app/__init__.pyi
+-rw-r--r--   0        0        0      497 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/app/_default_app.pyi
+-rw-r--r--   0        0        0     1087 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/app/application.pyi
+-rw-r--r--   0        0        0     1989 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/app/base.pyi
+-rw-r--r--   0        0        0     5239 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/app/canvas.pyi
+-rw-r--r--   0        0        0      681 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/color/__init__.pyi
+-rw-r--r--   0        0        0      679 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/color/_color_dict.pyi
+-rw-r--r--   0        0        0     3449 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/color/color_array.pyi
+-rw-r--r--   0        0        0     1558 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/color/color_space.pyi
+-rw-r--r--   0        0        0     5061 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/color/colormap.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/ext/__init__.pyi
+-rw-r--r--   0        0        0    26797 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/ext/cocoapy.pyi
+-rw-r--r--   0        0        0      402 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/ext/cubehelix.pyi
+-rw-r--r--   0        0        0     1231 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/__init__.pyi
+-rw-r--r--   0        0        0      511 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/calculations.pyi
+-rw-r--r--   0        0        0     3897 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/curves.pyi
+-rw-r--r--   0        0        0     1974 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/generation.pyi
+-rw-r--r--   0        0        0      476 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/isocurve.pyi
+-rw-r--r--   0        0        0      105 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/isosurface.pyi
+-rw-r--r--   0        0        0     2203 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/meshdata.pyi
+-rw-r--r--   0        0        0      460 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/normals.pyi
+-rw-r--r--   0        0        0      495 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/parametric.pyi
+-rw-r--r--   0        0        0     1000 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/polygon.pyi
+-rw-r--r--   0        0        0     1250 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/rect.pyi
+-rw-r--r--   0        0        0      922 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/torusknot.pyi
+-rw-r--r--   0        0        0     1539 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/geometry/triangulation.pyi
+-rw-r--r--   0        0        0      933 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/__init__.pyi
+-rw-r--r--   0        0        0     2975 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/buffer.pyi
+-rw-r--r--   0        0        0     1775 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/context.pyi
+-rw-r--r--   0        0        0     2143 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/framebuffer.pyi
+-rw-r--r--   0        0        0     1137 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/__init__.pyi
+-rw-r--r--   0        0        0     7548 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/_constants.pyi
+-rw-r--r--   0        0        0    12870 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/_gl2.pyi
+-rw-r--r--   0        0        0     7129 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/_proxy.pyi
+-rw-r--r--   0        0        0     1735 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/_pyopengl2.pyi
+-rw-r--r--   0        0        0      381 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/dummy.pyi
+-rw-r--r--   0        0        0      599 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/gl2.pyi
+-rw-r--r--   0        0        0      353 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/glplus.pyi
+-rw-r--r--   0        0        0      501 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/gl/pyopengl2.pyi
+-rw-r--r--   0        0        0     6313 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/glir.pyi
+-rw-r--r--   0        0        0      683 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/globject.pyi
+-rw-r--r--   0        0        0      463 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/preprocessor.pyi
+-rw-r--r--   0        0        0     2192 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/program.pyi
+-rw-r--r--   0        0        0     6738 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/texture.pyi
+-rw-r--r--   0        0        0      652 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/util.pyi
+-rw-r--r--   0        0        0     5067 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/gloo/wrappers.pyi
+-rw-r--r--   0        0        0      409 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/glsl/__init__.pyi
+-rw-r--r--   0        0        0     3529 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/glsl/build_spatial_filters.pyi
+-rw-r--r--   0        0        0      867 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/io/__init__.pyi
+-rw-r--r--   0        0        0      605 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/io/datasets.pyi
+-rw-r--r--   0        0        0      811 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/io/image.pyi
+-rw-r--r--   0        0        0      706 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/io/mesh.pyi
+-rw-r--r--   0        0        0      745 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/io/stl.pyi
+-rw-r--r--   0        0        0     1205 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/io/wavefront.pyi
+-rw-r--r--   0        0        0      283 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/plot/__init__.pyi
+-rw-r--r--   0        0        0      499 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/plot/fig.pyi
+-rw-r--r--   0        0        0     2967 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/plot/plotwidget.pyi
+-rw-r--r--   0        0        0      617 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/__init__.pyi
+-rw-r--r--   0        0        0      773 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/__init__.pyi
+-rw-r--r--   0        0        0      428 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/_base.pyi
+-rw-r--r--   0        0        0      751 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/arcball.pyi
+-rw-r--r--   0        0        0     2789 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/base_camera.pyi
+-rw-r--r--   0        0        0     1277 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/fly.pyi
+-rw-r--r--   0        0        0      851 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/magnify.pyi
+-rw-r--r--   0        0        0     1108 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/panzoom.pyi
+-rw-r--r--   0        0        0     1455 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/perspective.pyi
+-rw-r--r--   0        0        0     1066 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/cameras/turntable.pyi
+-rw-r--r--   0        0        0     3180 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/canvas.pyi
+-rw-r--r--   0        0        0      623 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/events.pyi
+-rw-r--r--   0        0        0     2954 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/node.pyi
+-rw-r--r--   0        0        0      244 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/subscene.pyi
+-rw-r--r--   0        0        0     1929 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/visuals.pyi
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/__init__.pyi
+-rw-r--r--   0        0        0       54 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/anchor.pyi
+-rw-r--r--   0        0        0      770 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/axis.pyi
+-rw-r--r--   0        0        0     1683 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/colorbar.pyi
+-rw-r--r--   0        0        0     1898 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/console.pyi
+-rw-r--r--   0        0        0     1994 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/grid.pyi
+-rw-r--r--   0        0        0      664 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/label.pyi
+-rw-r--r--   0        0        0      875 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/viewbox.pyi
+-rw-r--r--   0        0        0     2535 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/scene/widgets/widget.pyi
+-rw-r--r--   0        0        0     1085 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/testing/__init__.pyi
+-rw-r--r--   0        0        0      936 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/testing/_runners.pyi
+-rw-r--r--   0        0        0     2220 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/testing/_testing.pyi
+-rw-r--r--   0        0        0     1589 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/testing/image_tester.pyi
+-rw-r--r--   0        0        0      683 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/testing/rendered_array_tester.pyi
+-rw-r--r--   0        0        0      825 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/__init__.pyi
+-rw-r--r--   0        0        0      256 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/bunch.pyi
+-rw-r--r--   0        0        0      388 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/check_environment.pyi
+-rw-r--r--   0        0        0     1810 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/config.pyi
+-rw-r--r--   0        0        0      361 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/dpi/__init__.pyi
+-rw-r--r--   0        0        0      589 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/dpi/_linux.pyi
+-rw-r--r--   0        0        0      407 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/dpi/_quartz.pyi
+-rw-r--r--   0        0        0       76 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/eq.pyi
+-rw-r--r--   0        0        0     3281 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/event.pyi
+-rw-r--r--   0        0        0     1342 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/fetching.pyi
+-rw-r--r--   0        0        0      218 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/filter.pyi
+-rw-r--r--   0        0        0      506 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/fonts/__init__.pyi
+-rw-r--r--   0        0        0     1051 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/fonts/_quartz.pyi
+-rw-r--r--   0        0        0      463 2023-04-14 20:45:33.113518 boilercv-0.0.1/typings/sklearn/vispy/util/fonts/_triage.pyi
+-rw-r--r--   0        0        0      461 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/fonts/_vispy_fonts.pyi
+-rw-r--r--   0        0        0      418 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/fourier.pyi
+-rw-r--r--   0        0        0      376 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/frozen.pyi
+-rw-r--r--   0        0        0      706 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/keys.pyi
+-rw-r--r--   0        0        0     2228 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/logs.pyi
+-rw-r--r--   0        0        0       61 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/osmesa_gl.pyi
+-rw-r--r--   0        0        0      735 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/profiler.pyi
+-rw-r--r--   0        0        0      280 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/ptime.pyi
+-rw-r--r--   0        0        0      931 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/quaternion.pyi
+-rw-r--r--   0        0        0      487 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/__init__.pyi
+-rw-r--r--   0        0        0      356 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/base.pyi
+-rw-r--r--   0        0        0      653 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/color.pyi
+-rw-r--r--   0        0        0      598 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/element.pyi
+-rw-r--r--   0        0        0     3940 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/geometry.pyi
+-rw-r--r--   0        0        0      697 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/group.pyi
+-rw-r--r--   0        0        0      770 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/length.pyi
+-rw-r--r--   0        0        0      455 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/number.pyi
+-rw-r--r--   0        0        0     3106 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/path.pyi
+-rw-r--r--   0        0        0      770 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/shapes.pyi
+-rw-r--r--   0        0        0      561 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/style.pyi
+-rw-r--r--   0        0        0      574 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/svg.pyi
+-rw-r--r--   0        0        0     2002 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/transform.pyi
+-rw-r--r--   0        0        0      492 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/transformable.pyi
+-rw-r--r--   0        0        0      682 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/svg/viewport.pyi
+-rw-r--r--   0        0        0      785 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/transforms.pyi
+-rw-r--r--   0        0        0      411 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/util/wrappers.pyi
+-rw-r--r--   0        0        0     2494 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/__init__.pyi
+-rw-r--r--   0        0        0     2597 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/_scalable_textures.pyi
+-rw-r--r--   0        0        0     4469 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/axis.pyi
+-rw-r--r--   0        0        0     1454 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/border.pyi
+-rw-r--r--   0        0        0     1166 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/box.pyi
+-rw-r--r--   0        0        0      703 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/__init__.pyi
+-rw-r--r--   0        0        0      951 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/agg_fast_path_collection.pyi
+-rw-r--r--   0        0        0      927 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/agg_path_collection.pyi
+-rw-r--r--   0        0        0      725 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/agg_point_collection.pyi
+-rw-r--r--   0        0        0      779 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/agg_segment_collection.pyi
+-rw-r--r--   0        0        0     1170 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/array_list.pyi
+-rw-r--r--   0        0        0     1810 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/base_collection.pyi
+-rw-r--r--   0        0        0     1218 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/collection.pyi
+-rw-r--r--   0        0        0      515 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/path_collection.pyi
+-rw-r--r--   0        0        0      461 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/point_collection.pyi
+-rw-r--r--   0        0        0      539 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/polygon_collection.pyi
+-rw-r--r--   0        0        0      864 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/raw_path_collection.pyi
+-rw-r--r--   0        0        0      844 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/raw_point_collection.pyi
+-rw-r--r--   0        0        0      800 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/raw_polygon_collection.pyi
+-rw-r--r--   0        0        0      779 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/raw_segment_collection.pyi
+-rw-r--r--   0        0        0      659 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/raw_triangle_collection.pyi
+-rw-r--r--   0        0        0      475 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/segment_collection.pyi
+-rw-r--r--   0        0        0      417 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/triangle_collection.pyi
+-rw-r--r--   0        0        0      482 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/collections/util.pyi
+-rw-r--r--   0        0        0     2996 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/colorbar.pyi
+-rw-r--r--   0        0        0      729 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/cube.pyi
+-rw-r--r--   0        0        0     1341 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/ellipse.pyi
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/filters/__init__.pyi
+-rw-r--r--   0        0        0      740 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/filters/base_filter.pyi
+-rw-r--r--   0        0        0      555 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/filters/clipper.pyi
+-rw-r--r--   0        0        0      887 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/filters/clipping_planes.pyi
+-rw-r--r--   0        0        0     1372 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/filters/color.pyi
+-rw-r--r--   0        0        0     3953 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/filters/mesh.pyi
+-rw-r--r--   0        0        0      511 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/filters/picking.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/glsl/__init__.pyi
+-rw-r--r--   0        0        0      192 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/glsl/antialiasing.pyi
+-rw-r--r--   0        0        0      347 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/glsl/color.pyi
+-rw-r--r--   0        0        0       54 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/graphs/__init__.pyi
+-rw-r--r--   0        0        0     1665 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/graphs/graph.pyi
+-rw-r--r--   0        0        0      552 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/graphs/layouts/__init__.pyi
+-rw-r--r--   0        0        0      357 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/graphs/layouts/circular.pyi
+-rw-r--r--   0        0        0      754 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/graphs/layouts/force_directed.pyi
+-rw-r--r--   0        0        0      529 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/graphs/layouts/networkx_layout.pyi
+-rw-r--r--   0        0        0      444 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/graphs/layouts/random.pyi
+-rw-r--r--   0        0        0      460 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/graphs/util.pyi
+-rw-r--r--   0        0        0      544 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/gridlines.pyi
+-rw-r--r--   0        0        0      489 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/gridmesh.pyi
+-rw-r--r--   0        0        0      691 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/histogram.pyi
+-rw-r--r--   0        0        0     2839 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/image.pyi
+-rw-r--r--   0        0        0      999 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/image_complex.pyi
+-rw-r--r--   0        0        0     1015 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/infinite_line.pyi
+-rw-r--r--   0        0        0     1118 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/isocurve.pyi
+-rw-r--r--   0        0        0     1377 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/isoline.pyi
+-rw-r--r--   0        0        0     1013 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/isosurface.pyi
+-rw-r--r--   0        0        0      265 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/line/__init__.pyi
+-rw-r--r--   0        0        0     1810 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/line/arrow.pyi
+-rw-r--r--   0        0        0      377 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/line/dash_atlas.pyi
+-rw-r--r--   0        0        0     2231 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/line/line.pyi
+-rw-r--r--   0        0        0      955 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/line_plot.pyi
+-rw-r--r--   0        0        0      859 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/linear_region.pyi
+-rw-r--r--   0        0        0     2841 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/markers.pyi
+-rw-r--r--   0        0        0     2526 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/mesh.pyi
+-rw-r--r--   0        0        0     1066 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/mesh_normals.pyi
+-rw-r--r--   0        0        0      892 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/plane.pyi
+-rw-r--r--   0        0        0     1236 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/polygon.pyi
+-rw-r--r--   0        0        0     1151 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/rectangle.pyi
+-rw-r--r--   0        0        0      689 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/regular_polygon.pyi
+-rw-r--r--   0        0        0     1117 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/scrolling_lines.pyi
+-rw-r--r--   0        0        0      759 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/__init__.pyi
+-rw-r--r--   0        0        0      602 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/compiler.pyi
+-rw-r--r--   0        0        0      779 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/expression.pyi
+-rw-r--r--   0        0        0     2731 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/function.pyi
+-rw-r--r--   0        0        0      799 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/multiprogram.pyi
+-rw-r--r--   0        0        0     1383 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/parsing.pyi
+-rw-r--r--   0        0        0     1048 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/program.pyi
+-rw-r--r--   0        0        0      998 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/shader_object.pyi
+-rw-r--r--   0        0        0     1636 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/shaders/variable.pyi
+-rw-r--r--   0        0        0     1622 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/spectrogram.pyi
+-rw-r--r--   0        0        0     1040 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/sphere.pyi
+-rw-r--r--   0        0        0      997 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/surface_plot.pyi
+-rw-r--r--   0        0        0      371 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/text/__init__.pyi
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/text/_sdf_gpu.pyi
+-rw-r--r--   0        0        0     3315 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/text/text.pyi
+-rw-r--r--   0        0        0     1096 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/transforms/__init__.pyi
+-rw-r--r--   0        0        0      622 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/transforms/_util.pyi
+-rw-r--r--   0        0        0     2058 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/transforms/base_transform.pyi
+-rw-r--r--   0        0        0     1490 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/transforms/chain.pyi
+-rw-r--r--   0        0        0      641 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/transforms/interactive.pyi
+-rw-r--r--   0        0        0     3779 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/transforms/linear.pyi
+-rw-r--r--   0        0        0     2366 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/transforms/nonlinear.pyi
+-rw-r--r--   0        0        0     1707 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/transforms/transform_system.pyi
+-rw-r--r--   0        0        0      740 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/tube.pyi
+-rw-r--r--   0        0        0     3913 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/visual.pyi
+-rw-r--r--   0        0        0     4899 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/volume.pyi
+-rw-r--r--   0        0        0     1270 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/windbarb.pyi
+-rw-r--r--   0        0        0      121 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sklearn/vispy/visuals/xyz_axis.pyi
+-rw-r--r--   0        0        0     2654 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sympy-stubs/core/evalf.pyi
+-rw-r--r--   0        0        0     2322 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sympy-stubs/core/power.pyi
+-rw-r--r--   0        0        0        8 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sympy-stubs/py.typed
+-rw-r--r--   0        0        0      323 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sympy-stubs/simplify/powsimp.pyi
+-rw-r--r--   0        0        0     2015 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/sympy-stubs/simplify/simplify.pyi
+-rw-r--r--   0        0        0      751 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/transformers-stubs/models/auto/configuration_auto.pyi
+-rw-r--r--   0        0        0     1407 2023-04-14 20:45:33.117519 boilercv-0.0.1/typings/transformers-stubs/models/auto/tokenization_auto.pyi
+-rw-r--r--   0        0        0        8 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/transformers-stubs/py.typed
+-rw-r--r--   0        0        0      808 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/update.ps1
+-rw-r--r--   0        0        0       73 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/README.md
+-rw-r--r--   0        0        0      487 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/__init__.pyi
+-rw-r--r--   0        0        0      459 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/_typing.pyi
+-rw-r--r--   0        0        0      608 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/app/__init__.pyi
+-rw-r--r--   0        0        0      497 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/app/_default_app.pyi
+-rw-r--r--   0        0        0      920 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/app/application.pyi
+-rw-r--r--   0        0        0     1989 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/app/base.pyi
+-rw-r--r--   0        0        0     5199 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/app/canvas.pyi
+-rw-r--r--   0        0        0      681 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/color/__init__.pyi
+-rw-r--r--   0        0        0      679 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/color/_color_dict.pyi
+-rw-r--r--   0        0        0     3407 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/color/color_array.pyi
+-rw-r--r--   0        0        0     1558 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/color/color_space.pyi
+-rw-r--r--   0        0        0     5023 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/color/colormap.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/ext/__init__.pyi
+-rw-r--r--   0        0        0    26797 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/ext/cocoapy.pyi
+-rw-r--r--   0        0        0      402 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/ext/cubehelix.pyi
+-rw-r--r--   0        0        0     1231 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/__init__.pyi
+-rw-r--r--   0        0        0      511 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/calculations.pyi
+-rw-r--r--   0        0        0     3897 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/curves.pyi
+-rw-r--r--   0        0        0     1974 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/generation.pyi
+-rw-r--r--   0        0        0      476 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/isocurve.pyi
+-rw-r--r--   0        0        0      105 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/isosurface.pyi
+-rw-r--r--   0        0        0     2203 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/meshdata.pyi
+-rw-r--r--   0        0        0      460 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/normals.pyi
+-rw-r--r--   0        0        0      495 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/parametric.pyi
+-rw-r--r--   0        0        0     1000 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/polygon.pyi
+-rw-r--r--   0        0        0     1250 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/rect.pyi
+-rw-r--r--   0        0        0      922 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/torusknot.pyi
+-rw-r--r--   0        0        0     1539 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/geometry/triangulation.pyi
+-rw-r--r--   0        0        0      933 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/__init__.pyi
+-rw-r--r--   0        0        0     2975 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/buffer.pyi
+-rw-r--r--   0        0        0     1739 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/context.pyi
+-rw-r--r--   0        0        0     2143 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/framebuffer.pyi
+-rw-r--r--   0        0        0     1137 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/__init__.pyi
+-rw-r--r--   0        0        0     7548 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/_constants.pyi
+-rw-r--r--   0        0        0    12870 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/_gl2.pyi
+-rw-r--r--   0        0        0     7129 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/_proxy.pyi
+-rw-r--r--   0        0        0     1735 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/_pyopengl2.pyi
+-rw-r--r--   0        0        0      381 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/dummy.pyi
+-rw-r--r--   0        0        0      599 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/gl2.pyi
+-rw-r--r--   0        0        0      353 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/glplus.pyi
+-rw-r--r--   0        0        0      501 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/gl/pyopengl2.pyi
+-rw-r--r--   0        0        0     6313 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/glir.pyi
+-rw-r--r--   0        0        0      683 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/globject.pyi
+-rw-r--r--   0        0        0      463 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/preprocessor.pyi
+-rw-r--r--   0        0        0     2192 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/program.pyi
+-rw-r--r--   0        0        0     6738 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/texture.pyi
+-rw-r--r--   0        0        0      652 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/util.pyi
+-rw-r--r--   0        0        0     5067 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/gloo/wrappers.pyi
+-rw-r--r--   0        0        0      409 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/glsl/__init__.pyi
+-rw-r--r--   0        0        0     3529 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/glsl/build_spatial_filters.pyi
+-rw-r--r--   0        0        0      867 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/io/__init__.pyi
+-rw-r--r--   0        0        0      623 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/io/datasets.pyi
+-rw-r--r--   0        0        0      811 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/io/image.pyi
+-rw-r--r--   0        0        0      706 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/io/mesh.pyi
+-rw-r--r--   0        0        0      745 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/io/stl.pyi
+-rw-r--r--   0        0        0     1205 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/io/wavefront.pyi
+-rw-r--r--   0        0        0      283 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/plot/__init__.pyi
+-rw-r--r--   0        0        0      499 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/plot/fig.pyi
+-rw-r--r--   0        0        0     2929 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/plot/plotwidget.pyi
+-rw-r--r--   0        0        0      617 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/__init__.pyi
+-rw-r--r--   0        0        0      773 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/__init__.pyi
+-rw-r--r--   0        0        0      428 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/_base.pyi
+-rw-r--r--   0        0        0      751 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/arcball.pyi
+-rw-r--r--   0        0        0     2789 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/base_camera.pyi
+-rw-r--r--   0        0        0     1277 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/fly.pyi
+-rw-r--r--   0        0        0      851 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/magnify.pyi
+-rw-r--r--   0        0        0     1108 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/panzoom.pyi
+-rw-r--r--   0        0        0     1455 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/perspective.pyi
+-rw-r--r--   0        0        0     1066 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/cameras/turntable.pyi
+-rw-r--r--   0        0        0     3180 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/canvas.pyi
+-rw-r--r--   0        0        0      623 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/events.pyi
+-rw-r--r--   0        0        0     2894 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/node.pyi
+-rw-r--r--   0        0        0      244 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/subscene.pyi
+-rw-r--r--   0        0        0     2618 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/visuals.pyi
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/__init__.pyi
+-rw-r--r--   0        0        0       54 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/anchor.pyi
+-rw-r--r--   0        0        0      770 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/axis.pyi
+-rw-r--r--   0        0        0     1683 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/colorbar.pyi
+-rw-r--r--   0        0        0     1898 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/console.pyi
+-rw-r--r--   0        0        0     1994 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/grid.pyi
+-rw-r--r--   0        0        0      664 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/label.pyi
+-rw-r--r--   0        0        0      875 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/viewbox.pyi
+-rw-r--r--   0        0        0     2489 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/scene/widgets/widget.pyi
+-rw-r--r--   0        0        0     1085 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/testing/__init__.pyi
+-rw-r--r--   0        0        0      936 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/testing/_runners.pyi
+-rw-r--r--   0        0        0     2220 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/testing/_testing.pyi
+-rw-r--r--   0        0        0     1589 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/testing/image_tester.pyi
+-rw-r--r--   0        0        0      683 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/testing/rendered_array_tester.pyi
+-rw-r--r--   0        0        0      825 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/__init__.pyi
+-rw-r--r--   0        0        0      256 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/bunch.pyi
+-rw-r--r--   0        0        0      388 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/check_environment.pyi
+-rw-r--r--   0        0        0     1810 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/config.pyi
+-rw-r--r--   0        0        0      361 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/dpi/__init__.pyi
+-rw-r--r--   0        0        0      589 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/dpi/_linux.pyi
+-rw-r--r--   0        0        0      407 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/dpi/_quartz.pyi
+-rw-r--r--   0        0        0       76 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/eq.pyi
+-rw-r--r--   0        0        0     3247 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/event.pyi
+-rw-r--r--   0        0        0     1342 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/fetching.pyi
+-rw-r--r--   0        0        0      218 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/filter.pyi
+-rw-r--r--   0        0        0      506 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/fonts/__init__.pyi
+-rw-r--r--   0        0        0     1051 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/fonts/_quartz.pyi
+-rw-r--r--   0        0        0      463 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/fonts/_triage.pyi
+-rw-r--r--   0        0        0      461 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/fonts/_vispy_fonts.pyi
+-rw-r--r--   0        0        0      418 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/fourier.pyi
+-rw-r--r--   0        0        0      376 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/frozen.pyi
+-rw-r--r--   0        0        0      706 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/keys.pyi
+-rw-r--r--   0        0        0     2228 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/logs.pyi
+-rw-r--r--   0        0        0       61 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/osmesa_gl.pyi
+-rw-r--r--   0        0        0      735 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/profiler.pyi
+-rw-r--r--   0        0        0      280 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/ptime.pyi
+-rw-r--r--   0        0        0      931 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/quaternion.pyi
+-rw-r--r--   0        0        0      487 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/__init__.pyi
+-rw-r--r--   0        0        0      356 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/base.pyi
+-rw-r--r--   0        0        0      653 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/color.pyi
+-rw-r--r--   0        0        0      598 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/element.pyi
+-rw-r--r--   0        0        0     3940 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/geometry.pyi
+-rw-r--r--   0        0        0      697 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/group.pyi
+-rw-r--r--   0        0        0      770 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/length.pyi
+-rw-r--r--   0        0        0      455 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/number.pyi
+-rw-r--r--   0        0        0     3106 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/path.pyi
+-rw-r--r--   0        0        0      770 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/shapes.pyi
+-rw-r--r--   0        0        0      561 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/style.pyi
+-rw-r--r--   0        0        0      574 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/svg.pyi
+-rw-r--r--   0        0        0     2002 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/transform.pyi
+-rw-r--r--   0        0        0      492 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/transformable.pyi
+-rw-r--r--   0        0        0      682 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/svg/viewport.pyi
+-rw-r--r--   0        0        0      785 2023-04-14 20:45:33.121518 boilercv-0.0.1/typings/vispy/util/transforms.pyi
+-rw-r--r--   0        0        0      411 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/util/wrappers.pyi
+-rw-r--r--   0        0        0     2494 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/__init__.pyi
+-rw-r--r--   0        0        0     2597 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/_scalable_textures.pyi
+-rw-r--r--   0        0        0     4428 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/axis.pyi
+-rw-r--r--   0        0        0     1454 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/border.pyi
+-rw-r--r--   0        0        0     1166 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/box.pyi
+-rw-r--r--   0        0        0      703 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/__init__.pyi
+-rw-r--r--   0        0        0      951 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/agg_fast_path_collection.pyi
+-rw-r--r--   0        0        0      927 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/agg_path_collection.pyi
+-rw-r--r--   0        0        0      725 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/agg_point_collection.pyi
+-rw-r--r--   0        0        0      779 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/agg_segment_collection.pyi
+-rw-r--r--   0        0        0     1170 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/array_list.pyi
+-rw-r--r--   0        0        0     1810 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/base_collection.pyi
+-rw-r--r--   0        0        0     1218 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/collection.pyi
+-rw-r--r--   0        0        0      515 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/path_collection.pyi
+-rw-r--r--   0        0        0      461 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/point_collection.pyi
+-rw-r--r--   0        0        0      539 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/polygon_collection.pyi
+-rw-r--r--   0        0        0      864 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/raw_path_collection.pyi
+-rw-r--r--   0        0        0      844 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/raw_point_collection.pyi
+-rw-r--r--   0        0        0      800 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/raw_polygon_collection.pyi
+-rw-r--r--   0        0        0      779 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/raw_segment_collection.pyi
+-rw-r--r--   0        0        0      659 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/raw_triangle_collection.pyi
+-rw-r--r--   0        0        0      475 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/segment_collection.pyi
+-rw-r--r--   0        0        0      417 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/triangle_collection.pyi
+-rw-r--r--   0        0        0      482 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/collections/util.pyi
+-rw-r--r--   0        0        0     2996 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/colorbar.pyi
+-rw-r--r--   0        0        0      729 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/cube.pyi
+-rw-r--r--   0        0        0     1341 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/ellipse.pyi
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/filters/__init__.pyi
+-rw-r--r--   0        0        0      740 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/filters/base_filter.pyi
+-rw-r--r--   0        0        0      555 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/filters/clipper.pyi
+-rw-r--r--   0        0        0      887 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/filters/clipping_planes.pyi
+-rw-r--r--   0        0        0     1372 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/filters/color.pyi
+-rw-r--r--   0        0        0     3953 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/filters/mesh.pyi
+-rw-r--r--   0        0        0      511 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/filters/picking.pyi
+-rw-r--r--   0        0        0        0 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/glsl/__init__.pyi
+-rw-r--r--   0        0        0      192 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/glsl/antialiasing.pyi
+-rw-r--r--   0        0        0      347 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/glsl/color.pyi
+-rw-r--r--   0        0        0       54 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/graphs/__init__.pyi
+-rw-r--r--   0        0        0     1665 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/graphs/graph.pyi
+-rw-r--r--   0        0        0      552 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/graphs/layouts/__init__.pyi
+-rw-r--r--   0        0        0      357 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/graphs/layouts/circular.pyi
+-rw-r--r--   0        0        0      754 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/graphs/layouts/force_directed.pyi
+-rw-r--r--   0        0        0      529 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/graphs/layouts/networkx_layout.pyi
+-rw-r--r--   0        0        0      444 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/graphs/layouts/random.pyi
+-rw-r--r--   0        0        0      460 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/graphs/util.pyi
+-rw-r--r--   0        0        0      544 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/gridlines.pyi
+-rw-r--r--   0        0        0      489 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/gridmesh.pyi
+-rw-r--r--   0        0        0      691 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/histogram.pyi
+-rw-r--r--   0        0        0     2839 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/image.pyi
+-rw-r--r--   0        0        0      999 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/image_complex.pyi
+-rw-r--r--   0        0        0     1015 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/infinite_line.pyi
+-rw-r--r--   0        0        0     1118 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/isocurve.pyi
+-rw-r--r--   0        0        0     1377 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/isoline.pyi
+-rw-r--r--   0        0        0     1013 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/isosurface.pyi
+-rw-r--r--   0        0        0      265 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/line/__init__.pyi
+-rw-r--r--   0        0        0     1810 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/line/arrow.pyi
+-rw-r--r--   0        0        0      377 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/line/dash_atlas.pyi
+-rw-r--r--   0        0        0     2231 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/line/line.pyi
+-rw-r--r--   0        0        0      955 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/line_plot.pyi
+-rw-r--r--   0        0        0      859 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/linear_region.pyi
+-rw-r--r--   0        0        0     2795 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/markers.pyi
+-rw-r--r--   0        0        0     2526 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/mesh.pyi
+-rw-r--r--   0        0        0     1066 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/mesh_normals.pyi
+-rw-r--r--   0        0        0      892 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/plane.pyi
+-rw-r--r--   0        0        0     1236 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/polygon.pyi
+-rw-r--r--   0        0        0     1151 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/rectangle.pyi
+-rw-r--r--   0        0        0      689 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/regular_polygon.pyi
+-rw-r--r--   0        0        0     1117 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/scrolling_lines.pyi
+-rw-r--r--   0        0        0      759 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/__init__.pyi
+-rw-r--r--   0        0        0      602 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/compiler.pyi
+-rw-r--r--   0        0        0      779 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/expression.pyi
+-rw-r--r--   0        0        0     2731 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/function.pyi
+-rw-r--r--   0        0        0      799 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/multiprogram.pyi
+-rw-r--r--   0        0        0     1383 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/parsing.pyi
+-rw-r--r--   0        0        0     1048 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/program.pyi
+-rw-r--r--   0        0        0      998 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/shader_object.pyi
+-rw-r--r--   0        0        0     1636 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/shaders/variable.pyi
+-rw-r--r--   0        0        0     1622 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/spectrogram.pyi
+-rw-r--r--   0        0        0     1040 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/sphere.pyi
+-rw-r--r--   0        0        0      997 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/surface_plot.pyi
+-rw-r--r--   0        0        0      371 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/text/__init__.pyi
+-rw-r--r--   0        0        0      619 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/text/_sdf_gpu.pyi
+-rw-r--r--   0        0        0     3315 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/text/text.pyi
+-rw-r--r--   0        0        0     1096 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/transforms/__init__.pyi
+-rw-r--r--   0        0        0      622 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/transforms/_util.pyi
+-rw-r--r--   0        0        0     2058 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/transforms/base_transform.pyi
+-rw-r--r--   0        0        0     1490 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/transforms/chain.pyi
+-rw-r--r--   0        0        0      641 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/transforms/interactive.pyi
+-rw-r--r--   0        0        0     3779 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/transforms/linear.pyi
+-rw-r--r--   0        0        0     2366 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/transforms/nonlinear.pyi
+-rw-r--r--   0        0        0     1707 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/transforms/transform_system.pyi
+-rw-r--r--   0        0        0      740 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/tube.pyi
+-rw-r--r--   0        0        0     3850 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/visual.pyi
+-rw-r--r--   0        0        0     4879 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/volume.pyi
+-rw-r--r--   0        0        0     1270 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/windbarb.pyi
+-rw-r--r--   0        0        0      121 2023-04-14 20:45:33.125518 boilercv-0.0.1/typings/vispy/visuals/xyz_axis.pyi
+-rw-r--r--   0        0        0     1533 2023-04-14 20:46:11.697535 boilercv-0.0.1/update.ps1
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 boilercv-0.0.1/PKG-INFO
```

### Comparing `boilercv-0.0.0/.coveragerc` & `boilercv-0.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `boilercv-0.0.0/.env` & `boilercv-0.0.1/.env`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-OPENCV_SAMPLES_DATA_PATH=data/samples
-# Enable rich feedback and exceptions at the command line
-PYTHONSTARTUP = pythonrc.py
-# default: Warn for all warnings, even `DeprecationWarning`
-# pkg_resources: https://github.com/blakeNaccarato/copier-python/issues/319#issue-1609228740
-# Creating a LegacyVersion: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1454209165
-# pre_commit read_text and open_text: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1455177114
-# imp module and ABCs: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1455183241
-# dpath...pkg_resources: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1457219723
-# unclosed file...plumbum: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1458742412
-# ignore:is still running:subprocess:ResourceWarning:subprocess: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1493072447
-# ignore:BuiltinImporter.module_repr:DeprecationWarning:importlib._bootstrap: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1493542865
-# ignore:lib2to3: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1502112446
-PYTHONWARNINGS = default,ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning,ignore:Creating a LegacyVersion has been deprecated and will be removed in the next major release:DeprecationWarning:pip._vendor.packaging.version,ignore:read_text is deprecated:DeprecationWarning:pre_commit.util,ignore:open_text is deprecated:DeprecationWarning:importlib.resources._legacy,ignore:the imp module is deprecated in favour of importlib:DeprecationWarning:googlecloudsdk.core.util.importing,ignore:Using or importing the ABCs:DeprecationWarning:jsonschema.compat,ignore:The dpath.util package is being deprecated.:DeprecationWarning:dvc.dependency.param,ignore:unclosed file:ResourceWarning:dvc.stage.cache,ignore:the imp module is deprecated:DeprecationWarning:ansiwrap.core,ignore:unclosed file:ResourceWarning:ansiwrap.core,ignore:Jupyter is migrating its paths to use standard platformdirs:DeprecationWarning:jupyter_client.connect,ignore:the file is not specified with any extension:UserWarning:papermill.iorw,ignore:Passing unrecognized arguments to super:DeprecationWarning:traitlets.config.configurable,ignore:pkg_resources is deprecated as an API:DeprecationWarning:pkg_resources,ignore:unclosed file:ResourceWarning:plumbum.commands.base,ignore:Passing unrecognized arguments to super:DeprecationWarning:ipywidgets.widgets.widget,ignore:`ipykernel.pylab.backend_inline` is deprecated:DeprecationWarning:ipykernel.pylab.backend_inline,ignore:subprocess:ResourceWarning:subprocess,ignore:BuiltinImporter.module_repr:DeprecationWarning:importlib._bootstrap,ignore:lib2to3 package is deprecated and may not be able to parse Python:PendingDeprecationWarning,ignore:lib2to3 package is deprecated and may not be able to parse Python:DeprecationWarning
+OPENCV_SAMPLES_DATA_PATH=data/samples
+# Enable rich feedback and exceptions at the command line
+PYTHONSTARTUP = pythonrc.py
+# default: Warn for all warnings, even `DeprecationWarning`
+# pkg_resources: https://github.com/blakeNaccarato/copier-python/issues/319#issue-1609228740
+# Creating a LegacyVersion: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1454209165
+# pre_commit read_text and open_text: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1455177114
+# imp module and ABCs: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1455183241
+# dpath...pkg_resources: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1457219723
+# unclosed file...plumbum: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1458742412
+# ignore:is still running:subprocess:ResourceWarning:subprocess: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1493072447
+# ignore:BuiltinImporter.module_repr:DeprecationWarning:importlib._bootstrap: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1493542865
+# ignore:lib2to3: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1502112446
+PYTHONWARNINGS = default,ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning,ignore:Creating a LegacyVersion has been deprecated and will be removed in the next major release:DeprecationWarning:pip._vendor.packaging.version,ignore:read_text is deprecated:DeprecationWarning:pre_commit.util,ignore:open_text is deprecated:DeprecationWarning:importlib.resources._legacy,ignore:the imp module is deprecated in favour of importlib:DeprecationWarning:googlecloudsdk.core.util.importing,ignore:Using or importing the ABCs:DeprecationWarning:jsonschema.compat,ignore:The dpath.util package is being deprecated.:DeprecationWarning:dvc.dependency.param,ignore:unclosed file:ResourceWarning:dvc.stage.cache,ignore:the imp module is deprecated:DeprecationWarning:ansiwrap.core,ignore:unclosed file:ResourceWarning:ansiwrap.core,ignore:Jupyter is migrating its paths to use standard platformdirs:DeprecationWarning:jupyter_client.connect,ignore:the file is not specified with any extension:UserWarning:papermill.iorw,ignore:Passing unrecognized arguments to super:DeprecationWarning:traitlets.config.configurable,ignore:pkg_resources is deprecated as an API:DeprecationWarning:pkg_resources,ignore:unclosed file:ResourceWarning:plumbum.commands.base,ignore:Passing unrecognized arguments to super:DeprecationWarning:ipywidgets.widgets.widget,ignore:`ipykernel.pylab.backend_inline` is deprecated:DeprecationWarning:ipykernel.pylab.backend_inline,ignore:subprocess:ResourceWarning:subprocess,ignore:BuiltinImporter.module_repr:DeprecationWarning:importlib._bootstrap,ignore:lib2to3 package is deprecated and may not be able to parse Python:PendingDeprecationWarning,ignore:lib2to3 package is deprecated and may not be able to parse Python:DeprecationWarning
```

### Comparing `boilercv-0.0.0/.github/workflows/codeql.yml` & `boilercv-0.0.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `boilercv-0.0.0/.github/workflows/main.yml` & `boilercv-0.0.1/.github/workflows/main.yml`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-name: "main"
-
-on: ["push", "workflow_dispatch"]
-
-jobs:
-  # * ------------------------------------------------------------------------------ * #
-  # * Changes below may be lost in significant template updates.
-
-  pyright:
-    runs-on: "ubuntu-latest"
-    steps:
-      - uses: "blakeNaccarato/copier-python-workflow-setup@v0.0.12"
-        with:
-          python-version: "3.11"
-      - run: "pip install --no-deps --requirement .tools/requirements/requirements_nodeps.txt"
-      - run: "pyright"
-  pytest-cov:
-    permissions:
-      contents: "read"
-      id-token: "write"
-    runs-on: "ubuntu-latest"
-    steps:
-      - uses: "blakeNaccarato/copier-python-workflow-setup@v0.0.12"
-        with:
-          python-version: "3.11"
-      - run: "pip install --no-deps --requirement .tools/requirements/requirements_nodeps.txt"
-      - name: Install PySide6 system dependencies
-        run: |
-          # https://askubuntu.com/questions/900285/libegl-so-1-is-not-a-symbolic-link
-          sudo apt update
-          sudo apt install libegl1
-      # - uses: "google-github-actions/auth@v1.0.0"
-      #   with:
-      #     workload_identity_provider: "projects/326920613558/locations/global/workloadIdentityPools/github-com/providers/github-com-oidc"
-      #     service_account: "iterative-studio@secure-garden-355020.iam.gserviceaccount.com"
-      # - uses: "google-github-actions/setup-gcloud@v1.1.0"
-      - run: "pytest --cov"
-        env:
-          OPENCV_SAMPLES_DATA_PATH: data/samples
-          # GH_TOKEN: ${{ github.token }}
-      - uses: "codecov/codecov-action@v3.1.1"
-  bump_project:
-    needs: ["pyright", "pytest-cov"]
-    runs-on: "ubuntu-latest"
-    steps:
-      - uses: "blakeNaccarato/copier-python-workflow-setup@v0.0.12"
-        with:
-          python-version: "3.11"
-          install-project: false
-      - uses: "stefanzweifel/git-auto-commit-action@v4.16.0"
-        with:
-          commit_message: "Bump project template and compose `pyproject.toml`."
-
-  # * ------------------------------------------------------------------------------ * #
-  # * Changes below should persist in significant template updates.
+name: "main"
+
+on: ["push", "workflow_dispatch"]
+
+jobs:
+  # * ------------------------------------------------------------------------------ * #
+  # * Changes below may be lost in significant template updates.
+
+  pyright:
+    runs-on: "ubuntu-latest"
+    steps:
+      - uses: "blakeNaccarato/copier-python-workflow-setup@v0.0.12"
+        with:
+          python-version: "3.11"
+      - run: "pip install --no-deps --requirement .tools/requirements/requirements_nodeps.txt"
+      - run: "pyright"
+  pytest-cov:
+    permissions:
+      contents: "read"
+      id-token: "write"
+    runs-on: "ubuntu-latest"
+    steps:
+      - uses: "blakeNaccarato/copier-python-workflow-setup@v0.0.12"
+        with:
+          python-version: "3.11"
+      - run: "pip install --no-deps --requirement .tools/requirements/requirements_nodeps.txt"
+      - name: Install PySide6 system dependencies
+        run: |
+          # https://askubuntu.com/questions/900285/libegl-so-1-is-not-a-symbolic-link
+          sudo apt update
+          sudo apt install libegl1
+      # - uses: "google-github-actions/auth@v1.0.0"
+      #   with:
+      #     workload_identity_provider: "projects/326920613558/locations/global/workloadIdentityPools/github-com/providers/github-com-oidc"
+      #     service_account: "iterative-studio@secure-garden-355020.iam.gserviceaccount.com"
+      # - uses: "google-github-actions/setup-gcloud@v1.1.0"
+      - run: "pytest --cov"
+        env:
+          OPENCV_SAMPLES_DATA_PATH: data/samples
+          # GH_TOKEN: ${{ github.token }}
+      - uses: "codecov/codecov-action@v3.1.1"
+  bump_project:
+    needs: ["pyright", "pytest-cov"]
+    runs-on: "ubuntu-latest"
+    steps:
+      - uses: "blakeNaccarato/copier-python-workflow-setup@v0.0.12"
+        with:
+          python-version: "3.11"
+          install-project: false
+      - uses: "stefanzweifel/git-auto-commit-action@v4.16.0"
+        with:
+          commit_message: "Bump project template and compose `pyproject.toml`."
+
+  # * ------------------------------------------------------------------------------ * #
+  # * Changes below should persist in significant template updates.
```

### Comparing `boilercv-0.0.0/.gitignore` & `boilercv-0.0.1/.gitignore`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-# * -------------------------------------------------------------------------------- * #
-# * Changes below should persist in significant template updates.
-
-# * -------------------------------------------------------------------------------- * #
-# * Changes below may be lost in significant template updates.
-
-# To avoid committing profiler results
-*.prof
-# To avoid committing rejected changes upon bumping template
-*.rej
-# Don't commit first time setup script from copier-python-init
-first_time_setup.ps1
-# Don't commit code workspace files, which might be symlinked here
-*.code-workspace
-# Avoid committing local docs builds for previewing
-_site
-# If using Google Cloud Platform Workload Identity Federation, avoid committing keys
-# Ignore generated credentials from google-github-actions/auth
-gha-creds-*.json
-
-# * -------------------------------------------------------------------------------- * #
-# * Partial Node.gitignore
-# *
-# * https://raw.githubusercontent.com/github/gitignore/master/Node.gitignore
-
-# NPM/Node.JS because of Pyright CI/CD dependency
-node_modules/
-
-# * -------------------------------------------------------------------------------- * #
-# * Modifications to the below Python.gitignore
-# *
-# * https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore
-
-
-# IPython
-.ipython/profile_default/*
-!.ipython/profile_default/startup/
-.ipython/profile_default/startup/README
-ipython_config.py
-
-
-# * -------------------------------------------------------------------------------- * #
-# * Modifications to the below Python.gitignore
-# *
-# * https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore
-
-
-# IPython
-.ipython/profile_default/*
-!.ipython/profile_default/startup/
-.ipython/profile_default/startup/README
-ipython_config.py
-
-
-# * -------------------------------------------------------------------------------- * #
-# * Modified Python.gitignore
-# *
-# * https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore
-
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+# * -------------------------------------------------------------------------------- * #
+# * Changes below should persist in significant template updates.
+
+# * -------------------------------------------------------------------------------- * #
+# * Changes below may be lost in significant template updates.
+
+# To avoid committing profiler results
+*.prof
+# To avoid committing rejected changes upon bumping template
+*.rej
+# Don't commit first time setup script from copier-python-init
+first_time_setup.ps1
+# Don't commit code workspace files, which might be symlinked here
+*.code-workspace
+# Avoid committing local docs builds for previewing
+_site
+# If using Google Cloud Platform Workload Identity Federation, avoid committing keys
+# Ignore generated credentials from google-github-actions/auth
+gha-creds-*.json
+
+# * -------------------------------------------------------------------------------- * #
+# * Partial Node.gitignore
+# *
+# * https://raw.githubusercontent.com/github/gitignore/master/Node.gitignore
+
+# NPM/Node.JS because of Pyright CI/CD dependency
+node_modules/
+
+# * -------------------------------------------------------------------------------- * #
+# * Modifications to the below Python.gitignore
+# *
+# * https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore
+
+
+# IPython
+.ipython/profile_default/*
+!.ipython/profile_default/startup/
+.ipython/profile_default/startup/README
+ipython_config.py
+
+
+# * -------------------------------------------------------------------------------- * #
+# * Modifications to the below Python.gitignore
+# *
+# * https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore
+
+
+# IPython
+.ipython/profile_default/*
+!.ipython/profile_default/startup/
+.ipython/profile_default/startup/README
+ipython_config.py
+
+
+# * -------------------------------------------------------------------------------- * #
+# * Modified Python.gitignore
+# *
+# * https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore
+
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
```

### Comparing `boilercv-0.0.0/.gitmodules` & `boilercv-0.0.1/.gitmodules`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# * -------------------------------------------------------------------------------- * #
-# * Changes below should persist in significant template updates.
-
-# * -------------------------------------------------------------------------------- * #
-# * Changes below may be lost in significant template updates.
-
-[submodule "template"]
-	path = template
-	url = https://github.com/blakeNaccarato/copier-python.git
-[submodule "typings"]
-	path = typings
-	url = https://github.com/blakeNaccarato/pylance-stubs-unofficial.git
+# * -------------------------------------------------------------------------------- * #
+# * Changes below should persist in significant template updates.
+
+# * -------------------------------------------------------------------------------- * #
+# * Changes below may be lost in significant template updates.
+
+[submodule "template"]
+	path = template
+	url = https://github.com/blakeNaccarato/copier-python.git
+[submodule "typings"]
+	path = typings
+	url = https://github.com/blakeNaccarato/pylance-stubs-unofficial.git
```

### Comparing `boilercv-0.0.0/.pre-commit-config.yaml` & `boilercv-0.0.1/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,79 @@
-# Note: Can't use anything in `.venv` for local hooks when commiting from VSCode GUI.
-# This is because VSCode Source Control doesn't activate `.venv` before running `git
-# commit`.
-#
-# Example script to run via "target: pwsh script.ps1"
-#
-#     & ./.venv/Scripts/Activate.ps1
-#     foreach ($arg in $args) {
-#         autoflake -i --remove-all-unused-imports --ignore-init-module-imports $arg
-#     }
-#
-# (https://github.com/microsoft/vscode-python/issues/10165)
-
-ci:
-  skip:
-    - "pytest"
-    - "pyright"
-    - "dvc-pre-commit"
-    - "dvc-post-checkout"
-    - "dvc-pre-push"
-  autoupdate_schedule: "quarterly"
-
-repos:
-  # * ------------------------------------------------------------------------------ * #
-  # * Changes below should persist in significant template updates.
-
-  - repo: "https://github.com/iterative/dvc"
-    rev: "2.53.0"
-    hooks:
-      - id: "dvc-pre-commit"
-      - id: "dvc-post-checkout"
-      - id: "dvc-pre-push"
-        additional_dependencies: ["dvc[gs]"]
-
-  # * ------------------------------------------------------------------------------ * #
-  # * Changes below may be lost in significant template updates.
-
-  - repo: local
-    hooks:
-      - id: pytest
-        name: pytest
-        language: system
-        entry: pwsh -Command pytest
-        pass_filenames: false
-        always_run: true
-      - id: pyright
-        name: pyright
-        language: system
-        entry: pwsh -Command pyright
-  - repo: "https://github.com/pre-commit/pre-commit-hooks"
-    rev: "v4.4.0"
-    hooks:
-      - id: "end-of-file-fixer"
-      - id: "trailing-whitespace"
-  - repo: "https://github.com/DavidAnson/markdownlint-cli2"
-    rev: "v0.6.0"
-    hooks:
-      - id: "markdownlint-cli2-fix"
-  - repo: "https://github.com/psf/black"
-    rev: "23.3.0"
-    hooks:
-      - id: "black"
-  - repo: "https://github.com/charliermarsh/ruff-pre-commit"
-    rev: "v0.0.260"
-    hooks:
-      - id: "ruff"
-  - repo: "https://github.com/srstevenson/nb-clean"
-    rev: "2.4.0"
-    hooks:
-      - id: "nb-clean"
-        args:
-          - "--remove-empty-cells"
-          - "--preserve-cell-metadata"
-          - "tags"
-          - "slideshow"
-          - "special"
-          - "--"
-  - repo: "https://github.com/asottile/blacken-docs"
-    rev: "1.13.0"
-    hooks:
-      - id: "blacken-docs"
-        additional_dependencies: ["black==23.3.0"]
-  - repo: "https://github.com/nbQA-dev/nbQA"
-    rev: "1.7.0"
-    hooks:
-      - id: "nbqa-black"
-        additional_dependencies: ["black==23.3.0"]
-      - id: "nbqa-ruff"
-        additional_dependencies: ["ruff==0.0.260"]
+ci:
+  skip:
+    - "pytest"
+    - "pyright"
+    - "dvc-pre-commit"
+    - "dvc-post-checkout"
+    - "dvc-pre-push"
+  autoupdate_schedule: "quarterly"
+
+repos:
+  # * ------------------------------------------------------------------------------ * #
+  # * Changes below should persist in significant template updates.
+
+  - repo: "https://github.com/iterative/dvc"
+    rev: "2.53.0"
+    hooks:
+      - id: "dvc-pre-commit"
+      - id: "dvc-post-checkout"
+      - id: "dvc-pre-push"
+        additional_dependencies: ["dvc[gs]"]
+
+  # * ------------------------------------------------------------------------------ * #
+  # * Changes below may be lost in significant template updates.
+
+  - repo: local
+    hooks:
+      - id: pytest
+        name: pytest
+        language: system
+        entry: pwsh -Command pytest
+        pass_filenames: false
+        files: '^((tests\/)|(src\/)).*$'
+      - id: pyright
+        name: pyright
+        language: system
+        entry: pwsh -Command pyright
+        pass_filenames: false
+        files: '^((tests\/)|(src\/)).*$'
+
+  - repo: "https://github.com/pre-commit/pre-commit-hooks"
+    rev: "v4.4.0"
+    hooks:
+      - id: "end-of-file-fixer"
+      - id: "trailing-whitespace"
+  - repo: "https://github.com/DavidAnson/markdownlint-cli2"
+    rev: "v0.6.0"
+    hooks:
+      - id: "markdownlint-cli2-fix"
+  - repo: "https://github.com/psf/black"
+    rev: "23.3.0"
+    hooks:
+      - id: "black"
+  - repo: "https://github.com/charliermarsh/ruff-pre-commit"
+    rev: "v0.0.260"
+    hooks:
+      - id: "ruff"
+  - repo: "https://github.com/srstevenson/nb-clean"
+    rev: "2.4.0"
+    hooks:
+      - id: "nb-clean"
+        args:
+          - "--remove-empty-cells"
+          - "--preserve-cell-metadata"
+          - "tags"
+          - "slideshow"
+          - "special"
+          - "--"
+  - repo: "https://github.com/asottile/blacken-docs"
+    rev: "1.13.0"
+    hooks:
+      - id: "blacken-docs"
+        additional_dependencies: ["black==23.3.0"]
+  - repo: "https://github.com/nbQA-dev/nbQA"
+    rev: "1.7.0"
+    hooks:
+      - id: "nbqa-black"
+        additional_dependencies: ["black==23.3.0"]
+      - id: "nbqa-ruff"
+        additional_dependencies: ["ruff==0.0.260"]
```

### Comparing `boilercv-0.0.0/.tools/pyproject.toml` & `boilercv-0.0.1/.tools/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-# * -------------------------------------------------------------------------------- * #
-# * Changes below should persist in significant template updates.
-
-# * -------------------------------------------------------------------------------- * #
-# * Changes below may be lost in significant template updates.
-
-[build-system]
-requires = ["flit_core >=3.3,<4"]
-build-backend = "flit_core.buildapi"
-
-
-[project]
-name = "boilercv"
-version = "0.0.0"
-description = "Computer vision routines suitable for nucleate pool boiling bubble analysis"
-readme = "README.md"
-license = { file = "LICENSE" }
-requires-python = ">=3.11"
-classifiers = ["License :: OSI Approved :: MIT License"]
-[[project.authors]]
-name = "Blake Naccarato"
-email = "blake.naccarato+captivate@gmail.com"
-[[project.authors]]
-name = "Kwang Jin Kim"
-
-[project.urls]
-changes = "https://blakenaccarato.github.io/boilercv/changelog.html"
-docs = "https://blakenaccarato.github.io/boilercv/"
-home = "https://github.com/blakeNaccarato/boilercv"
-tracker = "https://github.com/blakeNaccarato/boilercv/issues"
-
-[tool.ruff]
-fix = true
-select = ["ALL"]
-src = ["src", "tests"]
-target-version = "py311"
-extend-exclude = ["template", "typings", ".github", ".tools", ".venv"]
-ignore = [
-    # * ---------------------------------------------------------------------------- * #
-    # * Changes below should persist in significant template updates.
-
-    # * ---------------------------------------------------------------------------- * #
-    # * Changes below may be lost in significant template updates.
-
-    "ANN",     # Don't require type annotations
-    "ARG005",  # Allow unused lambda argument. For consistency across df pipelines.
-    "C408",    # Allow dict calls
-    "COM",     # Allow magic commas and magic missing commas
-    "D10",     # Missing docstrings
-    "D20",     # Don't reformat docstrings in these ways
-    "D213",    # Multi-line docstring summary should start at the second line
-    "D402",    # False positives for parens in first line
-    "DTZ",     # Timezones are important, but only contextually necessary.
-    "E501",    # Don't check line length. Black handles this.
-    "EM",      # Don't check for exception message issues
-    "ERA",     # False positives. Don't get rid of commented out code.
-    "FBT",     # Allow boolean "traps"
-    "F841",    # Don't check for or fix unused variables
-    "G0",      # Allow f-strings, etc. in Loguru logging
-    "INP001",  # False positives. Checks for packages missing `__init__.py`
-    "ISC",     # False positives. Implicit string concatenation is fine.
-    "PD013",   # Allow `stack` instead of `melt`. They're not a direct swap.
-    "PD901",   # Allow `df` variable name. We are all consenting adults here.
-    "PD011",   # Allow use of `.values`. False positives.
-    "PGH003",  # Until black stops wrapping special ignores, let's allow bare
-    "PLR0913", # Allow more than five function arguments
-    "PLR2004", # Allow magic values. This check is too sensitive
-    "PLW2901", # For loop variable
-    "RET",     # Return checks are flaky, Sourcery does fine analysing these paths
-    "S301",    # Don't warn about pickling. Allow me to shoot myself in the foot.
-    "TCH",     # Type checking linter doesn't play nicely with pydantic
-    "TRY003",  # Allow long exception messages
-    "W2",      # Allow whitespace issues. Fixed automatically by black.
-    # * ---------------------------------------------------------------------------- * #
-    # * These Jupyter-specific ignores can't be per-file-ignores
-    # * https://nbqa.readthedocs.io/en/latest/known-limitations.html
-    "B018", # Allow "useless" expressions, which do suppress outputs in notebooks
-    "F821", # Allow undefined names, such as `display`
-    "S101", # Allow assert
-    "T201", # Allow print in notebooks
-]
-unfixable = [
-    # * ---------------------------------------------------------------------------- * #
-    # * Changes below should persist in significant template updates.
-
-    # * ---------------------------------------------------------------------------- * #
-    # * Changes below may be lost in significant template updates.
-
-    "F601", # Don't fix duplicate mapping keys
-]
-
-[tool.ruff.pydocstyle]
-convention = "google"
-
-[tool.ruff.isort]
-# * ---------------------------------------------------------------------------- * #
-# * Changes below should persist in significant template updates.
-
-# * ---------------------------------------------------------------------------- * #
-# * Changes below may be lost in significant template updates.
-split-on-trailing-comma = false
-
-[tool.ruff.per-file-ignores]
-"tests/**" = [
-    # * ---------------------------------------------------------------------------- * #
-    # * Changes below should persist in significant template updates.
-
-    "N815", # Allow camelCase in cine metadata models, which map to C structures
-
-    # * ---------------------------------------------------------------------------- * #
-    # * Changes below may be lost in significant template updates.
-
-    "ARG001", # Allow unused arguments in tests
-    "S101",   # Allow assert in tests
-]
-"src/boilercv/video/cine/**" = [
-    "N815", # Allow camelCase in cine metadata models, which map to C structures
-]
-
-[tool.ruff.flake8-bugbear]
-extend-immutable-calls = ["typer.Argument", "typer.Option"]
-
-[tool.ruff.pep8-naming]
-classmethod-decorators = ["pydantic.validator"]
+# * -------------------------------------------------------------------------------- * #
+# * Changes below should persist in significant template updates.
+
+# * -------------------------------------------------------------------------------- * #
+# * Changes below may be lost in significant template updates.
+
+[build-system]
+requires = ["flit_core >=3.3,<4"]
+build-backend = "flit_core.buildapi"
+
+
+[project]
+name = "boilercv"
+version = "0.0.1"
+description = "Computer vision routines suitable for nucleate pool boiling bubble analysis"
+readme = "README.md"
+license = { file = "LICENSE" }
+requires-python = ">=3.11"
+classifiers = ["License :: OSI Approved :: MIT License"]
+[[project.authors]]
+name = "Blake Naccarato"
+email = "blake.naccarato+boilercv@gmail.com"
+[[project.authors]]
+name = "Kwang Jin Kim"
+
+[project.urls]
+changes = "https://blakenaccarato.github.io/boilercv/changelog.html"
+docs = "https://blakenaccarato.github.io/boilercv/"
+home = "https://github.com/blakeNaccarato/boilercv"
+tracker = "https://github.com/blakeNaccarato/boilercv/issues"
+
+[tool.ruff]
+fix = true
+select = ["ALL"]
+src = ["src", "tests"]
+target-version = "py311"
+extend-exclude = ["template", "typings", ".github", ".tools", ".venv"]
+ignore = [
+    # * ---------------------------------------------------------------------------- * #
+    # * Changes below should persist in significant template updates.
+
+    # * ---------------------------------------------------------------------------- * #
+    # * Changes below may be lost in significant template updates.
+
+    "ANN",     # Don't require type annotations
+    "ARG005",  # Allow unused lambda argument. For consistency across df pipelines.
+    "C408",    # Allow dict calls
+    "COM",     # Allow magic commas and magic missing commas
+    "D10",     # Missing docstrings
+    "D20",     # Don't reformat docstrings in these ways
+    "D213",    # Multi-line docstring summary should start at the second line
+    "D402",    # False positives for parens in first line
+    "DTZ",     # Timezones are important, but only contextually necessary.
+    "E501",    # Don't check line length. Black handles this.
+    "EM",      # Don't check for exception message issues
+    "ERA",     # False positives. Don't get rid of commented out code.
+    "FBT",     # Allow boolean "traps"
+    "F841",    # Don't check for or fix unused variables
+    "G0",      # Allow f-strings, etc. in Loguru logging
+    "INP001",  # False positives. Checks for packages missing `__init__.py`
+    "ISC",     # False positives. Implicit string concatenation is fine.
+    "PD013",   # Allow `stack` instead of `melt`. They're not a direct swap.
+    "PD901",   # Allow `df` variable name. We are all consenting adults here.
+    "PD011",   # Allow use of `.values`. False positives.
+    "PGH003",  # Until black stops wrapping special ignores, let's allow bare
+    "PLR0913", # Allow more than five function arguments
+    "PLR2004", # Allow magic values. This check is too sensitive
+    "PLW2901", # For loop variable
+    "RET",     # Return checks are flaky, Sourcery does fine analysing these paths
+    "S301",    # Don't warn about pickling. Allow me to shoot myself in the foot.
+    "TCH",     # Type checking linter doesn't play nicely with pydantic
+    "TRY003",  # Allow long exception messages
+    "W2",      # Allow whitespace issues. Fixed automatically by black.
+    # * ---------------------------------------------------------------------------- * #
+    # * These Jupyter-specific ignores can't be per-file-ignores
+    # * https://nbqa.readthedocs.io/en/latest/known-limitations.html
+    "B018", # Allow "useless" expressions, which do suppress outputs in notebooks
+    "F821", # Allow undefined names, such as `display`
+    "S101", # Allow assert
+    "T201", # Allow print in notebooks
+]
+unfixable = [
+    # * ---------------------------------------------------------------------------- * #
+    # * Changes below should persist in significant template updates.
+
+    # * ---------------------------------------------------------------------------- * #
+    # * Changes below may be lost in significant template updates.
+
+    "F601", # Don't fix duplicate mapping keys
+]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.ruff.isort]
+# * ---------------------------------------------------------------------------- * #
+# * Changes below should persist in significant template updates.
+
+# * ---------------------------------------------------------------------------- * #
+# * Changes below may be lost in significant template updates.
+split-on-trailing-comma = false
+
+[tool.ruff.per-file-ignores]
+"tests/**" = [
+    # * ---------------------------------------------------------------------------- * #
+    # * Changes below should persist in significant template updates.
+
+    "N815", # Allow camelCase in cine metadata models, which map to C structures
+
+    # * ---------------------------------------------------------------------------- * #
+    # * Changes below may be lost in significant template updates.
+
+    "ARG001", # Allow unused arguments in tests
+    "S101",   # Allow assert in tests
+]
+"src/boilercv/video/cine/**" = [
+    "N815", # Allow camelCase in cine metadata models, which map to C structures
+]
+
+[tool.ruff.flake8-bugbear]
+extend-immutable-calls = ["typer.Argument", "typer.Option"]
+
+[tool.ruff.pep8-naming]
+classmethod-decorators = ["pydantic.validator"]
```

### Comparing `boilercv-0.0.0/.tools/scripts/compose_pyproject.py` & `boilercv-0.0.1/template/.tools/scripts/compose_pyproject.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Bump `pyproject.toml` with changes in `requirements.txt`."""
-
-from pathlib import Path
-
-import toml
-
-PYPROJECT = Path("pyproject.toml")
-REQUIREMENTS = Path("requirements.txt")
-SOURCE = ".tools" / PYPROJECT
-DESTINATION = Path("pyproject.toml")
-requirements = REQUIREMENTS.read_text(encoding="utf-8").splitlines()
-dependencies = [
-    line.rstrip().replace("==", ">=")
-    for line in requirements
-    if line and not line.startswith("#")
-]
-source = toml.loads(SOURCE.read_text(encoding="utf-8"))
-source["project"]["dependencies"] = dependencies
-DESTINATION.write_text(encoding="utf-8", data=toml.dumps(source))
+"""Bump `pyproject.toml` with changes in `requirements.txt`."""
+
+from pathlib import Path
+
+import toml
+
+PYPROJECT = Path("pyproject.toml")
+REQUIREMENTS = Path("requirements.txt")
+SOURCE = ".tools" / PYPROJECT
+DESTINATION = Path("pyproject.toml")
+requirements = REQUIREMENTS.read_text(encoding="utf-8").splitlines()
+dependencies = [
+    line.rstrip().replace("==", ">=")
+    for line in requirements
+    if line != "\n" and not line.startswith("#")
+]
+source = toml.loads(SOURCE.read_text(encoding="utf-8"))
+source["project"]["dependencies"] = dependencies
+DESTINATION.write_text(encoding="utf-8", data=toml.dumps(source))
```

### Comparing `boilercv-0.0.0/.vscode/c_cpp_properties.json` & `boilercv-0.0.1/.vscode/c_cpp_properties.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-00000000: 7b0d 0a20 2022 636f 6e66 6967 7572 6174  {..  "configurat
-00000010: 696f 6e73 223a 205b 0d0a 2020 2020 7b0d  ions": [..    {.
-00000020: 0a20 2020 2020 2022 6e61 6d65 223a 2022  .      "name": "
-00000030: 4c69 6e75 7822 2c0d 0a20 2020 2020 2022  Linux",..      "
-00000040: 696e 636c 7564 6550 6174 6822 3a20 5b22  includePath": ["
-00000050: 2f68 6f6d 652f 7573 6572 2f6f 7065 6e63  /home/user/openc
-00000060: 762d 7079 7468 6f6e 2f2a 2a22 5d2c 0d0a  v-python/**"],..
-00000070: 2020 2020 2020 2263 6f6d 7069 6c65 7250        "compilerP
-00000080: 6174 6822 3a20 222f 7573 722f 6269 6e2f  ath": "/usr/bin/
-00000090: 6763 6322 2c0d 0a20 2020 2020 2022 6353  gcc",..      "cS
-000000a0: 7461 6e64 6172 6422 3a20 2267 6e75 3137  tandard": "gnu17
-000000b0: 222c 0d0a 2020 2020 2020 2263 7070 5374  ",..      "cppSt
-000000c0: 616e 6461 7264 223a 2022 676e 752b 2b31  andard": "gnu++1
-000000d0: 3722 2c0d 0a20 2020 2020 2022 696e 7465  7",..      "inte
-000000e0: 6c6c 6953 656e 7365 4d6f 6465 223a 2022  lliSenseMode": "
-000000f0: 6c69 6e75 782d 6763 632d 7836 3422 0d0a  linux-gcc-x64"..
-00000100: 2020 2020 7d2c 0d0a 2020 2020 7b0d 0a20      },..    {.. 
-00000110: 2020 2020 2022 6e61 6d65 223a 2022 5769       "name": "Wi
-00000120: 6e33 3222 2c0d 0a20 2020 2020 2022 696e  n32",..      "in
-00000130: 636c 7564 6550 6174 6822 3a20 5b22 247b  cludePath": ["${
-00000140: 776f 726b 7370 6163 6546 6f6c 6465 727d  workspaceFolder}
-00000150: 2f2a 2a22 5d2c 0d0a 2020 2020 2020 2264  /**"],..      "d
-00000160: 6566 696e 6573 223a 205b 225f 4445 4255  efines": ["_DEBU
-00000170: 4722 2c20 2255 4e49 434f 4445 222c 2022  G", "UNICODE", "
-00000180: 5f55 4e49 434f 4445 225d 2c0d 0a20 2020  _UNICODE"],..   
-00000190: 2020 2022 7769 6e64 6f77 7353 646b 5665     "windowsSdkVe
-000001a0: 7273 696f 6e22 3a20 2231 302e 302e 3139  rsion": "10.0.19
-000001b0: 3034 312e 3022 2c0d 0a20 2020 2020 2022  041.0",..      "
-000001c0: 636f 6d70 696c 6572 5061 7468 223a 2022  compilerPath": "
-000001d0: 433a 2f50 726f 6772 616d 2046 696c 6573  C:/Program Files
-000001e0: 2028 7838 3629 2f4d 6963 726f 736f 6674   (x86)/Microsoft
-000001f0: 2056 6973 7561 6c20 5374 7564 696f 2f32   Visual Studio/2
-00000200: 3032 322f 4275 696c 6454 6f6f 6c73 2f56  022/BuildTools/V
-00000210: 432f 546f 6f6c 732f 4d53 5643 2f31 342e  C/Tools/MSVC/14.
-00000220: 3332 2e33 3133 3236 2f62 696e 2f48 6f73  32.31326/bin/Hos
-00000230: 7478 3634 2f78 3634 2f63 6c2e 6578 6522  tx64/x64/cl.exe"
-00000240: 2c0d 0a20 2020 2020 2022 6353 7461 6e64  ,..      "cStand
-00000250: 6172 6422 3a20 2263 3137 222c 0d0a 2020  ard": "c17",..  
-00000260: 2020 2020 2263 7070 5374 616e 6461 7264      "cppStandard
-00000270: 223a 2022 632b 2b31 3722 2c0d 0a20 2020  ": "c++17",..   
-00000280: 2020 2022 696e 7465 6c6c 6953 656e 7365     "intelliSense
-00000290: 4d6f 6465 223a 2022 7769 6e64 6f77 732d  Mode": "windows-
-000002a0: 6d73 7663 2d78 3634 220d 0a20 2020 207d  msvc-x64"..    }
-000002b0: 0d0a 2020 5d2c 0d0a 2020 2276 6572 7369  ..  ],..  "versi
-000002c0: 6f6e 223a 2034 0d0a 7d0d 0a              on": 4..}..
+00000000: 7b0a 2020 2263 6f6e 6669 6775 7261 7469  {.  "configurati
+00000010: 6f6e 7322 3a20 5b0a 2020 2020 7b0a 2020  ons": [.    {.  
+00000020: 2020 2020 226e 616d 6522 3a20 224c 696e      "name": "Lin
+00000030: 7578 222c 0a20 2020 2020 2022 696e 636c  ux",.      "incl
+00000040: 7564 6550 6174 6822 3a20 5b22 2f68 6f6d  udePath": ["/hom
+00000050: 652f 7573 6572 2f6f 7065 6e63 762d 7079  e/user/opencv-py
+00000060: 7468 6f6e 2f2a 2a22 5d2c 0a20 2020 2020  thon/**"],.     
+00000070: 2022 636f 6d70 696c 6572 5061 7468 223a   "compilerPath":
+00000080: 2022 2f75 7372 2f62 696e 2f67 6363 222c   "/usr/bin/gcc",
+00000090: 0a20 2020 2020 2022 6353 7461 6e64 6172  .      "cStandar
+000000a0: 6422 3a20 2267 6e75 3137 222c 0a20 2020  d": "gnu17",.   
+000000b0: 2020 2022 6370 7053 7461 6e64 6172 6422     "cppStandard"
+000000c0: 3a20 2267 6e75 2b2b 3137 222c 0a20 2020  : "gnu++17",.   
+000000d0: 2020 2022 696e 7465 6c6c 6953 656e 7365     "intelliSense
+000000e0: 4d6f 6465 223a 2022 6c69 6e75 782d 6763  Mode": "linux-gc
+000000f0: 632d 7836 3422 0a20 2020 207d 2c0a 2020  c-x64".    },.  
+00000100: 2020 7b0a 2020 2020 2020 226e 616d 6522    {.      "name"
+00000110: 3a20 2257 696e 3332 222c 0a20 2020 2020  : "Win32",.     
+00000120: 2022 696e 636c 7564 6550 6174 6822 3a20   "includePath": 
+00000130: 5b22 247b 776f 726b 7370 6163 6546 6f6c  ["${workspaceFol
+00000140: 6465 727d 2f2a 2a22 5d2c 0a20 2020 2020  der}/**"],.     
+00000150: 2022 6465 6669 6e65 7322 3a20 5b22 5f44   "defines": ["_D
+00000160: 4542 5547 222c 2022 554e 4943 4f44 4522  EBUG", "UNICODE"
+00000170: 2c20 225f 554e 4943 4f44 4522 5d2c 0a20  , "_UNICODE"],. 
+00000180: 2020 2020 2022 7769 6e64 6f77 7353 646b       "windowsSdk
+00000190: 5665 7273 696f 6e22 3a20 2231 302e 302e  Version": "10.0.
+000001a0: 3139 3034 312e 3022 2c0a 2020 2020 2020  19041.0",.      
+000001b0: 2263 6f6d 7069 6c65 7250 6174 6822 3a20  "compilerPath": 
+000001c0: 2243 3a2f 5072 6f67 7261 6d20 4669 6c65  "C:/Program File
+000001d0: 7320 2878 3836 292f 4d69 6372 6f73 6f66  s (x86)/Microsof
+000001e0: 7420 5669 7375 616c 2053 7475 6469 6f2f  t Visual Studio/
+000001f0: 3230 3232 2f42 7569 6c64 546f 6f6c 732f  2022/BuildTools/
+00000200: 5643 2f54 6f6f 6c73 2f4d 5356 432f 3134  VC/Tools/MSVC/14
+00000210: 2e33 322e 3331 3332 362f 6269 6e2f 486f  .32.31326/bin/Ho
+00000220: 7374 7836 342f 7836 342f 636c 2e65 7865  stx64/x64/cl.exe
+00000230: 222c 0a20 2020 2020 2022 6353 7461 6e64  ",.      "cStand
+00000240: 6172 6422 3a20 2263 3137 222c 0a20 2020  ard": "c17",.   
+00000250: 2020 2022 6370 7053 7461 6e64 6172 6422     "cppStandard"
+00000260: 3a20 2263 2b2b 3137 222c 0a20 2020 2020  : "c++17",.     
+00000270: 2022 696e 7465 6c6c 6953 656e 7365 4d6f   "intelliSenseMo
+00000280: 6465 223a 2022 7769 6e64 6f77 732d 6d73  de": "windows-ms
+00000290: 7663 2d78 3634 220a 2020 2020 7d0a 2020  vc-x64".    }.  
+000002a0: 5d2c 0a20 2022 7665 7273 696f 6e22 3a20  ],.  "version": 
+000002b0: 340a 7d0a                                4.}.
```

### Comparing `boilercv-0.0.0/.vscode/launch.json` & `boilercv-0.0.1/.vscode/launch.json`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-{
-  "version": "0.2.0",
-  "configurations": [
-    // * -------------------------------------------------------------------------- * //
-    // * Changes below should persist in significant template updates.
-
-    {
-      "name": "auto",
-      "type": "auto-debug",
-      "request": "launch",
-      "map": {
-        "*.py": "Python: Current file, OpenCV debug",
-        "*.ps1": "pwsh",
-        "*": "C++"
-      }
-    },
-    {
-      "name": "Python: Current file, OpenCV debug",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "console": "integratedTerminal",
-      "stopOnEntry": true,
-      "justMyCode": true,
-      "env": {
-        "OPENCV_LOG_LEVEL": "DEBUG"
-      }
-    },
-    {
-      "name": "pwsh",
-      "type": "PowerShell",
-      "request": "launch",
-      "script": "${file}",
-      "cwd": "${file}"
-    },
-    {
-      "name": "C++",
-      "type": "cppdbg",
-      "request": "attach",
-      "program": "${workspaceFolder}/.venv/bin/python",
-      "processId": "${command:pickProcess}",
-      "MIMode": "gdb",
-      "setupCommands": [
-        {
-          "description": "Enable pretty-printing for gdb",
-          "text": "-enable-pretty-printing",
-          "ignoreFailures": true
-        },
-        {
-          "description": "Set Disassembly Flavor to Intel",
-          "text": "-gdb-set disassembly-flavor intel",
-          "ignoreFailures": true
-        }
-      ]
-    },
-    {
-      "name": "Python: WRITE/PREVIEW",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "console": "internalConsole",
-      "justMyCode": true,
-      "env": {
-        "BOILERCV_DEBUG": "True",
-        "BOILERCV_WRITE": "True",
-        "BOILERCV_PREVIEW": "True"
-      }
-    },
-    {
-      "name": "Python: WRITE/PREVIEW, not just my code",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "console": "internalConsole",
-      "justMyCode": false,
-      "env": {
-        "BOILERCV_DEBUG": "True",
-        "BOILERCV_WRITE": "True",
-        "BOILERCV_PREVIEW": "True"
-      }
-    },
-    {
-      "name": "Python: WRITE",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "console": "internalConsole",
-      "justMyCode": true,
-      "env": {
-        "BOILERCV_DEBUG": "True",
-        "BOILERCV_WRITE": "True"
-      }
-    },
-    {
-      "name": "Python: WRITE, not just my code",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "console": "internalConsole",
-      "justMyCode": false,
-      "env": {
-        "BOILERCV_DEBUG": "True",
-        "BOILERCV_WRITE": "True"
-      }
-    },
-    {
-      "name": "Python: PREVIEW",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "console": "internalConsole",
-      "justMyCode": true,
-      "env": {
-        "BOILERCV_DEBUG": "True",
-        "BOILERCV_PREVIEW": "True"
-      }
-    },
-    {
-      "name": "Python: PREVIEW, not just my code",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "console": "internalConsole",
-      "justMyCode": false,
-      "env": {
-        "BOILERCV_DEBUG": "True",
-        "BOILERCV_PREVIEW": "True"
-      }
-    },
-
-    // * -------------------------------------------------------------------------- * //
-    // * Changes below may be lost in significant template updates.
-    {
-      "name": "Python: Current file",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "console": "internalConsole",
-      "env": {
-        "BOILERCV_DEBUG": "True"
-      }
-    },
-    {
-      "name": "Python: Current file, not just my code",
-      "type": "python",
-      "request": "launch",
-      "program": "${file}",
-      "justMyCode": false,
-      // "purpose": ["debug-test"], // Uncomment to debug tests more deeply.
-      "console": "internalConsole",
-      "env": {
-        "BOILERCV_DEBUG": "True"
-      }
-    }
-  ]
-}
+{
+  "version": "0.2.0",
+  "configurations": [
+    // * -------------------------------------------------------------------------- * //
+    // * Changes below should persist in significant template updates.
+
+    {
+      "name": "auto",
+      "type": "auto-debug",
+      "request": "launch",
+      "map": {
+        "*.py": "Python: Current file, OpenCV debug",
+        "*.ps1": "pwsh",
+        "*": "C++"
+      }
+    },
+    {
+      "name": "Python: Current file, OpenCV debug",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "console": "integratedTerminal",
+      "stopOnEntry": true,
+      "justMyCode": true,
+      "env": {
+        "OPENCV_LOG_LEVEL": "DEBUG"
+      }
+    },
+    {
+      "name": "pwsh",
+      "type": "PowerShell",
+      "request": "launch",
+      "script": "${file}",
+      "cwd": "${file}"
+    },
+    {
+      "name": "C++",
+      "type": "cppdbg",
+      "request": "attach",
+      "program": "${workspaceFolder}/.venv/bin/python",
+      "processId": "${command:pickProcess}",
+      "MIMode": "gdb",
+      "setupCommands": [
+        {
+          "description": "Enable pretty-printing for gdb",
+          "text": "-enable-pretty-printing",
+          "ignoreFailures": true
+        },
+        {
+          "description": "Set Disassembly Flavor to Intel",
+          "text": "-gdb-set disassembly-flavor intel",
+          "ignoreFailures": true
+        }
+      ]
+    },
+    {
+      "name": "Python: WRITE/PREVIEW",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "console": "internalConsole",
+      "justMyCode": true,
+      "env": {
+        "BOILERCV_DEBUG": "True",
+        "BOILERCV_WRITE": "True",
+        "BOILERCV_PREVIEW": "True"
+      }
+    },
+    {
+      "name": "Python: WRITE/PREVIEW, not just my code",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "console": "internalConsole",
+      "justMyCode": false,
+      "env": {
+        "BOILERCV_DEBUG": "True",
+        "BOILERCV_WRITE": "True",
+        "BOILERCV_PREVIEW": "True"
+      }
+    },
+    {
+      "name": "Python: WRITE",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "console": "internalConsole",
+      "justMyCode": true,
+      "env": {
+        "BOILERCV_DEBUG": "True",
+        "BOILERCV_WRITE": "True"
+      }
+    },
+    {
+      "name": "Python: WRITE, not just my code",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "console": "internalConsole",
+      "justMyCode": false,
+      "env": {
+        "BOILERCV_DEBUG": "True",
+        "BOILERCV_WRITE": "True"
+      }
+    },
+    {
+      "name": "Python: PREVIEW",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "console": "internalConsole",
+      "justMyCode": true,
+      "env": {
+        "BOILERCV_DEBUG": "True",
+        "BOILERCV_PREVIEW": "True"
+      }
+    },
+    {
+      "name": "Python: PREVIEW, not just my code",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "console": "internalConsole",
+      "justMyCode": false,
+      "env": {
+        "BOILERCV_DEBUG": "True",
+        "BOILERCV_PREVIEW": "True"
+      }
+    },
+
+    // * -------------------------------------------------------------------------- * //
+    // * Changes below may be lost in significant template updates.
+    {
+      "name": "Python: Current file",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "console": "internalConsole",
+      "env": {
+        "BOILERCV_DEBUG": "True"
+      }
+    },
+    {
+      "name": "Python: Current file, not just my code",
+      "type": "python",
+      "request": "launch",
+      "program": "${file}",
+      "justMyCode": false,
+      // "purpose": ["debug-test"], // Uncomment to debug tests more deeply.
+      "console": "internalConsole",
+      "env": {
+        "BOILERCV_DEBUG": "True"
+      }
+    }
+  ]
+}
```

### Comparing `boilercv-0.0.0/.vscode/settings.json` & `boilercv-0.0.1/template/.vscode/settings.json`

 * *Files 19% similar despite different names*

```diff
@@ -1,255 +1,220 @@
-{
-  // * ---------------------------------------------------------------------------- * //
-  // * Changes below should persist in significant template updates.
-
-  //! Schema
-  "yaml.schemas": {
-    "data/schema/params_schema.json": "params.yaml"
-  },
-
-  "git.ignoredRepositories": [
-    "/home/user/.cache",
-    "/home/user/opencv-python",
-    "/home/user/opencv-python/multibuild",
-    "/home/user/opencv-python/opencv_contrib",
-    "/home/user/opencv-python/opencv_extra",
-    "/home/user/opencv-python/opencv"
-  ],
-
-  // * ---------------------------------------------------------------------------- * //
-  // * Changes below may be lost in significant template updates.
-
-  // Environment variables don't load properly otherwise
-  // See: https://github.com/microsoft/vscode-python/issues/944#issuecomment-808516207
-  "terminal.integrated.defaultProfile.linux": "pwsh",
-
-  //! Pylance
-  "python.languageServer": "Pylance",
-  "python.analysis.diagnosticMode": "workspace",
-  "python.analysis.indexing": true,
-  //? These are safer defaults which are overridden in `pyrightconfig.json`.
-  "python.analysis.typeCheckingMode": "off",
-  "python.analysis.useLibraryCodeForTypes": false,
-  //? Refactoring
-  "python.analysis.fixAll": [
-    "source.convertImportFormat",
-    "source.unusedImports"
-  ],
-  "python.analysis.completeFunctionParens": false, // Buggy
-  "python.analysis.refactoring.allowMovingSymbols": true,
-  //? Auto imports
-  "python.analysis.importFormat": "absolute",
-  "python.analysis.autoImportUserSymbols": true,
-  "python.analysis.autoImportCompletions": true,
-  "python.analysis.extraCommitChars": true,
-  "python.analysis.addImport.exactMatchOnly": false,
-  //? Inlay hints
-  "editor.inlayHints.enabled": "offUnlessPressed",
-  "python.analysis.inlayHints.functionReturnTypes": true,
-  "python.analysis.inlayHints.variableTypes": true,
-  "python.analysis.inlayHints.pytestParameters": true,
-  //? See "include" and "extrapaths" in pyrightconfig.json
-  "python.analysis.autoSearchPaths": false,
-  //? Zero out the depth for packages which slow down Pylance
-  "python.analysis.packageIndexDepths": [
-    {
-      "name": "boilercine",
-      "depth": 0
-    },
-    {
-      "name": "matplotlib",
-      "depth": 2
-    },
-    {
-      "name": "cv2",
-      "depth": 0
-    },
-    {
-      "name": "PySide6",
-      "depth": 0
-    },
-    {
-      "name": "pyqtgraph",
-      "depth": 0
-    },
-    {
-      "name": "xarray",
-      "depth": 2
-    }
-  ],
-
-  //! Lint, test, format
-  //* pytest
-  "python.testing.unittestEnabled": false,
-  "python.testing.pytestEnabled": true,
-  //* markdownlint
-  "markdownlint.config": {
-    "first-line-heading": false
-  },
-  //* black
-  "black-formatter.importStrategy": "fromEnvironment",
-  //? Ensure user setting args are cleared
-  "black-formatter.logLevel": "warn",
-  "black-formatter.args": [],
-  //* ruff
-  "ruff.importStrategy": "fromEnvironment",
-  //? Ensure user setting args are cleared
-  "ruff.logLevel": "warn",
-  "ruff.args": [],
-
-  //! GitHub Actions
-  "github-actions.workflows.pinned.workflows": [".github/workflows/main.yml"],
-
-  //! Shell Launcher
-  "shellLauncher.shells.windows": [
-    {
-      //* Launches IPython in the virtual environment. Lets you try things out in without having to fire up an entire Jupyter notebook.
-      //*
-      //* Use alongside the following keybind in your "keybindings.json".
-      //*
-      //? {
-      //?   "key": "ctrl+alt+1",
-      //?   "command": "shellLauncher.launch"
-      //? },
-      "label": "IPython (.venv)",
-      "shell": "pwsh.exe",
-      "args": ["-NoExit", "-Command", "python", "-m", "IPython"]
-    }
-  ],
-
-  //! Files
-  //* Experimental file nesting
-  "explorer.sortOrder": "foldersNestsFiles",
-  "explorer.fileNesting.enabled": true,
-  "explorer.fileNesting.expand": false,
-  "explorer.fileNesting.patterns": {
-    "*.ts": "${capture}.js",
-    "*.js": "${capture}.js.map, ${capture}.min.js, ${capture}.d.ts",
-    "*.jsx": "${capture}.js",
-    "*.tsx": "${capture}.ts",
-    "tsconfig.json": "tsconfig.*.json",
-    "package.json": "package-lock.json, yarn.lock, pnpm-lock.yaml",
-    ".nest_tools_config": "coverage.xml, setup.ps1, update.ps1, *.code-workspace, *.prof, .copier-answers.yml, .coverage, .coveragerc, .env, .gitattributes, .gitmodules, .markdownlint.yaml, .pre-commit-config.yaml, .pytest_cache, .sourcery.yaml, codecov.yml, pyproject.toml, pyrightconfig.json, pytest.ini, pythonrc.py, renovate.json",
-    ".nest_md": "*.md, CITATION.cff, LICENSE"
-  },
-  //* File associations
-  "files.associations": {
-    ".coveragerc": "ini",
-    "*.env": "dotenv",
-    ".pylintrc": "ini",
-    "pyrightconfig.json": "jsonc",
-    "*requirements*.txt": "pip-requirements",
-    "repro.txt": "pip-requirements",
-    ".nest_md": "markdown",
-    ".nest_tools_config": "plaintext",
-    ".sourcery.yaml": "yaml"
-  },
-  //* File icon associations
-  "workbench.iconTheme": "vscode-icons",
-  "vsicons.presets.hideExplorerArrows": true,
-  "vsicons.dontShowNewVersionMessage": false,
-  "vsicons.associations.files": [
-    { "icon": "ini", "extensions": ["nest_tools_config"], "format": "svg" },
-    { "icon": "markdown", "extensions": ["nest_md"], "format": "svg" }
-  ],
-
-  //! Built-in
-  //* Allow auto-running tasks
-  "task.allowAutomaticTasks": "on",
-  //* Enable native bracket pair colorization
-  "editor.bracketPairColorization.enabled": true,
-  "editor.guides.bracketPairs": true,
-  //* Editor format on save and more. Can run "File: Save without formatting" to skip.
-  "editor.formatOnType": true,
-  "editor.formatOnSave": true,
-  "python.formatting.provider": "black",
-  "editor.codeActionsOnSave": {
-    "source.fixAll": false,
-    "source.organizeImports": false
-  },
-  //* Enforce whitespace and newlines.
-  "files.insertFinalNewline": true,
-  "files.trimTrailingWhitespace": true,
-  "files.trimFinalNewlines": true,
-  //* Periodically fetch changes to tracked repo. Don't confirm on push/pull.
-  "git.autofetch": true,
-  "git.confirmSync": false,
-  //* Markdown editor moves jarringly when this is "true"
-  "markdown.preview.scrollEditorWithPreview": false,
-  //* Exclude
-  "search.exclude": {
-    "**/node_modules": true,
-    "**/bower_components": true,
-    "**/*.code-search": true,
-    "typings": true,
-    "template": true
-  },
-
-  //! Line-width
-  //* Formatting
-  "rewrap.wrappingColumn": 88,
-  "rewrap.wholeComment": false,
-  //* Don't validate the body of a commit. Assume people can wrap it in their IDE.
-  "git.inputValidationSubjectLength": 88,
-  "git.inputValidationLength": 1e100,
-  //* Default wrapping
-  "editor.wordWrapColumn": 88,
-  "editor.rulers": [88],
-
-  //! Filetype specifics
-  //* .ENV
-  "[dotenv]": {
-    "editor.wordWrap": "wordWrapColumn",
-    "rewrap.autoWrap.enabled": false
-  },
-  //* MD
-  "[markdown]": {
-    "editor.defaultFormatter": "DavidAnson.vscode-markdownlint",
-    "editor.wordWrap": "wordWrapColumn",
-    //? Roughly matches the width of GitHub Markdown
-    "editor.wordWrapColumn": 124,
-    "editor.rulers": [124],
-    "rewrap.autoWrap.enabled": false
-  },
-  //* JSON
-  "[json]": {
-    "editor.wordWrap": "wordWrapColumn",
-    "editor.defaultFormatter": "esbenp.prettier-vscode"
-  },
-  "[jsonc]": {
-    "editor.wordWrap": "wordWrapColumn",
-    "editor.defaultFormatter": "esbenp.prettier-vscode"
-  },
-  //* PYTHON
-  "[python]": {
-    "editor.defaultFormatter": "ms-python.black-formatter"
-  },
-  //* IPYNB
-  "[ipynb]": {
-    "editor.defaultFormatter": "ms-python.black-formatter"
-  },
-  //* TXT
-  "[plaintext]": {
-    "editor.wordWrap": "wordWrapColumn"
-  },
-  //* TOML
-  "evenBetterToml.formatter.columnWidth": 88,
-  "[toml]": {
-    "editor.wordWrap": "wordWrapColumn",
-    "editor.defaultFormatter": "tamasfe.even-better-toml"
-  },
-  //* TSV
-  "[tsv]": {
-    //? Indent with tabs
-    "editor.insertSpaces": false
-  },
-  //* YAML
-  "yaml.format.printWidth": 88,
-  "[yaml]": {
-    "editor.defaultFormatter": "esbenp.prettier-vscode",
-    "editor.wordWrap": "wordWrapColumn"
-  },
-
-  //! Extension: Jupyter Notebooks
-  "jupyter.notebookFileRoot": "${workspaceFolder}"
-}
+{
+  // * ---------------------------------------------------------------------------- * //
+  // * Changes below should persist in significant template updates.
+
+  //! Files
+  "explorer.fileNesting.patterns": {
+    "*.ts": "${capture}.js",
+    "*.js": "${capture}.js.map, ${capture}.min.js, ${capture}.d.ts",
+    "*.jsx": "${capture}.js",
+    "*.tsx": "${capture}.ts",
+    "tsconfig.json": "tsconfig.*.json",
+    "package.json": "package-lock.json, yarn.lock, pnpm-lock.yaml",
+    "*.nest_tools_config": "coverage.xml, setup.ps1, update.ps1, *.code-workspace, *.prof, .copier-answers.yml, .coverage, .coveragerc, .env, .gitattributes, .gitmodules, .markdownlint.yaml, .pre-commit-config.yaml, .pytest_cache, .sourcery.yaml, codecov.yml, pyrightconfig.json, pytest.ini, pythonrc.py, renovate.json, *.jinja",
+    "*.nest_md": "*.md.jinja, LICENSE.jinja",
+    ".nest_tools_config_top": "coverage.xml, setup.ps1, update.ps1, *.code-workspace, *.prof, .copier-answers.yml, .coverage, .coveragerc, .env, .gitattributes, .gitmodules, .markdownlint.yaml, .pre-commit-config.yaml, .pytest_cache, .sourcery.yaml, codecov.yml, pyrightconfig.json, pytest.ini, pythonrc.py, renovate.json",
+    ".nest_md_top": "*.md, LICENSE"
+  },
+  //* File associations
+  "files.associations": {
+    ".coveragerc": "ini",
+    ".env": "dotenv",
+    ".pylintrc": "ini",
+    "pyrightconfig.json": "jsonc",
+    "*requirements*.txt": "pip-requirements",
+    ".nest_md*": "markdown",
+    ".nest_tools_config*": "plaintext",
+    ".sourcery.yaml": "yaml"
+  },
+
+  "yaml.schemas": {
+    "https://json.schemastore.org/github-workflow.json": ["*.yml.jinja"]
+  },
+
+  //! Jinja
+  "[jinja-md]": {
+    //* Roughly matches the width of GitHub Markdown
+    "editor.wordWrap": "wordWrapColumn",
+    "editor.wordWrapColumn": 124,
+    "editor.rulers": [124]
+  },
+  "[jinja-yaml]": {
+    "editor.wordWrap": "wordWrapColumn"
+  },
+  "[jinja-toml]": {
+    "editor.wordWrap": "wordWrapColumn"
+  },
+
+  // * ---------------------------------------------------------------------------- * //
+  // * Changes below may be lost in significant template updates.
+
+  // Environment variables don't load properly otherwise
+  // See: https://github.com/microsoft/vscode-python/issues/944#issuecomment-808516207
+  "terminal.integrated.defaultProfile.linux": "pwsh",
+
+  //! Pylance
+  //* Pylance settings aren't very discoverable.
+  //* https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance
+  "python.languageServer": "Pylance",
+  "python.analysis.diagnosticMode": "workspace",
+  "python.analysis.indexing": true,
+  //? Auto imports
+  "python.analysis.autoImportCompletions": true,
+  "python.analysis.extraCommitChars": true,
+  //? Inlay hints
+  "editor.inlayHints.enabled": "offUnlessPressed",
+  "python.analysis.inlayHints.functionReturnTypes": true,
+  "python.analysis.inlayHints.variableTypes": true,
+  //? See "include" and "extrapaths" in pyrightconfig.json
+  "python.analysis.autoSearchPaths": false,
+  //? See "useLibraryCodeForTypes" in pyrightconfig.json
+  "python.analysis.typeCheckingMode": "off",
+  "python.analysis.completeFunctionParens": false, // Buggy for now
+
+  //! Lint, test, format
+  //* pytest
+  "python.testing.unittestEnabled": false,
+  "python.testing.pytestEnabled": true,
+  //* markdownlint
+  "markdownlint.config": {
+    "first-line-heading": false
+  },
+  //* black
+  "black-formatter.importStrategy": "fromEnvironment",
+  "black-formatter.args": [],
+  //* ruff
+  "ruff.importStrategy": "fromEnvironment",
+
+  //! GitHub Actions
+  "github-actions.workflows.pinned.workflows": [".github/workflows/main.yml"],
+
+  //! Shell Launcher
+  "shellLauncher.shells.windows": [
+    {
+      //* Launches IPython in the virtual environment. Lets you try things out in without having to fire up an entire Jupyter notebook.
+      //*
+      //* Use alongside the following keybind in your "keybindings.json".
+      //*
+      //? {
+      //?   "key": "ctrl+alt+1",
+      //?   "command": "shellLauncher.launch"
+      //? },
+      "label": "IPython (.venv)",
+      "shell": "pwsh.exe",
+      "args": ["-NoExit", "-Command", "python", "-m", "IPython"]
+    }
+  ],
+
+  //! Files
+  //* Experimental file nesting
+  "explorer.sortOrder": "foldersNestsFiles",
+  "explorer.fileNesting.enabled": true,
+  "explorer.fileNesting.expand": false,
+  //* File icon associations
+  "workbench.iconTheme": "vscode-icons",
+  "vsicons.presets.hideExplorerArrows": true,
+  "vsicons.dontShowNewVersionMessage": false,
+  "vsicons.associations.files": [
+    { "icon": "ini", "extensions": ["nest_tools_config"], "format": "svg" },
+    { "icon": "markdown", "extensions": ["nest_md"], "format": "svg" }
+  ],
+
+  //! Built-in
+  //* Allow auto-running tasks
+  "task.allowAutomaticTasks": "on",
+  //* Enable native bracket pair colorization
+  "editor.bracketPairColorization.enabled": true,
+  "editor.guides.bracketPairs": true,
+  //* Editor format on save and more. Can run "File: Save without formatting" to skip.
+  "editor.formatOnPaste": true,
+  "editor.formatOnType": true,
+  "editor.formatOnSave": true,
+  "editor.formatOnSaveMode": "file",
+  "editor.codeActionsOnSave": {
+    "source.fixAll": true,
+    "source.organizeImports": true
+  },
+  //* Enforce whitespace and newlines.
+  "files.insertFinalNewline": true,
+  "files.trimTrailingWhitespace": true,
+  "files.trimFinalNewlines": true,
+  //* Periodically fetch changes to tracked repo. Don't confirm on push/pull.
+  "git.autofetch": true,
+  "git.confirmSync": false,
+  //* Markdown editor moves jarringly when this is "true"
+  "markdown.preview.scrollEditorWithPreview": false,
+  //* Exclude
+  "search.exclude": {
+    "**/node_modules": true,
+    "**/bower_components": true,
+    "**/*.code-search": true
+  },
+
+  //! Line-width
+  //* Formatting
+  "rewrap.wrappingColumn": 88,
+  "rewrap.wholeComment": false,
+  //* Don't validate the body of a commit. Assume people can wrap it in their IDE.
+  "git.inputValidationSubjectLength": 88,
+  "git.inputValidationLength": 1e100,
+  //* Default wrapping
+  "editor.wordWrapColumn": 88,
+  "editor.rulers": [88],
+
+  //! Filetype specifics
+  //* .ENV
+  "[dotenv]": {
+    "editor.wordWrap": "wordWrapColumn",
+    "rewrap.autoWrap.enabled": false
+  },
+  //* IPYNB
+  "[ipynb]": {
+    "editor.defaultFormatter": "ms-python.black-formatter"
+  },
+  //* MD
+  "[markdown]": {
+    "editor.defaultFormatter": "DavidAnson.vscode-markdownlint",
+    "editor.wordWrap": "wordWrapColumn",
+    //? Roughly matches the width of GitHub Markdown
+    "editor.wordWrapColumn": 124,
+    "editor.rulers": [124],
+    "rewrap.autoWrap.enabled": false
+  },
+  //* JSON
+  "[json]": {
+    "editor.wordWrap": "wordWrapColumn",
+    "editor.defaultFormatter": "esbenp.prettier-vscode"
+  },
+  "[jsonc]": {
+    "editor.wordWrap": "wordWrapColumn",
+    "editor.defaultFormatter": "esbenp.prettier-vscode"
+  },
+  //* PYTHON
+  "[python]": {
+    "editor.defaultFormatter": "ms-python.black-formatter"
+  },
+  //* TXT
+  "[plaintext]": {
+    "editor.wordWrap": "wordWrapColumn"
+  },
+  //* TOML
+  "evenBetterToml.formatter.columnWidth": 88,
+  "[toml]": {
+    "editor.wordWrap": "wordWrapColumn",
+    "editor.defaultFormatter": "tamasfe.even-better-toml"
+  },
+  //* TSV
+  "[tsv]": {
+    //? Indent with tabs
+    "editor.insertSpaces": false
+  },
+  //* YAML
+  "yaml.format.printWidth": 88,
+  "[yaml]": {
+    "editor.defaultFormatter": "esbenp.prettier-vscode",
+    "editor.wordWrap": "wordWrapColumn"
+  },
+
+  //! Extension: Jupyter Notebooks
+  "jupyter.notebookFileRoot": "${workspaceFolder}"
+}
```

### Comparing `boilercv-0.0.0/.vscode/tasks.json` & `boilercv-0.0.1/.vscode/tasks.json`

 * *Files 24% similar despite different names*

```diff
@@ -1,390 +1,389 @@
-// Calling `pwsh` first leverages my personal $PROFILE to activate `.venv`.
-// Alternatively, we could use `.venv/Scripts/python.exe` and change the `args`, but
-// this is platform-specific anyways.
-
-{
-  "version": "2.0.0",
-  "inputs": [
-    {
-      "id": "stage",
-      "type": "pickString",
-      "description": "stage",
-      "default": "",
-      "options": [
-        "",
-        "schema",
-        "check_cv",
-        "update_binarized_preview",
-        "contours",
-        "fill",
-        "update_filled_preview"
-      ]
-    },
-    {
-      "id": "preview",
-      "type": "pickString",
-      "description": "preview",
-      "default": "",
-      "options": ["binarized", "filled", "overlaid"]
-    }
-  ],
-  "tasks": [
-    // * -------------------------------------------------------------------------- * //
-    // * Changes below should persist in significant template updates.
-    {
-      "label": "proj: Run file PREVIEW/WRITE",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "python ${file}"],
-      "icon": { "id": "repo" },
-      "problemMatcher": [],
-      "options": {
-        "env": {
-          "BOILERCV_PREVIEW": "True",
-          "BOILERCV_WRITE": "True"
-        }
-      }
-    },
-    {
-      "label": "proj: Run file DEBUG/PREVIEW/WRITE",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "python ${file}"],
-      "icon": { "id": "repo" },
-      "problemMatcher": [],
-      "options": {
-        "env": {
-          "BOILERCV_DEBUG": "True",
-          "BOILERCV_PREVIEW": "True",
-          "BOILERCV_WRITE": "True"
-        }
-      }
-    },
-    {
-      "label": "proj: Run file PREVIEW",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "python ${file}"],
-      "icon": { "id": "repo" },
-      "problemMatcher": [],
-      "options": {
-        "env": { "BOILERCV_PREVIEW": "True" }
-      }
-    },
-    {
-      "label": "proj: Run file WRITE",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "python ${file}"],
-      "icon": { "id": "repo" },
-      "problemMatcher": [],
-      "options": {
-        "env": { "BOILERCV_WRITE": "True" }
-      }
-    },
-    {
-      "label": "proj: preview",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "python -m boilercv.previews.${input:preview}"],
-      "icon": { "id": "graph" },
-      "options": {
-        "env": { "BOILERCV_PREVIEW": "True" }
-      },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: repro force downstream (debug)",
-      "dependsOrder": "sequence",
-      "dependsOn": ["dvc: synchronize paths"],
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "dvc repro --force --downstream ${input:stage}"],
-      "icon": { "id": "graph" },
-      "options": {
-        "env": { "BOILERCV_DEBUG": "True" }
-      },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: repro (debug)",
-      "dependsOrder": "sequence",
-      "dependsOn": ["dvc: synchronize paths"],
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "dvc repro ${input:stage}"],
-      "icon": { "id": "graph" },
-      "options": {
-        "env": { "BOILERCV_DEBUG": "True" }
-      },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: repro force downstream",
-      "dependsOrder": "sequence",
-      "dependsOn": ["dvc: synchronize paths"],
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "dvc repro --force --downstream ${input:stage}"],
-      "icon": { "id": "graph" },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: repro",
-      "dependsOrder": "sequence",
-      "dependsOn": ["dvc: synchronize paths"],
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "dvc repro ${input:stage}"],
-      "icon": { "id": "graph" },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: repro force all",
-      "dependsOrder": "sequence",
-      "dependsOn": [
-        "setup: Update project",
-        "dvc: synchronize paths",
-        "dvc: freeze",
-        "git: Stage all files",
-        "pre-commit",
-        "git: Stage all files"
-      ],
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "dvc repro --force"],
-      "icon": { "id": "graph" },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: repro all",
-      "dependsOrder": "sequence",
-      "dependsOn": [
-        "setup: Update project",
-        "dvc: synchronize paths",
-        "dvc: freeze",
-        "git: Stage all files",
-        "pre-commit",
-        "git: Stage all files"
-      ],
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "dvc repro"],
-      "icon": { "id": "graph" },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: dag",
-      "dependsOrder": "sequence",
-      "dependsOn": ["dvc: synchronize paths"],
-      "type": "process",
-      "command": "pwsh",
-      "args": [
-        "-Command",
-        "(dvc dag --md) -Replace 'mermaid', '{mermaid}' > docs/dag.md && . '~/.local/nodeenvs/markdownlint/Scripts/Activate.ps1' && markdownlint --fix docs/dag.md"
-      ],
-      "icon": { "id": "graph" },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: synchronize paths",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "python -m boilercv.models.paths"],
-      "icon": { "id": "graph" },
-      "problemMatcher": []
-    },
-    {
-      "label": "dvc: freeze",
-      "type": "process",
-      "command": "pwsh",
-      "args": [
-        "-Command",
-        "pip freeze --requirement requirements.txt --local --exclude-editable > repro.txt"
-      ],
-      "icon": { "id": "graph" },
-      "problemMatcher": []
-    },
-    // * -------------------------------------------------------------------------- * //
-    // * WSL-SPECIFIC * //
-    {
-      "label": "wsl: Copy PID of Python Debugger",
-      "type": "shell",
-      "command": "ps aux | grep python | grep --max-count 1 -- --adapter-access-token | grep --only-matching --perl-regexp 'user\\s+\\d+' | grep --only-matching --perl-regexp '\\d+' | clip.exe",
-      "group": {
-        "kind": "test",
-        "isDefault": true
-      },
-      "presentation": {
-        "close": false,
-        "focus": true,
-        "reveal": "always"
-      },
-      "icon": { "id": "terminal-linux" },
-      "problemMatcher": []
-    },
-
-    // * -------------------------------------------------------------------------- * //
-    // * Changes below may be lost in significant template updates.
-
-    // * -------------------------------------------------------------------------- * //
-    // * PROJECT SETUP * //
-    {
-      "label": "setup: Compose pyproject.toml",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "python .tools/scripts/compose_pyproject.py"],
-      "icon": { "id": "file-symlink-directory" },
-      "problemMatcher": []
-    },
-    {
-      "label": "setup: Re-answer template questions",
-      "type": "process",
-      "command": "pwsh",
-      "args": [".tools/scripts/Update-Template.ps1"],
-      "icon": { "id": "file-symlink-directory" },
-      "problemMatcher": []
-    },
-    {
-      "label": "setup: Bump template",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", ".tools/scripts/Update-Template.ps1 -Remote -Force"],
-      "icon": { "id": "file-symlink-directory" },
-      "problemMatcher": []
-    },
-    {
-      "label": "setup: Setup project",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["setup.ps1"],
-      "icon": { "id": "file-symlink-directory" },
-      "problemMatcher": []
-    },
-    {
-      "label": "setup: Update project",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["update.ps1"],
-      "icon": { "id": "file-symlink-directory" },
-      // "runOptions": {
-      //   "runOn": "folderOpen"
-      // },
-      "problemMatcher": []
-    },
-    {
-      "label": "task: Remove *.rej",
-      "type": "process",
-      "command": "pwsh",
-      "args": [
-        "-Command",
-        "Get-ChildItem -Recurse -Filter *.rej | Remove-Item"
-      ],
-      "icon": { "id": "file-symlink-directory" },
-      "problemMatcher": []
-    },
-
-    // * -------------------------------------------------------------------------- * //
-    // * PRE-COMMIT * //
-    {
-      "label": "pre-commit",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "pre-commit"],
-      "icon": { "id": "git-commit" },
-      "problemMatcher": []
-    },
-    {
-      "label": "pre-commit: all",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "pre-commit run --all-files"],
-      "icon": { "id": "git-commit" },
-      "problemMatcher": []
-    },
-
-    // * -------------------------------------------------------------------------- * //
-    // * GIT * //
-    {
-      "label": "git: Rebase back to fork",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "git rebase -i --fork-point main"],
-      "icon": { "id": "git-branch" },
-      "problemMatcher": []
-    },
-    {
-      "label": "git: Stage all files",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "git add -A"],
-      "icon": { "id": "git-branch" },
-      "problemMatcher": []
-    },
-
-    // * -------------------------------------------------------------------------- * //
-    // * BLACK * //
-    {
-      "label": "task: black: Ignore magic comma in this file",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "black -C ${file}"],
-      "icon": { "id": "code" },
-      "problemMatcher": []
-    },
-    {
-      "label": "task: black: Ignore magic comma in all project files",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "black -C src tests"],
-      "icon": { "id": "code" },
-      "problemMatcher": []
-    },
-
-    // * -------------------------------------------------------------------------- * //
-    // * OTHER TASKS * //
-    {
-      "label": "task: sphinx-autobuild docs (preview)",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "sphinx-autobuild docs _site"],
-      "icon": { "id": "book" },
-      "problemMatcher": []
-    },
-    {
-      "label": "task: profile this file",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "python -m cProfile -o .prof ${file}"],
-      "icon": { "id": "graph-line" },
-      "problemMatcher": []
-    },
-    {
-      "label": "task: view profile results with snakeviz",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "snakeviz .prof"],
-      "icon": { "id": "graph-line" },
-      "problemMatcher": []
-    },
-    {
-      "label": "task: autoflake current file",
-      "type": "process",
-      "command": "pwsh",
-      "args": [
-        "-Command",
-        "autoflake -i --remove-all-unused-imports --ignore-init-module-imports ${file}"
-      ],
-      "icon": { "id": "code" },
-      "problemMatcher": []
-    },
-    {
-      "label": "task: pytest-cov: Generate coverage",
-      "type": "process",
-      "command": "pwsh",
-      "args": ["-Command", "pytest --cov --cov-report xml"],
-      "icon": { "id": "beaker" },
-      "problemMatcher": []
-    }
-  ]
-}
+// Calling `pwsh` first leverages my personal $PROFILE to activate `.venv`.
+// Alternatively, we could use `.venv/Scripts/python.exe` and change the `args`, but
+// this is platform-specific anyways.
+
+{
+  "version": "2.0.0",
+  "inputs": [
+    {
+      "id": "stage",
+      "type": "pickString",
+      "description": "stage",
+      "default": "",
+      "options": [
+        "",
+        "schema",
+        "update_binarized_preview",
+        "contours",
+        "fill",
+        "update_filled_preview"
+      ]
+    },
+    {
+      "id": "preview",
+      "type": "pickString",
+      "description": "preview",
+      "default": "",
+      "options": ["gray", "binarized", "filled", "composite"]
+    }
+  ],
+  "tasks": [
+    // * -------------------------------------------------------------------------- * //
+    // * Changes below should persist in significant template updates.
+    {
+      "label": "proj: Run file PREVIEW/WRITE",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "python ${file}"],
+      "icon": { "id": "repo" },
+      "problemMatcher": [],
+      "options": {
+        "env": {
+          "BOILERCV_PREVIEW": "True",
+          "BOILERCV_WRITE": "True"
+        }
+      }
+    },
+    {
+      "label": "proj: Run file DEBUG/PREVIEW/WRITE",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "python ${file}"],
+      "icon": { "id": "repo" },
+      "problemMatcher": [],
+      "options": {
+        "env": {
+          "BOILERCV_DEBUG": "True",
+          "BOILERCV_PREVIEW": "True",
+          "BOILERCV_WRITE": "True"
+        }
+      }
+    },
+    {
+      "label": "proj: Run file PREVIEW",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "python ${file}"],
+      "icon": { "id": "repo" },
+      "problemMatcher": [],
+      "options": {
+        "env": { "BOILERCV_PREVIEW": "True" }
+      }
+    },
+    {
+      "label": "proj: Run file WRITE",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "python ${file}"],
+      "icon": { "id": "repo" },
+      "problemMatcher": [],
+      "options": {
+        "env": { "BOILERCV_WRITE": "True" }
+      }
+    },
+    {
+      "label": "proj: preview",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "python -m boilercv.previews.${input:preview}"],
+      "icon": { "id": "graph" },
+      "options": {
+        "env": { "BOILERCV_PREVIEW": "True" }
+      },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: repro force downstream (debug)",
+      "dependsOrder": "sequence",
+      "dependsOn": ["dvc: synchronize paths"],
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "dvc repro --force --downstream ${input:stage}"],
+      "icon": { "id": "graph" },
+      "options": {
+        "env": { "BOILERCV_DEBUG": "True" }
+      },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: repro (debug)",
+      "dependsOrder": "sequence",
+      "dependsOn": ["dvc: synchronize paths"],
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "dvc repro ${input:stage}"],
+      "icon": { "id": "graph" },
+      "options": {
+        "env": { "BOILERCV_DEBUG": "True" }
+      },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: repro force downstream",
+      "dependsOrder": "sequence",
+      "dependsOn": ["dvc: synchronize paths"],
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "dvc repro --force --downstream ${input:stage}"],
+      "icon": { "id": "graph" },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: repro",
+      "dependsOrder": "sequence",
+      "dependsOn": ["dvc: synchronize paths"],
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "dvc repro ${input:stage}"],
+      "icon": { "id": "graph" },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: repro force all",
+      "dependsOrder": "sequence",
+      "dependsOn": [
+        "setup: Update project",
+        "dvc: synchronize paths",
+        "dvc: freeze",
+        "git: Stage all files",
+        "pre-commit",
+        "git: Stage all files"
+      ],
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "dvc repro --force"],
+      "icon": { "id": "graph" },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: repro all",
+      "dependsOrder": "sequence",
+      "dependsOn": [
+        "setup: Update project",
+        "dvc: synchronize paths",
+        "dvc: freeze",
+        "git: Stage all files",
+        "pre-commit",
+        "git: Stage all files"
+      ],
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "dvc repro"],
+      "icon": { "id": "graph" },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: dag",
+      "dependsOrder": "sequence",
+      "dependsOn": ["dvc: synchronize paths"],
+      "type": "process",
+      "command": "pwsh",
+      "args": [
+        "-Command",
+        "(dvc dag --md) -Replace 'mermaid', '{mermaid}' > docs/dag.md && . '~/.local/nodeenvs/markdownlint/Scripts/Activate.ps1' && markdownlint --fix docs/dag.md"
+      ],
+      "icon": { "id": "graph" },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: synchronize paths",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "python -m boilercv.models.paths"],
+      "icon": { "id": "graph" },
+      "problemMatcher": []
+    },
+    {
+      "label": "dvc: freeze",
+      "type": "process",
+      "command": "pwsh",
+      "args": [
+        "-Command",
+        "pip freeze --requirement requirements.txt --local --exclude-editable > repro.txt"
+      ],
+      "icon": { "id": "graph" },
+      "problemMatcher": []
+    },
+    // * -------------------------------------------------------------------------- * //
+    // * WSL-SPECIFIC * //
+    {
+      "label": "wsl: Copy PID of Python Debugger",
+      "type": "shell",
+      "command": "ps aux | grep python | grep --max-count 1 -- --adapter-access-token | grep --only-matching --perl-regexp 'user\\s+\\d+' | grep --only-matching --perl-regexp '\\d+' | clip.exe",
+      "group": {
+        "kind": "test",
+        "isDefault": true
+      },
+      "presentation": {
+        "close": false,
+        "focus": true,
+        "reveal": "always"
+      },
+      "icon": { "id": "terminal-linux" },
+      "problemMatcher": []
+    },
+
+    // * -------------------------------------------------------------------------- * //
+    // * Changes below may be lost in significant template updates.
+
+    // * -------------------------------------------------------------------------- * //
+    // * PROJECT SETUP * //
+    {
+      "label": "setup: Compose pyproject.toml",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "python .tools/scripts/compose_pyproject.py"],
+      "icon": { "id": "file-symlink-directory" },
+      "problemMatcher": []
+    },
+    {
+      "label": "setup: Re-answer template questions",
+      "type": "process",
+      "command": "pwsh",
+      "args": [".tools/scripts/Update-Template.ps1"],
+      "icon": { "id": "file-symlink-directory" },
+      "problemMatcher": []
+    },
+    {
+      "label": "setup: Bump template",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", ".tools/scripts/Update-Template.ps1 -Remote -Force"],
+      "icon": { "id": "file-symlink-directory" },
+      "problemMatcher": []
+    },
+    {
+      "label": "setup: Setup project",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["setup.ps1"],
+      "icon": { "id": "file-symlink-directory" },
+      "problemMatcher": []
+    },
+    {
+      "label": "setup: Update project",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["update.ps1"],
+      "icon": { "id": "file-symlink-directory" },
+      // "runOptions": {
+      //   "runOn": "folderOpen"
+      // },
+      "problemMatcher": []
+    },
+    {
+      "label": "task: Remove *.rej",
+      "type": "process",
+      "command": "pwsh",
+      "args": [
+        "-Command",
+        "Get-ChildItem -Recurse -Filter *.rej | Remove-Item"
+      ],
+      "icon": { "id": "file-symlink-directory" },
+      "problemMatcher": []
+    },
+
+    // * -------------------------------------------------------------------------- * //
+    // * PRE-COMMIT * //
+    {
+      "label": "pre-commit",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "pre-commit"],
+      "icon": { "id": "git-commit" },
+      "problemMatcher": []
+    },
+    {
+      "label": "pre-commit: all",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "pre-commit run --all-files"],
+      "icon": { "id": "git-commit" },
+      "problemMatcher": []
+    },
+
+    // * -------------------------------------------------------------------------- * //
+    // * GIT * //
+    {
+      "label": "git: Rebase back to fork",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "git rebase -i --fork-point main"],
+      "icon": { "id": "git-branch" },
+      "problemMatcher": []
+    },
+    {
+      "label": "git: Stage all files",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "git add -A"],
+      "icon": { "id": "git-branch" },
+      "problemMatcher": []
+    },
+
+    // * -------------------------------------------------------------------------- * //
+    // * BLACK * //
+    {
+      "label": "task: black: Ignore magic comma in this file",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "black -C ${file}"],
+      "icon": { "id": "code" },
+      "problemMatcher": []
+    },
+    {
+      "label": "task: black: Ignore magic comma in all project files",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "black -C src tests"],
+      "icon": { "id": "code" },
+      "problemMatcher": []
+    },
+
+    // * -------------------------------------------------------------------------- * //
+    // * OTHER TASKS * //
+    {
+      "label": "task: sphinx-autobuild docs (preview)",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "sphinx-autobuild docs _site"],
+      "icon": { "id": "book" },
+      "problemMatcher": []
+    },
+    {
+      "label": "task: profile this file",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "python -m cProfile -o .prof ${file}"],
+      "icon": { "id": "graph-line" },
+      "problemMatcher": []
+    },
+    {
+      "label": "task: view profile results with snakeviz",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "snakeviz .prof"],
+      "icon": { "id": "graph-line" },
+      "problemMatcher": []
+    },
+    {
+      "label": "task: autoflake current file",
+      "type": "process",
+      "command": "pwsh",
+      "args": [
+        "-Command",
+        "autoflake -i --remove-all-unused-imports --ignore-init-module-imports ${file}"
+      ],
+      "icon": { "id": "code" },
+      "problemMatcher": []
+    },
+    {
+      "label": "task: pytest-cov: Generate coverage",
+      "type": "process",
+      "command": "pwsh",
+      "args": ["-Command", "pytest --cov --cov-report xml"],
+      "icon": { "id": "beaker" },
+      "problemMatcher": []
+    }
+  ]
+}
```

### Comparing `boilercv-0.0.0/CODE_OF_CONDUCT.md` & `boilercv-0.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `boilercv-0.0.0/LICENSE` & `boilercv-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boilercv-0.0.0/build.txt` & `boilercv-0.0.1/build.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-
-General configuration for OpenCV 4.6.0 =====================================
-  Version control:               4.6.0
-
-  Extra modules:
-    Location (extra):            /home/user/opencv-python/opencv_contrib/modules
-    Version control (extra):     4.6.0
-
-  Platform:
-    Timestamp:                   2022-06-14T19:39:17Z
-    Host:                        Linux 5.10.102.1-microsoft-standard-WSL2 x86_64
-    CMake:                       3.22.5
-    CMake generator:             Unix Makefiles
-    CMake build tool:            /usr/bin/gmake
-    Configuration:               Debug
-
-  CPU/HW features:
-    Baseline:                    SSE SSE2 SSE3
-      requested:                 SSE3
-    Dispatched code generation:  SSE4_1 SSE4_2 FP16 AVX AVX2 AVX512_SKX
-      requested:                 SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
-      SSE4_1 (16 files):         + SSSE3 SSE4_1
-      SSE4_2 (1 files):          + SSSE3 SSE4_1 POPCNT SSE4_2
-      FP16 (0 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 AVX
-      AVX (4 files):             + SSSE3 SSE4_1 POPCNT SSE4_2 AVX
-      AVX2 (31 files):           + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2
-      AVX512_SKX (5 files):      + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2 AVX_512F AVX512_COMMON AVX512_SKX
-
-  C/C++:
-    Built as dynamic libs?:      NO
-    C++ standard:                11
-    C++ Compiler:                /usr/bin/c++  (ver 11.2.0)
-    C++ flags (Release):         -fsigned-char -W -Wall -Wreturn-type -Wnon-virtual-dtor -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -O3 -DNDEBUG  -DNDEBUG
-    C++ flags (Debug):           -fsigned-char -W -Wall -Wreturn-type -Wnon-virtual-dtor -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
-    C Compiler:                  /usr/bin/cc
-    C flags (Release):           -fsigned-char -W -Wall -Wreturn-type -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -O3 -DNDEBUG  -DNDEBUG
-    C flags (Debug):             -fsigned-char -W -Wall -Wreturn-type -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -g  -O0 -DDEBUG -D_DEBUG
-    Linker flags (Release):      -Wl,--exclude-libs,libippicv.a -Wl,--exclude-libs,libippiw.a   -Wl,--gc-sections -Wl,--as-needed -Wl,--no-undefined
-    Linker flags (Debug):        -Wl,--exclude-libs,libippicv.a -Wl,--exclude-libs,libippiw.a   -Wl,--gc-sections -Wl,--as-needed -Wl,--no-undefined
-    ccache:                      NO
-    Precompiled headers:         NO
-    Extra dependencies:          /usr/lib/x86_64-linux-gnu/libjpeg.so /usr/lib/x86_64-linux-gnu/libwebp.so /usr/lib/x86_64-linux-gnu/libpng.so /usr/lib/x86_64-linux-gnu/libtiff.so /usr/lib/x86_64-linux-gnu/libz.so Iconv::Iconv dl m pthread rt
-    3rdparty dependencies:       libprotobuf ade ittnotify libopenjp2 IlmImf quirc ippiw ippicv
-
-  OpenCV modules:
-    To be built:                 aruco barcode bgsegm bioinspired calib3d ccalib core datasets dnn dnn_objdetect dnn_superres dpm face features2d flann fuzzy gapi hfs highgui img_hash imgcodecs imgproc intensity_transform line_descriptor mcc ml objdetect optflow phase_unwrapping photo plot python3 quality rapid reg rgbd saliency shape stereo stitching structured_light superres surface_matching text tracking video videoio videostab wechat_qrcode xfeatures2d ximgproc xobjdetect xphoto
-    Disabled:                    freetype world
-    Disabled by dependency:      -
-    Unavailable:                 alphamat cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping cudev cvv hdf java julia matlab ovis python2 sfm ts viz
-    Applications:                -
-    Documentation:               NO
-    Non-free algorithms:         NO
-
-  GUI:                           GTK3
-    GTK+:                        YES (ver 3.24.33)
-      GThread :                  YES (ver 2.72.1)
-      GtkGlExt:                  NO
-    VTK support:                 NO
-
-  Media I/O:
-    ZLib:                        /usr/lib/x86_64-linux-gnu/libz.so (ver 1.2.11)
-    JPEG:                        /usr/lib/x86_64-linux-gnu/libjpeg.so (ver 80)
-    WEBP:                        /usr/lib/x86_64-linux-gnu/libwebp.so (ver encoder: 0x020f)
-    PNG:                         /usr/lib/x86_64-linux-gnu/libpng.so (ver 1.6.37)
-    TIFF:                        /usr/lib/x86_64-linux-gnu/libtiff.so (ver 42 / 4.3.0)
-    JPEG 2000:                   build (ver 2.4.0)
-    OpenEXR:                     build (ver 2.3.0)
-    HDR:                         YES
-    SUNRASTER:                   YES
-    PXM:                         YES
-    PFM:                         YES
-
-  Video I/O:
-    DC1394:                      NO
-    FFMPEG:                      YES
-      avcodec:                   YES (58.134.100)
-      avformat:                  YES (58.76.100)
-      avutil:                    YES (56.70.100)
-      swscale:                   YES (5.9.100)
-      avresample:                NO
-    GStreamer:                   YES (1.20.1)
-    v4l/v4l2:                    YES (linux/videodev2.h)
-
-  Parallel framework:            pthreads
-
-  Trace:                         YES (with Intel ITT)
-
-  Other third-party libraries:
-    Intel IPP:                   2020.0.0 Gold [2020.0.0]
-           at:                   /home/user/opencv-python/_skbuild/linux-x86_64-3.10/cmake-build/3rdparty/ippicv/ippicv_lnx/icv
-    Intel IPP IW:                sources (2020.0.0)
-              at:                /home/user/opencv-python/_skbuild/linux-x86_64-3.10/cmake-build/3rdparty/ippicv/ippicv_lnx/iw
-    VA:                          NO
-    Lapack:                      NO
-    Eigen:                       NO
-    Custom HAL:                  NO
-    Protobuf:                    build (3.19.1)
-
-  OpenCL:                        YES (no extra features)
-    Include path:                /home/user/opencv-python/opencv/3rdparty/include/opencl/1.2
-    Link libraries:              Dynamic load
-
-  Python 3:
-    Interpreter:                 /usr/bin/python3 (ver 3.10.4)
-    Libraries:                   /usr/lib/x86_64-linux-gnu/libpython3.10.so (ver 3.10.4)
-    numpy:                       /home/user/.local/lib/python3.10/site-packages/numpy/core/include (ver 1.22.4)
-    install path:                python/cv2/python-3
-
-  Python (for build):            /usr/bin/python3
-
-  Java:
-    ant:                         NO
-    JNI:                         NO
-    Java wrappers:               NO
-    Java tests:                  NO
-
-  Install to:                    /home/user/opencv-python/_skbuild/linux-x86_64-3.10/cmake-install
------------------------------------------------------------------
+
+General configuration for OpenCV 4.6.0 =====================================
+  Version control:               4.6.0
+
+  Extra modules:
+    Location (extra):            /home/user/opencv-python/opencv_contrib/modules
+    Version control (extra):     4.6.0
+
+  Platform:
+    Timestamp:                   2022-06-14T19:39:17Z
+    Host:                        Linux 5.10.102.1-microsoft-standard-WSL2 x86_64
+    CMake:                       3.22.5
+    CMake generator:             Unix Makefiles
+    CMake build tool:            /usr/bin/gmake
+    Configuration:               Debug
+
+  CPU/HW features:
+    Baseline:                    SSE SSE2 SSE3
+      requested:                 SSE3
+    Dispatched code generation:  SSE4_1 SSE4_2 FP16 AVX AVX2 AVX512_SKX
+      requested:                 SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
+      SSE4_1 (16 files):         + SSSE3 SSE4_1
+      SSE4_2 (1 files):          + SSSE3 SSE4_1 POPCNT SSE4_2
+      FP16 (0 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 AVX
+      AVX (4 files):             + SSSE3 SSE4_1 POPCNT SSE4_2 AVX
+      AVX2 (31 files):           + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2
+      AVX512_SKX (5 files):      + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2 AVX_512F AVX512_COMMON AVX512_SKX
+
+  C/C++:
+    Built as dynamic libs?:      NO
+    C++ standard:                11
+    C++ Compiler:                /usr/bin/c++  (ver 11.2.0)
+    C++ flags (Release):         -fsigned-char -W -Wall -Wreturn-type -Wnon-virtual-dtor -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -O3 -DNDEBUG  -DNDEBUG
+    C++ flags (Debug):           -fsigned-char -W -Wall -Wreturn-type -Wnon-virtual-dtor -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
+    C Compiler:                  /usr/bin/cc
+    C flags (Release):           -fsigned-char -W -Wall -Wreturn-type -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -O3 -DNDEBUG  -DNDEBUG
+    C flags (Debug):             -fsigned-char -W -Wall -Wreturn-type -Waddress -Wsequence-point -Wformat -Wformat-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -g  -O0 -DDEBUG -D_DEBUG
+    Linker flags (Release):      -Wl,--exclude-libs,libippicv.a -Wl,--exclude-libs,libippiw.a   -Wl,--gc-sections -Wl,--as-needed -Wl,--no-undefined
+    Linker flags (Debug):        -Wl,--exclude-libs,libippicv.a -Wl,--exclude-libs,libippiw.a   -Wl,--gc-sections -Wl,--as-needed -Wl,--no-undefined
+    ccache:                      NO
+    Precompiled headers:         NO
+    Extra dependencies:          /usr/lib/x86_64-linux-gnu/libjpeg.so /usr/lib/x86_64-linux-gnu/libwebp.so /usr/lib/x86_64-linux-gnu/libpng.so /usr/lib/x86_64-linux-gnu/libtiff.so /usr/lib/x86_64-linux-gnu/libz.so Iconv::Iconv dl m pthread rt
+    3rdparty dependencies:       libprotobuf ade ittnotify libopenjp2 IlmImf quirc ippiw ippicv
+
+  OpenCV modules:
+    To be built:                 aruco barcode bgsegm bioinspired calib3d ccalib core datasets dnn dnn_objdetect dnn_superres dpm face features2d flann fuzzy gapi hfs highgui img_hash imgcodecs imgproc intensity_transform line_descriptor mcc ml objdetect optflow phase_unwrapping photo plot python3 quality rapid reg rgbd saliency shape stereo stitching structured_light superres surface_matching text tracking video videoio videostab wechat_qrcode xfeatures2d ximgproc xobjdetect xphoto
+    Disabled:                    freetype world
+    Disabled by dependency:      -
+    Unavailable:                 alphamat cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping cudev cvv hdf java julia matlab ovis python2 sfm ts viz
+    Applications:                -
+    Documentation:               NO
+    Non-free algorithms:         NO
+
+  GUI:                           GTK3
+    GTK+:                        YES (ver 3.24.33)
+      GThread :                  YES (ver 2.72.1)
+      GtkGlExt:                  NO
+    VTK support:                 NO
+
+  Media I/O:
+    ZLib:                        /usr/lib/x86_64-linux-gnu/libz.so (ver 1.2.11)
+    JPEG:                        /usr/lib/x86_64-linux-gnu/libjpeg.so (ver 80)
+    WEBP:                        /usr/lib/x86_64-linux-gnu/libwebp.so (ver encoder: 0x020f)
+    PNG:                         /usr/lib/x86_64-linux-gnu/libpng.so (ver 1.6.37)
+    TIFF:                        /usr/lib/x86_64-linux-gnu/libtiff.so (ver 42 / 4.3.0)
+    JPEG 2000:                   build (ver 2.4.0)
+    OpenEXR:                     build (ver 2.3.0)
+    HDR:                         YES
+    SUNRASTER:                   YES
+    PXM:                         YES
+    PFM:                         YES
+
+  Video I/O:
+    DC1394:                      NO
+    FFMPEG:                      YES
+      avcodec:                   YES (58.134.100)
+      avformat:                  YES (58.76.100)
+      avutil:                    YES (56.70.100)
+      swscale:                   YES (5.9.100)
+      avresample:                NO
+    GStreamer:                   YES (1.20.1)
+    v4l/v4l2:                    YES (linux/videodev2.h)
+
+  Parallel framework:            pthreads
+
+  Trace:                         YES (with Intel ITT)
+
+  Other third-party libraries:
+    Intel IPP:                   2020.0.0 Gold [2020.0.0]
+           at:                   /home/user/opencv-python/_skbuild/linux-x86_64-3.10/cmake-build/3rdparty/ippicv/ippicv_lnx/icv
+    Intel IPP IW:                sources (2020.0.0)
+              at:                /home/user/opencv-python/_skbuild/linux-x86_64-3.10/cmake-build/3rdparty/ippicv/ippicv_lnx/iw
+    VA:                          NO
+    Lapack:                      NO
+    Eigen:                       NO
+    Custom HAL:                  NO
+    Protobuf:                    build (3.19.1)
+
+  OpenCL:                        YES (no extra features)
+    Include path:                /home/user/opencv-python/opencv/3rdparty/include/opencl/1.2
+    Link libraries:              Dynamic load
+
+  Python 3:
+    Interpreter:                 /usr/bin/python3 (ver 3.10.4)
+    Libraries:                   /usr/lib/x86_64-linux-gnu/libpython3.10.so (ver 3.10.4)
+    numpy:                       /home/user/.local/lib/python3.10/site-packages/numpy/core/include (ver 1.22.4)
+    install path:                python/cv2/python-3
+
+  Python (for build):            /usr/bin/python3
+
+  Java:
+    ant:                         NO
+    JNI:                         NO
+    Java wrappers:               NO
+    Java tests:                  NO
+
+  Install to:                    /home/user/opencv-python/_skbuild/linux-x86_64-3.10/cmake-install
+-----------------------------------------------------------------
```

### Comparing `boilercv-0.0.0/docs/_static/multicolor.png` & `boilercv-0.0.1/docs/_static/multicolor.png`

 * *Files identical despite different names*

### Comparing `boilercv-0.0.0/dvc.lock` & `boilercv-0.0.1/dvc.lock`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-schema: '2.0'
-stages:
-  schema:
-    cmd: python -m boilercv.stages.schema
-    deps:
-    - path: src/boilercv/models/paths.py
-      md5: 011cf73b6178fdaa01d4a96150d0b4ba
-      size: 5163
-    - path: src/boilercv/stages/schema.py
-      md5: 6eaac97ab24e94f410ccff1517f42d0e
-      size: 641
-    outs:
-    - path: data/schema
-      md5: b2ffbd511ccedec91631fcf3f530d9e4.dir
-      size: 5437
-      nfiles: 1
-  update_binarized_preview:
-    cmd: python -m boilercv.stages.update_binarized_preview
-    deps:
-    - path: data/rois
-      md5: 1300e5dce1774bdc91feb6365369c7d8.dir
-      size: 186726548
-      nfiles: 308
-    - path: data/sources
-      md5: a409ab9bcababc1baaea4dc53e312bda.dir
-      size: 7424602696
-      nfiles: 308
-    - path: src/boilercv/stages/update_binarized_preview.py
-      md5: 186799fb6a90ec27a63cb274e05eca54
-      size: 1153
-    outs:
-    - path: data/previews/binarized.nc
-      md5: 5598ee8b69f8591e2035194a9054f2c3
-      size: 147879321
-  preview_binarized:
-    cmd: python -m boilercv.stages.preview_binarized
-    deps:
-    - path: data/previews/binarized.nc
-      md5: 312b51939f1ac4ae21bffd45ad91f854
-      size: 38903364
-    - path: src/boilercv/stages/preview_binarized.py
-      md5: aa0adbd6d0409460b55b55ce0a1a5b96
-      size: 349
-  contours:
-    cmd: python -m boilercv.stages.contours
-    deps:
-    - path: data/sources
-      md5: a409ab9bcababc1baaea4dc53e312bda.dir
-      size: 7424602696
-      nfiles: 308
-    - path: src/boilercv/stages/contours.py
-      md5: 48714d9e75d983498dca309896c2c011
-      size: 1889
-    outs:
-    - path: data/contours
-      md5: d43be95333c9df0e76d570f8b11aada2.dir
-      size: 4279876062
-      nfiles: 308
-  fill:
-    cmd: python -m boilercv.stages.fill
-    deps:
-    - path: data/contours
-      md5: d43be95333c9df0e76d570f8b11aada2.dir
-      size: 4279876062
-      nfiles: 308
-    - path: data/sources
-      md5: a409ab9bcababc1baaea4dc53e312bda.dir
-      size: 7424602696
-      nfiles: 308
-    - path: src/boilercv/stages/fill.py
-      md5: d6e9e5582c2f4f24d8e80b7a5c917e27
-      size: 1583
-    outs:
-    - path: data/filled
-      md5: 9d9b406833ae3911940fd4d717bb20e1.dir
-      size: 3482532424
-      nfiles: 308
-  update_filled_preview:
-    cmd: python -m boilercv.stages.update_filled_preview
-    deps:
-    - path: data/filled
-      md5: 9d9b406833ae3911940fd4d717bb20e1.dir
-      size: 3482532424
-      nfiles: 308
-    - path: src/boilercv/stages/update_filled_preview.py
-      md5: 2b467aa2304c045ab9acd4a3c429dd39
-      size: 1273
-    outs:
-    - path: data/previews/filled.nc
-      md5: 913c0dca978f8f3ff088adb765bf8029
-      size: 147879321
-  check_cv:
-    cmd: python -m boilercv.stages.check_cv
-    deps:
-    - path: data/samples
-      md5: 2039f3ac1b4df1e9059cfb4d74b8c1db.dir
-      size: 22147287
-      nfiles: 113
-    - path: src/boilercv/stages/check_cv.py
-      md5: fb029ebceb5076c48f032c9b2ae3da1e
-      size: 97
-  binarized_preview:
-    cmd: python -m boilercv.stages.update_previews.binarized
-    deps:
-    - path: data/rois
-      md5: 1300e5dce1774bdc91feb6365369c7d8.dir
-      size: 186726548
-      nfiles: 308
-    - path: data/sources
-      md5: a409ab9bcababc1baaea4dc53e312bda.dir
-      size: 7424602696
-      nfiles: 308
-    - path: src/boilercv/stages/update_previews/binarized.py
-      md5: 0c528f648e4975729f1642c77e3ae15e
-      size: 835
-    outs:
-    - path: data/previews/binarized.nc
-      md5: a254f85beabe041bf6c4b0820024465d
-      size: 3446443
-  gray_preview:
-    cmd: python -m boilercv.stages.update_previews.gray
-    deps:
-    - path: data/sources
-      md5: a409ab9bcababc1baaea4dc53e312bda.dir
-      size: 7424602696
-      nfiles: 308
-    - path: src/boilercv/stages/update_previews/gray.py
-      md5: 089e35a18791e628d5bcd75e7fdca100
-      size: 768
-    outs:
-    - path: data/previews/gray.nc
-      md5: bca01dd9d72e5a7c25db766c5522652e
-      size: 18686615
-  filled_preview:
-    cmd: python -m boilercv.stages.update_previews.filled
-    deps:
-    - path: data/filled
-      md5: 9d9b406833ae3911940fd4d717bb20e1.dir
-      size: 3482532424
-      nfiles: 308
-    - path: data/sources
-      md5: a409ab9bcababc1baaea4dc53e312bda.dir
-      size: 7424602696
-      nfiles: 308
-    - path: src/boilercv/stages/update_previews/filled.py
-      md5: 879e5a5452d1e5ecc5dfaa79789f3840
-      size: 767
-    outs:
-    - path: data/previews/filled.nc
-      md5: f3596d4b5c08d8701b7630f1136c45aa
-      size: 1661392
+schema: '2.0'
+stages:
+  schema:
+    cmd: python -m boilercv.stages.schema
+    deps:
+    - path: src/boilercv/models/paths.py
+      md5: 346ad282f672dcefa9bfda19a5e7ef3d
+      size: 5137
+    - path: src/boilercv/stages/schema.py
+      md5: 6eaac97ab24e94f410ccff1517f42d0e
+      size: 641
+    outs:
+    - path: data/schema
+      md5: 234ccf8253abff5e1930719f6dc56de9.dir
+      size: 5239
+      nfiles: 1
+  update_binarized_preview:
+    cmd: python -m boilercv.stages.update_binarized_preview
+    deps:
+    - path: data/rois
+      md5: 1300e5dce1774bdc91feb6365369c7d8.dir
+      size: 186726548
+      nfiles: 308
+    - path: data/sources
+      md5: a409ab9bcababc1baaea4dc53e312bda.dir
+      size: 7424602696
+      nfiles: 308
+    - path: src/boilercv/stages/update_binarized_preview.py
+      md5: 186799fb6a90ec27a63cb274e05eca54
+      size: 1153
+    outs:
+    - path: data/previews/binarized.nc
+      md5: 5598ee8b69f8591e2035194a9054f2c3
+      size: 147879321
+  preview_binarized:
+    cmd: python -m boilercv.stages.preview_binarized
+    deps:
+    - path: data/previews/binarized.nc
+      md5: 312b51939f1ac4ae21bffd45ad91f854
+      size: 38903364
+    - path: src/boilercv/stages/preview_binarized.py
+      md5: aa0adbd6d0409460b55b55ce0a1a5b96
+      size: 349
+  contours:
+    cmd: python -m boilercv.stages.contours
+    deps:
+    - path: data/sources
+      md5: a409ab9bcababc1baaea4dc53e312bda.dir
+      size: 7424602696
+      nfiles: 308
+    - path: src/boilercv/stages/contours.py
+      md5: 26bf1bf4419d40f1c90d771a6aaea0fa
+      size: 3041
+    outs:
+    - path: data/contours
+      md5: d43be95333c9df0e76d570f8b11aada2.dir
+      size: 4279876062
+      nfiles: 308
+  fill:
+    cmd: python -m boilercv.stages.fill
+    deps:
+    - path: data/contours
+      md5: d43be95333c9df0e76d570f8b11aada2.dir
+      size: 4279876062
+      nfiles: 308
+    - path: data/sources
+      md5: a409ab9bcababc1baaea4dc53e312bda.dir
+      size: 7424602696
+      nfiles: 308
+    - path: src/boilercv/stages/fill.py
+      md5: ed95bf998ce5a00102bf753660cb3215
+      size: 1429
+    outs:
+    - path: data/filled
+      md5: 9d9b406833ae3911940fd4d717bb20e1.dir
+      size: 3482532424
+      nfiles: 308
+  update_filled_preview:
+    cmd: python -m boilercv.stages.update_filled_preview
+    deps:
+    - path: data/filled
+      md5: 9d9b406833ae3911940fd4d717bb20e1.dir
+      size: 3482532424
+      nfiles: 308
+    - path: src/boilercv/stages/update_filled_preview.py
+      md5: 2b467aa2304c045ab9acd4a3c429dd39
+      size: 1273
+    outs:
+    - path: data/previews/filled.nc
+      md5: 913c0dca978f8f3ff088adb765bf8029
+      size: 147879321
+  check_cv:
+    cmd: python -m boilercv.stages.check_cv
+    deps:
+    - path: data/samples
+      md5: 2039f3ac1b4df1e9059cfb4d74b8c1db.dir
+      size: 22147287
+      nfiles: 113
+    - path: src/boilercv/stages/check_cv.py
+      md5: fb029ebceb5076c48f032c9b2ae3da1e
+      size: 97
+  binarized_preview:
+    cmd: python -m boilercv.stages.update_previews.binarized
+    deps:
+    - path: data/rois
+      md5: 1300e5dce1774bdc91feb6365369c7d8.dir
+      size: 186726548
+      nfiles: 308
+    - path: data/sources
+      md5: a409ab9bcababc1baaea4dc53e312bda.dir
+      size: 7424602696
+      nfiles: 308
+    - path: src/boilercv/stages/update_previews/binarized.py
+      md5: 0c528f648e4975729f1642c77e3ae15e
+      size: 835
+    outs:
+    - path: data/previews/binarized.nc
+      md5: a254f85beabe041bf6c4b0820024465d
+      size: 3446443
+  gray_preview:
+    cmd: python -m boilercv.stages.update_previews.gray
+    deps:
+    - path: data/sources
+      md5: a409ab9bcababc1baaea4dc53e312bda.dir
+      size: 7424602696
+      nfiles: 308
+    - path: src/boilercv/stages/update_previews/gray.py
+      md5: 089e35a18791e628d5bcd75e7fdca100
+      size: 768
+    outs:
+    - path: data/previews/gray.nc
+      md5: bca01dd9d72e5a7c25db766c5522652e
+      size: 18686615
+  filled_preview:
+    cmd: python -m boilercv.stages.update_previews.filled
+    deps:
+    - path: data/filled
+      md5: 9d9b406833ae3911940fd4d717bb20e1.dir
+      size: 3482532424
+      nfiles: 308
+    - path: data/sources
+      md5: a409ab9bcababc1baaea4dc53e312bda.dir
+      size: 7424602696
+      nfiles: 308
+    - path: src/boilercv/stages/update_previews/filled.py
+      md5: 879e5a5452d1e5ecc5dfaa79789f3840
+      size: 767
+    outs:
+    - path: data/previews/filled.nc
+      md5: f3596d4b5c08d8701b7630f1136c45aa
+      size: 1661392
```

### Comparing `boilercv-0.0.0/dvc_repro.ps1` & `boilercv-0.0.1/dvc_repro.ps1`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-<#.SYNOPSIS
-Reproduce the exact results during this commit.
-#>
-
-# Create the frozen virtual environment
-$FROZEN_VENV = '.venv-frozen'
-if ($Env:VIRTUAL_ENV) { 'deactivate' }
-if (Test-Path $FROZEN_VENV) { Remove-Item -Recurse -Force $FROZEN_VENV }
-$GLOBAL_PYTHON = 'py -3.11'
-try { Invoke-Expression $("$GLOBAL_PYTHON --version") }
-catch [System.Management.Automation.CommandNotFoundException] {
-    $GLOBAL_PYTHON = 'python3.11'
-}
-Invoke-Expression "$GLOBAL_PYTHON -m venv $FROZEN_VENV"
-
-# Activate environment
-$VENV_ACTIVATE_WINDOWS = "$FROZEN_VENV/Scripts/activate"
-$VENV_ACTIVATE_UNIX = "$FROZEN_VENV/bin/Activate.ps1"
-if ( Test-Path $VENV_ACTIVATE_WINDOWS ) { . $VENV_ACTIVATE_WINDOWS }
-elseif ( Test-Path $VENV_ACTIVATE_UNIX ) { . $VENV_ACTIVATE_UNIX }
-else {
-    throw [System.Management.Automation.ItemNotFoundException] 'Could not find a virtual environment.'
-}
-
-# Install the package and all frozen requirements
-pip install --no-deps '.'
-pip install --requirement 'repro.txt'
-
-# Reproduce the results using DVC
-dvc repro
+<#.SYNOPSIS
+Reproduce the exact results during this commit.
+#>
+
+# Create the frozen virtual environment
+$FROZEN_VENV = '.venv-frozen'
+if ($Env:VIRTUAL_ENV) { 'deactivate' }
+if (Test-Path $FROZEN_VENV) { Remove-Item -Recurse -Force $FROZEN_VENV }
+$GLOBAL_PYTHON = 'py -3.11'
+try { Invoke-Expression $("$GLOBAL_PYTHON --version") }
+catch [System.Management.Automation.CommandNotFoundException] {
+    $GLOBAL_PYTHON = 'python3.11'
+}
+Invoke-Expression "$GLOBAL_PYTHON -m venv $FROZEN_VENV"
+
+# Activate environment
+$VENV_ACTIVATE_WINDOWS = "$FROZEN_VENV/Scripts/activate"
+$VENV_ACTIVATE_UNIX = "$FROZEN_VENV/bin/Activate.ps1"
+if ( Test-Path $VENV_ACTIVATE_WINDOWS ) { . $VENV_ACTIVATE_WINDOWS }
+elseif ( Test-Path $VENV_ACTIVATE_UNIX ) { . $VENV_ACTIVATE_UNIX }
+else {
+    throw [System.Management.Automation.ItemNotFoundException] 'Could not find a virtual environment.'
+}
+
+# Install the package and all frozen requirements
+pip install --no-deps '.'
+pip install --requirement 'repro.txt'
+
+# Reproduce the results using DVC
+dvc repro
```

### Comparing `boilercv-0.0.0/params.yaml` & `boilercv-0.0.1/params.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-paths:
-  file_params: params.yaml
-  requirements: requirements.txt
-  dev_requirements: .tools/requirements
-  package: src/boilercv
-  stages: src/boilercv/stages
-  models: src/boilercv/models
-  paths_module: src/boilercv/models/paths.py
-  stage_check_cv: src/boilercv/stages/check_cv.py
-  stage_contours: src/boilercv/stages/contours.py
-  stage_fill: src/boilercv/stages/fill.py
-  stage_schema: src/boilercv/stages/schema.py
-  update_previews: src/boilercv/stages/update_previews
-  stage_binarized_preview: src/boilercv/stages/update_previews/binarized.py
-  stage_gray_preview: src/boilercv/stages/update_previews/gray.py
-  stage_filled_preview: src/boilercv/stages/update_previews/filled.py
-  data: data
-  contours: data/contours
-  examples: data/examples
-  filled: data/filled
-  rois: data/rois
-  samples: data/samples
-  sources: data/sources
-  previews: data/previews
-  binarized_preview: data/previews/binarized.nc
-  gray_preview: data/previews/gray.nc
-  filled_preview: data/previews/filled.nc
-  project_schema: data/schema
+paths:
+  file_params: params.yaml
+  requirements: requirements.txt
+  dev_requirements: .tools/requirements
+  package: src/boilercv
+  stages: src/boilercv/stages
+  models: src/boilercv/models
+  paths_module: src/boilercv/models/paths.py
+  stage_contours: src/boilercv/stages/contours.py
+  stage_fill: src/boilercv/stages/fill.py
+  stage_schema: src/boilercv/stages/schema.py
+  update_previews: src/boilercv/stages/update_previews
+  stage_binarized_preview: src/boilercv/stages/update_previews/binarized.py
+  stage_gray_preview: src/boilercv/stages/update_previews/gray.py
+  stage_filled_preview: src/boilercv/stages/update_previews/filled.py
+  data: data
+  contours: data/contours
+  examples: data/examples
+  filled: data/filled
+  rois: data/rois
+  samples: data/samples
+  sources: data/sources
+  previews: data/previews
+  binarized_preview: data/previews/binarized.nc
+  gray_preview: data/previews/gray.nc
+  filled_preview: data/previews/filled.nc
+  project_schema: data/schema
```

### Comparing `boilercv-0.0.0/pyproject.toml` & `boilercv-0.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-[build-system]
-requires = [ "flit_core >=3.3,<4",]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "boilercv"
-version = "0.0.0"
-description = "Computer vision routines suitable for nucleate pool boiling bubble analysis"
-readme = "README.md"
-requires-python = ">=3.11"
-classifiers = [ "License :: OSI Approved :: MIT License",]
-dependencies = [ "dvc[gs]>=2.53.0", "imageio[pyav]>=2.27.0", "loguru>=0.6.0", "matplotlib>=3.7.1", "numpy>=1.24.2", "opencv-contrib-python>=4.7.0.72", "pandera>=0.14.5", "pillow>=9.5.0", "pyarrow>=11.0.0", "pydantic>=1.10.7", "pyjanitor>=0.24.0", "pytz>=2023.3", "pyyaml>=6.0", "ruamel.yaml>=0.17.21", "scikit-image>=0.20.0", "scipy>=1.10.1", "seaborn>=0.12.2", "bottleneck>=1.3.7", "pandas[hdf5,parquet]>=2.0.0", "numexpr>=2.8.4", "pyqtgraph>=0.13.2", "pyside6>=6.4.3,<6.5", "netcdf4>=1.6.3", "python-dateutil>=2.8.2",]
-[[project.authors]]
-name = "Blake Naccarato"
-email = "blake.naccarato+captivate@gmail.com"
-
-[[project.authors]]
-name = "Kwang Jin Kim"
-
-[project.license]
-file = "LICENSE"
-
-[project.urls]
-changes = "https://blakenaccarato.github.io/boilercv/changelog.html"
-docs = "https://blakenaccarato.github.io/boilercv/"
-home = "https://github.com/blakeNaccarato/boilercv"
-tracker = "https://github.com/blakeNaccarato/boilercv/issues"
-
-[tool.ruff]
-fix = true
-select = [ "ALL",]
-src = [ "src", "tests",]
-target-version = "py311"
-extend-exclude = [ "template", "typings", ".github", ".tools", ".venv",]
-ignore = [ "ANN", "ARG005", "C408", "COM", "D10", "D20", "D213", "D402", "DTZ", "E501", "EM", "ERA", "FBT", "F841", "G0", "INP001", "ISC", "PD013", "PD901", "PD011", "PGH003", "PLR0913", "PLR2004", "PLW2901", "RET", "S301", "TCH", "TRY003", "W2", "B018", "F821", "S101", "T201",]
-unfixable = [ "F601",]
-
-[tool.ruff.pydocstyle]
-convention = "google"
-
-[tool.ruff.isort]
-split-on-trailing-comma = false
-
-[tool.ruff.per-file-ignores]
-"tests/**" = [ "N815", "ARG001", "S101",]
-"src/boilercv/video/cine/**" = [ "N815",]
-
-[tool.ruff.flake8-bugbear]
-extend-immutable-calls = [ "typer.Argument", "typer.Option",]
-
-[tool.ruff.pep8-naming]
-classmethod-decorators = [ "pydantic.validator",]
+[build-system]
+requires = [ "flit_core >=3.3,<4",]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "boilercv"
+version = "0.0.1"
+description = "Computer vision routines suitable for nucleate pool boiling bubble analysis"
+readme = "README.md"
+requires-python = ">=3.11"
+classifiers = [ "License :: OSI Approved :: MIT License",]
+dependencies = [ "dvc[gs]>=2.53.0", "imageio[pyav]>=2.27.0", "loguru>=0.6.0", "matplotlib>=3.7.1", "numpy>=1.24.2", "opencv-contrib-python>=4.7.0.72", "pandera>=0.14.5", "pillow>=9.5.0", "pyarrow>=11.0.0", "pydantic>=1.10.7", "pyjanitor>=0.24.0", "pytz>=2023.3", "pyyaml>=6.0", "ruamel.yaml>=0.17.21", "scikit-image>=0.20.0", "scipy>=1.10.1", "seaborn>=0.12.2", "bottleneck>=1.3.7", "pandas[hdf5,parquet]>=2.0.0", "numexpr>=2.8.4", "pyqtgraph>=0.13.2", "pyside6>=6.4.3,<6.5", "netcdf4>=1.6.3", "python-dateutil>=2.8.2",]
+[[project.authors]]
+name = "Blake Naccarato"
+email = "blake.naccarato+boilercv@gmail.com"
+
+[[project.authors]]
+name = "Kwang Jin Kim"
+
+[project.license]
+file = "LICENSE"
+
+[project.urls]
+changes = "https://blakenaccarato.github.io/boilercv/changelog.html"
+docs = "https://blakenaccarato.github.io/boilercv/"
+home = "https://github.com/blakeNaccarato/boilercv"
+tracker = "https://github.com/blakeNaccarato/boilercv/issues"
+
+[tool.ruff]
+fix = true
+select = [ "ALL",]
+src = [ "src", "tests",]
+target-version = "py311"
+extend-exclude = [ "template", "typings", ".github", ".tools", ".venv",]
+ignore = [ "ANN", "ARG005", "C408", "COM", "D10", "D20", "D213", "D402", "DTZ", "E501", "EM", "ERA", "FBT", "F841", "G0", "INP001", "ISC", "PD013", "PD901", "PD011", "PGH003", "PLR0913", "PLR2004", "PLW2901", "RET", "S301", "TCH", "TRY003", "W2", "B018", "F821", "S101", "T201",]
+unfixable = [ "F601",]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.ruff.isort]
+split-on-trailing-comma = false
+
+[tool.ruff.per-file-ignores]
+"tests/**" = [ "N815", "ARG001", "S101",]
+"src/boilercv/video/cine/**" = [ "N815",]
+
+[tool.ruff.flake8-bugbear]
+extend-immutable-calls = [ "typer.Argument", "typer.Option",]
+
+[tool.ruff.pep8-naming]
+classmethod-decorators = [ "pydantic.validator",]
```

### Comparing `boilercv-0.0.0/pytest.ini` & `boilercv-0.0.1/pytest.ini`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[pytest]
-addopts = -ra
-testpaths = tests
-# error: Raise for all warnings, even `DeprecationWarning`
-# pkg_resources: https://github.com/blakeNaccarato/copier-python/issues/319#issue-1609228740
-# Creating a LegacyVersion: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1454209165
-# pre_commit read_text and open_text: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1455177114
-# imp module and ABCs: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1455183241
-# dpath...pkg_resources: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1457219723
-# unclosed file...plumbum: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1458742412
-# ignore:is still running:subprocess:ResourceWarning:subprocess: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1493072447
-# ignore:BuiltinImporter.module_repr:DeprecationWarning:importlib._bootstrap: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1493542865
-# ignore:lib2to3: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1502112446
-filterwarnings =
-    error
-    ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning
-    ignore:Creating a LegacyVersion has been deprecated and will be removed in the next major release:DeprecationWarning:pip._vendor.packaging.version
-    ignore:read_text is deprecated:DeprecationWarning:pre_commit.util
-    ignore:open_text is deprecated:DeprecationWarning:importlib.resources._legacy
-    ignore:the imp module is deprecated in favour of importlib:DeprecationWarning:googlecloudsdk.core.util.importing
-    ignore:Using or importing the ABCs:DeprecationWarning:jsonschema.compat
-    ignore:The dpath.util package is being deprecated.:DeprecationWarning:dvc.dependency.param
-    ignore:unclosed file:ResourceWarning:dvc.stage.cache
-    ignore:the imp module is deprecated:DeprecationWarning:ansiwrap.core
-    ignore:unclosed file:ResourceWarning:ansiwrap.core
-    ignore:Jupyter is migrating its paths to use standard platformdirs:DeprecationWarning:jupyter_client.connect
-    ignore:the file is not specified with any extension:UserWarning:papermill.iorw
-    ignore:Passing unrecognized arguments to super:DeprecationWarning:traitlets.config.configurable
-    ignore:pkg_resources is deprecated as an API:DeprecationWarning:pkg_resources
-    ignore:unclosed file:ResourceWarning:plumbum.commands.base
-    ignore:Passing unrecognized arguments to super:DeprecationWarning:ipywidgets.widgets.widget
-    ignore:`ipykernel.pylab.backend_inline` is deprecated:DeprecationWarning:ipykernel.pylab.backend_inline
-    ignore:subprocess:ResourceWarning:subprocess
-    ignore:BuiltinImporter.module_repr:DeprecationWarning:importlib._bootstrap
-    ignore:lib2to3 package is deprecated and may not be able to parse Python:PendingDeprecationWarning
-    ignore:lib2to3 package is deprecated and may not be able to parse Python:DeprecationWarning
+[pytest]
+addopts = -ra
+testpaths = tests
+# error: Raise for all warnings, even `DeprecationWarning`
+# pkg_resources: https://github.com/blakeNaccarato/copier-python/issues/319#issue-1609228740
+# Creating a LegacyVersion: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1454209165
+# pre_commit read_text and open_text: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1455177114
+# imp module and ABCs: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1455183241
+# dpath...pkg_resources: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1457219723
+# unclosed file...plumbum: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1458742412
+# ignore:is still running:subprocess:ResourceWarning:subprocess: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1493072447
+# ignore:BuiltinImporter.module_repr:DeprecationWarning:importlib._bootstrap: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1493542865
+# ignore:lib2to3: https://github.com/blakeNaccarato/copier-python/issues/319#issuecomment-1502112446
+filterwarnings =
+    error
+    ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning
+    ignore:Creating a LegacyVersion has been deprecated and will be removed in the next major release:DeprecationWarning:pip._vendor.packaging.version
+    ignore:read_text is deprecated:DeprecationWarning:pre_commit.util
+    ignore:open_text is deprecated:DeprecationWarning:importlib.resources._legacy
+    ignore:the imp module is deprecated in favour of importlib:DeprecationWarning:googlecloudsdk.core.util.importing
+    ignore:Using or importing the ABCs:DeprecationWarning:jsonschema.compat
+    ignore:The dpath.util package is being deprecated.:DeprecationWarning:dvc.dependency.param
+    ignore:unclosed file:ResourceWarning:dvc.stage.cache
+    ignore:the imp module is deprecated:DeprecationWarning:ansiwrap.core
+    ignore:unclosed file:ResourceWarning:ansiwrap.core
+    ignore:Jupyter is migrating its paths to use standard platformdirs:DeprecationWarning:jupyter_client.connect
+    ignore:the file is not specified with any extension:UserWarning:papermill.iorw
+    ignore:Passing unrecognized arguments to super:DeprecationWarning:traitlets.config.configurable
+    ignore:pkg_resources is deprecated as an API:DeprecationWarning:pkg_resources
+    ignore:unclosed file:ResourceWarning:plumbum.commands.base
+    ignore:Passing unrecognized arguments to super:DeprecationWarning:ipywidgets.widgets.widget
+    ignore:`ipykernel.pylab.backend_inline` is deprecated:DeprecationWarning:ipykernel.pylab.backend_inline
+    ignore:subprocess:ResourceWarning:subprocess
+    ignore:BuiltinImporter.module_repr:DeprecationWarning:importlib._bootstrap
+    ignore:lib2to3 package is deprecated and may not be able to parse Python:PendingDeprecationWarning
+    ignore:lib2to3 package is deprecated and may not be able to parse Python:DeprecationWarning
```

### Comparing `boilercv-0.0.0/pythonrc.py` & `boilercv-0.0.1/pythonrc.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""Startup for Python.
-
-Avoid activating Rich features that break functionality outside of the REPL.
-"""
-
-
-def main():
-    from rich import inspect, traceback  # noqa: F401  # pyright: ignore
-
-    traceback.install()
-
-    if not is_notebook_or_ipython():
-        from rich import pretty, print  # noqa: F401  # pyright: ignore
-
-        pretty.install()
-
-
-# https://stackoverflow.com/a/39662359
-def is_notebook_or_ipython() -> bool:
-    try:
-        shell = get_ipython().__class__.__name__  # pyright: ignore  # Dynamic
-    except NameError:
-        return False  # Probably standard Python interpreter
-    else:
-        return shell == "TerminalInteractiveShell"
-
-
-main()
+"""Startup for Python.
+
+Avoid activating Rich features that break functionality outside of the REPL.
+"""
+
+
+def main():
+    from rich import inspect, traceback  # noqa: F401  # pyright: ignore
+
+    traceback.install()
+
+    if not is_notebook_or_ipython():
+        from rich import pretty, print  # noqa: F401  # pyright: ignore
+
+        pretty.install()
+
+
+# https://stackoverflow.com/a/39662359
+def is_notebook_or_ipython() -> bool:
+    try:
+        shell = get_ipython().__class__.__name__  # pyright: ignore  # Dynamic
+    except NameError:
+        return False  # Probably standard Python interpreter
+    else:
+        return shell == "TerminalInteractiveShell"
+
+
+main()
```

### Comparing `boilercv-0.0.0/renovate.json` & `boilercv-0.0.1/renovate.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 23% similar despite different names*

```diff
@@ -1,182 +1,176 @@
-00000000: 7b0d 0a20 2022 2473 6368 656d 6122 3a20  {..  "$schema": 
-00000010: 2268 7474 7073 3a2f 2f64 6f63 732e 7265  "https://docs.re
-00000020: 6e6f 7661 7465 626f 742e 636f 6d2f 7265  novatebot.com/re
-00000030: 6e6f 7661 7465 2d73 6368 656d 612e 6a73  novate-schema.js
-00000040: 6f6e 222c 0d0a 2020 2264 6573 6372 6970  on",..  "descrip
-00000050: 7469 6f6e 223a 2022 4573 7461 626c 6973  tion": "Establis
-00000060: 6820 6261 7365 2063 6f6e 6669 672c 2073  h base config, s
-00000070: 6368 6564 756c 652c 2061 6e64 206d 616e  chedule, and man
-00000080: 6167 6572 2064 6566 6175 6c74 732e 222c  ager defaults.",
-00000090: 0d0a 2020 2265 7874 656e 6473 223a 205b  ..  "extends": [
-000000a0: 2263 6f6e 6669 673a 6261 7365 222c 2022  "config:base", "
-000000b0: 3a65 6e61 626c 6550 7265 436f 6d6d 6974  :enablePreCommit
-000000c0: 222c 2022 3a64 6973 6162 6c65 5261 7465  ", ":disableRate
-000000d0: 4c69 6d69 7469 6e67 225d 2c0d 0a20 2022  Limiting"],..  "
-000000e0: 7363 6865 6475 6c65 223a 205b 226f 6e20  schedule": ["on 
-000000f0: 7468 6520 3136 7468 2064 6179 206f 6620  the 16th day of 
-00000100: 7468 6520 6d6f 6e74 6822 5d2c 0d0a 2020  the month"],..  
-00000110: 2267 6974 2d73 7562 6d6f 6475 6c65 7322  "git-submodules"
-00000120: 3a20 7b20 2265 6e61 626c 6564 223a 2074  : { "enabled": t
-00000130: 7275 6520 7d2c 0d0a 2020 2265 6e61 626c  rue },..  "enabl
-00000140: 6564 4d61 6e61 6765 7273 223a 205b 0d0a  edManagers": [..
-00000150: 2020 2020 2267 6974 2d73 7562 6d6f 6475      "git-submodu
-00000160: 6c65 7322 2c0d 0a20 2020 2022 6769 7468  les",..    "gith
-00000170: 7562 2d61 6374 696f 6e73 222c 0d0a 2020  ub-actions",..  
-00000180: 2020 2270 6970 5f72 6571 7569 7265 6d65    "pip_requireme
-00000190: 6e74 7322 2c0d 0a20 2020 2022 7072 652d  nts",..    "pre-
-000001a0: 636f 6d6d 6974 220d 0a20 205d 2c0d 0a20  commit"..  ],.. 
-000001b0: 2022 7069 705f 7265 7175 6972 656d 656e   "pip_requiremen
-000001c0: 7473 223a 207b 0d0a 2020 2020 2264 6573  ts": {..    "des
-000001d0: 6372 6970 7469 6f6e 223a 2022 4164 6469  cription": "Addi
-000001e0: 7469 6f6e 616c 6c79 206d 6f6e 6974 6f72  tionally monitor
-000001f0: 2074 6865 7365 2066 696c 6573 2e22 2c0d   these files.",.
-00000200: 0a20 2020 2022 6669 6c65 4d61 7463 6822  .    "fileMatch"
-00000210: 3a20 5b22 5e5c 5c2e 746f 6f6c 732f 7265  : ["^\\.tools/re
-00000220: 7175 6972 656d 656e 7473 2f2a 225d 0d0a  quirements/*"]..
-00000230: 2020 7d2c 0d0a 2020 2270 6163 6b61 6765    },..  "package
-00000240: 5275 6c65 7322 3a20 5b0d 0a20 2020 207b  Rules": [..    {
-00000250: 0d0a 2020 2020 2020 2264 6573 6372 6970  ..      "descrip
-00000260: 7469 6f6e 223a 2022 4967 6e6f 7265 2064  tion": "Ignore d
-00000270: 6570 656e 6465 6e63 6965 7320 7769 7468  ependencies with
-00000280: 2069 7373 7565 7320 7370 6563 6966 6963   issues specific
-00000290: 2074 6f20 7468 6973 2070 726f 6a65 6374   to this project
-000002a0: 2e22 2c0d 0a20 2020 2020 2022 6d61 7463  .",..      "matc
-000002b0: 684d 616e 6167 6572 7322 3a20 5b22 7069  hManagers": ["pi
-000002c0: 705f 7265 7175 6972 656d 656e 7473 225d  p_requirements"]
-000002d0: 2c0d 0a20 2020 2020 2022 6967 6e6f 7265  ,..      "ignore
-000002e0: 4465 7073 223a 205b 2270 7973 6964 6536  Deps": ["pyside6
-000002f0: 225d 0d0a 2020 2020 7d2c 0d0a 2020 2020  "]..    },..    
-00000300: 7b0d 0a20 2020 2020 2022 6772 6f75 704e  {..      "groupN
-00000310: 616d 6522 3a20 2270 7972 6967 6874 2061  ame": "pyright a
-00000320: 6e64 2074 7970 6520 7374 7562 7322 2c0d  nd type stubs",.
-00000330: 0a20 2020 2020 2022 6772 6f75 7053 6c75  .      "groupSlu
-00000340: 6722 3a20 2270 7972 6967 6874 2d61 6e64  g": "pyright-and
-00000350: 2d74 7970 652d 7374 7562 7322 2c0d 0a20  -type-stubs",.. 
-00000360: 2020 2020 2022 6d61 7463 6850 6163 6b61       "matchPacka
-00000370: 6765 5061 7474 6572 6e73 223a 205b 222a  gePatterns": ["*
-00000380: 225d 2c0d 0a20 2020 2020 2022 6d61 7463  "],..      "matc
-00000390: 684d 616e 6167 6572 7322 3a20 5b22 7069  hManagers": ["pi
-000003a0: 705f 7265 7175 6972 656d 656e 7473 222c  p_requirements",
-000003b0: 2022 6769 742d 7375 626d 6f64 756c 6573   "git-submodules
-000003c0: 225d 2c0d 0a20 2020 2020 2022 6d61 7463  "],..      "matc
-000003d0: 6850 6163 6b61 6765 4e61 6d65 7322 3a20  hPackageNames": 
-000003e0: 5b22 7079 7269 6768 7422 2c20 2274 7970  ["pyright", "typ
-000003f0: 696e 6773 225d 0d0a 2020 2020 7d2c 0d0a  ings"]..    },..
-00000400: 2020 2020 7b0d 0a20 2020 2020 2022 6772      {..      "gr
-00000410: 6f75 704e 616d 6522 3a20 2261 6c6c 206e  oupName": "all n
-00000420: 6f6e 2d6d 616a 6f72 2064 6570 656e 6465  on-major depende
-00000430: 6e63 6965 7320 6578 6365 7074 2070 7972  ncies except pyr
-00000440: 6967 6874 222c 0d0a 2020 2020 2020 2267  ight",..      "g
-00000450: 726f 7570 536c 7567 223a 2022 616c 6c2d  roupSlug": "all-
-00000460: 6d69 6e6f 722d 7061 7463 6822 2c0d 0a20  minor-patch",.. 
-00000470: 2020 2020 2022 6d61 7463 6850 6163 6b61       "matchPacka
-00000480: 6765 5061 7474 6572 6e73 223a 205b 222a  gePatterns": ["*
-00000490: 225d 2c0d 0a20 2020 2020 2022 6d61 7463  "],..      "matc
-000004a0: 6855 7064 6174 6554 7970 6573 223a 205b  hUpdateTypes": [
-000004b0: 226d 696e 6f72 222c 2022 7061 7463 6822  "minor", "patch"
-000004c0: 5d2c 0d0a 2020 2020 2020 2265 7863 6c75  ],..      "exclu
-000004d0: 6465 4465 704e 616d 6573 223a 205b 2270  deDepNames": ["p
-000004e0: 7972 6967 6874 225d 0d0a 2020 2020 7d2c  yright"]..    },
-000004f0: 0d0a 2020 2020 7b0d 0a20 2020 2020 2022  ..    {..      "
-00000500: 6465 7363 7269 7074 696f 6e22 3a20 2249  description": "I
-00000510: 676e 6f72 6520 6769 7468 7562 2d61 6374  gnore github-act
-00000520: 696f 6e73 2064 6570 656e 6465 6e63 6965  ions dependencie
-00000530: 7320 6d61 6e61 6765 6420 6279 2074 6865  s managed by the
-00000540: 2074 656d 706c 6174 652e 222c 0d0a 2020   template.",..  
-00000550: 2020 2020 226d 6174 6368 4d61 6e61 6765      "matchManage
-00000560: 7273 223a 205b 2267 6974 6875 622d 6163  rs": ["github-ac
-00000570: 7469 6f6e 7322 5d2c 0d0a 2020 2020 2020  tions"],..      
-00000580: 2269 676e 6f72 6544 6570 7322 3a20 5b0d  "ignoreDeps": [.
-00000590: 0a20 2020 2020 2020 2022 6472 6f70 7365  .        "dropse
-000005a0: 6564 2f63 6861 6e67 6572 656c 6561 7365  ed/changerelease
-000005b0: 222c 0d0a 2020 2020 2020 2020 2261 6374  ",..        "act
-000005c0: 696f 6e73 2f63 6865 636b 6f75 7422 2c0d  ions/checkout",.
-000005d0: 0a20 2020 2020 2020 2022 6769 7468 7562  .        "github
-000005e0: 2f63 6f64 6571 6c2d 6163 7469 6f6e 222c  /codeql-action",
-000005f0: 0d0a 2020 2020 2020 2020 2262 6c61 6b65  ..        "blake
-00000600: 4e61 6363 6172 6174 6f2f 636f 7069 6572  Naccarato/copier
-00000610: 2d70 7974 686f 6e2d 776f 726b 666c 6f77  -python-workflow
-00000620: 2d73 6574 7570 222c 0d0a 2020 2020 2020  -setup",..      
-00000630: 2020 2263 6f64 6563 6f76 2f63 6f64 6563    "codecov/codec
-00000640: 6f76 2d61 6374 696f 6e22 2c0d 0a20 2020  ov-action",..   
-00000650: 2020 2020 2022 7374 6566 616e 7a77 6569       "stefanzwei
-00000660: 6665 6c2f 6769 742d 6175 746f 2d63 6f6d  fel/git-auto-com
-00000670: 6d69 742d 6163 7469 6f6e 222c 0d0a 2020  mit-action",..  
-00000680: 2020 2020 2020 2261 6374 696f 6e73 2f75        "actions/u
-00000690: 706c 6f61 642d 7061 6765 732d 6172 7469  pload-pages-arti
-000006a0: 6661 6374 222c 0d0a 2020 2020 2020 2020  fact",..        
-000006b0: 2261 6374 696f 6e73 2f64 6570 6c6f 792d  "actions/deploy-
-000006c0: 7061 6765 7322 0d0a 2020 2020 2020 5d0d  pages"..      ].
-000006d0: 0a20 2020 207d 2c0d 0a20 2020 207b 0d0a  .    },..    {..
-000006e0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-000006f0: 6f6e 223a 2022 4967 6e6f 7265 2070 7265  on": "Ignore pre
-00000700: 2d63 6f6d 6d69 7420 6465 7065 6e64 656e  -commit dependen
-00000710: 6369 6573 206d 616e 6167 6564 2062 7920  cies managed by 
-00000720: 7468 6520 7465 6d70 6c61 7465 2e22 2c0d  the template.",.
-00000730: 0a20 2020 2020 2022 6d61 7463 684d 616e  .      "matchMan
-00000740: 6167 6572 7322 3a20 5b22 7072 652d 636f  agers": ["pre-co
-00000750: 6d6d 6974 225d 2c0d 0a20 2020 2020 2022  mmit"],..      "
-00000760: 6967 6e6f 7265 4465 7073 223a 205b 0d0a  ignoreDeps": [..
-00000770: 2020 2020 2020 2020 2270 7265 2d63 6f6d          "pre-com
-00000780: 6d69 742f 7072 652d 636f 6d6d 6974 2d68  mit/pre-commit-h
-00000790: 6f6f 6b73 222c 0d0a 2020 2020 2020 2020  ooks",..        
-000007a0: 2270 7366 2f62 6c61 636b 222c 0d0a 2020  "psf/black",..  
-000007b0: 2020 2020 2020 2263 6861 726c 6965 726d        "charlierm
-000007c0: 6172 7368 2f72 7566 662d 7072 652d 636f  arsh/ruff-pre-co
-000007d0: 6d6d 6974 222c 0d0a 2020 2020 2020 2020  mmit",..        
-000007e0: 2273 7273 7465 7665 6e73 6f6e 2f6e 622d  "srstevenson/nb-
-000007f0: 636c 6561 6e22 2c0d 0a20 2020 2020 2020  clean",..       
-00000800: 2022 6e62 5141 2d64 6576 2f6e 6251 4122   "nbQA-dev/nbQA"
-00000810: 2c0d 0a20 2020 2020 2020 2022 6173 6f74  ,..        "asot
-00000820: 7469 6c65 2f62 6c61 636b 656e 2d64 6f63  tile/blacken-doc
-00000830: 7322 2c0d 0a20 2020 2020 2020 2022 4461  s",..        "Da
-00000840: 7669 6441 6e73 6f6e 2f6d 6172 6b64 6f77  vidAnson/markdow
-00000850: 6e6c 696e 742d 636c 6932 220d 0a20 2020  nlint-cli2"..   
-00000860: 2020 205d 0d0a 2020 2020 7d2c 0d0a 2020     ]..    },..  
-00000870: 2020 7b0d 0a20 2020 2020 2022 6465 7363    {..      "desc
-00000880: 7269 7074 696f 6e22 3a20 2249 676e 6f72  ription": "Ignor
-00000890: 6520 6465 7065 6e64 656e 6369 6573 206d  e dependencies m
-000008a0: 616e 6167 6564 2062 7920 7468 6520 7465  anaged by the te
-000008b0: 6d70 6c61 7465 2e20 446f 206d 616e 6167  mplate. Do manag
-000008c0: 6520 7079 7269 6768 742e 222c 0d0a 2020  e pyright.",..  
-000008d0: 2020 2020 226d 6174 6368 4d61 6e61 6765      "matchManage
-000008e0: 7273 223a 205b 2270 6970 5f72 6571 7569  rs": ["pip_requi
-000008f0: 7265 6d65 6e74 7322 5d2c 0d0a 2020 2020  rements"],..    
-00000900: 2020 226d 6174 6368 5061 7468 7322 3a20    "matchPaths": 
-00000910: 5b22 2e74 6f6f 6c73 2f72 6571 7569 7265  [".tools/require
-00000920: 6d65 6e74 732f 2a22 5d2c 0d0a 2020 2020  ments/*"],..    
-00000930: 2020 2269 676e 6f72 6544 6570 7322 3a20    "ignoreDeps": 
-00000940: 5b0d 0a20 2020 2020 2020 2022 6a75 7079  [..        "jupy
-00000950: 7465 722d 626f 6f6b 222c 0d0a 2020 2020  ter-book",..    
-00000960: 2020 2020 2277 6174 6368 2d66 696c 6573      "watch-files
-00000970: 222c 0d0a 2020 2020 2020 2020 226d 7973  ",..        "mys
-00000980: 742d 7061 7273 6572 222c 0d0a 2020 2020  t-parser",..    
-00000990: 2020 2020 2273 7068 696e 782d 6175 746f      "sphinx-auto
-000009a0: 6275 696c 6422 2c0d 0a20 2020 2020 2020  build",..       
-000009b0: 2022 7370 6869 6e78 2d62 6f6f 6b2d 7468   "sphinx-book-th
-000009c0: 656d 6522 2c0d 0a20 2020 2020 2020 2022  eme",..        "
-000009d0: 7370 6869 6e78 2d64 6573 6967 6e22 2c0d  sphinx-design",.
-000009e0: 0a20 2020 2020 2020 2022 636f 7069 6572  .        "copier
-000009f0: 222c 0d0a 2020 2020 2020 2020 2274 6f6d  ",..        "tom
-00000a00: 6c22 2c0d 0a20 2020 2020 2020 2022 666c  l",..        "fl
-00000a10: 6974 222c 0d0a 2020 2020 2020 2020 2272  it",..        "r
-00000a20: 7566 6622 2c0d 0a20 2020 2020 2020 2022  uff",..        "
-00000a30: 7079 7465 7374 222c 0d0a 2020 2020 2020  pytest",..      
-00000a40: 2020 2270 7974 6573 742d 636f 7622 2c0d    "pytest-cov",.
-00000a50: 0a20 2020 2020 2020 2022 6a75 7079 7465  .        "jupyte
-00000a60: 7222 2c0d 0a20 2020 2020 2020 2022 6970  r",..        "ip
-00000a70: 796d 706c 222c 0d0a 2020 2020 2020 2020  ympl",..        
-00000a80: 2264 6562 7567 7079 222c 0d0a 2020 2020  "debugpy",..    
-00000a90: 2020 2020 2272 6963 6822 2c0d 0a20 2020      "rich",..   
-00000aa0: 2020 2020 2022 6970 7974 686f 6e22 2c0d       "ipython",.
-00000ab0: 0a20 2020 2020 2020 2022 626c 6163 6b22  .        "black"
-00000ac0: 2c0d 0a20 2020 2020 2020 2022 6e62 7161  ,..        "nbqa
-00000ad0: 222c 0d0a 2020 2020 2020 2020 2272 7566  ",..        "ruf
-00000ae0: 6622 2c0d 0a20 2020 2020 2020 2022 736f  f",..        "so
-00000af0: 7572 6365 7279 2d63 6c69 222c 0d0a 2020  urcery-cli",..  
-00000b00: 2020 2020 2020 2273 6e61 6b65 7669 7a22        "snakeviz"
-00000b10: 2c0d 0a20 2020 2020 2020 2022 7072 652d  ,..        "pre-
-00000b20: 636f 6d6d 6974 222c 0d0a 2020 2020 2020  commit",..      
-00000b30: 2020 226b 6579 7269 6e67 220d 0a20 2020    "keyring"..   
-00000b40: 2020 205d 0d0a 2020 2020 7d0d 0a20 205d     ]..    }..  ]
-00000b50: 0d0a 7d0d 0a                             ..}..
+00000000: 7b0a 2020 2224 7363 6865 6d61 223a 2022  {.  "$schema": "
+00000010: 6874 7470 733a 2f2f 646f 6373 2e72 656e  https://docs.ren
+00000020: 6f76 6174 6562 6f74 2e63 6f6d 2f72 656e  ovatebot.com/ren
+00000030: 6f76 6174 652d 7363 6865 6d61 2e6a 736f  ovate-schema.jso
+00000040: 6e22 2c0a 2020 2264 6573 6372 6970 7469  n",.  "descripti
+00000050: 6f6e 223a 2022 4573 7461 626c 6973 6820  on": "Establish 
+00000060: 6261 7365 2063 6f6e 6669 672c 2073 6368  base config, sch
+00000070: 6564 756c 652c 2061 6e64 206d 616e 6167  edule, and manag
+00000080: 6572 2064 6566 6175 6c74 732e 222c 0a20  er defaults.",. 
+00000090: 2022 6578 7465 6e64 7322 3a20 5b22 636f   "extends": ["co
+000000a0: 6e66 6967 3a62 6173 6522 2c20 223a 656e  nfig:base", ":en
+000000b0: 6162 6c65 5072 6543 6f6d 6d69 7422 2c20  ablePreCommit", 
+000000c0: 223a 6469 7361 626c 6552 6174 654c 696d  ":disableRateLim
+000000d0: 6974 696e 6722 5d2c 0a20 2022 7363 6865  iting"],.  "sche
+000000e0: 6475 6c65 223a 205b 226f 6e20 7468 6520  dule": ["on the 
+000000f0: 3136 7468 2064 6179 206f 6620 7468 6520  16th day of the 
+00000100: 6d6f 6e74 6822 5d2c 0a20 2022 6769 742d  month"],.  "git-
+00000110: 7375 626d 6f64 756c 6573 223a 207b 2022  submodules": { "
+00000120: 656e 6162 6c65 6422 3a20 7472 7565 207d  enabled": true }
+00000130: 2c0a 2020 2265 6e61 626c 6564 4d61 6e61  ,.  "enabledMana
+00000140: 6765 7273 223a 205b 0a20 2020 2022 6769  gers": [.    "gi
+00000150: 742d 7375 626d 6f64 756c 6573 222c 0a20  t-submodules",. 
+00000160: 2020 2022 6769 7468 7562 2d61 6374 696f     "github-actio
+00000170: 6e73 222c 0a20 2020 2022 7069 705f 7265  ns",.    "pip_re
+00000180: 7175 6972 656d 656e 7473 222c 0a20 2020  quirements",.   
+00000190: 2022 7072 652d 636f 6d6d 6974 220a 2020   "pre-commit".  
+000001a0: 5d2c 0a20 2022 7069 705f 7265 7175 6972  ],.  "pip_requir
+000001b0: 656d 656e 7473 223a 207b 0a20 2020 2022  ements": {.    "
+000001c0: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
+000001d0: 6464 6974 696f 6e61 6c6c 7920 6d6f 6e69  dditionally moni
+000001e0: 746f 7220 7468 6573 6520 6669 6c65 732e  tor these files.
+000001f0: 222c 0a20 2020 2022 6669 6c65 4d61 7463  ",.    "fileMatc
+00000200: 6822 3a20 5b22 5e5c 5c2e 746f 6f6c 732f  h": ["^\\.tools/
+00000210: 7265 7175 6972 656d 656e 7473 2f2a 225d  requirements/*"]
+00000220: 0a20 207d 2c0a 2020 2270 6163 6b61 6765  .  },.  "package
+00000230: 5275 6c65 7322 3a20 5b0a 2020 2020 7b0a  Rules": [.    {.
+00000240: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000250: 6f6e 223a 2022 4967 6e6f 7265 2064 6570  on": "Ignore dep
+00000260: 656e 6465 6e63 6965 7320 7769 7468 2069  endencies with i
+00000270: 7373 7565 7320 7370 6563 6966 6963 2074  ssues specific t
+00000280: 6f20 7468 6973 2070 726f 6a65 6374 2e22  o this project."
+00000290: 2c0a 2020 2020 2020 226d 6174 6368 4d61  ,.      "matchMa
+000002a0: 6e61 6765 7273 223a 205b 2270 6970 5f72  nagers": ["pip_r
+000002b0: 6571 7569 7265 6d65 6e74 7322 5d2c 0a20  equirements"],. 
+000002c0: 2020 2020 2022 6967 6e6f 7265 4465 7073       "ignoreDeps
+000002d0: 223a 205b 2270 7973 6964 6536 225d 0a20  ": ["pyside6"]. 
+000002e0: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+000002f0: 2020 2267 726f 7570 4e61 6d65 223a 2022    "groupName": "
+00000300: 7079 7269 6768 7420 616e 6420 7479 7065  pyright and type
+00000310: 2073 7475 6273 222c 0a20 2020 2020 2022   stubs",.      "
+00000320: 6772 6f75 7053 6c75 6722 3a20 2270 7972  groupSlug": "pyr
+00000330: 6967 6874 2d61 6e64 2d74 7970 652d 7374  ight-and-type-st
+00000340: 7562 7322 2c0a 2020 2020 2020 226d 6174  ubs",.      "mat
+00000350: 6368 5061 636b 6167 6550 6174 7465 726e  chPackagePattern
+00000360: 7322 3a20 5b22 2a22 5d2c 0a20 2020 2020  s": ["*"],.     
+00000370: 2022 6d61 7463 684d 616e 6167 6572 7322   "matchManagers"
+00000380: 3a20 5b22 7069 705f 7265 7175 6972 656d  : ["pip_requirem
+00000390: 656e 7473 222c 2022 6769 742d 7375 626d  ents", "git-subm
+000003a0: 6f64 756c 6573 225d 2c0a 2020 2020 2020  odules"],.      
+000003b0: 226d 6174 6368 5061 636b 6167 654e 616d  "matchPackageNam
+000003c0: 6573 223a 205b 2270 7972 6967 6874 222c  es": ["pyright",
+000003d0: 2022 7479 7069 6e67 7322 5d0a 2020 2020   "typings"].    
+000003e0: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
+000003f0: 6772 6f75 704e 616d 6522 3a20 2261 6c6c  groupName": "all
+00000400: 206e 6f6e 2d6d 616a 6f72 2064 6570 656e   non-major depen
+00000410: 6465 6e63 6965 7320 6578 6365 7074 2070  dencies except p
+00000420: 7972 6967 6874 222c 0a20 2020 2020 2022  yright",.      "
+00000430: 6772 6f75 7053 6c75 6722 3a20 2261 6c6c  groupSlug": "all
+00000440: 2d6d 696e 6f72 2d70 6174 6368 222c 0a20  -minor-patch",. 
+00000450: 2020 2020 2022 6d61 7463 6850 6163 6b61       "matchPacka
+00000460: 6765 5061 7474 6572 6e73 223a 205b 222a  gePatterns": ["*
+00000470: 225d 2c0a 2020 2020 2020 226d 6174 6368  "],.      "match
+00000480: 5570 6461 7465 5479 7065 7322 3a20 5b22  UpdateTypes": ["
+00000490: 6d69 6e6f 7222 2c20 2270 6174 6368 225d  minor", "patch"]
+000004a0: 2c0a 2020 2020 2020 2265 7863 6c75 6465  ,.      "exclude
+000004b0: 4465 704e 616d 6573 223a 205b 2270 7972  DepNames": ["pyr
+000004c0: 6967 6874 225d 0a20 2020 207d 2c0a 2020  ight"].    },.  
+000004d0: 2020 7b0a 2020 2020 2020 2264 6573 6372    {.      "descr
+000004e0: 6970 7469 6f6e 223a 2022 4967 6e6f 7265  iption": "Ignore
+000004f0: 2067 6974 6875 622d 6163 7469 6f6e 7320   github-actions 
+00000500: 6465 7065 6e64 656e 6369 6573 206d 616e  dependencies man
+00000510: 6167 6564 2062 7920 7468 6520 7465 6d70  aged by the temp
+00000520: 6c61 7465 2e22 2c0a 2020 2020 2020 226d  late.",.      "m
+00000530: 6174 6368 4d61 6e61 6765 7273 223a 205b  atchManagers": [
+00000540: 2267 6974 6875 622d 6163 7469 6f6e 7322  "github-actions"
+00000550: 5d2c 0a20 2020 2020 2022 6967 6e6f 7265  ],.      "ignore
+00000560: 4465 7073 223a 205b 0a20 2020 2020 2020  Deps": [.       
+00000570: 2022 6472 6f70 7365 6564 2f63 6861 6e67   "dropseed/chang
+00000580: 6572 656c 6561 7365 222c 0a20 2020 2020  erelease",.     
+00000590: 2020 2022 6163 7469 6f6e 732f 6368 6563     "actions/chec
+000005a0: 6b6f 7574 222c 0a20 2020 2020 2020 2022  kout",.        "
+000005b0: 6769 7468 7562 2f63 6f64 6571 6c2d 6163  github/codeql-ac
+000005c0: 7469 6f6e 222c 0a20 2020 2020 2020 2022  tion",.        "
+000005d0: 626c 616b 654e 6163 6361 7261 746f 2f63  blakeNaccarato/c
+000005e0: 6f70 6965 722d 7079 7468 6f6e 2d77 6f72  opier-python-wor
+000005f0: 6b66 6c6f 772d 7365 7475 7022 2c0a 2020  kflow-setup",.  
+00000600: 2020 2020 2020 2263 6f64 6563 6f76 2f63        "codecov/c
+00000610: 6f64 6563 6f76 2d61 6374 696f 6e22 2c0a  odecov-action",.
+00000620: 2020 2020 2020 2020 2273 7465 6661 6e7a          "stefanz
+00000630: 7765 6966 656c 2f67 6974 2d61 7574 6f2d  weifel/git-auto-
+00000640: 636f 6d6d 6974 2d61 6374 696f 6e22 2c0a  commit-action",.
+00000650: 2020 2020 2020 2020 2261 6374 696f 6e73          "actions
+00000660: 2f75 706c 6f61 642d 7061 6765 732d 6172  /upload-pages-ar
+00000670: 7469 6661 6374 222c 0a20 2020 2020 2020  tifact",.       
+00000680: 2022 6163 7469 6f6e 732f 6465 706c 6f79   "actions/deploy
+00000690: 2d70 6167 6573 220a 2020 2020 2020 5d0a  -pages".      ].
+000006a0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
+000006b0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000006c0: 3a20 2249 676e 6f72 6520 7072 652d 636f  : "Ignore pre-co
+000006d0: 6d6d 6974 2064 6570 656e 6465 6e63 6965  mmit dependencie
+000006e0: 7320 6d61 6e61 6765 6420 6279 2074 6865  s managed by the
+000006f0: 2074 656d 706c 6174 652e 222c 0a20 2020   template.",.   
+00000700: 2020 2022 6d61 7463 684d 616e 6167 6572     "matchManager
+00000710: 7322 3a20 5b22 7072 652d 636f 6d6d 6974  s": ["pre-commit
+00000720: 225d 2c0a 2020 2020 2020 2269 676e 6f72  "],.      "ignor
+00000730: 6544 6570 7322 3a20 5b0a 2020 2020 2020  eDeps": [.      
+00000740: 2020 2270 7265 2d63 6f6d 6d69 742f 7072    "pre-commit/pr
+00000750: 652d 636f 6d6d 6974 2d68 6f6f 6b73 222c  e-commit-hooks",
+00000760: 0a20 2020 2020 2020 2022 7073 662f 626c  .        "psf/bl
+00000770: 6163 6b22 2c0a 2020 2020 2020 2020 2263  ack",.        "c
+00000780: 6861 726c 6965 726d 6172 7368 2f72 7566  harliermarsh/ruf
+00000790: 662d 7072 652d 636f 6d6d 6974 222c 0a20  f-pre-commit",. 
+000007a0: 2020 2020 2020 2022 7372 7374 6576 656e         "srsteven
+000007b0: 736f 6e2f 6e62 2d63 6c65 616e 222c 0a20  son/nb-clean",. 
+000007c0: 2020 2020 2020 2022 6e62 5141 2d64 6576         "nbQA-dev
+000007d0: 2f6e 6251 4122 2c0a 2020 2020 2020 2020  /nbQA",.        
+000007e0: 2261 736f 7474 696c 652f 626c 6163 6b65  "asottile/blacke
+000007f0: 6e2d 646f 6373 222c 0a20 2020 2020 2020  n-docs",.       
+00000800: 2022 4461 7669 6441 6e73 6f6e 2f6d 6172   "DavidAnson/mar
+00000810: 6b64 6f77 6e6c 696e 742d 636c 6932 220a  kdownlint-cli2".
+00000820: 2020 2020 2020 5d0a 2020 2020 7d2c 0a20        ].    },. 
+00000830: 2020 207b 0a20 2020 2020 2022 6465 7363     {.      "desc
+00000840: 7269 7074 696f 6e22 3a20 2249 676e 6f72  ription": "Ignor
+00000850: 6520 6465 7065 6e64 656e 6369 6573 206d  e dependencies m
+00000860: 616e 6167 6564 2062 7920 7468 6520 7465  anaged by the te
+00000870: 6d70 6c61 7465 2e20 446f 206d 616e 6167  mplate. Do manag
+00000880: 6520 7079 7269 6768 742e 222c 0a20 2020  e pyright.",.   
+00000890: 2020 2022 6d61 7463 684d 616e 6167 6572     "matchManager
+000008a0: 7322 3a20 5b22 7069 705f 7265 7175 6972  s": ["pip_requir
+000008b0: 656d 656e 7473 225d 2c0a 2020 2020 2020  ements"],.      
+000008c0: 226d 6174 6368 5061 7468 7322 3a20 5b22  "matchPaths": ["
+000008d0: 2e74 6f6f 6c73 2f72 6571 7569 7265 6d65  .tools/requireme
+000008e0: 6e74 732f 2a22 5d2c 0a20 2020 2020 2022  nts/*"],.      "
+000008f0: 6967 6e6f 7265 4465 7073 223a 205b 0a20  ignoreDeps": [. 
+00000900: 2020 2020 2020 2022 6a75 7079 7465 722d         "jupyter-
+00000910: 626f 6f6b 222c 0a20 2020 2020 2020 2022  book",.        "
+00000920: 7761 7463 682d 6669 6c65 7322 2c0a 2020  watch-files",.  
+00000930: 2020 2020 2020 226d 7973 742d 7061 7273        "myst-pars
+00000940: 6572 222c 0a20 2020 2020 2020 2022 7370  er",.        "sp
+00000950: 6869 6e78 2d61 7574 6f62 7569 6c64 222c  hinx-autobuild",
+00000960: 0a20 2020 2020 2020 2022 7370 6869 6e78  .        "sphinx
+00000970: 2d62 6f6f 6b2d 7468 656d 6522 2c0a 2020  -book-theme",.  
+00000980: 2020 2020 2020 2273 7068 696e 782d 6465        "sphinx-de
+00000990: 7369 676e 222c 0a20 2020 2020 2020 2022  sign",.        "
+000009a0: 636f 7069 6572 222c 0a20 2020 2020 2020  copier",.       
+000009b0: 2022 746f 6d6c 222c 0a20 2020 2020 2020   "toml",.       
+000009c0: 2022 666c 6974 222c 0a20 2020 2020 2020   "flit",.       
+000009d0: 2022 7275 6666 222c 0a20 2020 2020 2020   "ruff",.       
+000009e0: 2022 7079 7465 7374 222c 0a20 2020 2020   "pytest",.     
+000009f0: 2020 2022 7079 7465 7374 2d63 6f76 222c     "pytest-cov",
+00000a00: 0a20 2020 2020 2020 2022 6a75 7079 7465  .        "jupyte
+00000a10: 7222 2c0a 2020 2020 2020 2020 2269 7079  r",.        "ipy
+00000a20: 6d70 6c22 2c0a 2020 2020 2020 2020 2264  mpl",.        "d
+00000a30: 6562 7567 7079 222c 0a20 2020 2020 2020  ebugpy",.       
+00000a40: 2022 7269 6368 222c 0a20 2020 2020 2020   "rich",.       
+00000a50: 2022 6970 7974 686f 6e22 2c0a 2020 2020   "ipython",.    
+00000a60: 2020 2020 2262 6c61 636b 222c 0a20 2020      "black",.   
+00000a70: 2020 2020 2022 6e62 7161 222c 0a20 2020       "nbqa",.   
+00000a80: 2020 2020 2022 7275 6666 222c 0a20 2020       "ruff",.   
+00000a90: 2020 2020 2022 736f 7572 6365 7279 2d63       "sourcery-c
+00000aa0: 6c69 222c 0a20 2020 2020 2020 2022 736e  li",.        "sn
+00000ab0: 616b 6576 697a 222c 0a20 2020 2020 2020  akeviz",.       
+00000ac0: 2022 7072 652d 636f 6d6d 6974 222c 0a20   "pre-commit",. 
+00000ad0: 2020 2020 2020 2022 6b65 7972 696e 6722         "keyring"
+00000ae0: 0a20 2020 2020 205d 0a20 2020 207d 0a20  .      ].    }. 
+00000af0: 205d 0a7d 0a                              ].}.
```

### Comparing `boilercv-0.0.0/repro.txt` & `boilercv-0.0.1/repro.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-# List project dependencies here. A workflow ports them to `pyproject.toml`
-dvc==2.53.0
-imageio==2.27.0
-loguru==0.6.0
-matplotlib==3.7.1
-numpy==1.24.2
-opencv-contrib-python==4.7.0.72
-pandera==0.14.5
-Pillow==9.5.0
-pyarrow==11.0.0
-pydantic==1.10.7
-pyjanitor==0.24.0
-pytz==2023.3
-PyYAML==6.0
-ruamel.yaml==0.17.21
-scikit-image==0.20.0
-scipy==1.10.1
-seaborn==0.12.2
-
-# * extra dependencies shared by pandas and xarray
-# TODO: Revisit pandas `performance` and xarray `accel` extras once numba supports 3.11
-# ? https://github.com/numba/numba/issues/8304
-Bottleneck==1.3.7
-# * pandas and its extra dependencies
-pandas==2.0.0
-# ? Can't specify `performance` extras until Numba supports Python 3.11
-numexpr==2.8.4
-# * pyqtgraph and its extra dependencies
-pyqtgraph==0.13.2
-# ? https://github.com/pyqtgraph/pyqtgraph/issues/2672
-PySide6==6.4.3
-# * xarray and its extra dependencies
-# ? Can't specify `accel` extras until Numba supports Python 3.11
-# ! Install xarray with nodeps until Pandas 2 is allowed
-# TODO: Take xarray out of nodeps when reverting
-# xarray==2023.3.0
-netCDF4==1.6.3
-# ! Once Pandas 2 is allowed, remove these manually-specified deps
-python-dateutil==2.8.2
-## The following requirements were added by pip freeze:
-accessible-pygments==0.0.4
-aiohttp==3.8.4
-aiohttp-retry==2.8.3
-aiosignal==1.3.1
-alabaster==0.7.13
-amqp==5.1.1
-antlr4-python3-runtime==4.9.3
-anyio==3.6.2
-appdirs==1.4.4
-argon2-cffi==21.3.0
-argon2-cffi-bindings==21.2.0
-arrow==1.2.3
-asttokens==2.2.1
-async-timeout==4.0.2
-asyncssh==2.13.1
-atpublic==3.1.1
-attrs==22.2.0
-autopep8==2.0.2
-av==10.0.0
-Babel==2.12.1
-backcall==0.2.0
-beautifulsoup4==4.12.2
-billiard==3.6.4.0
-black==23.3.0
-bleach==6.0.0
-blosc2==2.0.0
-boilercine @ git+https://github.com/blakeNaccarato/boilercine@c2e9a0c18f3b3d06f4d96c2bb5329de287d85f7f
-cachetools==5.3.0
-celery==5.2.7
-certifi==2022.12.7
-cffi==1.15.1
-cfgv==3.3.1
-cftime==1.6.2
-charset-normalizer==3.1.0
-click==8.1.3
-click-didyoumean==0.3.0
-click-plugins==1.1.1
-click-repl==0.2.0
-colorama==0.4.6
-comm==0.1.3
-configobj==5.0.8
-contourpy==1.0.7
-copier==7.0.1
-coverage==7.2.3
-cryptography==40.0.1
-cycler==0.11.0
-Cython==0.29.34
-debugpy==1.6.6
-decorator==5.1.1
-defusedxml==0.7.1
-dictdiffer==0.9.0
-diskcache==5.5.1
-distlib==0.3.6
-distro==1.8.0
-docopt==0.6.2
-docutils==0.19
-dpath==2.1.5
-dulwich==0.21.3
-dunamai==1.16.0
-dvc-data==0.47.1
-dvc-gs==2.22.0
-dvc-http==2.30.2
-dvc-objects==0.21.1
-dvc-render==0.3.1
-dvc-studio-client==0.6.2
-dvc-task==0.2.0
-executing==1.2.0
-fastjsonschema==2.16.3
-filelock==3.11.0
-flatten-dict==0.4.2
-flit==3.8.0
-flit_core==3.8.0
-flufl.lock==7.1.1
-fonttools==4.39.3
-fqdn==1.5.1
-frozenlist==1.3.3
-fsspec==2023.4.0
-funcy==2.0
-gcsfs==2023.4.0
-gitdb==4.0.10
-GitPython==3.1.31
-google-api-core==2.11.0
-google-auth==2.17.3
-google-auth-oauthlib==1.0.0
-google-cloud-core==2.3.2
-google-cloud-storage==2.8.0
-google-crc32c==1.5.0
-google-resumable-media==2.4.1
-googleapis-common-protos==1.59.0
-grandalf==0.8
-hydra-core==1.3.2
-identify==2.5.22
-idna==3.4
-imagesize==1.4.1
-importlib-metadata==6.3.0
-iniconfig==2.0.0
-ipykernel==6.22.0
-ipympl==0.9.3
-ipython==8.12.0
-ipython-genutils==0.2.0
-ipywidgets==8.0.6
-isoduration==20.11.0
-iteration-utilities==0.11.0
-iterative-telemetry==0.0.8
-jaraco.classes==3.2.3
-jedi==0.18.2
-Jinja2==3.1.2
-jinja2-ansible-filters==1.3.2
-jsonpointer==2.3
-jsonschema==4.17.3
-jupyter==1.0.0
-jupyter-console==6.6.3
-jupyter-events==0.6.3
-jupyter_client==8.1.0
-jupyter_core==5.3.0
-jupyter_server==2.5.0
-jupyter_server_terminals==0.4.4
-jupyterlab-pygments==0.2.2
-jupyterlab-widgets==3.0.7
-keyring==23.13.1
-kiwisolver==1.4.4
-kombu==5.2.4
-lazy_loader==0.2
-livereload==2.6.3
-markdown-it-py==2.2.0
-MarkupSafe==2.1.2
-matplotlib-inline==0.1.6
-mdit-py-plugins==0.3.5
-mdurl==0.1.2
-mistune==2.0.5
-more-itertools==9.1.0
-msgpack==1.0.5
-multidict==6.0.4
-multimethod==1.9.1
-multipledispatch==0.6.0
-mypy-extensions==1.0.0
-myst-parser==1.0.0
-nanotime==0.5.2
-natsort==8.3.1
-nbclassic==0.5.5
-nbclient==0.7.3
-nbconvert==7.3.1
-nbformat==5.8.0
-nbqa==1.7.0
-nest-asyncio==1.5.6
-networkx==3.1
-nodeenv==1.7.0
-notebook==6.5.4
-notebook_shim==0.2.2
-oauthlib==3.2.2
-omegaconf==2.3.0
-orjson==3.8.10
-packaging==23.1
-pandas-flavor==0.5.0
-pandocfilters==1.5.0
-parso==0.8.3
-pathspec==0.11.1
-pickleshare==0.7.5
-platformdirs==3.2.0
-pluggy==1.0.0
-plumbum==1.8.1
-pre-commit==3.2.2
-prometheus-client==0.16.0
-prompt-toolkit==3.0.38
-protobuf==4.22.3
-psutil==5.9.4
-pure-eval==0.2.2
-py-cpuinfo==9.0.0
-pyasn1==0.4.8
-pyasn1-modules==0.2.8
-pycine @ git+https://github.com/ottomatic-io/pycine@815cfca06cafc50745a43b2cd0168982225c6dca
-pycodestyle==2.10.0
-pycparser==2.21
-pydata-sphinx-theme==0.13.3
-pydot==1.4.2
-pygit2==1.12.0
-Pygments==2.15.0
-pygtrie==2.5.0
-pyparsing==3.0.9
-pyright==1.1.302
-pyrsistent==0.19.3
-PySide6-Addons==6.4.3
-PySide6-Essentials==6.4.3
-pytest==7.2.2
-pytest-cov==4.0.0
-python-json-logger==2.0.7
-PyWavelets==1.4.1
-pywin32==306
-pywin32-ctypes==0.2.0
-pywinpty==2.0.10
-pyyaml-include==1.3
-pyzmq==25.0.2
-qtconsole==5.4.2
-QtPy==2.3.1
-questionary==1.10.0
-requests==2.28.2
-requests-oauthlib==1.3.1
-rfc3339-validator==0.1.4
-rfc3986-validator==0.1.1
-rich==13.3.3
-rsa==4.9
-ruff==0.0.260
-scmrepo==0.2.1
-Send2Trash==1.8.0
-shiboken6==6.4.3
-shortuuid==1.0.11
-shtab==1.6.1
-six==1.16.0
-smmap==5.0.0
-snakeviz==2.1.1
-sniffio==1.3.0
-snowballstemmer==2.2.0
-soupsieve==2.4
-sourcery-cli==1.1.0
-Sphinx==5.3.0
-sphinx-autobuild==2021.3.14
-sphinx-book-theme==1.0.1
-sphinx_design==0.3.0
-sphinxcontrib-applehelp==1.0.4
-sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.1
-sphinxcontrib-jsmath==1.0.1
-sphinxcontrib-mermaid==0.8.1
-sphinxcontrib-qthelp==1.0.3
-sphinxcontrib-serializinghtml==1.1.5
-sqltrie==0.3.1
-stack-data==0.6.2
-tables==3.8.0
-tabulate==0.9.0
-terminado==0.17.1
-tifffile==2023.4.12
-timecode==1.3.1
-tinycss2==1.2.1
-tokenize-rt==5.0.0
-toml==0.10.2
-tomli==2.0.1
-tomli_w==1.0.0
-tomlkit==0.11.7
-tornado==6.2
-tqdm==4.65.0
-traitlets==5.9.0
-typing-inspect==0.8.0
-typing_extensions==4.5.0
-tzdata==2023.3
-uri-template==1.2.0
-urllib3==1.26.15
-vine==5.0.0
-virtualenv==20.21.0
-voluptuous==0.13.1
-wcwidth==0.2.6
-webcolors==1.13
-webencodings==0.5.1
-websocket-client==1.5.1
-widgetsnbextension==4.0.7
-win32-setctime==1.1.0
-wrapt==1.15.0
-xarray==2023.3.0
-yarl==1.8.2
-zc.lockfile==3.0.post1
-zipp==3.15.0
+# List project dependencies here. A workflow ports them to `pyproject.toml`
+dvc==2.53.0
+imageio==2.27.0
+loguru==0.6.0
+matplotlib==3.7.1
+numpy==1.24.2
+opencv-contrib-python==4.7.0.72
+pandera==0.14.5
+Pillow==9.5.0
+pyarrow==11.0.0
+pydantic==1.10.7
+pyjanitor==0.24.0
+pytz==2023.3
+PyYAML==6.0
+ruamel.yaml==0.17.21
+scikit-image==0.20.0
+scipy==1.10.1
+seaborn==0.12.2
+
+# * extra dependencies shared by pandas and xarray
+# TODO: Revisit pandas `performance` and xarray `accel` extras once numba supports 3.11
+# ? https://github.com/numba/numba/issues/8304
+Bottleneck==1.3.7
+# * pandas and its extra dependencies
+pandas==2.0.0
+# ? Can't specify `performance` extras until Numba supports Python 3.11
+numexpr==2.8.4
+# * pyqtgraph and its extra dependencies
+pyqtgraph==0.13.2
+# ? https://github.com/pyqtgraph/pyqtgraph/issues/2672
+PySide6==6.4.3
+# * xarray and its extra dependencies
+# ? Can't specify `accel` extras until Numba supports Python 3.11
+# ! Install xarray with nodeps until Pandas 2 is allowed
+# TODO: Take xarray out of nodeps when reverting
+# xarray==2023.3.0
+netCDF4==1.6.3
+# ! Once Pandas 2 is allowed, remove these manually-specified deps
+python-dateutil==2.8.2
+## The following requirements were added by pip freeze:
+accessible-pygments==0.0.4
+aiohttp==3.8.4
+aiohttp-retry==2.8.3
+aiosignal==1.3.1
+alabaster==0.7.13
+amqp==5.1.1
+antlr4-python3-runtime==4.9.3
+anyio==3.6.2
+appdirs==1.4.4
+argon2-cffi==21.3.0
+argon2-cffi-bindings==21.2.0
+arrow==1.2.3
+asttokens==2.2.1
+async-timeout==4.0.2
+asyncssh==2.13.1
+atpublic==3.1.1
+attrs==22.2.0
+autopep8==2.0.2
+av==10.0.0
+Babel==2.12.1
+backcall==0.2.0
+beautifulsoup4==4.12.2
+billiard==3.6.4.0
+black==23.3.0
+bleach==6.0.0
+blosc2==2.0.0
+boilercine @ git+https://github.com/blakeNaccarato/boilercine@c2e9a0c18f3b3d06f4d96c2bb5329de287d85f7f
+cachetools==5.3.0
+celery==5.2.7
+certifi==2022.12.7
+cffi==1.15.1
+cfgv==3.3.1
+cftime==1.6.2
+charset-normalizer==3.1.0
+click==8.1.3
+click-didyoumean==0.3.0
+click-plugins==1.1.1
+click-repl==0.2.0
+colorama==0.4.6
+comm==0.1.3
+configobj==5.0.8
+contourpy==1.0.7
+copier==7.0.1
+coverage==7.2.3
+cryptography==40.0.1
+cycler==0.11.0
+Cython==0.29.34
+debugpy==1.6.6
+decorator==5.1.1
+defusedxml==0.7.1
+dictdiffer==0.9.0
+diskcache==5.5.1
+distlib==0.3.6
+distro==1.8.0
+docopt==0.6.2
+docutils==0.19
+dpath==2.1.5
+dulwich==0.21.3
+dunamai==1.16.0
+dvc-data==0.47.1
+dvc-gs==2.22.0
+dvc-http==2.30.2
+dvc-objects==0.21.1
+dvc-render==0.3.1
+dvc-studio-client==0.6.2
+dvc-task==0.2.0
+executing==1.2.0
+fastjsonschema==2.16.3
+filelock==3.11.0
+flatten-dict==0.4.2
+flit==3.8.0
+flit_core==3.8.0
+flufl.lock==7.1.1
+fonttools==4.39.3
+fqdn==1.5.1
+frozenlist==1.3.3
+fsspec==2023.4.0
+funcy==2.0
+gcsfs==2023.4.0
+gitdb==4.0.10
+GitPython==3.1.31
+google-api-core==2.11.0
+google-auth==2.17.3
+google-auth-oauthlib==1.0.0
+google-cloud-core==2.3.2
+google-cloud-storage==2.8.0
+google-crc32c==1.5.0
+google-resumable-media==2.4.1
+googleapis-common-protos==1.59.0
+grandalf==0.8
+hydra-core==1.3.2
+identify==2.5.22
+idna==3.4
+imagesize==1.4.1
+importlib-metadata==6.3.0
+iniconfig==2.0.0
+ipykernel==6.22.0
+ipympl==0.9.3
+ipython==8.12.0
+ipython-genutils==0.2.0
+ipywidgets==8.0.6
+isoduration==20.11.0
+iteration-utilities==0.11.0
+iterative-telemetry==0.0.8
+jaraco.classes==3.2.3
+jedi==0.18.2
+Jinja2==3.1.2
+jinja2-ansible-filters==1.3.2
+jsonpointer==2.3
+jsonschema==4.17.3
+jupyter==1.0.0
+jupyter-console==6.6.3
+jupyter-events==0.6.3
+jupyter_client==8.1.0
+jupyter_core==5.3.0
+jupyter_server==2.5.0
+jupyter_server_terminals==0.4.4
+jupyterlab-pygments==0.2.2
+jupyterlab-widgets==3.0.7
+keyring==23.13.1
+kiwisolver==1.4.4
+kombu==5.2.4
+lazy_loader==0.2
+livereload==2.6.3
+markdown-it-py==2.2.0
+MarkupSafe==2.1.2
+matplotlib-inline==0.1.6
+mdit-py-plugins==0.3.5
+mdurl==0.1.2
+mistune==2.0.5
+more-itertools==9.1.0
+msgpack==1.0.5
+multidict==6.0.4
+multimethod==1.9.1
+multipledispatch==0.6.0
+mypy-extensions==1.0.0
+myst-parser==1.0.0
+nanotime==0.5.2
+natsort==8.3.1
+nbclassic==0.5.5
+nbclient==0.7.3
+nbconvert==7.3.1
+nbformat==5.8.0
+nbqa==1.7.0
+nest-asyncio==1.5.6
+networkx==3.1
+nodeenv==1.7.0
+notebook==6.5.4
+notebook_shim==0.2.2
+oauthlib==3.2.2
+omegaconf==2.3.0
+orjson==3.8.10
+packaging==23.1
+pandas-flavor==0.5.0
+pandocfilters==1.5.0
+parso==0.8.3
+pathspec==0.11.1
+pickleshare==0.7.5
+platformdirs==3.2.0
+pluggy==1.0.0
+plumbum==1.8.1
+pre-commit==3.2.2
+prometheus-client==0.16.0
+prompt-toolkit==3.0.38
+protobuf==4.22.3
+psutil==5.9.4
+pure-eval==0.2.2
+py-cpuinfo==9.0.0
+pyasn1==0.4.8
+pyasn1-modules==0.2.8
+pycine @ git+https://github.com/ottomatic-io/pycine@815cfca06cafc50745a43b2cd0168982225c6dca
+pycodestyle==2.10.0
+pycparser==2.21
+pydata-sphinx-theme==0.13.3
+pydot==1.4.2
+pygit2==1.12.0
+Pygments==2.15.0
+pygtrie==2.5.0
+pyparsing==3.0.9
+pyright==1.1.302
+pyrsistent==0.19.3
+PySide6-Addons==6.4.3
+PySide6-Essentials==6.4.3
+pytest==7.2.2
+pytest-cov==4.0.0
+python-json-logger==2.0.7
+PyWavelets==1.4.1
+pywin32==306
+pywin32-ctypes==0.2.0
+pywinpty==2.0.10
+pyyaml-include==1.3
+pyzmq==25.0.2
+qtconsole==5.4.2
+QtPy==2.3.1
+questionary==1.10.0
+requests==2.28.2
+requests-oauthlib==1.3.1
+rfc3339-validator==0.1.4
+rfc3986-validator==0.1.1
+rich==13.3.3
+rsa==4.9
+ruff==0.0.260
+scmrepo==0.2.1
+Send2Trash==1.8.0
+shiboken6==6.4.3
+shortuuid==1.0.11
+shtab==1.6.1
+six==1.16.0
+smmap==5.0.0
+snakeviz==2.1.1
+sniffio==1.3.0
+snowballstemmer==2.2.0
+soupsieve==2.4
+sourcery-cli==1.1.0
+Sphinx==5.3.0
+sphinx-autobuild==2021.3.14
+sphinx-book-theme==1.0.1
+sphinx_design==0.3.0
+sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-jsmath==1.0.1
+sphinxcontrib-mermaid==0.8.1
+sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-serializinghtml==1.1.5
+sqltrie==0.3.1
+stack-data==0.6.2
+tables==3.8.0
+tabulate==0.9.0
+terminado==0.17.1
+tifffile==2023.4.12
+timecode==1.3.1
+tinycss2==1.2.1
+tokenize-rt==5.0.0
+toml==0.10.2
+tomli==2.0.1
+tomli_w==1.0.0
+tomlkit==0.11.7
+tornado==6.2
+tqdm==4.65.0
+traitlets==5.9.0
+typing-inspect==0.8.0
+typing_extensions==4.5.0
+tzdata==2023.3
+uri-template==1.2.0
+urllib3==1.26.15
+vine==5.0.0
+virtualenv==20.21.0
+voluptuous==0.13.1
+wcwidth==0.2.6
+webcolors==1.13
+webencodings==0.5.1
+websocket-client==1.5.1
+widgetsnbextension==4.0.7
+win32-setctime==1.1.0
+wrapt==1.15.0
+xarray==2023.3.0
+yarl==1.8.2
+zc.lockfile==3.0.post1
+zipp==3.15.0
```

### Comparing `boilercv-0.0.0/setup.ps1` & `boilercv-0.0.1/setup.ps1`

 * *Files identical despite different names*

### Comparing `boilercv-0.0.0/src/boilercv/captivate/previews.py` & `boilercv-0.0.1/src/boilercv/captivate/previews.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,351 +1,351 @@
-"""Image and video previews."""
-
-import inspect
-from collections.abc import Callable, Mapping, MutableSequence, Sequence
-from contextlib import contextmanager
-from pathlib import Path
-from typing import Any, Literal, TypeAlias
-
-import numpy as np
-import pandas as pd
-import pyqtgraph as pg
-import yaml
-from PySide6.QtCore import QEvent, Qt, Signal
-from PySide6.QtGui import QKeyEvent
-from PySide6.QtWidgets import QGridLayout, QHBoxLayout, QLayout, QPushButton
-
-from boilercv import FRAMERATE_CONT
-from boilercv.images import scale_bool
-from boilercv.types import DA, ArrInt, Img
-
-
-def init():
-    """Initialize `boilercv.gui`."""
-    pg.setConfigOption("imageAxisOrder", "row-major")
-
-
-Viewable: TypeAlias = Any  # The true type is a complex union of lots of array types
-NamedViewable: TypeAlias = Mapping[str | int, Viewable]
-MultipleViewable: TypeAlias = Sequence[Viewable]
-MutableViewable: TypeAlias = MutableSequence[Viewable]
-AllViewable: TypeAlias = Viewable | NamedViewable | MultipleViewable
-
-# * -------------------------------------------------------------------------------- * #
-# * IMAGE VIEWER
-
-WINDOW_SIZE = (800, 600)
-WINDOW_NAME = "Image viewer"
-SMALLER_GRIDS = {
-    1: (1, 1),
-    2: (1, 2),
-    3: (1, 3),
-    4: (2, 2),
-    5: (2, 3),
-    6: (2, 3),
-    7: (2, 4),
-    8: (2, 4),
-    9: (2, 5),
-    10: (2, 5),
-    11: (3, 4),
-    12: (3, 4),
-}
-"""Rectangular grid sizes for up to twelve views. Use square grids beyond that."""
-
-
-def view_images(images: AllViewable, name: str = "", framerate: int = FRAMERATE_CONT):
-    """Compare multiple images or videos."""
-    with image_viewer(images, name, framerate):
-        pass
-
-
-@contextmanager
-def image_viewer(images: AllViewable, name: str = "", framerate: int = FRAMERATE_CONT):  # type: ignore  # noqa: C901
-    """View and interact with images and video."""
-
-    images: NamedViewable = coerce_images(images)
-    num_views = len(images)
-    shape = SMALLER_GRIDS.get(num_views, get_square_grid(num_views))
-    height, width = shape
-    coords = get_grid_coordinates(shape)
-    image_views, app, window, layout, button_layout = make_window(name)
-
-    def main():
-        """Handle required setup and teardown."""
-        add_image_views()
-        add_actions()
-        image_view_mapping = set_images(images, image_views)
-        try:
-            yield image_view_mapping, app, window, layout, button_layout
-        finally:
-            window.show()
-            app.exec()
-
-    def add_image_views():
-        """Add image views in a grid."""
-        for column in range(width):
-            layout.setColumnStretch(column, 1)
-        for coord in coords:
-            image_view = get_image_view(framerate)
-            layout.addWidget(image_view, *coord)
-            image_views.append(image_view)
-
-    def add_actions():
-        """Add buttons and keypress events to the window."""
-        window.key_signal.connect(keyPressEvent)
-        layout.addLayout(button_layout, height, 0, 1, width)
-        if num_views > 1:
-            add_button(button_layout, "Toggle Play All", trigger_space).setFocus()
-        add_button(button_layout, "Continue", app.quit)
-
-    def trigger_space():
-        """Trigger a spacebar keypress event. For propagating logic to image views."""
-        keyPressEvent(
-            QKeyEvent(
-                QEvent.Type.KeyPress, Qt.Key.Key_Space, Qt.KeyboardModifier.NoModifier
-            )
-        )
-
-    def keyPressEvent(ev: QKeyEvent):  # noqa: N802
-        """Handle quit events and propagate keypresses to image views."""
-        if ev.key() in (Qt.Key.Key_Escape, Qt.Key.Key_Q, Qt.Key.Key_Enter):
-            app.quit()
-            ev.accept()
-        for image_view in image_views:
-            image_view.keyPressEvent(ev)
-
-    yield from main()
-
-
-# * -------------------------------------------------------------------------------- * #
-
-
-def make_window(name: str = ""):
-    """Start a PyQtGraph app and prepare an app window with a default layout."""
-    # Isolate pg.ImageView in a layout cell. It is complicated to directly modify the UI
-    # of pg.ImageView. Can't use the convenient pg.LayoutWidget because
-    # GraphicsLayoutWidget cannot contain it, and GraphicsLayoutWidget is convenient on
-    # its own.
-    app = pg.mkQApp()
-    image_views: list[pg.ImageView] = []
-    layout = QGridLayout()
-    button_layout = QHBoxLayout()
-    window = GraphicsLayoutWidgetWithKeySignal(size=WINDOW_SIZE)
-    window.setLayout(layout)
-    window.setWindowTitle(f"{WINDOW_NAME}: {name or get_calling_scope_name()}")
-    return image_views, app, window, layout, button_layout
-
-
-def get_grid_coordinates(shape: tuple[int, int]) -> list[tuple[int, int]]:
-    """Get the coordinates of a grid."""
-    (y, x) = np.ones(shape).nonzero()
-    return list(zip(y, x, strict=True))
-
-
-def get_square_grid(num_views: int) -> tuple[int, int]:
-    """Get the dimensions of a square grid for the given number of views."""
-    minimum_side_length = np.ceil(np.sqrt(num_views))
-    side_length = int(minimum_side_length)
-    (height, width) = (side_length,) * 2
-    return height, width
-
-
-def coerce_images(images: AllViewable) -> NamedViewable:
-    """Coerce images to a mapping of title to image."""
-    if isinstance(images, Mapping):
-        images_ = images
-    elif isinstance(images, np.ndarray | DA):
-        images_ = [images]
-    elif isinstance(images, Sequence):
-        # If given a sequence that could be a video or a set of images/videos to
-        # compare, assume it is a video if it is too long to be a set of comparisons.
-        largest_grid = 16
-        if len(images) > largest_grid:
-            images_ = [np.array(pad_images(images))]
-        else:
-            images_ = images
-    else:
-        raise TypeError(f"Unsupported type for images: {type(images)}")
-
-    return (
-        {title: np.array(pad_images(viewable)) for title, viewable in images_.items()}
-        if isinstance(images_, Mapping)
-        else {i: np.array(pad_images(viewable)) for i, viewable in enumerate(images_)}
-    )
-
-
-def pad_images(images: MultipleViewable) -> MutableViewable:  # type: ignore
-    """Pad images to a common size and pack into an array."""
-    flat_image = isinstance(images, np.ndarray | DA) and (
-        # One-channel
-        images.ndim == 2  # type: ignore
-        # Up to four-channel
-        or images.ndim == 3  # type: ignore
-        and images.shape[-1] <= 4  # type: ignore
-    )
-    images: MutableViewable = [images] if flat_image else list(images)
-    shapes = pd.DataFrame(
-        columns=["height", "width"], data=list({image.shape[:2] for image in images})
-    ).set_index(["height", "width"], drop=False)
-    if len(shapes) == 1:
-        return images
-
-    pads = (
-        (shapes[["height", "width"]].max() - shapes[["height", "width"]]) // 2
-    ).set_axis(axis="columns", labels=["hpad", "wpad"])
-    for i, image in enumerate(images):
-        pad: tuple[int, int] = pads.loc[image.shape[:2], :]  # type: ignore
-        hpad, wpad = pad
-        zero_pad_for_additional_dims = ((0, 0),) * (image.ndim - 2)
-        pad_width = ((hpad, hpad), (wpad, wpad), *zero_pad_for_additional_dims)
-        images[i] = np.pad(image, pad_width)
-    return images
-
-
-def set_images(
-    images: NamedViewable, image_views: list[pg.ImageView]
-) -> dict[str | int, pg.ImageView]:
-    """Set images into the image views."""
-    for (title, viewable), image_view in zip(images.items(), image_views, strict=False):
-        if np.issubdtype(viewable.dtype, bool):
-            viewable = scale_bool(viewable)
-        image_view.setImage(viewable.squeeze())
-        if isinstance(title, str):
-            image_view.addItem(pg.TextItem(title, fill=pg.mkBrush("black")))
-    return dict(zip(images.keys(), image_views, strict=False))
-
-
-class GraphicsLayoutWidgetWithKeySignal(pg.GraphicsLayoutWidget):
-    """Emit key signals on `key_signal`."""
-
-    key_signal = Signal(QKeyEvent)
-
-    def keyPressEvent(self, ev: QKeyEvent):  # noqa: N802
-        super().keyPressEvent(ev)
-        self.key_signal.emit(ev)
-
-
-def add_button(layout: QLayout, label: str, func: Callable[..., Any]) -> QPushButton:
-    """Add a named button to a layout and connect it to a callback."""
-    button = QPushButton(label)
-    button.clicked.connect(func)  # type: ignore
-    layout.addWidget(button)
-    return button
-
-
-def get_image_view(framerate: int = FRAMERATE_CONT) -> pg.ImageView:
-    """Get an image view suitable for previewing images."""
-    image_view = pg.ImageView()
-    image_view.playRate = framerate
-    image_view.ui.histogram.hide()
-    image_view.ui.roiBtn.hide()
-    image_view.ui.menuBtn.hide()
-    return image_view
-
-
-def get_calling_scope_name():
-    """Get the name of the calling scope."""
-    current_frame = inspect.currentframe()
-    scope_name = current_frame.f_back.f_code.co_name  # type: ignore
-    while scope_name in {
-        "image_viewer",
-        "view_images",
-        "preview_images",
-        "make_window",
-        "__enter__",
-        "eval_in_context",
-        "evaluate_expression",
-        "_run_with_interrupt_thread",
-        "_run_with_unblock_threads",
-        "new_func",
-        "internal_evaluate_expression_json",
-        "do_it",
-        "process_internal_commands",
-    }:
-        current_frame = current_frame.f_back  # type: ignore
-        scope_name = current_frame.f_back.f_code.co_name  # type: ignore
-    return scope_name
-
-
-# * -------------------------------------------------------------------------------- * #
-
-
-def save_roi(roi_vertices: ArrInt, roi_path: Path):
-    """Save an ROI represented by an ordered array of vertices."""
-    roi_path.write_text(
-        encoding="utf-8", data=yaml.safe_dump(roi_vertices.tolist(), indent=2)
-    )
-
-
-def edit_roi(
-    image: ArrInt, roi_path: Path, roi_type: Literal["poly", "line"] = "poly"
-) -> ArrInt:
-    """Edit the region of interest for an image."""
-
-    with image_viewer(image) as (image_views, _app, window, _layout, button_layout):
-        common_roi_args = dict(
-            pen=pg.mkPen("red"),
-            hoverPen=pg.mkPen("magenta"),
-            handlePen=pg.mkPen("blue"),
-            handleHoverPen=pg.mkPen("magenta"),
-            positions=np.fliplr(load_roi(image, roi_path, roi_type)),
-        )
-        roi = (
-            pg.PolyLineROI(
-                **common_roi_args,
-                closed=True,
-            )
-            if roi_type == "poly"
-            else pg.LineSegmentROI(**common_roi_args)
-        )
-
-        def main():
-            """Allow ROI interaction."""
-            window.key_signal.connect(keyPressEvent)
-            button = QPushButton("Save ROI")
-            button.clicked.connect(save_roi_)  # type: ignore
-            button_layout.addWidget(button)
-            image_views[0].addItem(roi)
-
-        def keyPressEvent(ev: QKeyEvent):  # noqa: N802
-            """Save ROI or quit on key presses."""
-            if ev.key() == Qt.Key.Key_S:
-                save_roi_()
-                ev.accept()
-
-        def save_roi_():
-            """Save the ROI."""
-            vertices = get_roi_vertices()
-            save_roi(vertices, roi_path)
-
-        def get_roi_vertices() -> ArrInt:
-            """Get the vertices of the ROI."""
-            return np.fliplr(np.array(roi.saveState()["points"], dtype=int))
-
-        main()
-
-    return get_roi_vertices()
-
-
-def load_roi(
-    img: Img,
-    roi_path: Path,
-    roi_type: Literal["poly", "line"] = "poly",
-) -> ArrInt:
-    """Load the region of interest for an image."""
-    (width, height) = img.shape[-2:]
-    if roi_path.exists():
-        vertices: list[tuple[int, int]] = yaml.safe_load(
-            roi_path.read_text(encoding="utf-8")
-        )
-    else:
-        vertices = (
-            [(0, 0), (0, width), (height, width), (height, 0)]
-            if roi_type == "poly"
-            else [(0, 0), (height, width)]
-        )
-    return np.array(vertices, dtype=int)
-
-
-# * -------------------------------------------------------------------------------- * #
-
-init()
+"""Image and video previews."""
+
+import inspect
+from collections.abc import Callable, Mapping, MutableSequence, Sequence
+from contextlib import contextmanager
+from pathlib import Path
+from typing import Any, Literal, TypeAlias
+
+import numpy as np
+import pandas as pd
+import pyqtgraph as pg
+import yaml
+from PySide6.QtCore import QEvent, Qt, Signal
+from PySide6.QtGui import QKeyEvent
+from PySide6.QtWidgets import QGridLayout, QHBoxLayout, QLayout, QPushButton
+
+from boilercv import FRAMERATE_CONT
+from boilercv.images import scale_bool
+from boilercv.types import DA, ArrInt, Img
+
+
+def init():
+    """Initialize `boilercv.gui`."""
+    pg.setConfigOption("imageAxisOrder", "row-major")
+
+
+Viewable: TypeAlias = Any  # The true type is a complex union of lots of array types
+NamedViewable: TypeAlias = Mapping[str | int, Viewable]
+MultipleViewable: TypeAlias = Sequence[Viewable]
+MutableViewable: TypeAlias = MutableSequence[Viewable]
+AllViewable: TypeAlias = Viewable | NamedViewable | MultipleViewable
+
+# * -------------------------------------------------------------------------------- * #
+# * IMAGE VIEWER
+
+WINDOW_SIZE = (800, 600)
+WINDOW_NAME = "Image viewer"
+SMALLER_GRIDS = {
+    1: (1, 1),
+    2: (1, 2),
+    3: (1, 3),
+    4: (2, 2),
+    5: (2, 3),
+    6: (2, 3),
+    7: (2, 4),
+    8: (2, 4),
+    9: (2, 5),
+    10: (2, 5),
+    11: (3, 4),
+    12: (3, 4),
+}
+"""Rectangular grid sizes for up to twelve views. Use square grids beyond that."""
+
+
+def view_images(images: AllViewable, name: str = "", framerate: int = FRAMERATE_CONT):
+    """Compare multiple images or videos."""
+    with image_viewer(images, name, framerate):
+        pass
+
+
+@contextmanager
+def image_viewer(images: AllViewable, name: str = "", framerate: int = FRAMERATE_CONT):  # type: ignore  # noqa: C901
+    """View and interact with images and video."""
+
+    images: NamedViewable = coerce_images(images)
+    num_views = len(images)
+    shape = SMALLER_GRIDS.get(num_views, get_square_grid(num_views))
+    height, width = shape
+    coords = get_grid_coordinates(shape)
+    image_views, app, window, layout, button_layout = make_window(name)
+
+    def main():
+        """Handle required setup and teardown."""
+        add_image_views()
+        add_actions()
+        image_view_mapping = set_images(images, image_views)
+        try:
+            yield image_view_mapping, app, window, layout, button_layout
+        finally:
+            window.show()
+            app.exec()
+
+    def add_image_views():
+        """Add image views in a grid."""
+        for column in range(width):
+            layout.setColumnStretch(column, 1)
+        for coord in coords:
+            image_view = get_image_view(framerate)
+            layout.addWidget(image_view, *coord)
+            image_views.append(image_view)
+
+    def add_actions():
+        """Add buttons and keypress events to the window."""
+        window.key_signal.connect(keyPressEvent)
+        layout.addLayout(button_layout, height, 0, 1, width)
+        if num_views > 1:
+            add_button(button_layout, "Toggle Play All", trigger_space).setFocus()
+        add_button(button_layout, "Continue", app.quit)
+
+    def trigger_space():
+        """Trigger a spacebar keypress event. For propagating logic to image views."""
+        keyPressEvent(
+            QKeyEvent(
+                QEvent.Type.KeyPress, Qt.Key.Key_Space, Qt.KeyboardModifier.NoModifier
+            )
+        )
+
+    def keyPressEvent(ev: QKeyEvent):  # noqa: N802
+        """Handle quit events and propagate keypresses to image views."""
+        if ev.key() in (Qt.Key.Key_Escape, Qt.Key.Key_Q, Qt.Key.Key_Enter):
+            app.quit()
+            ev.accept()
+        for image_view in image_views:
+            image_view.keyPressEvent(ev)
+
+    yield from main()
+
+
+# * -------------------------------------------------------------------------------- * #
+
+
+def make_window(name: str = ""):
+    """Start a PyQtGraph app and prepare an app window with a default layout."""
+    # Isolate pg.ImageView in a layout cell. It is complicated to directly modify the UI
+    # of pg.ImageView. Can't use the convenient pg.LayoutWidget because
+    # GraphicsLayoutWidget cannot contain it, and GraphicsLayoutWidget is convenient on
+    # its own.
+    app = pg.mkQApp()
+    image_views: list[pg.ImageView] = []
+    layout = QGridLayout()
+    button_layout = QHBoxLayout()
+    window = GraphicsLayoutWidgetWithKeySignal(size=WINDOW_SIZE)
+    window.setLayout(layout)
+    window.setWindowTitle(f"{WINDOW_NAME}: {name or get_calling_scope_name()}")
+    return image_views, app, window, layout, button_layout
+
+
+def get_grid_coordinates(shape: tuple[int, int]) -> list[tuple[int, int]]:
+    """Get the coordinates of a grid."""
+    (y, x) = np.ones(shape).nonzero()
+    return list(zip(y, x, strict=True))
+
+
+def get_square_grid(num_views: int) -> tuple[int, int]:
+    """Get the dimensions of a square grid for the given number of views."""
+    minimum_side_length = np.ceil(np.sqrt(num_views))
+    side_length = int(minimum_side_length)
+    (height, width) = (side_length,) * 2
+    return height, width
+
+
+def coerce_images(images: AllViewable) -> NamedViewable:
+    """Coerce images to a mapping of title to image."""
+    if isinstance(images, Mapping):
+        images_ = images
+    elif isinstance(images, np.ndarray | DA):
+        images_ = [images]
+    elif isinstance(images, Sequence):
+        # If given a sequence that could be a video or a set of images/videos to
+        # compare, assume it is a video if it is too long to be a set of comparisons.
+        largest_grid = 16
+        if len(images) > largest_grid:
+            images_ = [np.array(pad_images(images))]
+        else:
+            images_ = images
+    else:
+        raise TypeError(f"Unsupported type for images: {type(images)}")
+
+    return (
+        {title: np.array(pad_images(viewable)) for title, viewable in images_.items()}
+        if isinstance(images_, Mapping)
+        else {i: np.array(pad_images(viewable)) for i, viewable in enumerate(images_)}
+    )
+
+
+def pad_images(images: MultipleViewable) -> MutableViewable:  # type: ignore
+    """Pad images to a common size and pack into an array."""
+    flat_image = isinstance(images, np.ndarray | DA) and (
+        # One-channel
+        images.ndim == 2  # type: ignore  # CI
+        # Up to four-channel
+        or images.ndim == 3  # type: ignore  # CI
+        and images.shape[-1] <= 4  # type: ignore  # CI
+    )
+    images: MutableViewable = [images] if flat_image else list(images)
+    shapes = pd.DataFrame(
+        columns=["height", "width"], data=list({image.shape[:2] for image in images})
+    ).set_index(["height", "width"], drop=False)
+    if len(shapes) == 1:
+        return images
+
+    pads = (
+        (shapes[["height", "width"]].max() - shapes[["height", "width"]]) // 2
+    ).set_axis(axis="columns", labels=["hpad", "wpad"])
+    for i, image in enumerate(images):
+        pad: tuple[int, int] = pads.loc[image.shape[:2], :]  # type: ignore
+        hpad, wpad = pad
+        zero_pad_for_additional_dims = ((0, 0),) * (image.ndim - 2)
+        pad_width = ((hpad, hpad), (wpad, wpad), *zero_pad_for_additional_dims)
+        images[i] = np.pad(image, pad_width)
+    return images
+
+
+def set_images(
+    images: NamedViewable, image_views: list[pg.ImageView]
+) -> dict[str | int, pg.ImageView]:
+    """Set images into the image views."""
+    for (title, viewable), image_view in zip(images.items(), image_views, strict=False):
+        if np.issubdtype(viewable.dtype, bool):
+            viewable = scale_bool(viewable)
+        image_view.setImage(viewable.squeeze())
+        if isinstance(title, str):
+            image_view.addItem(pg.TextItem(title, fill=pg.mkBrush("black")))
+    return dict(zip(images.keys(), image_views, strict=False))
+
+
+class GraphicsLayoutWidgetWithKeySignal(pg.GraphicsLayoutWidget):
+    """Emit key signals on `key_signal`."""
+
+    key_signal = Signal(QKeyEvent)
+
+    def keyPressEvent(self, ev: QKeyEvent):  # noqa: N802
+        super().keyPressEvent(ev)
+        self.key_signal.emit(ev)
+
+
+def add_button(layout: QLayout, label: str, func: Callable[..., Any]) -> QPushButton:
+    """Add a named button to a layout and connect it to a callback."""
+    button = QPushButton(label)
+    button.clicked.connect(func)
+    layout.addWidget(button)
+    return button
+
+
+def get_image_view(framerate: int = FRAMERATE_CONT) -> pg.ImageView:
+    """Get an image view suitable for previewing images."""
+    image_view = pg.ImageView()
+    image_view.playRate = framerate
+    image_view.ui.histogram.hide()
+    image_view.ui.roiBtn.hide()
+    image_view.ui.menuBtn.hide()
+    return image_view
+
+
+def get_calling_scope_name():
+    """Get the name of the calling scope."""
+    current_frame = inspect.currentframe()
+    scope_name = current_frame.f_back.f_code.co_name  # type: ignore
+    while scope_name in {
+        "image_viewer",
+        "view_images",
+        "preview_images",
+        "make_window",
+        "__enter__",
+        "eval_in_context",
+        "evaluate_expression",
+        "_run_with_interrupt_thread",
+        "_run_with_unblock_threads",
+        "new_func",
+        "internal_evaluate_expression_json",
+        "do_it",
+        "process_internal_commands",
+    }:
+        current_frame = current_frame.f_back  # type: ignore
+        scope_name = current_frame.f_back.f_code.co_name  # type: ignore
+    return scope_name
+
+
+# * -------------------------------------------------------------------------------- * #
+
+
+def save_roi(roi_vertices: ArrInt, roi_path: Path):
+    """Save an ROI represented by an ordered array of vertices."""
+    roi_path.write_text(
+        encoding="utf-8", data=yaml.safe_dump(roi_vertices.tolist(), indent=2)
+    )
+
+
+def edit_roi(
+    image: ArrInt, roi_path: Path, roi_type: Literal["poly", "line"] = "poly"
+) -> ArrInt:
+    """Edit the region of interest for an image."""
+
+    with image_viewer(image) as (image_views, _app, window, _layout, button_layout):
+        common_roi_args = dict(
+            pen=pg.mkPen("red"),
+            hoverPen=pg.mkPen("magenta"),
+            handlePen=pg.mkPen("blue"),
+            handleHoverPen=pg.mkPen("magenta"),
+            positions=np.fliplr(load_roi(image, roi_path, roi_type)),
+        )
+        roi = (
+            pg.PolyLineROI(
+                **common_roi_args,
+                closed=True,
+            )
+            if roi_type == "poly"
+            else pg.LineSegmentROI(**common_roi_args)
+        )
+
+        def main():
+            """Allow ROI interaction."""
+            window.key_signal.connect(keyPressEvent)
+            button = QPushButton("Save ROI")
+            button.clicked.connect(save_roi_)
+            button_layout.addWidget(button)
+            image_views[0].addItem(roi)
+
+        def keyPressEvent(ev: QKeyEvent):  # noqa: N802
+            """Save ROI or quit on key presses."""
+            if ev.key() == Qt.Key.Key_S:
+                save_roi_()
+                ev.accept()
+
+        def save_roi_():
+            """Save the ROI."""
+            vertices = get_roi_vertices()
+            save_roi(vertices, roi_path)
+
+        def get_roi_vertices() -> ArrInt:
+            """Get the vertices of the ROI."""
+            return np.fliplr(np.array(roi.saveState()["points"], dtype=int))
+
+        main()
+
+    return get_roi_vertices()
+
+
+def load_roi(
+    img: Img,
+    roi_path: Path,
+    roi_type: Literal["poly", "line"] = "poly",
+) -> ArrInt:
+    """Load the region of interest for an image."""
+    (width, height) = img.shape[-2:]
+    if roi_path.exists():
+        vertices: list[tuple[int, int]] = yaml.safe_load(
+            roi_path.read_text(encoding="utf-8")
+        )
+    else:
+        vertices = (
+            [(0, 0), (0, width), (height, width), (height, 0)]
+            if roi_type == "poly"
+            else [(0, 0), (height, width)]
+        )
+    return np.array(vertices, dtype=int)
+
+
+# * -------------------------------------------------------------------------------- * #
+
+init()
```

### Comparing `boilercv-0.0.0/src/boilercv/data/__init__.py` & `boilercv-0.0.1/src/boilercv/data/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-"""Tools for datasets."""
-
-from collections.abc import Callable, Sequence
-from itertools import chain
-from typing import Any
-
-import numpy as np
-import pandas as pd
-import xarray as xr
-from pytz import timezone
-
-from boilercv.data.models import Dimension, get_dims
-from boilercv.types import DA, DS, ArrLike
-
-VIDEO = "video"
-ROI = "roi"
-HEADER = "header"
-TIMEZONE = timezone("US/Pacific")
-
-FRAME = "frame"
-TIME = "time"
-UTC_TIME = "utc"
-
-Y = "y"
-X = "x"
-YX = ["y", "x"]
-
-PX = "px"
-YPX = f"{Y}{PX}"
-XPX = f"{X}{PX}"
-YX_PX = [YPX, XPX]
-
-DIMS = [FRAME, YPX, XPX]
-
-PACKED_DIM_INDEX = 2
-PACKED = "packed"
-XPX_PACKED = "xpx_packed"
-PACKED_DIMS = [FRAME, YPX, XPX_PACKED]
-
-VIDEO_NAME = "video_name"
-
-LENGTH = "um"
-SAMPLE_DIAMETER_UM = 9_525_000
-ROI = "roi"
-OTHER_ROI = "roi_other"
-
-IDX = pd.IndexSlice
-"""Helper for slicing multi-index dataframes."""
-
-
-def identity_da(da: DA, dim: str) -> DA:
-    """Construct a data array that maps a dimension's coordinates to itself.
-
-    Useful to apply `xr.apply_ufunc` along coordinate values.
-
-    Args:
-        da: Data array.
-        dim: The dimension to extract.
-    """
-    return xr.DataArray(
-        dims=(dim),
-        coords={dim: da[dim].values},
-        data=da[dim],
-    )
-
-
-def apply_to_img_da(
-    func: Callable[..., Any],
-    *args: Any,
-    returns: int | None = 1,
-    vectorize: bool = False,
-    name: Sequence[str] | str = "",
-    kwargs: dict[str, Any] | None = None,
-) -> Any:
-    """Apply functions that transform images to transform data arrays instead."""
-    core_dims = [YX_PX]
-    common_kwargs = dict(
-        input_core_dims=core_dims * len(args),
-        vectorize=vectorize,
-        keep_attrs=True,
-        kwargs=kwargs,
-    )
-    if returns and returns > 0:
-        result = xr.apply_ufunc(
-            func,
-            *args,
-            **common_kwargs,
-            output_core_dims=core_dims * returns,
-        )
-        if name and returns == 1:
-            result = result.rename(name)
-        if name and returns > 1:
-            result = tuple(
-                part.rename(name_) for name_, part in zip(name, result, strict=True)
-            )
-        return result
-    if not returns or returns == 0:
-        xr.apply_ufunc(
-            func,
-            *args,
-            **common_kwargs,
-        )
-
-
-def assign_ds(
-    name: str,
-    data: ArrLike,
-    dims: Sequence[Dimension],
-    secondary_dims: Sequence[Dimension] = (),
-    fixed_dims: Sequence[Dimension] = (),
-    fixed_secondary_dims: Sequence[Dimension] = (),
-    ds: DS | None = None,
-    long_name: str = "",
-    units: str = "",
-) -> DS:
-    """Build a data array and assign it to a dataset."""
-    if not ds:
-        ds = xr.Dataset()
-    da = build_da(
-        name,
-        data,
-        dims,
-        secondary_dims,
-        fixed_dims,
-        fixed_secondary_dims,
-        long_name,
-        units,
-    )
-    ds[name] = da
-    return ds
-
-
-def build_da(
-    name: str,
-    data: ArrLike,
-    dims: Sequence[Dimension],
-    secondary_dims: Sequence[Dimension] = (),
-    fixed_dims: Sequence[Dimension] = (),
-    fixed_secondary_dims: Sequence[Dimension] = (),
-    long_name: str = "",
-    units: str = "",
-):
-    """Build a data array."""
-    all_primary_dims = chain(fixed_dims, dims)
-    all_fixed_dims = chain(fixed_dims, fixed_secondary_dims)
-    all_variable_dims = chain(dims, secondary_dims)
-    if not long_name:
-        long_name = name.capitalize() if len(name) > 1 else name
-    if isinstance(data, Sequence) and not len(data):
-        shape: list[int] = []
-        for dim in all_primary_dims:
-            if dim.coords is None:
-                shape.append(1)
-            else:
-                shape.append(len(dim.coords))
-        data = np.full(shape, None)
-    attrs = {"long_name": long_name}
-    if units:
-        attrs["units"] = units
-    da = xr.DataArray(
-        name=name,
-        dims=get_dims(*all_primary_dims),
-        data=data,
-        attrs=attrs,
-    )
-    for dim in chain(all_fixed_dims, all_variable_dims):
-        da = dim.assign_to(da)
-    return da
+"""Tools for datasets."""
+
+from collections.abc import Callable, Sequence
+from itertools import chain
+from typing import Any
+
+import numpy as np
+import pandas as pd
+import xarray as xr
+from pytz import timezone
+
+from boilercv.data.models import Dimension, get_dims
+from boilercv.types import DA, DS, ArrLike
+
+VIDEO = "video"
+ROI = "roi"
+HEADER = "header"
+TIMEZONE = timezone("US/Pacific")
+
+FRAME = "frame"
+TIME = "time"
+UTC_TIME = "utc"
+
+Y = "y"
+X = "x"
+YX = ["y", "x"]
+
+PX = "px"
+YPX = f"{Y}{PX}"
+XPX = f"{X}{PX}"
+YX_PX = [YPX, XPX]
+
+DIMS = [FRAME, YPX, XPX]
+
+PACKED_DIM_INDEX = 2
+PACKED = "packed"
+XPX_PACKED = "xpx_packed"
+PACKED_DIMS = [FRAME, YPX, XPX_PACKED]
+
+VIDEO_NAME = "video_name"
+
+LENGTH = "um"
+SAMPLE_DIAMETER_UM = 9_525_000
+ROI = "roi"
+OTHER_ROI = "roi_other"
+
+IDX = pd.IndexSlice
+"""Helper for slicing multi-index dataframes."""
+
+
+def identity_da(da: DA, dim: str) -> DA:
+    """Construct a data array that maps a dimension's coordinates to itself.
+
+    Useful to apply `xr.apply_ufunc` along coordinate values.
+
+    Args:
+        da: Data array.
+        dim: The dimension to extract.
+    """
+    return xr.DataArray(
+        dims=(dim),
+        coords={dim: da[dim].values},
+        data=da[dim],
+    )
+
+
+def apply_to_img_da(
+    func: Callable[..., Any],
+    *args: Any,
+    returns: int | None = 1,
+    vectorize: bool = False,
+    name: Sequence[str] | str = "",
+    kwargs: dict[str, Any] | None = None,
+) -> Any:
+    """Apply functions that transform images to transform data arrays instead."""
+    core_dims = [YX_PX]
+    common_kwargs = dict(
+        input_core_dims=core_dims * len(args),
+        vectorize=vectorize,
+        keep_attrs=True,
+        kwargs=kwargs,
+    )
+    if returns and returns > 0:
+        result = xr.apply_ufunc(
+            func,
+            *args,
+            **common_kwargs,
+            output_core_dims=core_dims * returns,
+        )
+        if name and returns == 1:
+            result = result.rename(name)
+        if name and returns > 1:
+            result = tuple(
+                part.rename(name_) for name_, part in zip(name, result, strict=True)
+            )
+        return result
+    if not returns or returns == 0:
+        xr.apply_ufunc(
+            func,
+            *args,
+            **common_kwargs,
+        )
+
+
+def assign_ds(
+    name: str,
+    data: ArrLike,
+    dims: Sequence[Dimension],
+    secondary_dims: Sequence[Dimension] = (),
+    fixed_dims: Sequence[Dimension] = (),
+    fixed_secondary_dims: Sequence[Dimension] = (),
+    ds: DS | None = None,
+    long_name: str = "",
+    units: str = "",
+) -> DS:
+    """Build a data array and assign it to a dataset."""
+    if not ds:
+        ds = xr.Dataset()
+    da = build_da(
+        name,
+        data,
+        dims,
+        secondary_dims,
+        fixed_dims,
+        fixed_secondary_dims,
+        long_name,
+        units,
+    )
+    ds[name] = da
+    return ds
+
+
+def build_da(
+    name: str,
+    data: ArrLike,
+    dims: Sequence[Dimension],
+    secondary_dims: Sequence[Dimension] = (),
+    fixed_dims: Sequence[Dimension] = (),
+    fixed_secondary_dims: Sequence[Dimension] = (),
+    long_name: str = "",
+    units: str = "",
+):
+    """Build a data array."""
+    all_primary_dims = chain(fixed_dims, dims)
+    all_fixed_dims = chain(fixed_dims, fixed_secondary_dims)
+    all_variable_dims = chain(dims, secondary_dims)
+    if not long_name:
+        long_name = name.capitalize() if len(name) > 1 else name
+    if isinstance(data, Sequence) and not len(data):
+        shape: list[int] = []
+        for dim in all_primary_dims:
+            if dim.coords is None:
+                shape.append(1)
+            else:
+                shape.append(len(dim.coords))
+        data = np.full(shape, None)
+    attrs = {"long_name": long_name}
+    if units:
+        attrs["units"] = units
+    da = xr.DataArray(
+        name=name,
+        dims=get_dims(*all_primary_dims),
+        data=data,
+        attrs=attrs,
+    )
+    for dim in chain(all_fixed_dims, all_variable_dims):
+        da = dim.assign_to(da)
+    return da
```

### Comparing `boilercv-0.0.0/src/boilercv/data/frames.py` & `boilercv-0.0.1/src/boilercv/data/frames.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""Dataframes."""
-
-import numpy as np
-import pandas as pd
-
-from boilercv.data import YX_PX
-from boilercv.types import DF, ArrLike
-
-
-def df_points(points: ArrLike, dims=YX_PX) -> DF:
-    """Build a dataframe from an array of points."""
-    return (
-        pd.DataFrame(
-            columns=dims,
-            data=points,  # type: ignore
-        )
-        .rename_axis(axis="index", mapper="point")
-        .rename_axis(axis="columns", mapper="dim")
-    )
-
-
-def frame_lines(lines: ArrLike) -> DF:
-    """Build a dataframe from an array of line segments."""
-    ordered_pairs = [df_points(point) for point in np.split(lines, 2, axis=1)]
-    return (
-        pd.concat(axis="columns", keys=[0, 1], objs=ordered_pairs)
-        .rename_axis(axis="index", mapper="line")
-        .rename_axis(axis="columns", mapper=["coord", "dim"])
-        .reorder_levels(axis="columns", order=["dim", "coord"])
-    )
+"""Dataframes."""
+
+import numpy as np
+import pandas as pd
+
+from boilercv.data import YX_PX
+from boilercv.types import DF, ArrLike
+
+
+def df_points(points: ArrLike, dims=YX_PX) -> DF:
+    """Build a dataframe from an array of points."""
+    return (
+        pd.DataFrame(
+            columns=dims,
+            data=points,  # type: ignore
+        )
+        .rename_axis(axis="index", mapper="point")
+        .rename_axis(axis="columns", mapper="dim")
+    )
+
+
+def frame_lines(lines: ArrLike) -> DF:
+    """Build a dataframe from an array of line segments."""
+    ordered_pairs = [df_points(point) for point in np.split(lines, 2, axis=1)]
+    return (
+        pd.concat(axis="columns", keys=[0, 1], objs=ordered_pairs)
+        .rename_axis(axis="index", mapper="line")
+        .rename_axis(axis="columns", mapper=["coord", "dim"])
+        .reorder_levels(axis="columns", order=["dim", "coord"])
+    )
```

### Comparing `boilercv-0.0.0/src/boilercv/data/models.py` & `boilercv-0.0.1/src/boilercv/data/models.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-"""Models for image processing."""
-
-from dataclasses import dataclass
-from typing import Any
-
-from boilercv.types import DA, SupportsMul
-
-
-@dataclass
-class Dimension:
-    """A dimension.
-
-    Args:
-        dim: Dimension.
-        long_name: Long name.
-        coords: Coordinate values.
-        units: Units.
-        original_units: Original units to be converted from.
-        original_coords: Original coordinate values to be converted from.
-        scale: Scale factor to multiply the original coordinates by.
-        parent_dim: Existing dimension to associate this dimension with.
-    """
-
-    dim: str
-    """Dimension."""
-    long_name: str = ""
-    """Long name."""
-    coords: Any = None
-    """Coordinate values."""
-    units: str = ""
-    """Units."""
-    original_units: str = ""
-    """Original units to be converted from."""
-    original_coords: SupportsMul | None = None
-    """Original coordinate values to be converted from."""
-    scale: float = 1
-    """Scale factor to multiply the original coordinates by."""
-    parent_dim: str = ""
-    """Existing dimension to associate this dimension with."""
-
-    @property
-    def coordinate_units_match(self):
-        """Whether the coordinate units are in the desired units."""
-        return self.original_units == self.units
-
-    def __post_init__(self):
-        """Assign original units and long name if not specified."""
-        if self.units and not self.original_units:
-            self.original_units = self.units
-        if not self.long_name:
-            self.long_name = self.dim.capitalize() if len(self.dim) > 1 else self.dim
-        if not self.parent_dim:
-            self.parent_dim = self.dim
-
-    def assign_to(self, da: DA) -> DA:
-        """Assign this dimension and its coordinates."""
-        if self.coords is None and self.dim == self.parent_dim:
-            self.coords = da[self.parent_dim].values
-        if not self.coordinate_units_match:
-            self.convert()
-        if self.coords is not None:
-            da = da.assign_coords({self.dim: (self.parent_dim, self.coords)})
-        attrs = {"long_name": self.long_name}
-        if self.units:
-            attrs["units"] = self.units
-        da[self.dim] = da[self.dim].assign_attrs(attrs)
-        return da
-
-    def convert(self):
-        """Convert the original coordinates to the desired units."""
-        if self.original_coords is not None:
-            self.coords = self.original_coords * self.scale
-        self.original_units = self.units
-        self.original_coords = self.coords
-
-
-def get_dims(*dims: Dimension) -> tuple[str, ...]:
-    """Get a tuple of dimension names representing these dimensions."""
-    return tuple(dim.dim for dim in dims)
+"""Models for image processing."""
+
+from dataclasses import dataclass
+from typing import Any
+
+from boilercv.types import DA, SupportsMul
+
+
+@dataclass
+class Dimension:
+    """A dimension.
+
+    Args:
+        dim: Dimension.
+        long_name: Long name.
+        coords: Coordinate values.
+        units: Units.
+        original_units: Original units to be converted from.
+        original_coords: Original coordinate values to be converted from.
+        scale: Scale factor to multiply the original coordinates by.
+        parent_dim: Existing dimension to associate this dimension with.
+    """
+
+    dim: str
+    """Dimension."""
+    long_name: str = ""
+    """Long name."""
+    coords: Any = None
+    """Coordinate values."""
+    units: str = ""
+    """Units."""
+    original_units: str = ""
+    """Original units to be converted from."""
+    original_coords: SupportsMul | None = None
+    """Original coordinate values to be converted from."""
+    scale: float = 1
+    """Scale factor to multiply the original coordinates by."""
+    parent_dim: str = ""
+    """Existing dimension to associate this dimension with."""
+
+    @property
+    def coordinate_units_match(self):
+        """Whether the coordinate units are in the desired units."""
+        return self.original_units == self.units
+
+    def __post_init__(self):
+        """Assign original units and long name if not specified."""
+        if self.units and not self.original_units:
+            self.original_units = self.units
+        if not self.long_name:
+            self.long_name = self.dim.capitalize() if len(self.dim) > 1 else self.dim
+        if not self.parent_dim:
+            self.parent_dim = self.dim
+
+    def assign_to(self, da: DA) -> DA:
+        """Assign this dimension and its coordinates."""
+        if self.coords is None and self.dim == self.parent_dim:
+            self.coords = da[self.parent_dim].values
+        if not self.coordinate_units_match:
+            self.convert()
+        if self.coords is not None:
+            da = da.assign_coords({self.dim: (self.parent_dim, self.coords)})
+        attrs = {"long_name": self.long_name}
+        if self.units:
+            attrs["units"] = self.units
+        da[self.dim] = da[self.dim].assign_attrs(attrs)
+        return da
+
+    def convert(self):
+        """Convert the original coordinates to the desired units."""
+        if self.original_coords is not None:
+            self.coords = self.original_coords * self.scale
+        self.original_units = self.units
+        self.original_coords = self.coords
+
+
+def get_dims(*dims: Dimension) -> tuple[str, ...]:
+    """Get a tuple of dimension names representing these dimensions."""
+    return tuple(dim.dim for dim in dims)
```

### Comparing `boilercv-0.0.0/src/boilercv/data/video.py` & `boilercv-0.0.1/src/boilercv/data/video.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-"""Video dataset model."""
-
-from dataclasses import asdict
-from pathlib import Path
-
-import xarray as xr
-from boilercine import get_cine_attributes, get_cine_images
-from scipy.spatial.distance import euclidean
-
-from boilercv.captivate.previews import load_roi
-from boilercv.data import (
-    FRAME,
-    HEADER,
-    LENGTH,
-    SAMPLE_DIAMETER_UM,
-    TIME,
-    TIMEZONE,
-    UTC_TIME,
-    VIDEO,
-    XPX,
-    YPX,
-    YX,
-    assign_ds,
-)
-from boilercv.data.models import Dimension
-from boilercv.models.params import PARAMS
-from boilercv.types import DA, DS
-
-
-def prepare_dataset(
-    cine_source: Path, num_frames: int | None = None, start_frame: int = 0
-) -> DS:
-    """Prepare a dataset from a CINE."""
-
-    # Header
-    header, utc_arr = get_cine_attributes(
-        cine_source, TIMEZONE, num_frames, start_frame
-    )
-    header_da = xr.DataArray(name=HEADER, attrs=asdict(header))
-
-    # Dimensions
-    frame_dim = Dimension(
-        dim=FRAME,
-        long_name="Frame number",
-    )
-    time = Dimension(
-        parent_dim=frame_dim.dim,
-        dim=TIME,
-        long_name="Time elapsed",
-        units="s",
-        original_units="ns",
-        original_coords=(utc_arr - utc_arr[0]).astype(float),
-        scale=1e-9,
-    )
-    utc = Dimension(
-        parent_dim=frame_dim.dim,
-        dim=UTC_TIME,
-        long_name="UTC time",
-        coords=utc_arr,
-    )
-
-    # Dataset
-    ds = assign_ds(
-        name=VIDEO,
-        long_name="High-speed video data",
-        units="Pixel intensity",
-        fixed_dims=(frame_dim,),
-        dims=(
-            Dimension(
-                dim=YPX,
-                long_name="Height",
-                units="px",
-            ),
-            Dimension(
-                dim=XPX,
-                long_name="Width",
-                units="px",
-            ),
-        ),
-        fixed_secondary_dims=(time, utc),
-        data=list(get_cine_images(cine_source, num_frames, start_frame)),
-    )
-    ds[header_da.name] = header_da
-    return ds
-
-
-# * -------------------------------------------------------------------------------- * #
-# * SECONDARY LENGTH DIMENSIONS
-
-
-def assign_length_dims(dataset: DS) -> DS:
-    """Assign length scales to "x" and "y" coordinates."""
-    images = dataset[VIDEO]
-    parent_dim_units = "px"
-    roi = load_roi(images.data, PARAMS.paths.examples / "roi_line.yaml", "line")
-    pixels = euclidean(*iter(roi))
-    um_per_px = SAMPLE_DIAMETER_UM / pixels
-    y = get_length_dims(parent_dim_units, YX[0], "Height", um_per_px, images)
-    x = get_length_dims(parent_dim_units, YX[1], "Width", um_per_px, images)
-    images = y.assign_to(images)
-    images = x.assign_to(images)
-    return dataset
-
-
-def get_length_dims(
-    parent_dim_units: str, dim: str, long_name: str, scale: float, images: DA
-) -> Dimension:
-    """Get a length scale."""
-    parent_dim = f"{dim}{parent_dim_units}"
-    return Dimension(
-        parent_dim=f"{dim}{parent_dim_units}",
-        dim=dim,
-        long_name=long_name,
-        units=LENGTH,
-        original_units=parent_dim_units,
-        original_coords=images[parent_dim].values,
-        scale=scale,
-    )
+"""Video dataset model."""
+
+from dataclasses import asdict
+from pathlib import Path
+
+import xarray as xr
+from boilercine import get_cine_attributes, get_cine_images
+from scipy.spatial.distance import euclidean
+
+from boilercv.captivate.previews import load_roi
+from boilercv.data import (
+    FRAME,
+    HEADER,
+    LENGTH,
+    SAMPLE_DIAMETER_UM,
+    TIME,
+    TIMEZONE,
+    UTC_TIME,
+    VIDEO,
+    XPX,
+    YPX,
+    YX,
+    assign_ds,
+)
+from boilercv.data.models import Dimension
+from boilercv.models.params import PARAMS
+from boilercv.types import DA, DS
+
+
+def prepare_dataset(
+    cine_source: Path, num_frames: int | None = None, start_frame: int = 0
+) -> DS:
+    """Prepare a dataset from a CINE."""
+
+    # Header
+    header, utc_arr = get_cine_attributes(
+        cine_source, TIMEZONE, num_frames, start_frame
+    )
+    header_da = xr.DataArray(name=HEADER, attrs=asdict(header))
+
+    # Dimensions
+    frame_dim = Dimension(
+        dim=FRAME,
+        long_name="Frame number",
+    )
+    time = Dimension(
+        parent_dim=frame_dim.dim,
+        dim=TIME,
+        long_name="Time elapsed",
+        units="s",
+        original_units="ns",
+        original_coords=(utc_arr - utc_arr[0]).astype(float),
+        scale=1e-9,
+    )
+    utc = Dimension(
+        parent_dim=frame_dim.dim,
+        dim=UTC_TIME,
+        long_name="UTC time",
+        coords=utc_arr,
+    )
+
+    # Dataset
+    ds = assign_ds(
+        name=VIDEO,
+        long_name="High-speed video data",
+        units="Pixel intensity",
+        fixed_dims=(frame_dim,),
+        dims=(
+            Dimension(
+                dim=YPX,
+                long_name="Height",
+                units="px",
+            ),
+            Dimension(
+                dim=XPX,
+                long_name="Width",
+                units="px",
+            ),
+        ),
+        fixed_secondary_dims=(time, utc),
+        data=list(get_cine_images(cine_source, num_frames, start_frame)),
+    )
+    ds[header_da.name] = header_da
+    return ds
+
+
+# * -------------------------------------------------------------------------------- * #
+# * SECONDARY LENGTH DIMENSIONS
+
+
+def assign_length_dims(dataset: DS) -> DS:
+    """Assign length scales to "x" and "y" coordinates."""
+    images = dataset[VIDEO]
+    parent_dim_units = "px"
+    roi = load_roi(images.data, PARAMS.paths.examples / "roi_line.yaml", "line")
+    pixels = euclidean(*iter(roi))
+    um_per_px = SAMPLE_DIAMETER_UM / pixels
+    y = get_length_dims(parent_dim_units, YX[0], "Height", um_per_px, images)
+    x = get_length_dims(parent_dim_units, YX[1], "Width", um_per_px, images)
+    images = y.assign_to(images)
+    images = x.assign_to(images)
+    return dataset
+
+
+def get_length_dims(
+    parent_dim_units: str, dim: str, long_name: str, scale: float, images: DA
+) -> Dimension:
+    """Get a length scale."""
+    parent_dim = f"{dim}{parent_dim_units}"
+    return Dimension(
+        parent_dim=f"{dim}{parent_dim_units}",
+        dim=dim,
+        long_name=long_name,
+        units=LENGTH,
+        original_units=parent_dim_units,
+        original_coords=images[parent_dim].values,
+        scale=scale,
+    )
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/__init__.py` & `boilercv-0.0.1/src/boilercv/examples/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Examples, experiments, and demonstrations."""
-
-import xarray as xr
-
-from boilercv.data import VIDEO
-from boilercv.models.params import PARAMS
-from boilercv.types import DA
-
-EXAMPLE_NUM_FRAMES = 1000
-EXAMPLE_VIDEO_NAME = "2022-11-30T13-41-00"
-EXAMPLE_CONTOURS = PARAMS.paths.examples / f"{EXAMPLE_VIDEO_NAME}.h5"
-# TODO: Source the ROI from the dataset.
-EXAMPLE_ROI = PARAMS.paths.examples / f"{EXAMPLE_VIDEO_NAME}_roi.yaml"
-
-
-def get_images() -> DA:
-    with xr.open_dataset(PARAMS.paths.examples / f"{EXAMPLE_VIDEO_NAME}.nc") as ds:
-        return ds[VIDEO].sel(frame=slice(None, EXAMPLE_NUM_FRAMES))
-
-
-EXAMPLE_VIDEO = get_images()
-EXAMPLE_FRAME_LIST = list(EXAMPLE_VIDEO.values)
+"""Examples, experiments, and demonstrations."""
+
+import xarray as xr
+
+from boilercv.data import VIDEO
+from boilercv.models.params import PARAMS
+from boilercv.types import DA
+
+EXAMPLE_NUM_FRAMES = 1000
+EXAMPLE_VIDEO_NAME = "2022-11-30T13-41-00"
+EXAMPLE_CONTOURS = PARAMS.paths.examples / f"{EXAMPLE_VIDEO_NAME}.h5"
+# TODO: Source the ROI from the dataset.
+EXAMPLE_ROI = PARAMS.paths.examples / f"{EXAMPLE_VIDEO_NAME}_roi.yaml"
+
+
+def get_images() -> DA:
+    with xr.open_dataset(PARAMS.paths.examples / f"{EXAMPLE_VIDEO_NAME}.nc") as ds:
+        return ds[VIDEO].sel(frame=slice(None, EXAMPLE_NUM_FRAMES))
+
+
+EXAMPLE_VIDEO = get_images()
+EXAMPLE_FRAME_LIST = list(EXAMPLE_VIDEO.values)
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/blobs/__init__.py` & `boilercv-0.0.1/src/boilercv/examples/blobs/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from dataclasses import dataclass
-from math import sqrt
-
-from skimage.draw import disk, set_color
-from skimage.feature import blob_dog, blob_doh, blob_log
-
-
-def get_blobs_dog(image):
-    blobs = blob_dog(
-        image,
-        # max_sigma=30,
-        # threshold=0.1,
-    )
-    blobs[:, 2] = blobs[:, 2] * sqrt(2)
-    return (Blob(*blob) for blob in blobs)
-
-
-def get_blobs_log(image):
-    blobs = blob_log(
-        image,
-        max_sigma=30,
-        num_sigma=10,
-        threshold=0.1,
-    )
-    blobs[:, 2] = blobs[:, 2] * sqrt(2)
-    return (Blob(*blob) for blob in blobs)
-
-
-def get_blobs_doh(image):
-    blobs = blob_doh(
-        image,
-        # min_sigma=1,
-        # max_sigma=30,
-        # threshold=0.01,
-        # overlap=0.30,
-    )
-    return (Blob(*blob) for blob in blobs)
-
-
-@dataclass
-class Blob:
-    y: int
-    x: int
-    r: int
-
-
-def draw_blobs(result, blob, color):
-    rr, cc = disk(
-        (int(blob.y), int(blob.x)),
-        int(blob.r),
-    )
-    set_color(result, (rr, cc), color)
+from dataclasses import dataclass
+from math import sqrt
+
+from skimage.draw import disk, set_color
+from skimage.feature import blob_dog, blob_doh, blob_log
+
+
+def get_blobs_dog(image):
+    blobs = blob_dog(
+        image,
+        # max_sigma=30,
+        # threshold=0.1,
+    )
+    blobs[:, 2] = blobs[:, 2] * sqrt(2)
+    return (Blob(*blob) for blob in blobs)
+
+
+def get_blobs_log(image):
+    blobs = blob_log(
+        image,
+        max_sigma=30,
+        num_sigma=10,
+        threshold=0.1,
+    )
+    blobs[:, 2] = blobs[:, 2] * sqrt(2)
+    return (Blob(*blob) for blob in blobs)
+
+
+def get_blobs_doh(image):
+    blobs = blob_doh(
+        image,
+        # min_sigma=1,
+        # max_sigma=30,
+        # threshold=0.01,
+        # overlap=0.30,
+    )
+    return (Blob(*blob) for blob in blobs)
+
+
+@dataclass
+class Blob:
+    y: int
+    x: int
+    r: int
+
+
+def draw_blobs(result, blob, color):
+    rr, cc = disk(
+        (int(blob.y), int(blob.x)),
+        int(blob.r),
+    )
+    set_color(result, (rr, cc), color)
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/contours.py` & `boilercv-0.0.1/src/boilercv/examples/contours.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""Get bubble contours."""
-
-import cv2 as cv
-
-from boilercv.captivate.previews import view_images
-from boilercv.data import IDX, VIDEO
-from boilercv.data.sets import get_dataset
-from boilercv.examples import EXAMPLE_CONTOURS, EXAMPLE_NUM_FRAMES, EXAMPLE_VIDEO_NAME
-from boilercv.images import scale_bool
-from boilercv.images.cv import draw_contours
-from boilercv.stages.contours import get_all_contours
-from boilercv.types import ArrInt, Img
-
-
-def main():
-    ds = get_dataset(EXAMPLE_VIDEO_NAME, EXAMPLE_NUM_FRAMES)
-    video = ds[VIDEO]
-    df = get_all_contours(
-        cv.bitwise_not(scale_bool(video.values)), method=cv.CHAIN_APPROX_SIMPLE
-    )
-    df.to_hdf(EXAMPLE_CONTOURS, "contours", complib="zlib", complevel=9)
-    result: list[Img] = []
-    for frame_num, frame in enumerate(video):
-        contours: list[ArrInt] = list(  # type: ignore
-            df.loc[IDX[frame_num], :]  # type: ignore
-            .groupby("contour")
-            .apply(lambda grp: grp.values)  # type: ignore
-        )
-        result.append(draw_contours(scale_bool(frame.values), contours))
-    view_images(result)
-
-
-if __name__ == "__main__":
-    main()
+"""Get bubble contours."""
+
+import cv2 as cv
+
+from boilercv.captivate.previews import view_images
+from boilercv.data import IDX, VIDEO
+from boilercv.data.sets import get_dataset
+from boilercv.examples import EXAMPLE_CONTOURS, EXAMPLE_NUM_FRAMES, EXAMPLE_VIDEO_NAME
+from boilercv.images import scale_bool
+from boilercv.images.cv import draw_contours
+from boilercv.stages.contours import get_all_contours
+from boilercv.types import ArrInt, Img
+
+
+def main():
+    ds = get_dataset(EXAMPLE_VIDEO_NAME, EXAMPLE_NUM_FRAMES)
+    video = ds[VIDEO]
+    df = get_all_contours(
+        cv.bitwise_not(scale_bool(video.values)), method=cv.CHAIN_APPROX_SIMPLE
+    )
+    df.to_hdf(EXAMPLE_CONTOURS, "contours", complib="zlib", complevel=9)
+    result: list[Img] = []
+    for frame_num, frame in enumerate(video):
+        contours: list[ArrInt] = list(  # type: ignore
+            df.loc[IDX[frame_num], :]  # type: ignore
+            .groupby("contour")
+            .apply(lambda grp: grp.values)  # type: ignore
+        )
+        result.append(draw_contours(scale_bool(frame.values), contours))
+    view_images(result)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/cv/__init__.py` & `boilercv-0.0.1/src/boilercv/examples/cv/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""Basic examples using OpenCV sample files."""
-
-from collections.abc import Iterator
-from os import environ
-from pathlib import Path
-
-import cv2 as cv
-
-from boilercv.types import Img
-
-
-def init():
-    """Initialize `boilercv.examples.cv`."""
-    check_samples_env_var()
-
-
-def check_samples_env_var():
-    """Check that the OpenCV samples environment variable is set and is a folder."""
-    samples_env_var = "OPENCV_SAMPLES_DATA_PATH"
-    if (
-        not (samples_dir := environ.get(samples_env_var))
-        or not Path(samples_dir).is_dir()
-    ):
-        raise RuntimeError(
-            f"{samples_env_var} not set or specified directory does not exist."
-        )
-
-
-def capture_images(path: Path) -> Iterator[Img]:
-    """Load images from a video file."""
-    video_capture = cv.VideoCapture(str(path))
-    while True:
-        read_is_successful, image = video_capture.read()
-        if not read_is_successful:
-            break
-        yield image
-
-
-# * -------------------------------------------------------------------------------- * #
-
-init()
+"""Basic examples using OpenCV sample files."""
+
+from collections.abc import Iterator
+from os import environ
+from pathlib import Path
+
+import cv2 as cv
+
+from boilercv.types import Img
+
+
+def init():
+    """Initialize `boilercv.examples.cv`."""
+    check_samples_env_var()
+
+
+def check_samples_env_var():
+    """Check that the OpenCV samples environment variable is set and is a folder."""
+    samples_env_var = "OPENCV_SAMPLES_DATA_PATH"
+    if (
+        not (samples_dir := environ.get(samples_env_var))
+        or not Path(samples_dir).is_dir()
+    ):
+        raise RuntimeError(
+            f"{samples_env_var} not set or specified directory does not exist."
+        )
+
+
+def capture_images(path: Path) -> Iterator[Img]:
+    """Load images from a video file."""
+    video_capture = cv.VideoCapture(str(path))
+    while True:
+        read_is_successful, image = video_capture.read()
+        if not read_is_successful:
+            break
+        yield image
+
+
+# * -------------------------------------------------------------------------------- * #
+
+init()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/cv/basic_test.py` & `boilercv-0.0.1/src/boilercv/examples/cv/basic_test.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""Preview a video."""
-
-from pathlib import Path
-
-import cv2 as cv
-import numpy as np
-
-from boilercv import PREVIEW
-from boilercv.captivate.previews import view_images
-from boilercv.examples.cv import capture_images
-from boilercv.images.cv import convert_image
-from boilercv.types import Vid
-
-
-def main(preview: bool = PREVIEW) -> Vid:
-    images = capture_images(Path(cv.samples.findFile("vtest.avi")))
-    video = np.stack([convert_image(image, cv.COLOR_BGR2RGB) for image in images])
-    if preview:
-        view_images(video)
-    return video
-
-
-if __name__ == "__main__":
-    main()
+"""Preview a video."""
+
+from pathlib import Path
+
+import cv2 as cv
+import numpy as np
+
+from boilercv import PREVIEW
+from boilercv.captivate.previews import view_images
+from boilercv.examples.cv import capture_images
+from boilercv.images.cv import convert_image
+from boilercv.types import Vid
+
+
+def main(preview: bool = PREVIEW) -> Vid:
+    images = capture_images(Path(cv.samples.findFile("vtest.avi")))
+    video = np.stack([convert_image(image, cv.COLOR_BGR2RGB) for image in images])
+    if preview:
+        view_images(video)
+    return video
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/detect_surface.py` & `boilercv-0.0.1/src/boilercv/examples/detect_surface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-"""Detect the boiling surface."""
-
-from warnings import warn
-
-import cv2 as cv
-import numpy as np
-import xarray as xr
-from scipy.ndimage import (
-    center_of_mass,
-    generate_binary_structure,
-    label,
-    labeled_comprehension,
-)
-
-from boilercv import DEBUG
-from boilercv.captivate.previews import get_calling_scope_name, save_roi, view_images
-from boilercv.data import VIDEO, YX_PX, apply_to_img_da
-from boilercv.data.frames import df_points
-from boilercv.data.sets import get_dataset
-from boilercv.examples import EXAMPLE_NUM_FRAMES, EXAMPLE_ROI, EXAMPLE_VIDEO_NAME
-from boilercv.images import scale_bool
-from boilercv.images.cv import find_contours, get_wall
-from boilercv.types import DA, ArrInt, Img
-
-
-def main():
-    ds = get_dataset(EXAMPLE_VIDEO_NAME, EXAMPLE_NUM_FRAMES)
-    video = ds[VIDEO]
-    roi = ds["roi"]
-    wall: DA = apply_to_img_da(get_wall, scale_bool(roi), name="wall")
-    boiling_surface, boiling_surface_coords = xr.apply_ufunc(
-        find_boiling_surface,
-        scale_bool(wall),
-        input_core_dims=[YX_PX],
-        output_core_dims=[YX_PX, ["test"]],
-    )
-    contours = find_contours(scale_bool(wall.values), method=cv.CHAIN_APPROX_SIMPLE)
-    if len(contours) > 1:
-        warn("More than one contour found when searching for the ROI.", stacklevel=1)
-    save_roi(contours[0], EXAMPLE_ROI)
-    view_images(dict(boiling_surface=boiling_surface, roi=roi))
-
-
-def find_boiling_surface(img: Img) -> tuple[Img, ArrInt]:
-    """Find the boiling surface."""
-
-    # Parameters for finding prominent horizontal lines
-    wide_rectangular_ksize = [9, 3]  # Enhance horizontal lines
-    threshold = 0.6
-
-    # The range to consider a connected component to be the boiling surface
-    (height, width) = img.shape
-    min_size_px = 8
-    ypx_min = height / 2
-    xpx_mid = width / 2
-    xpx_max_dist = width / 8
-    xpx_min = xpx_mid - xpx_max_dist
-    xpx_max = xpx_mid + xpx_max_dist
-
-    # Find prominent horizontal lines
-    corners = cv.cornerHarris(src=img, blockSize=2, ksize=3, k=0.04)
-    lines = -1 * corners  # Linear features are strongly negative in Harris
-    blurred = cv.blur(lines, ksize=wide_rectangular_ksize)
-    scaled = (blurred - blurred.min()) / (blurred.max() - blurred.min())
-    binarized = scaled > threshold
-
-    # Find connected components and their centers
-    # ? cv.connectedComponents and cv.moments could also be used
-    # ? Consider re-implementing if slow
-    find_diag_conns = generate_binary_structure(rank=2, connectivity=2)
-    labeled_img, num_objects = label(input=binarized, structure=find_diag_conns)
-    labels = range(1, num_objects + 1)  # Exclude 0-labeled background
-    sizes_px = labeled_comprehension(
-        input=binarized,
-        labels=labeled_img,
-        index=labels,
-        func=np.count_nonzero,
-        out_dtype=int,
-        default=0,
-    )
-    objs = (
-        df_points(
-            np.array(center_of_mass(input=binarized, labels=labeled_img, index=labels))
-            .round()
-            .astype(int)  # Not img dtype. df contains coords, not pixel values
-        )
-        .assign(**dict(label=labels, size_px=sizes_px))
-        .rename(axis="columns", mapper=dict(ypx="ypx_center", xpx="xpx_center"))
-        .set_index("label", drop=True)
-    )
-
-    # Consider the boiling surface to be the largest object in range
-    objs_in_range = objs[
-        (objs.size > min_size_px)
-        & (objs.ypx_center > ypx_min)
-        & (objs.xpx_center > xpx_min)
-        & (objs.xpx_center < xpx_max)
-    ]
-    label_largest_in_range = objs_in_range.size_px.idxmax()
-    boiling_surface = labeled_img == label_largest_in_range
-
-    # Get a line segment corresponding to the boiling surface
-    points = df_points(np.array(boiling_surface.nonzero()).T)
-    xpx_left = points.xpx.min()
-    xpx_right = points.xpx.max()
-    ypx_horizontal = np.round(points.ypx.mean()).astype(int)
-    boiling_surface_coords = np.array(
-        [ypx_horizontal, xpx_left, ypx_horizontal, xpx_right]
-    ).astype(int)
-
-    if DEBUG:
-        view_images(
-            name=get_calling_scope_name(),
-            images=dict(
-                img=img,
-                corners=corners,
-                lines=lines,
-                blurred=blurred,
-                scaled=scaled,
-                binarized=binarized,
-                labeled_img=labeled_img,
-                boiling_surface=boiling_surface,
-            ),
-        )
-    return boiling_surface, boiling_surface_coords
-
-
-if __name__ == "__main__":
-    main()
+"""Detect the boiling surface."""
+
+from warnings import warn
+
+import cv2 as cv
+import numpy as np
+import xarray as xr
+from scipy.ndimage import (
+    center_of_mass,
+    generate_binary_structure,
+    label,
+    labeled_comprehension,
+)
+
+from boilercv import DEBUG
+from boilercv.captivate.previews import get_calling_scope_name, save_roi, view_images
+from boilercv.data import VIDEO, YX_PX, apply_to_img_da
+from boilercv.data.frames import df_points
+from boilercv.data.sets import get_dataset
+from boilercv.examples import EXAMPLE_NUM_FRAMES, EXAMPLE_ROI, EXAMPLE_VIDEO_NAME
+from boilercv.images import scale_bool
+from boilercv.images.cv import find_contours, get_wall
+from boilercv.types import DA, ArrInt, Img
+
+
+def main():
+    ds = get_dataset(EXAMPLE_VIDEO_NAME, EXAMPLE_NUM_FRAMES)
+    video = ds[VIDEO]
+    roi = ds["roi"]
+    wall: DA = apply_to_img_da(get_wall, scale_bool(roi), name="wall")
+    boiling_surface, boiling_surface_coords = xr.apply_ufunc(
+        find_boiling_surface,
+        scale_bool(wall),
+        input_core_dims=[YX_PX],
+        output_core_dims=[YX_PX, ["test"]],
+    )
+    contours = find_contours(scale_bool(wall.values), method=cv.CHAIN_APPROX_SIMPLE)
+    if len(contours) > 1:
+        warn("More than one contour found when searching for the ROI.", stacklevel=1)
+    save_roi(contours[0], EXAMPLE_ROI)
+    view_images(dict(boiling_surface=boiling_surface, roi=roi))
+
+
+def find_boiling_surface(img: Img) -> tuple[Img, ArrInt]:
+    """Find the boiling surface."""
+
+    # Parameters for finding prominent horizontal lines
+    wide_rectangular_ksize = [9, 3]  # Enhance horizontal lines
+    threshold = 0.6
+
+    # The range to consider a connected component to be the boiling surface
+    (height, width) = img.shape
+    min_size_px = 8
+    ypx_min = height / 2
+    xpx_mid = width / 2
+    xpx_max_dist = width / 8
+    xpx_min = xpx_mid - xpx_max_dist
+    xpx_max = xpx_mid + xpx_max_dist
+
+    # Find prominent horizontal lines
+    corners = cv.cornerHarris(src=img, blockSize=2, ksize=3, k=0.04)
+    lines = -1 * corners  # Linear features are strongly negative in Harris
+    blurred = cv.blur(lines, ksize=wide_rectangular_ksize)
+    scaled = (blurred - blurred.min()) / (blurred.max() - blurred.min())
+    binarized = scaled > threshold
+
+    # Find connected components and their centers
+    # ? cv.connectedComponents and cv.moments could also be used
+    # ? Consider re-implementing if slow
+    find_diag_conns = generate_binary_structure(rank=2, connectivity=2)
+    labeled_img, num_objects = label(input=binarized, structure=find_diag_conns)  # type: ignore
+    labels = range(1, num_objects + 1)  # Exclude 0-labeled background
+    sizes_px = labeled_comprehension(
+        input=binarized,
+        labels=labeled_img,
+        index=labels,
+        func=np.count_nonzero,
+        out_dtype=int,
+        default=0,
+    )
+    objs = (
+        df_points(
+            np.array(center_of_mass(input=binarized, labels=labeled_img, index=labels))
+            .round()
+            .astype(int)  # Not img dtype. df contains coords, not pixel values
+        )
+        .assign(**dict(label=labels, size_px=sizes_px))
+        .rename(axis="columns", mapper=dict(ypx="ypx_center", xpx="xpx_center"))
+        .set_index("label", drop=True)
+    )
+
+    # Consider the boiling surface to be the largest object in range
+    objs_in_range = objs[
+        (objs.size > min_size_px)
+        & (objs.ypx_center > ypx_min)
+        & (objs.xpx_center > xpx_min)
+        & (objs.xpx_center < xpx_max)
+    ]
+    label_largest_in_range = objs_in_range.size_px.idxmax()
+    boiling_surface = labeled_img == label_largest_in_range
+
+    # Get a line segment corresponding to the boiling surface
+    points = df_points(np.array(boiling_surface.nonzero()).T)
+    xpx_left = points.xpx.min()
+    xpx_right = points.xpx.max()
+    ypx_horizontal = np.round(points.ypx.mean()).astype(int)
+    boiling_surface_coords = np.array(
+        [ypx_horizontal, xpx_left, ypx_horizontal, xpx_right]
+    ).astype(int)
+
+    if DEBUG:
+        view_images(
+            name=get_calling_scope_name(),
+            images=dict(
+                img=img,
+                corners=corners,
+                lines=lines,
+                blurred=blurred,
+                scaled=scaled,
+                binarized=binarized,
+                labeled_img=labeled_img,
+                boiling_surface=boiling_surface,
+            ),
+        )
+    return boiling_surface, boiling_surface_coords
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/fill.py` & `boilercv-0.0.1/src/boilercv/examples/fill.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-"""Fill bubble contours."""
-
-import cv2 as cv
-import numpy as np
-import pandas as pd
-import xarray as xr
-from loguru import logger
-
-from boilercv import PREVIEW
-from boilercv.captivate.previews import view_images
-from boilercv.data import IDX, ROI, VIDEO
-from boilercv.data.packing import pack, unpack
-from boilercv.data.sets import get_contours_df, get_dataset
-from boilercv.examples import EXAMPLE_NUM_FRAMES, EXAMPLE_VIDEO_NAME
-from boilercv.images.cv import draw_contours
-from boilercv.models.params import PARAMS
-from boilercv.types import ArrInt
-
-TRY_EMPTY = False
-
-
-def main():
-    if TRY_EMPTY:
-        all_contours = np.empty((0, 4))
-        df = pd.DataFrame(
-            all_contours, columns=["frame", "contour", "ypx", "xpx"]
-        ).set_index(["frame", "contour"])
-    else:
-        df = get_contours_df(EXAMPLE_VIDEO_NAME)
-    ds = xr.zeros_like(
-        get_dataset(EXAMPLE_VIDEO_NAME, EXAMPLE_NUM_FRAMES), dtype=np.uint8
-    )
-    video = ds[VIDEO]
-    if not df.empty:
-        for frame_num, frame in enumerate(video):
-            contours: list[ArrInt] = list(  # type: ignore
-                df.loc[IDX[frame_num], :]  # type: ignore
-                .groupby("contour")
-                .apply(lambda grp: grp.values)  # type: ignore
-            )
-            video[frame_num, :, :] = draw_contours(
-                frame.values, contours, thickness=cv.FILLED
-            )
-    ds[VIDEO] = pack(video)
-    ds = ds.drop_vars(ROI)
-    destination = PARAMS.paths.examples / f"{EXAMPLE_VIDEO_NAME}_filled.nc"
-    ds.to_netcdf(path=destination)
-    if PREVIEW:
-        with xr.open_dataset(destination) as ds2:
-            view_images([unpack(ds[VIDEO]), unpack(ds2[VIDEO])])
-
-
-if __name__ == "__main__":
-    logger.info("start fill contours")
-    main()
-    logger.info("finish fill contours")
+"""Fill bubble contours."""
+
+import cv2 as cv
+import numpy as np
+import pandas as pd
+import xarray as xr
+from loguru import logger
+
+from boilercv import PREVIEW
+from boilercv.captivate.previews import view_images
+from boilercv.data import IDX, ROI, VIDEO
+from boilercv.data.packing import pack, unpack
+from boilercv.data.sets import get_contours_df, get_dataset
+from boilercv.examples import EXAMPLE_NUM_FRAMES, EXAMPLE_VIDEO_NAME
+from boilercv.images.cv import draw_contours
+from boilercv.models.params import PARAMS
+from boilercv.types import ArrInt
+
+TRY_EMPTY = False
+
+
+def main():
+    if TRY_EMPTY:
+        all_contours = np.empty((0, 4))
+        df = pd.DataFrame(
+            all_contours, columns=["frame", "contour", "ypx", "xpx"]
+        ).set_index(["frame", "contour"])
+    else:
+        df = get_contours_df(EXAMPLE_VIDEO_NAME)
+    ds = xr.zeros_like(
+        get_dataset(EXAMPLE_VIDEO_NAME, EXAMPLE_NUM_FRAMES), dtype=np.uint8
+    )
+    video = ds[VIDEO]
+    if not df.empty:
+        for frame_num, frame in enumerate(video):
+            contours: list[ArrInt] = list(  # type: ignore
+                df.loc[IDX[frame_num], :]  # type: ignore
+                .groupby("contour")
+                .apply(lambda grp: grp.values)  # type: ignore
+            )
+            video[frame_num, :, :] = draw_contours(
+                frame.values, contours, thickness=cv.FILLED
+            )
+    ds[VIDEO] = pack(video)
+    ds = ds.drop_vars(ROI)
+    destination = PARAMS.paths.examples / f"{EXAMPLE_VIDEO_NAME}_filled.nc"
+    ds.to_netcdf(path=destination)
+    if PREVIEW:
+        with xr.open_dataset(destination) as ds2:
+            view_images([unpack(ds[VIDEO]), unpack(ds2[VIDEO])])
+
+
+if __name__ == "__main__":
+    logger.info("start fill contours")
+    main()
+    logger.info("finish fill contours")
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/large/__init__.py` & `boilercv-0.0.1/src/boilercv/examples/large/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-"""Examples that operate on large files, which are not in the cloud."""
-
-from collections.abc import Iterator
-from contextlib import contextmanager
-
-import xarray as xr
-
-from boilercv.captivate.previews import view_images
-from boilercv.data import VIDEO
-from boilercv.models.params import LOCAL_PATHS
-from boilercv.types import DS
-
-EXAMPLE = LOCAL_PATHS.large_sources / "2022-09-14T13-20-54.nc"
-
-
-@contextmanager
-def example_dataset(
-    source: str = "",
-    destination: str = "",
-    preview: bool = True,
-    save: bool = True,
-    **kwargs,
-) -> Iterator[DS]:  # sourcery skip: move-assign
-    """Open the example dataset and write it to a destination file with a suffix.
-
-    Args:
-        source: If provided, use a dataset derived from the example with this suffix.
-        destination: If provided, add this suffix to the destination dataset file.
-        kwargs: Keyword arguments to pass to `xarray.Dataset.to_netcdf`.
-        preview: Preview the original and modified datasets.
-        save: Whether to save the file.
-    """
-    _source = (
-        LOCAL_PATHS.large_examples / f"{EXAMPLE.stem}_{source}.nc"
-        if source
-        else EXAMPLE
-    )
-    _destination = LOCAL_PATHS.large_examples / f"{EXAMPLE.stem}_{destination}.nc"
-    with xr.open_dataset(_source) as ds:
-        original = ds[VIDEO]
-        try:
-            yield ds
-        finally:
-            updated = ds[VIDEO]
-            if preview:
-                view_images(dict(original=original, updated=updated))
-            if save:
-                ds.to_netcdf(path=_destination, **kwargs)
+"""Examples that operate on large files, which are not in the cloud."""
+
+from collections.abc import Iterator
+from contextlib import contextmanager
+
+import xarray as xr
+
+from boilercv.captivate.previews import view_images
+from boilercv.data import VIDEO
+from boilercv.models.params import LOCAL_PATHS
+from boilercv.types import DS
+
+EXAMPLE = LOCAL_PATHS.large_sources / "2022-09-14T13-20-54.nc"
+
+
+@contextmanager
+def example_dataset(
+    source: str = "",
+    destination: str = "",
+    preview: bool = True,
+    save: bool = True,
+    **kwargs,
+) -> Iterator[DS]:  # sourcery skip: move-assign
+    """Open the example dataset and write it to a destination file with a suffix.
+
+    Args:
+        source: If provided, use a dataset derived from the example with this suffix.
+        destination: If provided, add this suffix to the destination dataset file.
+        kwargs: Keyword arguments to pass to `xarray.Dataset.to_netcdf`.
+        preview: Preview the original and modified datasets.
+        save: Whether to save the file.
+    """
+    _source = (
+        LOCAL_PATHS.large_examples / f"{EXAMPLE.stem}_{source}.nc"
+        if source
+        else EXAMPLE
+    )
+    _destination = LOCAL_PATHS.large_examples / f"{EXAMPLE.stem}_{destination}.nc"
+    with xr.open_dataset(_source) as ds:
+        original = ds[VIDEO]
+        try:
+            yield ds
+        finally:
+            updated = ds[VIDEO]
+            if preview:
+                view_images(dict(original=original, updated=updated))
+            if save:
+                ds.to_netcdf(path=_destination, **kwargs)
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/large/combined.py` & `boilercv-0.0.1/src/boilercv/examples/large/combined.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""Perform all of the steps."""
-
-from boilercv import DEBUG
-from boilercv.captivate.previews import view_images
-from boilercv.data import FRAME, VIDEO, apply_to_img_da
-from boilercv.data.packing import pack
-from boilercv.examples.large import example_dataset
-from boilercv.images import scale_bool
-from boilercv.images.cv import apply_mask, binarize, flood, get_roi
-from boilercv.types import DA
-
-
-def main():
-    with example_dataset(
-        destination="combined", preview=DEBUG, encoding={VIDEO: {"zlib": True}}
-    ) as ds:
-        video = ds[VIDEO]
-        maximum = video.max(FRAME)
-        flooded: DA = apply_to_img_da(flood, maximum)
-        roi = apply_to_img_da(get_roi, scale_bool(flooded))
-        masked: DA = apply_to_img_da(apply_mask, video, scale_bool(roi), vectorize=True)
-        binarized: DA = apply_to_img_da(binarize, masked, vectorize=True)
-        ds[VIDEO] = pack(binarized)
-        view_images(
-            dict(
-                video=video.isel(frame=0),
-                maximum=maximum,
-                flooded=flooded,
-                roi=roi,
-                masked=masked.isel(frame=0),
-                binarized=binarized.isel(frame=0),
-            )
-        )
-
-
-if __name__ == "__main__":
-    main()
+"""Perform all of the steps."""
+
+from boilercv import DEBUG
+from boilercv.captivate.previews import view_images
+from boilercv.data import FRAME, VIDEO, apply_to_img_da
+from boilercv.data.packing import pack
+from boilercv.examples.large import example_dataset
+from boilercv.images import scale_bool
+from boilercv.images.cv import apply_mask, binarize, flood, get_roi
+from boilercv.types import DA
+
+
+def main():
+    with example_dataset(
+        destination="combined", preview=DEBUG, encoding={VIDEO: {"zlib": True}}
+    ) as ds:
+        video = ds[VIDEO]
+        maximum = video.max(FRAME)
+        flooded: DA = apply_to_img_da(flood, maximum)
+        roi = apply_to_img_da(get_roi, scale_bool(flooded))
+        masked: DA = apply_to_img_da(apply_mask, video, scale_bool(roi), vectorize=True)
+        binarized: DA = apply_to_img_da(binarize, masked, vectorize=True)
+        ds[VIDEO] = pack(binarized)
+        view_images(
+            dict(
+                video=video.isel(frame=0),
+                maximum=maximum,
+                flooded=flooded,
+                roi=roi,
+                masked=masked.isel(frame=0),
+                binarized=binarized.isel(frame=0),
+            )
+        )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/previews/binarized_composite.py` & `boilercv-0.0.1/src/boilercv/examples/previews/binarized_composite.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""Overlay detected bubbles on the binarized stage."""
-
-from boilercv import FRAMERATE_CONT, PREVIEW, WRITE
-from boilercv.captivate.captures import write_video
-from boilercv.captivate.previews import view_images
-from boilercv.data import VIDEO
-from boilercv.data.sets import get_dataset
-from boilercv.examples.previews import _EXAMPLE, _NUM_FRAMES
-from boilercv.images import scale_bool
-from boilercv.models.params import LOCAL_PATHS
-from boilercv.previews import compose_da
-
-
-def main():
-    source = get_dataset(_EXAMPLE, _NUM_FRAMES, stage="sources")[VIDEO]
-    bubbles = get_dataset(_EXAMPLE, _NUM_FRAMES, stage="filled")[VIDEO]
-    highlighted_bubbles = compose_da(source, scale_bool(bubbles)).transpose(
-        "frame", "ypx", "xpx", "channel"
-    )
-    if PREVIEW:
-        view_images(bubbles.isel(frame=0))
-        view_images(highlighted_bubbles, framerate=FRAMERATE_CONT)
-    if WRITE:
-        write_video(LOCAL_PATHS.media / "binarized", source)
-        write_video(LOCAL_PATHS.media / "bubbles", bubbles, preview_frame=True)
-        write_video(LOCAL_PATHS.media / "binarized_highlighted", highlighted_bubbles)
-
-
-if __name__ == "__main__":
-    main()
+"""Overlay detected bubbles on the binarized stage."""
+
+from boilercv import FRAMERATE_CONT, PREVIEW, WRITE
+from boilercv.captivate.captures import write_video
+from boilercv.captivate.previews import view_images
+from boilercv.data import VIDEO
+from boilercv.data.sets import get_dataset
+from boilercv.examples.previews import _EXAMPLE, _NUM_FRAMES
+from boilercv.images import scale_bool
+from boilercv.models.params import LOCAL_PATHS
+from boilercv.previews import compose_da
+
+
+def main():
+    source = get_dataset(_EXAMPLE, _NUM_FRAMES, stage="sources")[VIDEO]
+    bubbles = get_dataset(_EXAMPLE, _NUM_FRAMES, stage="filled")[VIDEO]
+    highlighted_bubbles = compose_da(source, scale_bool(bubbles)).transpose(
+        "frame", "ypx", "xpx", "channel"
+    )
+    if PREVIEW:
+        view_images(bubbles.isel(frame=0))
+        view_images(highlighted_bubbles, framerate=FRAMERATE_CONT)
+    if WRITE:
+        write_video(LOCAL_PATHS.media / "binarized", source)
+        write_video(LOCAL_PATHS.media / "bubbles", bubbles, preview_frame=True)
+        write_video(LOCAL_PATHS.media / "binarized_highlighted", highlighted_bubbles)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/previews/gray_composite.py` & `boilercv-0.0.1/src/boilercv/examples/previews/gray_composite.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""Overlay detected bubbles on the gray stage."""
-
-from boilercv import FRAMERATE_CONT, PREVIEW, WRITE
-from boilercv.captivate.captures import write_video
-from boilercv.captivate.previews import view_images
-from boilercv.data import VIDEO
-from boilercv.data.sets import get_dataset
-from boilercv.examples.previews import _EXAMPLE, _NUM_FRAMES
-from boilercv.images import scale_bool
-from boilercv.models.params import LOCAL_PATHS
-from boilercv.previews import compose_da
-
-
-def main():
-    gray_source = get_dataset(_EXAMPLE, _NUM_FRAMES, stage="large_sources")[VIDEO]
-    bubbles = get_dataset(_EXAMPLE, _NUM_FRAMES, stage="filled")[VIDEO]
-    highlighted_bubbles = compose_da(gray_source, scale_bool(bubbles)).transpose(
-        "frame", "ypx", "xpx", "channel"
-    )
-    if PREVIEW:
-        view_images(highlighted_bubbles, framerate=FRAMERATE_CONT)
-    if WRITE:
-        path = LOCAL_PATHS.media / "examples" / _EXAMPLE / "gray_highlighted"
-        path.parent.mkdir(parents=True, exist_ok=True)
-        write_video(path, highlighted_bubbles, preview_frame=True)
-
-
-if __name__ == "__main__":
-    main()
+"""Overlay detected bubbles on the gray stage."""
+
+from boilercv import FRAMERATE_CONT, PREVIEW, WRITE
+from boilercv.captivate.captures import write_video
+from boilercv.captivate.previews import view_images
+from boilercv.data import VIDEO
+from boilercv.data.sets import get_dataset
+from boilercv.examples.previews import _EXAMPLE, _NUM_FRAMES
+from boilercv.images import scale_bool
+from boilercv.models.params import LOCAL_PATHS
+from boilercv.previews import compose_da
+
+
+def main():
+    gray_source = get_dataset(_EXAMPLE, _NUM_FRAMES, stage="large_sources")[VIDEO]
+    bubbles = get_dataset(_EXAMPLE, _NUM_FRAMES, stage="filled")[VIDEO]
+    highlighted_bubbles = compose_da(gray_source, scale_bool(bubbles)).transpose(
+        "frame", "ypx", "xpx", "channel"
+    )
+    if PREVIEW:
+        view_images(highlighted_bubbles, framerate=FRAMERATE_CONT)
+    if WRITE:
+        path = LOCAL_PATHS.media / "examples" / _EXAMPLE / "gray_highlighted"
+        path.parent.mkdir(parents=True, exist_ok=True)
+        write_video(path, highlighted_bubbles, preview_frame=True)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/previews/multicolor_composite.py` & `boilercv-0.0.1/src/boilercv/examples/previews/multicolor_composite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-"""Overlay detected bubbles on the gray stage."""
-
-from itertools import cycle
-
-import cv2 as cv
-import numpy as np
-import seaborn as sns
-from matplotlib import pyplot as plt
-
-from boilercv import DEBUG, PREVIEW, WRITE
-from boilercv.captivate.captures import write_image
-from boilercv.captivate.previews import view_images
-from boilercv.data import VIDEO
-from boilercv.data.sets import get_contours_df, get_dataset
-from boilercv.examples.previews import _EXAMPLE
-from boilercv.images import overlay
-from boilercv.images.cv import convert_image, draw_contours
-from boilercv.models.params import LOCAL_PATHS
-from boilercv.types import ArrInt
-
-_NUM_FRAMES = 1
-
-_PALETTE = [c for c in sns.color_palette("Set1") if not c[0] == c[1] == c[2]]
-_PALETTE_CV = [(int(255 * c[2]), int(255 * c[1]), int(255 * c[0])) for c in _PALETTE]
-
-
-def main():
-    frame = _NUM_FRAMES - 1
-    gray = (
-        get_dataset(_EXAMPLE, _NUM_FRAMES, stage="large_sources")[VIDEO]
-        .isel(frame=frame)
-        .values
-    )
-    contours: list[ArrInt] = list(
-        get_contours_df(_EXAMPLE)
-        .loc[frame, :]
-        .groupby("contour")
-        .apply(lambda grp: grp.values)
-    )
-    highlighted = np.zeros_like(convert_image(gray, cv.COLOR_GRAY2BGR))
-    for contour, color in zip(contours, cycle(_PALETTE_CV), strict=False):
-        highlighted = draw_contours(highlighted, [contour], color=color)
-    highlighted = convert_image(highlighted, cv.COLOR_BGR2RGB)
-    composed = overlay(gray, highlighted, alpha=0.7)
-    if PREVIEW:
-        if DEBUG:
-            sns.palplot(_PALETTE)
-        plt.show()
-        view_images(composed)
-    if WRITE:
-        path = LOCAL_PATHS.media / "examples" / _EXAMPLE / "multicolor"
-        path.parent.mkdir(parents=True, exist_ok=True)
-        write_image(path, composed)
-
-
-if __name__ == "__main__":
-    main()
+"""Overlay detected bubbles on the gray stage."""
+
+from itertools import cycle
+
+import cv2 as cv
+import numpy as np
+import seaborn as sns
+from matplotlib import pyplot as plt
+
+from boilercv import DEBUG, PREVIEW, WRITE
+from boilercv.captivate.captures import write_image
+from boilercv.captivate.previews import view_images
+from boilercv.data import VIDEO
+from boilercv.data.sets import get_contours_df, get_dataset
+from boilercv.examples.previews import _EXAMPLE
+from boilercv.images import overlay
+from boilercv.images.cv import convert_image, draw_contours
+from boilercv.models.params import LOCAL_PATHS
+from boilercv.types import ArrInt
+
+_NUM_FRAMES = 1
+
+_PALETTE = [c for c in sns.color_palette("Set1") if not c[0] == c[1] == c[2]]  # type: ignore
+_PALETTE_CV = [(int(255 * c[2]), int(255 * c[1]), int(255 * c[0])) for c in _PALETTE]
+
+
+def main():
+    frame = _NUM_FRAMES - 1
+    gray = (
+        get_dataset(_EXAMPLE, _NUM_FRAMES, stage="large_sources")[VIDEO]
+        .isel(frame=frame)
+        .values
+    )
+    contours: list[ArrInt] = list(
+        get_contours_df(_EXAMPLE)
+        .loc[frame, :]
+        .groupby("contour")
+        .apply(lambda grp: grp.values)
+    )
+    highlighted = np.zeros_like(convert_image(gray, cv.COLOR_GRAY2BGR))
+    for contour, color in zip(contours, cycle(_PALETTE_CV), strict=False):
+        highlighted = draw_contours(highlighted, [contour], color=color)
+    highlighted = convert_image(highlighted, cv.COLOR_BGR2RGB)
+    composed = overlay(gray, highlighted, alpha=0.7)
+    if PREVIEW:
+        if DEBUG:
+            sns.palplot(_PALETTE)
+        plt.show()
+        view_images(composed)
+    if WRITE:
+        path = LOCAL_PATHS.media / "examples" / _EXAMPLE / "multicolor"
+        path.parent.mkdir(parents=True, exist_ok=True)
+        write_image(path, composed)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/previews/triple_composite.py` & `boilercv-0.0.1/src/boilercv/examples/previews/triple_composite.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""Preview detected regions on an image from the dataset."""
-
-import xarray as xr
-
-from boilercv import PREVIEW, WRITE
-from boilercv.captivate.captures import write_image
-from boilercv.captivate.previews import view_images
-from boilercv.colors import BLUE, GREEN, RED
-from boilercv.data import ROI, VIDEO
-from boilercv.data.sets import get_dataset
-from boilercv.examples.detect_surface import find_boiling_surface
-from boilercv.examples.previews import _EXAMPLE
-from boilercv.images import overlay, scale_bool
-from boilercv.models.params import LOCAL_PATHS, PARAMS
-
-
-def main():
-    ds = get_dataset(_EXAMPLE)
-    gray = (
-        xr.open_dataset(PARAMS.paths.gray_preview)[VIDEO]
-        .sel(video_name=_EXAMPLE)
-        .values
-    )
-    roi = ds[ROI].values
-    highlighted_roi = overlay(gray, scale_bool(roi), color=BLUE, alpha=0.2)
-
-    surface, _ = find_boiling_surface(scale_bool(roi))
-    highlighted_surface = overlay(
-        highlighted_roi, scale_bool(surface), color=RED, alpha=1
-    )
-
-    filled = (
-        xr.open_dataset(PARAMS.paths.filled_preview)[VIDEO]
-        .sel(video_name=_EXAMPLE)
-        .values
-    )
-    highlighted_bubbles = overlay(
-        highlighted_surface, scale_bool(filled), color=GREEN, alpha=0.4
-    )
-
-    if PREVIEW:
-        view_images(highlighted_bubbles)
-    if WRITE:
-        write_image(LOCAL_PATHS.media / "roi", highlighted_roi)
-        write_image(LOCAL_PATHS.media / "composite", highlighted_bubbles)
-
-
-if __name__ == "__main__":
-    main()
+"""Preview detected regions on an image from the dataset."""
+
+import xarray as xr
+
+from boilercv import PREVIEW, WRITE
+from boilercv.captivate.captures import write_image
+from boilercv.captivate.previews import view_images
+from boilercv.colors import BLUE, GREEN, RED
+from boilercv.data import ROI, VIDEO
+from boilercv.data.sets import get_dataset
+from boilercv.examples.detect_surface import find_boiling_surface
+from boilercv.examples.previews import _EXAMPLE
+from boilercv.images import overlay, scale_bool
+from boilercv.models.params import LOCAL_PATHS, PARAMS
+
+
+def main():
+    ds = get_dataset(_EXAMPLE)
+    gray = (
+        xr.open_dataset(PARAMS.paths.gray_preview)[VIDEO]
+        .sel(video_name=_EXAMPLE)
+        .values
+    )
+    roi = ds[ROI].values
+    highlighted_roi = overlay(gray, scale_bool(roi), color=BLUE, alpha=0.2)
+
+    surface, _ = find_boiling_surface(scale_bool(roi))
+    highlighted_surface = overlay(
+        highlighted_roi, scale_bool(surface), color=RED, alpha=1
+    )
+
+    filled = (
+        xr.open_dataset(PARAMS.paths.filled_preview)[VIDEO]
+        .sel(video_name=_EXAMPLE)
+        .values
+    )
+    highlighted_bubbles = overlay(
+        highlighted_surface, scale_bool(filled), color=GREEN, alpha=0.4
+    )
+
+    if PREVIEW:
+        view_images(highlighted_bubbles)
+    if WRITE:
+        write_image(LOCAL_PATHS.media / "roi", highlighted_roi)
+        write_image(LOCAL_PATHS.media / "composite", highlighted_bubbles)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/examples/save_roi.py` & `boilercv-0.0.1/src/boilercv/examples/save_roi.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""Save the ROI to a legacy YAML format."""
-
-from warnings import warn
-
-import cv2 as cv
-
-from boilercv.captivate.previews import save_roi
-from boilercv.data import apply_to_img_da
-from boilercv.data.sets import get_dataset
-from boilercv.examples import EXAMPLE_ROI, EXAMPLE_VIDEO_NAME
-from boilercv.images import scale_bool
-from boilercv.images.cv import find_contours, get_wall
-from boilercv.types import DA
-
-
-def main():
-    ds = get_dataset(EXAMPLE_VIDEO_NAME)
-    roi = ds["roi"]
-    wall: DA = apply_to_img_da(get_wall, scale_bool(roi), name="wall")
-    contours = find_contours(scale_bool(wall.values), method=cv.CHAIN_APPROX_SIMPLE)
-    if len(contours) > 1:
-        warn("More than one contour found when searching for the ROI.", stacklevel=1)
-    save_roi(contours[0], EXAMPLE_ROI)
+"""Save the ROI to a legacy YAML format."""
+
+from warnings import warn
+
+import cv2 as cv
+
+from boilercv.captivate.previews import save_roi
+from boilercv.data import apply_to_img_da
+from boilercv.data.sets import get_dataset
+from boilercv.examples import EXAMPLE_ROI, EXAMPLE_VIDEO_NAME
+from boilercv.images import scale_bool
+from boilercv.images.cv import find_contours, get_wall
+from boilercv.types import DA
+
+
+def main():
+    ds = get_dataset(EXAMPLE_VIDEO_NAME)
+    roi = ds["roi"]
+    wall: DA = apply_to_img_da(get_wall, scale_bool(roi), name="wall")
+    contours = find_contours(scale_bool(wall.values), method=cv.CHAIN_APPROX_SIMPLE)
+    if len(contours) > 1:
+        warn("More than one contour found when searching for the ROI.", stacklevel=1)
+    save_roi(contours[0], EXAMPLE_ROI)
```

### Comparing `boilercv-0.0.0/src/boilercv/images/__init__.py` & `boilercv-0.0.1/src/boilercv/images/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,106 @@
-"""Image acquisition and processing."""
-
-# * Pure numpy image processing functions take lots of types, including DataArrays.
-# pyright: reportGeneralTypeIssues=none
-
-from typing import Any
-
-import numpy as np
-from matplotlib.font_manager import FontProperties, findfont
-from numpy import typing as npt
-from PIL import Image, ImageDraw, ImageFont, ImageOps
-
-from boilercv import DEBUG
-from boilercv.colors import BLACK, BLACK3, RED, WHITE, WHITE3
-from boilercv.types import Img, ImgLike, T
-
-if DEBUG:
-    from PIL import ImageShow  # noqa: F401
-
-# * -------------------------------------------------------------------------------- * #
-# * PURE NUMPY - TYPE PRESERVING
-
-
-def scale_float(img: T, dtype: npt.DTypeLike = np.uint8) -> T:
-    """Return the input as `dtype` multiplied by the max value of `dtype`.
-
-    Useful for scaling float-valued arrays to integer-valued images.
-    """
-    scaled = (img - img.min()) / (img.max() - img.min())
-    return scaled.astype(dtype) * np.iinfo(dtype).max
-
-
-def unpad(img: T, pad_width: int) -> T:
-    """Remove padding from an image."""
-    return img[pad_width:-pad_width, pad_width:-pad_width]
-
-
-# * -------------------------------------------------------------------------------- * #
-# * PURE NUMPY - NOT ALWAYS TYPE PRESERVING
-
-
-def scale_bool(img: Any, dtype: npt.DTypeLike = np.uint8) -> Any:
-    """Return the input as `dtype` multiplied by the max value of `dtype`.
-
-    Useful for functions (such as in OpenCV) which expect numeric bools.
-    """
-    return img.astype(dtype) * np.iinfo(dtype).max
-
-
-# * -------------------------------------------------------------------------------- * #
-# * OTHER - NOT ALWAYS TYPE PRESERVING
-
-FONT = ImageFont.truetype(findfont(FontProperties(family="dejavu sans")), 24)
-PAD = 10
-
-
-def draw_text(image: ImgLike, text: str = "") -> ImgLike:
-    """Draw text in the top-right corner of an image.
-
-    Args:
-        image: Image.
-        text: Text to draw.
-    """
-    if image.ndim == 3:
-        rectangle_fill = BLACK3
-        font_fill = WHITE3
-    else:
-        rectangle_fill = BLACK
-        font_fill = WHITE
-    _, image_width = image.shape[:2]
-    pil_image = Image.fromarray(image)
-    _, _, font_bbox_width, font_bbox_height = FONT.getbbox(text)
-    text_p0 = (image_width - PAD - font_bbox_width, PAD)
-    p0 = (text_p0[0] - PAD, text_p0[1] - PAD)
-    p1 = (text_p0[0] + PAD + font_bbox_width, text_p0[1] + PAD + font_bbox_height)
-    draw = ImageDraw.Draw(pil_image)
-    draw.rectangle((p0, p1), fill=rectangle_fill)
-    draw.text(text_p0, text, font=FONT, fill=font_fill)
-    return np.asarray(pil_image)
-
-
-def overlay(
-    image: ImgLike,
-    overlay: ImgLike,
-    color: tuple[int, int, int] = RED,
-    alpha: float = 0.3,
-) -> Img:
-    """Color an image given an overlay.
-
-    Args:
-        image: Image.
-        overlay: Overlay image.
-        color: Color for the overlay.
-        alpha: Alpha value for the overlay. Range: 0-1
-    """
-    background = Image.fromarray(image).convert("RGBA")
-    objects = Image.fromarray(overlay)
-    if overlay.ndim == 1:
-        objects = ImageOps.colorize(objects, WHITE3, color)
-        mask = Image.fromarray(~(overlay * alpha).astype(np.uint8))
-    else:
-        mask = Image.fromarray(~(np.mean(overlay, axis=-1) * alpha).astype(np.uint8))
-    composite = Image.composite(background, objects, mask)
-    return np.asarray(composite)
+"""Image acquisition and processing."""
+
+# * Pure numpy image processing functions take lots of types, including DataArrays.
+# pyright: reportGeneralTypeIssues=none
+
+from typing import Any
+
+import numpy as np
+from matplotlib.font_manager import FontProperties, findfont
+from numpy import typing as npt
+from PIL import Image, ImageDraw, ImageFont, ImageOps
+
+from boilercv import DEBUG
+from boilercv.colors import BLACK, BLACK3, RED, WHITE, WHITE3
+from boilercv.types import Img, ImgLike, T
+
+if DEBUG:
+    from PIL import ImageShow  # noqa: F401
+
+# * -------------------------------------------------------------------------------- * #
+# * PURE NUMPY - TYPE PRESERVING
+
+
+def scale_float(img: T, dtype: npt.DTypeLike = np.uint8) -> T:
+    """Return the input as `dtype` multiplied by the max value of `dtype`.
+
+    Useful for scaling float-valued arrays to integer-valued images.
+    """
+    scaled = (img - img.min()) / (img.max() - img.min())
+    return scaled.astype(dtype) * np.iinfo(dtype).max
+
+
+def unpad(img: T, pad_width: int) -> T:
+    """Remove padding from an image."""
+    return img[pad_width:-pad_width, pad_width:-pad_width]
+
+
+# * -------------------------------------------------------------------------------- * #
+# * PURE NUMPY - NOT ALWAYS TYPE PRESERVING
+
+
+def scale_bool(img: Any, dtype: npt.DTypeLike = np.uint8) -> Any:
+    """Return the input as `dtype` multiplied by the max value of `dtype`.
+
+    Useful for functions (such as in OpenCV) which expect numeric bools.
+    """
+    return img.astype(dtype) * np.iinfo(dtype).max
+
+
+# * -------------------------------------------------------------------------------- * #
+# * OTHER - NOT ALWAYS TYPE PRESERVING
+
+FONT = ImageFont.truetype(findfont(FontProperties(family="dejavu sans")), 24)
+PAD = 10
+
+
+def draw_text(image: ImgLike, text: str = "") -> ImgLike:
+    """Draw text in the top-right corner of an image.
+
+    Args:
+        image: Image.
+        text: Text to draw.
+    """
+    if image.ndim == 3:
+        rectangle_fill = BLACK3
+        font_fill = WHITE3
+    else:
+        rectangle_fill = BLACK
+        font_fill = WHITE
+    _, image_width = image.shape[:2]
+    pil_image = Image.fromarray(image)
+    _, _, font_bbox_width, font_bbox_height = FONT.getbbox(text)
+    text_p0 = (image_width - PAD - font_bbox_width, PAD)
+    p0 = (text_p0[0] - PAD, text_p0[1] - PAD)
+    p1 = (text_p0[0] + PAD + font_bbox_width, text_p0[1] + PAD + font_bbox_height)
+    draw = ImageDraw.Draw(pil_image)
+    draw.rectangle((p0, p1), fill=rectangle_fill)
+    draw.text(text_p0, text, font=FONT, fill=font_fill)
+    return np.asarray(pil_image)
+
+
+def overlay(
+    image: ImgLike,
+    overlay: ImgLike,
+    color: tuple[int, int, int] = RED,
+    alpha: float = 0.3,
+) -> Img:
+    """Color an image given an overlay.
+
+    Args:
+        image: Image.
+        overlay: Overlay image.
+        color: Color for the overlay.
+        alpha: Alpha value for the overlay. Range: 0-1
+    """
+    background = Image.fromarray(image).convert("RGBA")
+    objects = Image.fromarray(overlay)
+    if overlay.ndim == 2:
+        objects = ImageOps.colorize(objects, WHITE3, color)
+        mask = Image.fromarray(~(overlay * alpha).astype(np.uint8))
+    else:
+        mask = Image.fromarray(
+            ~(bool(np.mean(overlay, axis=-1)) * alpha).astype(np.uint8)
+        )
+    composite = Image.composite(background, objects, mask)
+    return np.asarray(composite)
```

### Comparing `boilercv-0.0.0/src/boilercv/images/cv.py` & `boilercv-0.0.1/src/boilercv/images/cv.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from collections.abc import Sequence
-
-import cv2 as cv
-import numpy as np
-
-from boilercv.colors import WHITE, WHITE3
-from boilercv.images import unpad
-from boilercv.types import ArrFloat, ArrInt, Img, ImgBool
-
-
-def convert_image(img: Img, code: int | None = None) -> Img:
-    """Convert image format, handling inconsistent type annotations."""
-    return cv.cvtColor(img, code)  # type: ignore
-
-
-def apply_mask(img: Img, mask: Img) -> Img:
-    """Mask an image, keeping parts where the mask is bright."""
-    return cv.add(img, cv.bitwise_not(mask))
-
-
-def pad(img: Img, pad_width: int, value: int) -> Img:
-    """Pad an image. Faster than np.pad()."""
-    return cv.copyMakeBorder(
-        img,
-        top=pad_width,
-        bottom=pad_width,
-        left=pad_width,
-        right=pad_width,
-        borderType=cv.BORDER_CONSTANT,
-        value=value,
-    )
-
-
-def binarize(img: Img, block_size: int = 11, thresh_dist_from_mean: int = 2) -> ImgBool:
-    """Binarize an image with an adaptive threshold."""
-    block_size += 1 if block_size % 2 == 0 else 0
-    return cv.adaptiveThreshold(
-        src=img,
-        maxValue=np.iinfo(img.dtype).max,
-        adaptiveMethod=cv.ADAPTIVE_THRESH_MEAN_C,
-        thresholdType=cv.THRESH_BINARY,
-        blockSize=block_size,
-        C=thresh_dist_from_mean,
-    ).astype(bool)
-
-
-def flood(img: Img) -> ImgBool:
-    """Flood the image, returning the resulting flood as a bright mask."""
-    seed_point = np.array(img.shape) // 2
-    max_value = np.iinfo(img.dtype).max
-    # OpenCV needs a masked array with a one-pixel pad
-    pad_width = 1
-    mask = pad(np.zeros_like(img), pad_width, value=1)
-    _retval, _image, mask, _rect = cv.floodFill(
-        image=img,
-        mask=mask,
-        seedPoint=seed_point,
-        newVal=None,  # Ignored in mask only mode
-        flags=cv.FLOODFILL_MASK_ONLY,
-    )
-    # Return the mask in original dimensions
-    return unpad(mask, pad_width).astype(bool)
-
-
-def get_roi(wall: Img) -> Img:
-    """Erode the wall to get the ROI."""
-    kernel_size = 9
-    close_kernel_size = 4
-    kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, [kernel_size] * 2)
-    close_kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, [close_kernel_size] * 2)
-    # Explicitly pad out the image since cv.morphologyEx boundary handling is weird
-    pad_width = max(close_kernel_size, kernel_size)
-    padded = pad(wall, pad_width, value=0)
-    wall = cv.morphologyEx(src=padded, op=cv.MORPH_CLOSE, kernel=close_kernel)
-    roi = cv.morphologyEx(src=wall, op=cv.MORPH_ERODE, kernel=kernel)
-    return unpad(roi, pad_width).astype(bool)
-
-
-def get_wall(roi: Img) -> Img:
-    """Dilate the ROI to get the wall."""
-    # Explicitly pad out the image since cv.morphologyEx boundary handling is weird
-    kernel_size = 9
-    kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, [kernel_size] * 2)
-    pad_width = kernel_size
-    padded = pad(roi, pad_width, value=0)
-    wall = cv.morphologyEx(src=padded, op=cv.MORPH_DILATE, kernel=kernel)
-    return unpad(wall, pad_width).astype(bool)
-
-
-def build_mask_from_polygons(img: Img, contours: Sequence[ArrInt]) -> Img:
-    """Build a mask from the intersection of a sequence of polygonal contours."""
-    # OpenCV expects contours as shape (N, 1, 2) instead of (N, 2)
-    contours = [np.fliplr(contour).reshape(-1, 1, 2) for contour in contours]
-    blank = np.zeros_like(img)
-    return cv.fillPoly(
-        img=blank,
-        pts=contours,  # Expects a list of coordinates, we have just one
-        color=WHITE3,
-    )
-
-
-def find_contours(img: Img, method: int = cv.CHAIN_APPROX_NONE) -> list[ArrInt]:
-    """Find external contours of bright objects in an image."""
-    contours, _hierarchy = cv.findContours(
-        image=img,
-        mode=cv.RETR_EXTERNAL,  # No hierarchy needed because we keep external contours
-        method=method,
-    )
-    # Despite images having dims (y, x) and shape (h, w), OpenCV returns contours with
-    # dims (point, 1, pair), where dim "pair" has coords (x, y).
-    contours = [np.fliplr(contour.reshape(-1, 2)) for contour in contours]
-    return contours
-
-
-def draw_contours(
-    img: Img,
-    contours: Sequence[ArrInt],
-    contour_index: int = -1,
-    thickness: int = -1,
-    color: int | tuple[int, ...] = WHITE,
-) -> Img:
-    """Draw contours on an image."""
-    # OpenCV expects contours as shape (N, 1, 2) instead of (N, 2)
-    contours = [np.fliplr(contour).reshape(-1, 1, 2) for contour in contours]
-    return cv.drawContours(
-        image=img,
-        contours=contours,
-        contourIdx=contour_index,
-        color=color,
-        thickness=thickness,
-    )
-
-
-def find_line_segments(img: Img) -> tuple[ArrFloat, cv.LineSegmentDetector]:
-    """Find line segments in an image."""
-    lsd = cv.createLineSegmentDetector()
-    lines, *_ = lsd.detect(img)
-    # OpenCV returns line segments as shape (N, 1, 4) instead of (N, 4)
-    lines = lines.reshape(-1, 4)
-    return lines, lsd
+from collections.abc import Sequence
+
+import cv2 as cv
+import numpy as np
+
+from boilercv.colors import WHITE, WHITE3
+from boilercv.images import unpad
+from boilercv.types import ArrFloat, ArrInt, Img, ImgBool
+
+
+def convert_image(img: Img, code: int | None = None) -> Img:
+    """Convert image format, handling inconsistent type annotations."""
+    return cv.cvtColor(img, code)  # type: ignore
+
+
+def apply_mask(img: Img, mask: Img) -> Img:
+    """Mask an image, keeping parts where the mask is bright."""
+    return cv.add(img, cv.bitwise_not(mask))
+
+
+def pad(img: Img, pad_width: int, value: int) -> Img:
+    """Pad an image. Faster than np.pad()."""
+    return cv.copyMakeBorder(
+        img,
+        top=pad_width,
+        bottom=pad_width,
+        left=pad_width,
+        right=pad_width,
+        borderType=cv.BORDER_CONSTANT,
+        value=value,
+    )
+
+
+def binarize(img: Img, block_size: int = 11, thresh_dist_from_mean: int = 2) -> ImgBool:
+    """Binarize an image with an adaptive threshold."""
+    block_size += 1 if block_size % 2 == 0 else 0
+    return cv.adaptiveThreshold(
+        src=img,
+        maxValue=np.iinfo(img.dtype).max,
+        adaptiveMethod=cv.ADAPTIVE_THRESH_MEAN_C,
+        thresholdType=cv.THRESH_BINARY,
+        blockSize=block_size,
+        C=thresh_dist_from_mean,
+    ).astype(bool)
+
+
+def flood(img: Img) -> ImgBool:
+    """Flood the image, returning the resulting flood as a bright mask."""
+    seed_point = np.array(img.shape) // 2
+    max_value = np.iinfo(img.dtype).max
+    # OpenCV needs a masked array with a one-pixel pad
+    pad_width = 1
+    mask = pad(np.zeros_like(img), pad_width, value=1)
+    _retval, _image, mask, _rect = cv.floodFill(
+        image=img,
+        mask=mask,
+        seedPoint=seed_point,
+        newVal=None,  # Ignored in mask only mode
+        flags=cv.FLOODFILL_MASK_ONLY,
+    )
+    # Return the mask in original dimensions
+    return unpad(mask, pad_width).astype(bool)
+
+
+def get_roi(wall: Img) -> Img:
+    """Erode the wall to get the ROI."""
+    kernel_size = 9
+    close_kernel_size = 4
+    kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, [kernel_size] * 2)
+    close_kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, [close_kernel_size] * 2)
+    # Explicitly pad out the image since cv.morphologyEx boundary handling is weird
+    pad_width = max(close_kernel_size, kernel_size)
+    padded = pad(wall, pad_width, value=0)
+    wall = cv.morphologyEx(src=padded, op=cv.MORPH_CLOSE, kernel=close_kernel)
+    roi = cv.morphologyEx(src=wall, op=cv.MORPH_ERODE, kernel=kernel)
+    return unpad(roi, pad_width).astype(bool)
+
+
+def get_wall(roi: Img) -> Img:
+    """Dilate the ROI to get the wall."""
+    # Explicitly pad out the image since cv.morphologyEx boundary handling is weird
+    kernel_size = 9
+    kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, [kernel_size] * 2)
+    pad_width = kernel_size
+    padded = pad(roi, pad_width, value=0)
+    wall = cv.morphologyEx(src=padded, op=cv.MORPH_DILATE, kernel=kernel)
+    return unpad(wall, pad_width).astype(bool)
+
+
+def build_mask_from_polygons(img: Img, contours: Sequence[ArrInt]) -> Img:
+    """Build a mask from the intersection of a sequence of polygonal contours."""
+    # OpenCV expects contours as shape (N, 1, 2) instead of (N, 2)
+    contours = [np.fliplr(contour).reshape(-1, 1, 2) for contour in contours]
+    blank = np.zeros_like(img)
+    return cv.fillPoly(
+        img=blank,
+        pts=contours,  # Expects a list of coordinates, we have just one
+        color=WHITE3,
+    )
+
+
+def find_contours(img: Img, method: int = cv.CHAIN_APPROX_NONE) -> list[ArrInt]:
+    """Find external contours of bright objects in an image."""
+    contours, _hierarchy = cv.findContours(
+        image=img,
+        mode=cv.RETR_EXTERNAL,  # No hierarchy needed because we keep external contours
+        method=method,
+    )
+    # Despite images having dims (y, x) and shape (h, w), OpenCV returns contours with
+    # dims (point, 1, pair), where dim "pair" has coords (x, y).
+    contours = [np.fliplr(contour.reshape(-1, 2)) for contour in contours]
+    return contours
+
+
+def draw_contours(
+    img: Img,
+    contours: Sequence[ArrInt],
+    contour_index: int = -1,
+    thickness: int = -1,
+    color: int | tuple[int, ...] = WHITE,
+) -> Img:
+    """Draw contours on an image."""
+    # OpenCV expects contours as shape (N, 1, 2) instead of (N, 2)
+    contours = [np.fliplr(contour).reshape(-1, 1, 2) for contour in contours]
+    return cv.drawContours(
+        image=img,
+        contours=contours,
+        contourIdx=contour_index,
+        color=color,
+        thickness=thickness,
+    )
+
+
+def find_line_segments(img: Img) -> tuple[ArrFloat, cv.LineSegmentDetector]:
+    """Find line segments in an image."""
+    lsd = cv.createLineSegmentDetector()
+    lines, *_ = lsd.detect(img)
+    # OpenCV returns line segments as shape (N, 1, 4) instead of (N, 4)
+    lines = lines.reshape(-1, 4)
+    return lines, lsd
```

### Comparing `boilercv-0.0.0/src/boilercv/manual/binarize.py` & `boilercv-0.0.1/src/boilercv/manual/binarize.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""Binarize all videos and export their ROIs."""
-
-import xarray as xr
-from loguru import logger
-
-from boilercv.data import FRAME, ROI, VIDEO, apply_to_img_da
-from boilercv.data.packing import pack
-from boilercv.images import scale_bool
-from boilercv.images.cv import apply_mask, binarize, flood, get_roi
-from boilercv.models.params import LOCAL_PATHS, PARAMS
-from boilercv.models.paths import get_sorted_paths
-from boilercv.types import DA
-
-
-def main():
-    logger.info("start binarize")
-    for source in get_sorted_paths(LOCAL_PATHS.large_sources):
-        destination = PARAMS.paths.sources / f"{source.stem}.nc"
-        if destination.exists():
-            continue
-        with xr.open_dataset(source) as ds:
-            video = ds[VIDEO]
-            maximum = video.max(FRAME)
-            flooded: DA = apply_to_img_da(flood, maximum)
-            roi: DA = apply_to_img_da(get_roi, scale_bool(flooded))
-            masked: DA = apply_to_img_da(
-                apply_mask, video, scale_bool(roi), vectorize=True
-            )
-            binarized: DA = apply_to_img_da(binarize, masked, vectorize=True)
-            ds[VIDEO] = pack(binarized)
-            ds.to_netcdf(
-                path=PARAMS.paths.sources / source.name,
-                encoding={VIDEO: {"zlib": True}},
-            )
-            ds[ROI] = roi
-            ds = ds.drop_vars(VIDEO)
-            ds.to_netcdf(path=PARAMS.paths.rois / source.name)
-    logger.info("finish binarize")
-
-
-if __name__ == "__main__":
-    main()
+"""Binarize all videos and export their ROIs."""
+
+import xarray as xr
+from loguru import logger
+
+from boilercv.data import FRAME, ROI, VIDEO, apply_to_img_da
+from boilercv.data.packing import pack
+from boilercv.images import scale_bool
+from boilercv.images.cv import apply_mask, binarize, flood, get_roi
+from boilercv.models.params import LOCAL_PATHS, PARAMS
+from boilercv.models.paths import get_sorted_paths
+from boilercv.types import DA
+
+
+def main():
+    logger.info("start binarize")
+    for source in get_sorted_paths(LOCAL_PATHS.large_sources):
+        destination = PARAMS.paths.sources / f"{source.stem}.nc"
+        if destination.exists():
+            continue
+        with xr.open_dataset(source) as ds:
+            video = ds[VIDEO]
+            maximum = video.max(FRAME)
+            flooded: DA = apply_to_img_da(flood, maximum)
+            roi: DA = apply_to_img_da(get_roi, scale_bool(flooded))
+            masked: DA = apply_to_img_da(
+                apply_mask, video, scale_bool(roi), vectorize=True
+            )
+            binarized: DA = apply_to_img_da(binarize, masked, vectorize=True)
+            ds[VIDEO] = pack(binarized)
+            ds.to_netcdf(
+                path=PARAMS.paths.sources / source.name,
+                encoding={VIDEO: {"zlib": True}},
+            )
+            ds[ROI] = roi
+            ds = ds.drop_vars(VIDEO)
+            ds.to_netcdf(path=PARAMS.paths.rois / source.name)
+    logger.info("finish binarize")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/manual/decompress.py` & `boilercv-0.0.1/src/boilercv/manual/decompress.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""Decompress sources to local storage."""
-
-
-import xarray as xr
-from loguru import logger
-
-from boilercv.data import HEADER, VIDEO
-from boilercv.data.sets import ALL_NAMES
-from boilercv.models.params import LOCAL_PATHS, PARAMS
-
-
-def main():
-    logger.info("start decompress")
-    for source_name in ALL_NAMES:
-        destination = LOCAL_PATHS.uncompressed_sources / f"{source_name}.nc"
-        if destination.exists():
-            continue
-        source = PARAMS.paths.sources / f"{source_name}.nc"
-        with xr.open_dataset(source) as ds:
-            xr.Dataset({VIDEO: ds[VIDEO], HEADER: ds[HEADER]}).to_netcdf(destination)
-    logger.info("finish decompress")
-
-
-if __name__ == "__main__":
-    main()
+"""Decompress sources to local storage."""
+
+
+import xarray as xr
+from loguru import logger
+
+from boilercv.data import HEADER, VIDEO
+from boilercv.data.sets import ALL_NAMES
+from boilercv.models.params import LOCAL_PATHS, PARAMS
+
+
+def main():
+    logger.info("start decompress")
+    for source_name in ALL_NAMES:
+        destination = LOCAL_PATHS.uncompressed_sources / f"{source_name}.nc"
+        if destination.exists():
+            continue
+        source = PARAMS.paths.sources / f"{source_name}.nc"
+        with xr.open_dataset(source) as ds:
+            xr.Dataset({VIDEO: ds[VIDEO], HEADER: ds[HEADER]}).to_netcdf(destination)
+    logger.info("finish decompress")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/manual/rename.py` & `boilercv-0.0.1/src/boilercv/manual/rename.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""Flatten the data directory structure.
-
-The directory structure looks like:
-
-    data
-    └───YYYY-MM-DD
-        ├───data
-        ├───notes
-        └───video
-"""
-
-from itertools import chain
-
-from boilercv.models.params import LOCAL_PATHS
-
-
-def main():
-    source = LOCAL_PATHS.hierarchical_data
-    rename_notes(source)
-    rename_cines(source)
-    rename_sheets(source)
-
-
-def rename_notes(source):
-    notes_dest = LOCAL_PATHS.notes
-    notes_dirs = {
-        trial.stem: trial / "notes"
-        for trial in sorted(source.iterdir())
-        if trial.is_dir()
-    }
-    for trial, note_dir in notes_dirs.items():
-        if not note_dir.exists():
-            continue
-        note_dir.rename(notes_dest / trial)
-
-
-def rename_cines(source):
-    destination = LOCAL_PATHS.cines
-    trials = [trial / "video" for trial in source.iterdir() if trial.is_dir()]
-    videos = chain.from_iterable(trial.glob("*.cine") for trial in trials)
-    for video in videos:
-        video.rename(destination / video.name.removeprefix("results_"))
-
-
-def rename_sheets(source):
-    sheets_dest = LOCAL_PATHS.sheets
-    data = [trial / "data" for trial in sorted(source.iterdir()) if trial.is_dir()]
-    sheets = chain.from_iterable(trial.glob("*.csv") for trial in data)
-    for sheet in sheets:
-        sheet.rename(sheets_dest / sheet.name.removeprefix("results_"))
-
-
-if __name__ == "__main__":
-    main()
+"""Flatten the data directory structure.
+
+The directory structure looks like:
+
+    data
+    └───YYYY-MM-DD
+        ├───data
+        ├───notes
+        └───video
+"""
+
+from itertools import chain
+
+from boilercv.models.params import LOCAL_PATHS
+
+
+def main():
+    source = LOCAL_PATHS.hierarchical_data
+    rename_notes(source)
+    rename_cines(source)
+    rename_sheets(source)
+
+
+def rename_notes(source):
+    notes_dest = LOCAL_PATHS.notes
+    notes_dirs = {
+        trial.stem: trial / "notes"
+        for trial in sorted(source.iterdir())
+        if trial.is_dir()
+    }
+    for trial, note_dir in notes_dirs.items():
+        if not note_dir.exists():
+            continue
+        note_dir.rename(notes_dest / trial)
+
+
+def rename_cines(source):
+    destination = LOCAL_PATHS.cines
+    trials = [trial / "video" for trial in source.iterdir() if trial.is_dir()]
+    videos = chain.from_iterable(trial.glob("*.cine") for trial in trials)
+    for video in videos:
+        video.rename(destination / video.name.removeprefix("results_"))
+
+
+def rename_sheets(source):
+    sheets_dest = LOCAL_PATHS.sheets
+    data = [trial / "data" for trial in sorted(source.iterdir()) if trial.is_dir()]
+    sheets = chain.from_iterable(trial.glob("*.csv") for trial in data)
+    for sheet in sheets:
+        sheet.rename(sheets_dest / sheet.name.removeprefix("results_"))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/models/__init__.py` & `boilercv-0.0.1/src/boilercv/models/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from pathlib import Path
-from typing import TypeVar
-
-import yaml
-from pydantic import BaseModel, Extra, MissingError, ValidationError
-
-PARAMS_FILE = Path("params.yaml")
-
-BaseModel_T = TypeVar("BaseModel_T", bound=BaseModel)
-
-
-class MyBaseModel(BaseModel):
-    """Base model and configuration for all models used in this project."""
-
-    class Config:
-        """Model configuration. Allow arbitrary types. Enables Numpy types in fields."""
-
-        # Don't specify as class kwargs for easier overriding, and "extra" acted weird.
-        extra = Extra.forbid  # To forbid extra fields
-
-
-# Can't type annotate `model` for some reason
-def load_config(path: Path, model: type[BaseModel_T]) -> BaseModel_T:
-    """Load a YAML file into a Pydantic model.
-
-    Given a path to a YAML file, automatically unpack its fields into the provided
-    Pydantic model.
-
-    Args:
-        path: The path to a YAML file.
-        model: The model class to pass the contents of the YAML file.
-
-    Returns:
-        An instance of the model after validation.
-
-    Raises:
-        ValueError: If an improper path is passed.
-        ValidationError: If a field is undefined in the configuration file.
-    """
-    if path.suffix != ".yaml":
-        raise ValueError(f"The path '{path}' does not refer to a YAML file.")
-    raw_config = yaml.safe_load(path.read_text(encoding="utf-8"))
-    if not raw_config:
-        raise ValueError("The configuration file is empty.")
-    try:
-        config = model(**{key: raw_config.get(key) for key in raw_config})
-    except ValidationError as exception:
-        addendum = "\n  The field may be undefined in the configuration file."
-        for error in exception.errors():
-            if error["msg"] == MissingError.msg_template:
-                error["msg"] += addendum
-        raise
-    return config
-
-
-def dump_model(path: Path, model: BaseModel):
-    """Dump a Pydantic model to a YAML file.
-
-    Given a path to a YAML file, write a Pydantic model to the file. Optionally add a
-    schema directive at the top of the file. Create the file if it doesn't exist.
-
-    Args:
-        path: The path to a YAML file. Will create it if it doesn't exist.
-        model: An instance of the Pydantic model to dump.
-    """
-    path = Path(path)
-    # ensure one \n and no leading \n, Pydantic sometimes does more
-    path.write_text(
-        encoding="utf-8",
-        data=yaml.safe_dump(model.dict(exclude_none=True), sort_keys=False),
-    )
-
-
-def write_schema(path: Path, model: type[BaseModel]):
-    """Write a Pydantic model schema to a JSON file.
-
-    Given a path to a JSON file, write a Pydantic model schema to the file. Create the
-    file if it doesn't exist.
-
-    Args:
-        path: The path to a JSON file. Will create it if it doesn't exist.
-        model: The Pydantic model class to get the schema from.
-    """
-    if path.suffix != ".json":
-        raise ValueError(f"The path '{path}' does not refer to a JSON file.")
-    path.write_text(model.schema_json(indent=2) + "\n", encoding="utf-8")
+from pathlib import Path
+from typing import TypeVar
+
+import yaml
+from pydantic import BaseModel, Extra, MissingError, ValidationError
+
+PARAMS_FILE = Path("params.yaml")
+
+BaseModel_T = TypeVar("BaseModel_T", bound=BaseModel)
+
+
+class MyBaseModel(BaseModel):
+    """Base model and configuration for all models used in this project."""
+
+    class Config:
+        """Model configuration. Allow arbitrary types. Enables Numpy types in fields."""
+
+        # Don't specify as class kwargs for easier overriding, and "extra" acted weird.
+        extra = Extra.forbid  # To forbid extra fields
+
+
+# Can't type annotate `model` for some reason
+def load_config(path: Path, model: type[BaseModel_T]) -> BaseModel_T:
+    """Load a YAML file into a Pydantic model.
+
+    Given a path to a YAML file, automatically unpack its fields into the provided
+    Pydantic model.
+
+    Args:
+        path: The path to a YAML file.
+        model: The model class to pass the contents of the YAML file.
+
+    Returns:
+        An instance of the model after validation.
+
+    Raises:
+        ValueError: If an improper path is passed.
+        ValidationError: If a field is undefined in the configuration file.
+    """
+    if path.suffix != ".yaml":
+        raise ValueError(f"The path '{path}' does not refer to a YAML file.")
+    raw_config = yaml.safe_load(path.read_text(encoding="utf-8"))
+    if not raw_config:
+        raise ValueError("The configuration file is empty.")
+    try:
+        config = model(**{key: raw_config.get(key) for key in raw_config})
+    except ValidationError as exception:
+        addendum = "\n  The field may be undefined in the configuration file."
+        for error in exception.errors():
+            if error["msg"] == MissingError.msg_template:
+                error["msg"] += addendum
+        raise
+    return config
+
+
+def dump_model(path: Path, model: BaseModel):
+    """Dump a Pydantic model to a YAML file.
+
+    Given a path to a YAML file, write a Pydantic model to the file. Optionally add a
+    schema directive at the top of the file. Create the file if it doesn't exist.
+
+    Args:
+        path: The path to a YAML file. Will create it if it doesn't exist.
+        model: An instance of the Pydantic model to dump.
+    """
+    path = Path(path)
+    # ensure one \n and no leading \n, Pydantic sometimes does more
+    path.write_text(
+        encoding="utf-8",
+        data=yaml.safe_dump(model.dict(exclude_none=True), sort_keys=False),
+    )
+
+
+def write_schema(path: Path, model: type[BaseModel]):
+    """Write a Pydantic model schema to a JSON file.
+
+    Given a path to a JSON file, write a Pydantic model schema to the file. Create the
+    file if it doesn't exist.
+
+    Args:
+        path: The path to a JSON file. Will create it if it doesn't exist.
+        model: The Pydantic model class to get the schema from.
+    """
+    if path.suffix != ".json":
+        raise ValueError(f"The path '{path}' does not refer to a JSON file.")
+    path.write_text(model.schema_json(indent=2) + "\n", encoding="utf-8")
```

### Comparing `boilercv-0.0.0/src/boilercv/models/paths.py` & `boilercv-0.0.1/src/boilercv/models/paths.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,151 +1,152 @@
-"""Paths for this project."""
-
-from pathlib import Path
-from typing import Any
-
-from pydantic import DirectoryPath, FilePath, validator
-from ruamel.yaml import YAML
-
-from boilercv.models import PARAMS_FILE, MyBaseModel
-
-
-def init():
-    """Synchronize project paths. Run on initial import of this module."""
-    yaml = YAML()
-    yaml.indent(offset=2)
-    paths = Paths()
-    params = yaml.load(paths.file_params) or {}
-    params["paths"] = repl_path(paths.dict(exclude_none=True))
-    yaml.dump(params, paths.file_params)
-
-
-def repl_path(dirs_dict: dict[str, Path]):
-    """Replace Windows path separator with POSIX separator."""
-    return {k: str(v).replace("\\", "/") for k, v in dirs_dict.items()}
-
-
-def get_sorted_paths(path: Path) -> list[Path]:
-    """Iterate over a sorted directory."""
-    return sorted(path.iterdir())
-
-
-class LocalPaths(MyBaseModel):
-    """Local paths for larger files not stored in the cloud."""
-
-    data: DirectoryPath = Path("~").expanduser() / ".local/boilercv"
-    hierarchical_data: DirectoryPath = data / "data"
-
-    large_examples: DirectoryPath = data / "large_examples"
-    large_sources: DirectoryPath = data / "large_sources"
-    notes: DirectoryPath = data / "notes"
-    sheets: DirectoryPath = data / "sheets"
-    uncompressed_contours: DirectoryPath = data / "uncompressed_contours"
-    uncompressed_filled: DirectoryPath = data / "uncompressed_filled"
-    uncompressed_sources: DirectoryPath = data / "uncompressed_sources"
-
-    cines: DirectoryPath = data / "cines"
-    large_example_cine: Path = cines / "2022-01-06T16-57-31.cine"
-
-    media: Path = Path("G:/My Drive/Blake/School/Grad/Reports/Content/boilercv")
-
-    # "always" so it'll run even if not in YAML
-    # "pre" because dir must exist pre-validation
-    @validator(
-        "hierarchical_data",
-        "large_examples",
-        "large_sources",
-        "notes",
-        "sheets",
-        "uncompressed_contours",
-        "uncompressed_filled",
-        "uncompressed_sources",
-        "cines",
-        always=True,
-        pre=True,
-    )
-    def validate_output_directories(cls, directory: Path) -> Path:
-        """Re-create designated output directories each run, for reproducibility."""
-        directory = Path(directory)
-        directory.mkdir(parents=True, exist_ok=True)
-        return directory
-
-
-class Paths(MyBaseModel):
-    """Directories relevant to the project."""
-
-    class Config(MyBaseModel.Config):
-        @staticmethod
-        def schema_extra(schema: dict[str, Any]):
-            for prop in schema.get("properties", {}).values():
-                default = prop.get("default")
-                if isinstance(default, str):
-                    prop["default"] = default.replace("\\", "/")
-
-    # ! PARAMS FILE
-    file_params: FilePath = PARAMS_FILE
-
-    # ! REQUIREMENTS
-    requirements: FilePath = Path("requirements.txt")
-    dev_requirements: DirectoryPath = Path(".tools/requirements")
-
-    # ! PACKAGE
-    package: DirectoryPath = Path("src") / "boilercv"
-    stages: DirectoryPath = package / "stages"
-    models: DirectoryPath = package / "models"
-    paths_module: FilePath = models / "paths.py"
-
-    # ! STAGES
-    stage_check_cv: FilePath = stages / "check_cv.py"
-    stage_contours: FilePath = stages / "contours.py"
-    stage_fill: FilePath = stages / "fill.py"
-    stage_schema: FilePath = stages / "schema.py"
-
-    # ! PREVIEW STAGES
-    update_previews: DirectoryPath = stages / "update_previews"
-    stage_binarized_preview: FilePath = update_previews / "binarized.py"
-    stage_gray_preview: FilePath = update_previews / "gray.py"
-    stage_filled_preview: FilePath = update_previews / "filled.py"
-
-    # ! DATA
-    data: DirectoryPath = Path("data")
-    contours: DirectoryPath = data / "contours"
-    examples: DirectoryPath = data / "examples"
-    filled: DirectoryPath = data / "filled"
-    rois: DirectoryPath = data / "rois"
-    samples: DirectoryPath = data / "samples"
-    sources: DirectoryPath = data / "sources"
-
-    # ! PREVIEW DATA
-    previews: DirectoryPath = data / "previews"
-    binarized_preview: Path = previews / "binarized.nc"
-    gray_preview: Path = previews / "gray.nc"
-    filled_preview: Path = previews / "filled.nc"
-
-    # ! SCHEMA
-    # Can't be "schema", which is a special member of BaseClass
-    project_schema: DirectoryPath = data / "schema"
-
-    # "always" so it'll run even if not in YAML
-    # "pre" because dir must exist pre-validation
-    @validator(
-        "contours",
-        "examples",
-        "filled",
-        "rois",
-        "samples",
-        "sources",
-        "previews",
-        "project_schema",
-        always=True,
-        pre=True,
-    )
-    def validate_output_directories(cls, directory: Path) -> Path:
-        """Re-create designated output directories each run, for reproducibility."""
-        directory = Path(directory)
-        directory.mkdir(parents=True, exist_ok=True)
-        return directory
-
-
-# * -------------------------------------------------------------------------------- * #
-
-init()
+"""Paths for this project."""
+
+from pathlib import Path
+from typing import Any
+
+from pydantic import DirectoryPath, FilePath, validator
+from ruamel.yaml import YAML
+
+from boilercv.models import PARAMS_FILE, MyBaseModel
+
+LOCAL_MEDIA = "G:/My Drive/Blake/School/Grad/Reports/Content/boilercv"
+
+
+def init():
+    """Synchronize project paths. Run on initial import of this module."""
+    yaml = YAML()
+    yaml.indent(offset=2)
+    paths = Paths()
+    params = yaml.load(paths.file_params) or {}
+    params["paths"] = repl_path(paths.dict(exclude_none=True))
+    yaml.dump(params, paths.file_params)
+
+
+def repl_path(dirs_dict: dict[str, Path]):
+    """Replace Windows path separator with POSIX separator."""
+    return {k: str(v).replace("\\", "/") for k, v in dirs_dict.items()}
+
+
+def get_sorted_paths(path: Path) -> list[Path]:
+    """Iterate over a sorted directory."""
+    return sorted(path.iterdir())
+
+
+class LocalPaths(MyBaseModel):
+    """Local paths for larger files not stored in the cloud."""
+
+    data: DirectoryPath = Path("~").expanduser() / ".local/boilercv"
+    hierarchical_data: DirectoryPath = data / "data"
+
+    large_examples: DirectoryPath = data / "large_examples"
+    large_sources: DirectoryPath = data / "large_sources"
+    notes: DirectoryPath = data / "notes"
+    sheets: DirectoryPath = data / "sheets"
+    uncompressed_contours: DirectoryPath = data / "uncompressed_contours"
+    uncompressed_filled: DirectoryPath = data / "uncompressed_filled"
+    uncompressed_sources: DirectoryPath = data / "uncompressed_sources"
+
+    cines: DirectoryPath = data / "cines"
+    large_example_cine: Path = cines / "2022-01-06T16-57-31.cine"
+
+    media: Path = Path(LOCAL_MEDIA)
+
+    # "always" so it'll run even if not in YAML
+    # "pre" because dir must exist pre-validation
+    @validator(
+        "hierarchical_data",
+        "large_examples",
+        "large_sources",
+        "notes",
+        "sheets",
+        "uncompressed_contours",
+        "uncompressed_filled",
+        "uncompressed_sources",
+        "cines",
+        always=True,
+        pre=True,
+    )
+    def validate_output_directories(cls, directory: Path) -> Path:
+        """Re-create designated output directories each run, for reproducibility."""
+        directory = Path(directory)
+        directory.mkdir(parents=True, exist_ok=True)
+        return directory
+
+
+class Paths(MyBaseModel):
+    """Directories relevant to the project."""
+
+    class Config(MyBaseModel.Config):
+        @staticmethod
+        def schema_extra(schema: dict[str, Any]):
+            for prop in schema.get("properties", {}).values():
+                default = prop.get("default")
+                if isinstance(default, str):
+                    prop["default"] = default.replace("\\", "/")
+
+    # ! PARAMS FILE
+    file_params: FilePath = PARAMS_FILE
+
+    # ! REQUIREMENTS
+    requirements: FilePath = Path("requirements.txt")
+    dev_requirements: DirectoryPath = Path(".tools/requirements")
+
+    # ! PACKAGE
+    package: DirectoryPath = Path("src") / "boilercv"
+    stages: DirectoryPath = package / "stages"
+    models: DirectoryPath = package / "models"
+    paths_module: FilePath = models / "paths.py"
+
+    # ! STAGES
+    stage_contours: FilePath = stages / "contours.py"
+    stage_fill: FilePath = stages / "fill.py"
+    stage_schema: FilePath = stages / "schema.py"
+
+    # ! PREVIEW STAGES
+    update_previews: DirectoryPath = stages / "update_previews"
+    stage_binarized_preview: FilePath = update_previews / "binarized.py"
+    stage_gray_preview: FilePath = update_previews / "gray.py"
+    stage_filled_preview: FilePath = update_previews / "filled.py"
+
+    # ! DATA
+    data: DirectoryPath = Path("data")
+    contours: DirectoryPath = data / "contours"
+    examples: DirectoryPath = data / "examples"
+    filled: DirectoryPath = data / "filled"
+    rois: DirectoryPath = data / "rois"
+    samples: DirectoryPath = data / "samples"
+    sources: DirectoryPath = data / "sources"
+
+    # ! PREVIEW DATA
+    previews: DirectoryPath = data / "previews"
+    binarized_preview: Path = previews / "binarized.nc"
+    gray_preview: Path = previews / "gray.nc"
+    filled_preview: Path = previews / "filled.nc"
+
+    # ! SCHEMA
+    # Can't be "schema", which is a special member of BaseClass
+    project_schema: DirectoryPath = data / "schema"
+
+    # "always" so it'll run even if not in YAML
+    # "pre" because dir must exist pre-validation
+    @validator(
+        "contours",
+        "examples",
+        "filled",
+        "rois",
+        "samples",
+        "sources",
+        "previews",
+        "project_schema",
+        always=True,
+        pre=True,
+    )
+    def validate_output_directories(cls, directory: Path) -> Path:
+        """Re-create designated output directories each run, for reproducibility."""
+        directory = Path(directory)
+        directory.mkdir(parents=True, exist_ok=True)
+        return directory
+
+
+# * -------------------------------------------------------------------------------- * #
+
+init()
```

### Comparing `boilercv-0.0.0/src/boilercv/old/_contours.py` & `boilercv-0.0.1/src/boilercv/old/_contours.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-"""Given a CINE, find ROI using `pyqtgraph` and find contours."""
-
-from matplotlib.pyplot import subplot_mosaic
-
-from boilercv.captivate.previews import edit_roi, load_roi, view_images
-from boilercv.examples import EXAMPLE_FRAME_LIST, EXAMPLE_ROI
-from boilercv.images import scale_bool
-from boilercv.images.cv import (
-    apply_mask,
-    binarize,
-    build_mask_from_polygons,
-    draw_contours,
-    find_contours,
-)
-from boilercv.types import ArrInt, Img, ImgBool
-
-
-def main():
-    preview_contours(
-        block_size=11,
-        thresh_dist_from_mean=2,
-        contour_index=-1,
-        thickness=2,
-    )
-
-
-def preview_contours(
-    block_size: int,
-    thresh_dist_from_mean: int,
-    contour_index: int,
-    thickness: int,
-    interact: bool = False,
-) -> list[list[ArrInt]] | None:
-    input_images = [EXAMPLE_FRAME_LIST[0]] if interact else EXAMPLE_FRAME_LIST
-    if interact:
-        roi = load_roi(input_images[0], EXAMPLE_ROI)
-    else:
-        roi = edit_roi(input_images[0], EXAMPLE_ROI)
-    all_contours: list[list[ArrInt]] = []
-    all_masked: list[Img] = []
-    all_thresholded: list[ImgBool] = []
-    contoured: list[Img] = []
-    to_preview = dict(
-        input_images=input_images,
-        all_masked=all_masked,
-        all_thresholded=all_thresholded,
-        contoured=contoured,
-    )
-    for image in input_images:
-        contours, masked, thresholded = _get_contours(
-            image, roi, block_size, thresh_dist_from_mean
-        )
-        all_contours.append(contours)
-        all_masked.append(masked)
-        all_thresholded.append(thresholded)
-        contoured.append(draw_contours(image, contours, contour_index, thickness))
-    if interact:
-        interact_with_images(*[image[0] for image in to_preview.values()])
-    else:
-        view_images(to_preview)
-        return all_contours
-
-
-def _get_contours(
-    input_image: ArrInt,
-    roi: ArrInt,
-    block_size: int,
-    thresh_dist_from_mean: int,
-) -> tuple[list[ArrInt], ArrInt, ImgBool]:
-    masked = apply_mask(input_image, build_mask_from_polygons(input_image, [roi]))
-    thresholded = binarize(masked, block_size, thresh_dist_from_mean)
-    return find_contours(scale_bool(~thresholded)), masked, thresholded
-
-
-def interact_with_images(_input_image, _masked, thresholded, contoured):
-    _plt, ax = subplot_mosaic(
-        [
-            [
-                # "input",
-                # "masked",
-                "thresholded",
-                "contoured",
-            ]
-        ]
-    )
-    for ax_ in ax.values():  # type: ignore
-        ax_.axis("off")
-    # ax["input"].imshow(input_image, cmap="gray")  # type: ignore
-    # ax["masked"].imshow(masked, cmap="gray")  # type: ignore
-    ax["thresholded"].imshow(thresholded, cmap="gray")  # type: ignore
-    ax["contoured"].imshow(contoured, cmap="gray")  # type: ignore
-
-
-if __name__ == "__main__":
-    main()
+"""Given a CINE, find ROI using `pyqtgraph` and find contours."""
+
+from matplotlib.pyplot import subplot_mosaic
+
+from boilercv.captivate.previews import edit_roi, load_roi, view_images
+from boilercv.examples import EXAMPLE_FRAME_LIST, EXAMPLE_ROI
+from boilercv.images import scale_bool
+from boilercv.images.cv import (
+    apply_mask,
+    binarize,
+    build_mask_from_polygons,
+    draw_contours,
+    find_contours,
+)
+from boilercv.types import ArrInt, Img, ImgBool
+
+
+def main():
+    preview_contours(
+        block_size=11,
+        thresh_dist_from_mean=2,
+        contour_index=-1,
+        thickness=2,
+    )
+
+
+def preview_contours(
+    block_size: int,
+    thresh_dist_from_mean: int,
+    contour_index: int,
+    thickness: int,
+    interact: bool = False,
+) -> list[list[ArrInt]] | None:
+    input_images = [EXAMPLE_FRAME_LIST[0]] if interact else EXAMPLE_FRAME_LIST
+    if interact:
+        roi = load_roi(input_images[0], EXAMPLE_ROI)
+    else:
+        roi = edit_roi(input_images[0], EXAMPLE_ROI)
+    all_contours: list[list[ArrInt]] = []
+    all_masked: list[Img] = []
+    all_thresholded: list[ImgBool] = []
+    contoured: list[Img] = []
+    to_preview = dict(
+        input_images=input_images,
+        all_masked=all_masked,
+        all_thresholded=all_thresholded,
+        contoured=contoured,
+    )
+    for image in input_images:
+        contours, masked, thresholded = _get_contours(
+            image, roi, block_size, thresh_dist_from_mean
+        )
+        all_contours.append(contours)
+        all_masked.append(masked)
+        all_thresholded.append(thresholded)
+        contoured.append(draw_contours(image, contours, contour_index, thickness))
+    if interact:
+        interact_with_images(*[image[0] for image in to_preview.values()])
+    else:
+        view_images(to_preview)
+        return all_contours
+
+
+def _get_contours(
+    input_image: ArrInt,
+    roi: ArrInt,
+    block_size: int,
+    thresh_dist_from_mean: int,
+) -> tuple[list[ArrInt], ArrInt, ImgBool]:
+    masked = apply_mask(input_image, build_mask_from_polygons(input_image, [roi]))
+    thresholded = binarize(masked, block_size, thresh_dist_from_mean)
+    return find_contours(scale_bool(~thresholded)), masked, thresholded
+
+
+def interact_with_images(_input_image, _masked, thresholded, contoured):
+    _plt, ax = subplot_mosaic(
+        [
+            [
+                # "input",
+                # "masked",
+                "thresholded",
+                "contoured",
+            ]
+        ]
+    )
+    for ax_ in ax.values():
+        ax_.axis("off")
+    # ax["input"].imshow(input_image, cmap="gray")
+    # ax["masked"].imshow(masked, cmap="gray")
+    ax["thresholded"].imshow(thresholded, cmap="gray")  # type: ignore
+    ax["contoured"].imshow(contoured, cmap="gray")  # type: ignore
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/old/_convert_2021_06.py` & `boilercv-0.0.1/src/boilercv/old/_convert_2021_06.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""Handle weird CINEs from 2021-06 to the end of the year.
-
-There is some state being shared between iterations, with the prior frame count
-poisoning the next iteration. There's probably a caching issue in the CINE reading
-library. Restarting this script after one successful conversion yields another
-successful conversion each time.
-"""
-
-from loguru import logger
-
-from boilercv.data.video import prepare_dataset
-from boilercv.models.params import LOCAL_PATHS
-from boilercv.models.paths import get_sorted_paths
-
-FRAMES = {
-    "2021-06-21T17-06-43": 3089,
-    "2021-08-31T13-59-08": 4411,
-    "2021-08-31T14-25-12": 1338,
-    "2021-08-31T14-56-17": 3330,
-    "2021-08-31T15-13-27": 4176,
-    "2021-10-12T12-52-44": 1820,
-    "2021-10-12T13-57-43": 4337,
-    "2021-10-12T14-37-32": 2368,
-    "2021-10-12T17-03-27": 2892,
-    "2021-10-13T13-10-59": 3650,
-    "2021-12-09T13-04-57": 3455,
-}
-
-
-def main():
-    sources = get_sorted_paths(LOCAL_PATHS.data / "weird")
-    for source in sources:
-        num_frames = FRAMES[source.stem] - 1
-        destination = LOCAL_PATHS.large_sources / f"{source.stem}.nc"
-        if destination.exists():
-            continue
-        try:
-            prepare_dataset(source, num_frames).to_netcdf(path=destination)
-        except Exception:
-            logger.exception(source.stem)
-            continue
-
-
-if __name__ == "__main__":
-    main()
+"""Handle weird CINEs from 2021-06 to the end of the year.
+
+There is some state being shared between iterations, with the prior frame count
+poisoning the next iteration. There's probably a caching issue in the CINE reading
+library. Restarting this script after one successful conversion yields another
+successful conversion each time.
+"""
+
+from loguru import logger
+
+from boilercv.data.video import prepare_dataset
+from boilercv.models.params import LOCAL_PATHS
+from boilercv.models.paths import get_sorted_paths
+
+FRAMES = {
+    "2021-06-21T17-06-43": 3089,
+    "2021-08-31T13-59-08": 4411,
+    "2021-08-31T14-25-12": 1338,
+    "2021-08-31T14-56-17": 3330,
+    "2021-08-31T15-13-27": 4176,
+    "2021-10-12T12-52-44": 1820,
+    "2021-10-12T13-57-43": 4337,
+    "2021-10-12T14-37-32": 2368,
+    "2021-10-12T17-03-27": 2892,
+    "2021-10-13T13-10-59": 3650,
+    "2021-12-09T13-04-57": 3455,
+}
+
+
+def main():
+    sources = get_sorted_paths(LOCAL_PATHS.data / "weird")
+    for source in sources:
+        num_frames = FRAMES[source.stem] - 1
+        destination = LOCAL_PATHS.large_sources / f"{source.stem}.nc"
+        if destination.exists():
+            continue
+        try:
+            prepare_dataset(source, num_frames).to_netcdf(path=destination)
+        except Exception:
+            logger.exception(source.stem)
+            continue
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/old/_detect_surface.py` & `boilercv-0.0.1/src/boilercv/old/_detect_surface.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-"""Old approach to detecting the boiling surface."""
-
-import numpy as np
-import pandas as pd
-
-from boilercv import DEBUG
-from boilercv.captivate.previews import view_images
-from boilercv.data import YX_PX, apply_to_img_da
-from boilercv.data.frames import df_points, frame_lines
-from boilercv.examples.detect_surface import find_boiling_surface
-from boilercv.images.cv import find_contours, find_line_segments
-from boilercv.types import DA, ArrInt
-
-
-def _find_boiling_surface(image: DA, preview: bool = DEBUG) -> ArrInt:
-    """Find the boiling surface."""
-    # Find corners and set index to contour points for later concatenation
-    (height, width) = image.shape
-    corns_ = apply_to_img_da(find_boiling_surface, image)
-    corns = df_points(np.nonzero(corns_.values))
-    corns = (
-        corns.set_index(pd.MultiIndex.from_frame(corns))
-        .drop(axis="columns", labels=YX_PX)
-        .assign(**dict(corner=True))
-    )
-    # Find the contour angles
-    contours = find_contours(image.values)
-    roi_poly_ = contours.pop()
-    roi_poly = df_points(roi_poly_)
-    distances = roi_poly.diff()
-    angles = (
-        pd.Series(np.degrees(np.arctan2(distances.ypx, distances.xpx)))
-        .rolling(window=2)
-        .mean()
-        .bfill()
-    ).rename("deg")
-    # Concatenate contour points with their angles
-    roi_poly = (
-        pd.concat(
-            axis="columns",
-            keys=["dim", "angle"],
-            objs=[roi_poly, angles],
-        )
-        .set_index(pd.MultiIndex.from_frame(roi_poly))
-        .drop(axis="columns", labels="dim")
-    )
-    # Set the index to the contour points and concatenate with corners
-    # Compute distance from midplanes for candidate corner selection
-    roi_poly = roi_poly.set_axis(axis="columns", labels=roi_poly.columns.droplevel(1))
-    corns = (
-        pd.concat(axis="columns", objs=[roi_poly, corns])
-        .dropna()
-        .drop(axis="columns", labels="corner")
-        .sort_index()
-        .reset_index()
-        .assign(
-            **dict(
-                xpx_mid_abs=lambda df: (df.xpx - width / 2).abs(),
-                ypx_mid=lambda df: df.ypx - height / 2,
-            )
-        )
-        .sort_values(axis="index", by="xpx_mid_abs")
-    )
-    # Consider the boiling surface to be described by the two corners with a low enough
-    # angle, below the horizontal midplane, and closest to the vertical midplane
-    max_angle = 30
-    candidates = (
-        corns[
-            (corns.angle > -max_angle) & (corns.angle < max_angle) & (corns.ypx_mid > 0)
-        ]
-        .reset_index(drop=True)
-        .loc[0:1, ["ypx", "xpx"]]
-    )
-    if preview:
-        view_images(dict(corn=corns_.values))
-    # TODO: Save to disk, draw on an image for previewing
-    return candidates.values.flatten()[:2]
-
-
-def _find_boiling_surface2(image):
-    """Get line segments in an image."""
-    lines_, lsd = find_line_segments(image)
-    lined = lsd.drawSegments(image, lines_)
-    lines = frame_lines(lines_)
-    midpoints = df_points([lines.ypx.T.mean(), lines.xpx.T.mean()])
-    distances = df_points([lines.ypx[1] - lines.ypx[0], lines.xpx[1] - lines.xpx[0]])
-    lengths = distances.T.pow(2).sum().pow(1 / 2).rename("px")
-    angles = pd.Series(np.arctan2(distances.ypx, distances.xpx)).rename("deg")
-    lines = (
-        pd.concat(
-            axis="columns",
-            keys=["line", "midpoint", "length", "angle"],
-            objs=[
-                lines.set_axis(axis="columns", labels=["ypx0", "xpx0", "ypx1", "xpx1"]),
-                midpoints,
-                lengths,
-                angles,
-            ],
-        )
-        .rename_axis(axis="index", mapper="line")
-        .rename_axis(axis="columns", mapper=["metric", "dim"])
-    )
-    return lined, lines
+"""Old approach to detecting the boiling surface."""
+
+import numpy as np
+import pandas as pd
+
+from boilercv import DEBUG
+from boilercv.captivate.previews import view_images
+from boilercv.data import YX_PX, apply_to_img_da
+from boilercv.data.frames import df_points, frame_lines
+from boilercv.examples.detect_surface import find_boiling_surface
+from boilercv.images.cv import find_contours, find_line_segments
+from boilercv.types import DA, ArrInt
+
+
+def _find_boiling_surface(image: DA, preview: bool = DEBUG) -> ArrInt:
+    """Find the boiling surface."""
+    # Find corners and set index to contour points for later concatenation
+    (height, width) = image.shape
+    corns_ = apply_to_img_da(find_boiling_surface, image)
+    corns = df_points(np.nonzero(corns_.values))
+    corns = (
+        corns.set_index(pd.MultiIndex.from_frame(corns))
+        .drop(axis="columns", labels=YX_PX)
+        .assign(**dict(corner=True))
+    )
+    # Find the contour angles
+    contours = find_contours(image.values)
+    roi_poly_ = contours.pop()
+    roi_poly = df_points(roi_poly_)
+    distances = roi_poly.diff()
+    angles = (
+        pd.Series(np.degrees(np.arctan2(distances.ypx, distances.xpx)))
+        .rolling(window=2)
+        .mean()
+        .bfill()
+    ).rename("deg")
+    # Concatenate contour points with their angles
+    roi_poly = (
+        pd.concat(
+            axis="columns",
+            keys=["dim", "angle"],
+            objs=[roi_poly, angles],
+        )
+        .set_index(pd.MultiIndex.from_frame(roi_poly))
+        .drop(axis="columns", labels="dim")
+    )
+    # Set the index to the contour points and concatenate with corners
+    # Compute distance from midplanes for candidate corner selection
+    roi_poly = roi_poly.set_axis(axis="columns", labels=roi_poly.columns.droplevel(1))
+    corns = (
+        pd.concat(axis="columns", objs=[roi_poly, corns])
+        .dropna()
+        .drop(axis="columns", labels="corner")
+        .sort_index()
+        .reset_index()
+        .assign(
+            **dict(
+                xpx_mid_abs=lambda df: (df.xpx - width / 2).abs(),
+                ypx_mid=lambda df: df.ypx - height / 2,
+            )
+        )
+        .sort_values(axis="index", by="xpx_mid_abs")
+    )
+    # Consider the boiling surface to be described by the two corners with a low enough
+    # angle, below the horizontal midplane, and closest to the vertical midplane
+    max_angle = 30
+    candidates = (
+        corns[
+            (corns.angle > -max_angle) & (corns.angle < max_angle) & (corns.ypx_mid > 0)
+        ]
+        .reset_index(drop=True)
+        .loc[0:1, ["ypx", "xpx"]]
+    )
+    if preview:
+        view_images(dict(corn=corns_.values))
+    # TODO: Save to disk, draw on an image for previewing
+    return candidates.values.flatten()[:2]
+
+
+def _find_boiling_surface2(image):
+    """Get line segments in an image."""
+    lines_, lsd = find_line_segments(image)
+    lined = lsd.drawSegments(image, lines_)
+    lines = frame_lines(lines_)
+    midpoints = df_points([lines.ypx.T.mean(), lines.xpx.T.mean()])
+    distances = df_points([lines.ypx[1] - lines.ypx[0], lines.xpx[1] - lines.xpx[0]])
+    lengths = distances.T.pow(2).sum().pow(1 / 2).rename("px")
+    angles = pd.Series(np.arctan2(distances.ypx, distances.xpx)).rename("deg")
+    lines = (
+        pd.concat(
+            axis="columns",
+            keys=["line", "midpoint", "length", "angle"],
+            objs=[
+                lines.set_axis(axis="columns", labels=["ypx0", "xpx0", "ypx1", "xpx1"]),
+                midpoints,
+                lengths,
+                angles,
+            ],
+        )
+        .rename_axis(axis="index", mapper="line")
+        .rename_axis(axis="columns", mapper=["metric", "dim"])
+    )
+    return lined, lines
```

### Comparing `boilercv-0.0.0/src/boilercv/previews/__init__.py` & `boilercv-0.0.1/src/boilercv/previews/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-"""Preview results."""
-
-from pathlib import Path
-
-import xarray as xr
-
-from boilercv import DEBUG
-from boilercv.colors import RED
-from boilercv.data import VIDEO, YX_PX, identity_da
-from boilercv.data.sets import slice_frames
-from boilercv.images import draw_text, overlay
-from boilercv.types import DA, DS
-
-_NUM_FRAMES = 100 if DEBUG else 0
-
-
-def get_preview(path: Path) -> DS:
-    """Get a preview dataset.
-
-    Args:
-        path: Path to dataset.
-    """
-    with xr.open_dataset(path) as ds:
-        return xr.Dataset({VIDEO: ds[VIDEO][slice_frames(_NUM_FRAMES)]})
-
-
-def draw_text_da(da: DA) -> DA:
-    """Draw text on images in a data array."""
-    frames_dim = str(da.dims[0])
-    if da.ndim == 4:
-        # We have a color video
-        return xr.apply_ufunc(
-            draw_text,
-            da,
-            identity_da(da, frames_dim),
-            input_core_dims=([*YX_PX, "channel"], []),
-            output_core_dims=([*YX_PX, "channel"],),
-            vectorize=True,
-        )
-    else:
-        return xr.apply_ufunc(
-            draw_text,
-            da,
-            identity_da(da, frames_dim),
-            input_core_dims=(YX_PX, []),
-            output_core_dims=(YX_PX,),
-            vectorize=True,
-        )
-
-
-def compose_da(da_image: DA, da_overlay: DA, color: tuple[int, int, int] = RED) -> DA:
-    """Draw text on images in a data array.
-
-    Args:
-        da_image: Image data array.
-        da_overlay: Overlay data array.
-        color: Color for the overlay.
-    """
-    return xr.apply_ufunc(
-        overlay,
-        da_image,
-        da_overlay,
-        input_core_dims=(YX_PX, YX_PX),
-        output_core_dims=([*YX_PX, "channel"],),
-        vectorize=True,
-        kwargs=dict(color=color),
-    )
+"""Preview results."""
+
+from pathlib import Path
+
+import xarray as xr
+
+from boilercv import DEBUG
+from boilercv.colors import RED
+from boilercv.data import VIDEO, YX_PX, identity_da
+from boilercv.data.sets import slice_frames
+from boilercv.images import draw_text, overlay
+from boilercv.types import DA, DS
+
+_NUM_FRAMES = 100 if DEBUG else 0
+
+
+def get_preview(path: Path) -> DS:
+    """Get a preview dataset.
+
+    Args:
+        path: Path to dataset.
+    """
+    with xr.open_dataset(path) as ds:
+        return xr.Dataset({VIDEO: ds[VIDEO][slice_frames(_NUM_FRAMES)]})
+
+
+def draw_text_da(da: DA) -> DA:
+    """Draw text on images in a data array."""
+    frames_dim = str(da.dims[0])
+    if da.ndim == 4:
+        # We have a color video
+        return xr.apply_ufunc(
+            draw_text,
+            da,
+            identity_da(da, frames_dim),
+            input_core_dims=([*YX_PX, "channel"], []),
+            output_core_dims=([*YX_PX, "channel"],),
+            vectorize=True,
+        )
+    else:
+        return xr.apply_ufunc(
+            draw_text,
+            da,
+            identity_da(da, frames_dim),
+            input_core_dims=(YX_PX, []),
+            output_core_dims=(YX_PX,),
+            vectorize=True,
+        )
+
+
+def compose_da(da_image: DA, da_overlay: DA, color: tuple[int, int, int] = RED) -> DA:
+    """Draw text on images in a data array.
+
+    Args:
+        da_image: Image data array.
+        da_overlay: Overlay data array.
+        color: Color for the overlay.
+    """
+    return xr.apply_ufunc(
+        overlay,
+        da_image,
+        da_overlay,
+        input_core_dims=(YX_PX, YX_PX),
+        output_core_dims=([*YX_PX, "channel"],),
+        vectorize=True,
+        kwargs=dict(color=color),
+    )
```

### Comparing `boilercv-0.0.0/src/boilercv/previews/binarized.py` & `boilercv-0.0.1/src/boilercv/previews/gray.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-"""Preview the binarization stage."""
-
-import xarray as xr
-
-from boilercv import FRAMERATE_PREV, PREVIEW
-from boilercv.captivate.previews import view_images
-from boilercv.data import VIDEO
-from boilercv.images import scale_bool
-from boilercv.models.params import PARAMS
-from boilercv.previews import draw_text_da
-from boilercv.types import DA
-
-
-def main(preview: bool = PREVIEW) -> DA:
-    with xr.open_dataset(PARAMS.paths.binarized_preview) as ds:
-        da = draw_text_da(scale_bool(ds[VIDEO]))
-    if preview:
-        view_images(da, framerate=FRAMERATE_PREV)
-    return da
-
-
-if __name__ == "__main__":
-    main()
+"""Preview the grayscale stage."""
+
+import xarray as xr
+
+from boilercv import FRAMERATE_PREV, PREVIEW
+from boilercv.captivate.previews import view_images
+from boilercv.data import VIDEO
+from boilercv.models.params import PARAMS
+from boilercv.previews import draw_text_da
+from boilercv.types import DA
+
+
+def main(preview: bool = PREVIEW) -> DA:
+    with xr.open_dataset(PARAMS.paths.gray_preview) as ds:
+        da = draw_text_da(ds[VIDEO])
+    if preview:
+        view_images(da, framerate=FRAMERATE_PREV)
+    return da
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/previews/filled.py` & `boilercv-0.0.1/src/boilercv/previews/binarized.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""Preview the filled contours stage."""
-
-import xarray as xr
-
-from boilercv import FRAMERATE_PREV, PREVIEW
-from boilercv.captivate.previews import view_images
-from boilercv.data import VIDEO
-from boilercv.images import scale_bool
-from boilercv.models.params import PARAMS
-from boilercv.previews import draw_text_da
-from boilercv.types import DA
-
-
-def main(preview: bool = PREVIEW) -> DA:
-    with xr.open_dataset(PARAMS.paths.filled_preview) as ds:
-        da = draw_text_da(scale_bool(ds[VIDEO]))
-    if preview:
-        view_images(da, framerate=FRAMERATE_PREV)
-    return da
-
-
-if __name__ == "__main__":
-    main()
+"""Preview the binarization stage."""
+
+import xarray as xr
+
+from boilercv import FRAMERATE_PREV, PREVIEW
+from boilercv.captivate.previews import view_images
+from boilercv.data import VIDEO
+from boilercv.images import scale_bool
+from boilercv.models.params import PARAMS
+from boilercv.previews import draw_text_da
+from boilercv.types import DA
+
+
+def main(preview: bool = PREVIEW) -> DA:
+    with xr.open_dataset(PARAMS.paths.binarized_preview) as ds:
+        da = draw_text_da(scale_bool(ds[VIDEO]))
+    if preview:
+        view_images(da, framerate=FRAMERATE_PREV)
+    return da
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/previews/gray.py` & `boilercv-0.0.1/src/boilercv/previews/filled.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""Preview the grayscale stage."""
-
-import xarray as xr
-
-from boilercv import FRAMERATE_PREV, PREVIEW
-from boilercv.captivate.previews import view_images
-from boilercv.data import VIDEO
-from boilercv.models.params import PARAMS
-from boilercv.previews import draw_text_da
-from boilercv.types import DA
-
-
-def main(preview: bool = PREVIEW) -> DA:
-    with xr.open_dataset(PARAMS.paths.gray_preview) as ds:
-        da = draw_text_da(ds[VIDEO])
-    if preview:
-        view_images(da, framerate=FRAMERATE_PREV)
-    return da
-
-
-if __name__ == "__main__":
-    main()
+"""Preview the filled contours stage."""
+
+import xarray as xr
+
+from boilercv import FRAMERATE_PREV, PREVIEW
+from boilercv.captivate.previews import view_images
+from boilercv.data import VIDEO
+from boilercv.images import scale_bool
+from boilercv.models.params import PARAMS
+from boilercv.previews import draw_text_da
+from boilercv.types import DA
+
+
+def main(preview: bool = PREVIEW) -> DA:
+    with xr.open_dataset(PARAMS.paths.filled_preview) as ds:
+        da = draw_text_da(scale_bool(ds[VIDEO]))
+    if preview:
+        view_images(da, framerate=FRAMERATE_PREV)
+    return da
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boilercv-0.0.0/src/boilercv/stages/update_previews/__init__.py` & `boilercv-0.0.1/src/boilercv/stages/update_previews/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,88 @@
-"""Update previews for various stages."""
-
-from collections.abc import Iterator
-from contextlib import contextmanager
-from pathlib import Path
-from typing import Any
-
-import xarray as xr
-
-from boilercv.captivate.previews import pad_images
-from boilercv.data import VIDEO, VIDEO_NAME, XPX, YPX, assign_ds
-from boilercv.data.models import Dimension
-from boilercv.data.sets import ALL_NAMES
-from boilercv.types import DS
-
-
-@contextmanager
-def new_videos_to_preview(
-    destination: Path, rebuild: bool = False
-) -> Iterator[dict[str, Any]]:
-    """Get an empty mapping of new videos to preview and write to disk."""
-
-    # Yield a mapping of new video names to previews, to be populated by the user
-    if rebuild:
-        new_video_names = ALL_NAMES
-    else:
-        existing_names: list[str] = []
-        if destination.exists():
-            with xr.open_dataset(destination) as existing_ds:
-                existing_names.extend(list(existing_ds[VIDEO_NAME].values))
-        new_video_names = [name for name in ALL_NAMES if name not in existing_names]
-    videos_to_preview = dict.fromkeys(new_video_names)
-
-    yield videos_to_preview
-
-    # Keep only valid received previews and build a dataset of new previews
-    if received_previews := {
-        video_name: preview
-        for video_name, preview in videos_to_preview.items()
-        if preview is not None and video_name in new_video_names
-    }:
-        received_video_names = list(received_previews.keys())
-        received_previews = list(received_previews.values())
-        new_ds = get_preview_ds(received_video_names, received_previews)
-
-        if destination.exists():
-            with xr.open_dataset(destination) as existing_ds:
-                if new_ds[VIDEO].shape == existing_ds[VIDEO].shape:
-                    # Combine datasets if they're the same shape
-                    new_ds = xr.combine_by_coords([existing_ds, new_ds])
-                else:
-                    # Otherwise, destructure, pad, and rebuild them together
-                    existing_names = list(existing_ds[VIDEO_NAME].values)
-                    new_ds = get_preview_ds(
-                        existing_names + received_video_names,
-                        received_previews + list(existing_ds.video.values),
-                    )
-
-        new_ds.to_netcdf(path=destination, encoding={VIDEO: {"zlib": True}})
-
-
-def get_preview_ds(preview_names: list[str], previews: list[Any]) -> DS:
-    """Get a dataset of preview images, padding sizes as necessary."""
-    return assign_ds(
-        name=VIDEO,
-        long_name="Video preview",
-        units="Pixel state",
-        dims=(
-            Dimension(
-                dim=VIDEO_NAME,
-                long_name="Video name",
-                coords=preview_names,
-            ),
-            Dimension(
-                dim=YPX,
-                long_name="Height",
-                units="px",
-            ),
-            Dimension(
-                dim=XPX,
-                long_name="Width",
-                units="px",
-            ),
-        ),
-        data=pad_images(previews),
-    )
+"""Update previews for various stages."""
+
+from collections.abc import Iterator
+from contextlib import contextmanager
+from pathlib import Path
+from typing import Any
+
+import xarray as xr
+
+from boilercv.captivate.previews import pad_images
+from boilercv.data import VIDEO, VIDEO_NAME, XPX, YPX, assign_ds
+from boilercv.data.models import Dimension
+from boilercv.data.sets import ALL_NAMES
+from boilercv.types import DS
+
+
+@contextmanager
+def new_videos_to_preview(
+    destination: Path, reprocess: bool = False
+) -> Iterator[dict[str, Any]]:
+    """An empty mapping of new videos to preview and write to disk."""
+
+    # Yield a mapping of new video names to previews, to be populated by the user
+    if reprocess:
+        # Reprocess all names
+        new_video_names = ALL_NAMES
+    else:
+        # Get the names missing from the destination
+        existing_names: list[str] = []
+        if destination.exists():
+            with xr.open_dataset(destination) as existing_ds:
+                existing_names.extend(list(existing_ds[VIDEO_NAME].values))
+        new_video_names = [name for name in ALL_NAMES if name not in existing_names]
+    videos_to_preview = dict.fromkeys(new_video_names)
+
+    yield videos_to_preview
+
+    # Keep only valid received previews and build a dataset of new previews
+    if received_previews := {
+        video_name: preview
+        for video_name, preview in videos_to_preview.items()
+        if preview is not None and video_name in new_video_names
+    }:
+        received_video_names = list(received_previews.keys())
+        received_previews = list(received_previews.values())
+        new_ds = get_preview_ds(received_video_names, received_previews)
+
+        if destination.exists():
+            with xr.open_dataset(destination) as existing_ds:
+                if new_ds[VIDEO].shape == existing_ds[VIDEO].shape:
+                    # Combine datasets if they're the same shape
+                    new_ds = xr.combine_by_coords([existing_ds, new_ds])
+                else:
+                    # Otherwise: destructure, pad, and rebuild them together
+                    existing_names = list(existing_ds[VIDEO_NAME].values)
+                    new_ds = get_preview_ds(
+                        existing_names + received_video_names,
+                        received_previews + list(existing_ds.video.values),
+                    )
+
+        new_ds.to_netcdf(path=destination, encoding={VIDEO: {"zlib": True}})
+
+
+def get_preview_ds(preview_names: list[str], previews: list[Any]) -> DS:
+    """Get a dataset of preview images, padding sizes as necessary."""
+    return assign_ds(
+        name=VIDEO,
+        long_name="Video preview",
+        units="Pixel state",
+        data=pad_images(previews),
+        dims=(
+            Dimension(
+                dim=VIDEO_NAME,
+                long_name="Video name",
+                coords=preview_names,
+            ),
+            Dimension(
+                dim=YPX,
+                long_name="Height",
+                units="px",
+            ),
+            Dimension(
+                dim=XPX,
+                long_name="Width",
+                units="px",
+            ),
+        ),
+    )
```

### Comparing `boilercv-0.0.0/src/boilercv/stages/update_previews/binarized.py` & `boilercv-0.0.1/src/boilercv/stages/update_previews/binarized.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""Update previews for the binarization stage."""
-
-from loguru import logger
-
-from boilercv.data import FRAME, ROI, VIDEO
-from boilercv.data.sets import get_dataset
-from boilercv.models.params import PARAMS
-from boilercv.stages.update_previews import new_videos_to_preview
-
-
-def main():
-    stage = "sources"
-    destination = PARAMS.paths.binarized_preview
-    with new_videos_to_preview(destination) as videos_to_preview:
-        for video_name in videos_to_preview:
-            ds = get_dataset(video_name, stage=stage, num_frames=1)
-            first_frame = ds[VIDEO].isel({FRAME: 0}).values
-            videos_to_preview[video_name] = first_frame & ds[ROI].values
-
-
-if __name__ == "__main__":
-    logger.info("Start update binarized preview")
-    main()
-    logger.info("Finish update binarized preview")
+"""Update previews for the binarization stage."""
+
+from loguru import logger
+
+from boilercv.data import FRAME, ROI, VIDEO
+from boilercv.data.sets import get_dataset
+from boilercv.models.params import PARAMS
+from boilercv.stages.update_previews import new_videos_to_preview
+
+
+def main():
+    stage = "sources"
+    destination = PARAMS.paths.binarized_preview
+    with new_videos_to_preview(destination) as videos_to_preview:
+        for video_name in videos_to_preview:
+            ds = get_dataset(video_name, stage=stage, num_frames=1)
+            first_frame = ds[VIDEO].isel({FRAME: 0}).values
+            videos_to_preview[video_name] = first_frame & ds[ROI].values
+
+
+if __name__ == "__main__":
+    logger.info("Start update binarized preview")
+    main()
+    logger.info("Finish update binarized preview")
```

### Comparing `boilercv-0.0.0/update.ps1` & `boilercv-0.0.1/template/template/update.ps1`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-<#.SYNOPSIS
-Update the local virtual environment to the latest tracked dependencies.
-#>
-
-# * ------------------------------------------------------------------------------ * #
-# * Changes below may be lost in significant template updates.
-
-# Activate environment
-$VENV_ACTIVATE_WINDOWS = '.venv/Scripts/activate'
-$VENV_ACTIVATE_UNIX = '.venv/bin/Activate.ps1'
-if ( Test-Path $VENV_ACTIVATE_WINDOWS ) { . $VENV_ACTIVATE_WINDOWS }
-elseif ( Test-Path $VENV_ACTIVATE_UNIX ) { . $VENV_ACTIVATE_UNIX }
-else {
-    throw [System.Management.Automation.ItemNotFoundException] 'Could not find a virtual environment.'
-}
-
-# Install dev requirements
-python -m pip install --upgrade pip # Instructed to do this by pip
-pip install --upgrade setuptools wheel # Must be done separately from above
-pip install --upgrade --requirement '.tools/requirements/requirements_dev.txt'
-# Need `toml` in dev requirements prior to bumping `pyproject.toml`
-python '.tools/scripts/compose_pyproject.py'
-
-# Install the package and the lower bound of its requirements
-pip install --no-deps --editable '.'
-pip install --upgrade --requirement 'requirements.txt'
-
-# Ensure pre-commit hooks are applied and updated
-pre-commit install --install-hooks
-
-# * -------------------------------------------------------------------------------- * #
-# * Changes below should persist in significant template updates.
-
-pip install --no-deps --requirement '.tools/requirements/requirements_nodeps.txt'
-pre-commit install --install-hooks --hook-type pre-push --hook-type post-checkout
+<#.SYNOPSIS
+Update the local virtual environment to the latest tracked dependencies.
+#>
+
+# * -------------------------------------------------------------------------------- * #
+# * Changes below may be lost in significant template updates.
+
+# Activate environment
+$VENV_ACTIVATE_WINDOWS = '.venv/Scripts/activate'
+$VENV_ACTIVATE_UNIX = '.venv/bin/Activate.ps1'
+if ( Test-Path $VENV_ACTIVATE_WINDOWS ) { . $VENV_ACTIVATE_WINDOWS }
+elseif ( Test-Path $VENV_ACTIVATE_UNIX ) { . $VENV_ACTIVATE_UNIX }
+else {
+throw [System.Management.Automation.ItemNotFoundException] 'Could not find a virtual environment.'
+}
+
+# Install dev requirements
+python -m pip install --upgrade pip # Instructed to do this by pip
+pip install --upgrade setuptools wheel # Must be done separately from above
+pip install --upgrade --requirement '.tools/requirements/requirements_dev.txt'
+# Need `toml` in dev requirements prior to bumping `pyproject.toml`
+python '.tools/scripts/compose_pyproject.py'
+
+# Install the package and the lower bound of its requirements
+pip install --no-deps --editable '.'
+pip install --upgrade --requirement 'requirements.txt'
+
+# Ensure pre-commit hooks are applied and updated
+pre-commit install --install-hooks
+
+# * -------------------------------------------------------------------------------- * #
+# * Changes below should persist in significant template updates.
```

