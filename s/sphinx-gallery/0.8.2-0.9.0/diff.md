# Comparing `tmp/sphinx-gallery-0.8.2.tar.gz` & `tmp/sphinx-gallery-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinx-gallery-0.8.2.tar", last modified: Thu Dec 17 21:25:14 2020, max compression
+gzip compressed data, was "dist/sphinx-gallery-0.9.0.tar", last modified: Sun Apr 25 05:37:32 2021, max compression
```

## Comparing `sphinx-gallery-0.8.2.tar` & `sphinx-gallery-0.9.0.tar`

### file list

```diff
@@ -1,534 +1,535 @@
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    68652 2020-12-17 21:23:01.000000 sphinx-gallery-0.8.2/CHANGES.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1486 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/LICENSE
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      864 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/MANIFEST.in
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4723 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/PKG-INFO
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3389 2020-10-25 22:19:02.000000 sphinx-gallery-0.8.2/README.rst
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/bin/
--rwxrwxr-x   0 lucy      (1000) lucy      (1000)      292 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/bin/copy_sphinxgallery.sh
--rwxrwxr-x   0 lucy      (1000) lucy      (1000)      460 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/bin/sphx_glr_python_to_jupyter.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/examples/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      753 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/examples/README.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      199 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/examples/local_module.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/examples/no_output/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      250 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/examples/no_output/README.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      423 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/examples/no_output/just_code.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1038 2020-03-27 12:49:06.000000 sphinx-gallery-0.8.2/examples/no_output/plot_raise.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      414 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/examples/no_output/plot_strings.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      369 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/examples/no_output/plot_syntaxerror.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3368 2020-09-05 20:35:03.000000 sphinx-gallery-0.8.2/examples/plot_0_sin.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1109 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/examples/plot_1_exp.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      942 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/examples/plot_2_seaborn.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4917 2020-10-07 18:28:05.000000 sphinx-gallery-0.8.2/examples/plot_3_capture_repr.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1122 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/examples/plot_4_choose_thumbnail.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      938 2020-03-27 12:49:06.000000 sphinx-gallery-0.8.2/examples/plot_4b_provide_thumbnail.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1011 2020-03-27 12:49:06.000000 sphinx-gallery-0.8.2/examples/plot_5_unicode_everywhere.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1937 2020-03-27 12:49:06.000000 sphinx-gallery-0.8.2/examples/plot_6_function_identifier.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      760 2020-08-28 08:44:51.000000 sphinx-gallery-0.8.2/examples/plot_7_sys_argv.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      599 2020-06-23 08:35:31.000000 sphinx-gallery-0.8.2/examples/plot_8_animations.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2741 2020-10-25 22:19:02.000000 sphinx-gallery-0.8.2/examples/plot_9_plotly.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/mayavi_examples/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      229 2020-10-25 22:19:02.000000 sphinx-gallery-0.8.2/mayavi_examples/README.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      844 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/mayavi_examples/plot_3d.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       14 2020-03-06 11:08:45.000000 sphinx-gallery-0.8.2/requirements.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      585 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/setup.cfg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1874 2020-10-07 18:28:05.000000 sphinx-gallery-0.8.2/setup.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      346 2020-12-17 21:23:01.000000 sphinx-gallery-0.8.2/sphinx_gallery/__init__.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/_static/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3380 2020-09-02 17:13:45.000000 sphinx-gallery-0.8.2/sphinx_gallery/_static/binder_badge_logo.svg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    21404 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/_static/broken_example.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      101 2020-03-06 11:08:45.000000 sphinx-gallery-0.8.2/sphinx_gallery/_static/gallery-binder.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      829 2020-03-06 11:08:45.000000 sphinx-gallery-0.8.2/sphinx_gallery/_static/gallery-dataframe.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3714 2020-10-07 18:28:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/_static/gallery-rendered-html.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4071 2020-06-05 19:46:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/_static/gallery.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4315 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/_static/no_image.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12437 2020-10-25 22:19:02.000000 sphinx-gallery-0.8.2/sphinx_gallery/backreferences.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     9758 2020-10-25 22:19:02.000000 sphinx-gallery-0.8.2/sphinx_gallery/binder.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3035 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/directives.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    16690 2020-06-22 14:17:02.000000 sphinx-gallery-0.8.2/sphinx_gallery/docs_resolv.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4044 2020-06-22 14:17:02.000000 sphinx-gallery-0.8.2/sphinx_gallery/downloads.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    32422 2020-10-25 22:19:02.000000 sphinx-gallery-0.8.2/sphinx_gallery/gen_gallery.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    37008 2020-10-25 22:19:02.000000 sphinx-gallery-0.8.2/sphinx_gallery/gen_rst.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      580 2020-03-06 11:08:45.000000 sphinx-gallery-0.8.2/sphinx_gallery/load_style.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    10205 2020-07-31 08:56:42.000000 sphinx-gallery-0.8.2/sphinx_gallery/notebook.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     6840 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/py_source_parser.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    15061 2020-10-07 06:37:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/scrapers.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3576 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/sorting.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2140 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/sphinx_compatibility.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/__init__.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     6981 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/conftest.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3395 2020-03-27 12:49:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/reference_parse.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4551 2020-10-25 22:19:02.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_backreferences.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     5273 2020-09-09 20:02:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_binder.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2807 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_docs_resolv.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    39421 2020-10-23 07:11:49.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_full.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    15476 2020-06-22 14:17:02.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_gen_gallery.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    29277 2020-11-05 22:26:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_gen_rst.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      676 2020-03-06 11:08:45.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_load_style.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     9343 2020-12-13 00:46:16.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_notebook.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2664 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_py_source_parser.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     8127 2020-09-01 19:12:52.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_scrapers.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1830 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_sorting.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2900 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_sphinx_compatibility.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      668 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/test_utils.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/testconfs/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       57 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/testconfs/index.rst
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/testconfs/src/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       34 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/testconfs/src/README.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      112 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/testconfs/src/plot_1.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       84 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/testconfs/src/plot_2.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      319 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/testconfs/src/plot_3.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      501 2020-08-31 19:26:33.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/Makefile
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    13025 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/plot_future_imports.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11885 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/plot_future_imports_broken.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     6594 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/sg_execution_times.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    29953 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/index.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    10131 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/local_module.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)  3290349 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_animation.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11643 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_command_line_args.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11908 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_log.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    13094 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_matplotlib_alt.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    16382 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_numpy_matplotlib.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11672 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_pickle.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    10704 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_repr.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11287 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_scraper_broken.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12163 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_second_future_imports.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11617 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_svg.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    17038 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/sg_execution_times.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)  4665324 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/environment.pickle
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/examples/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/examples/future/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2627 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/examples/future/README.doctree
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    24238 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.backreferences.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    27583 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.docs_resolv.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    23240 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.downloads.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    54703 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.gen_gallery.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    72707 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.gen_rst.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    45530 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.notebook.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    25989 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.py_source_parser.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    30747 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.sorting.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    16862 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/index.doctree
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    32286 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/minigallery.doctree
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      230 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/.buildinfo
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     8160 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/0945e908cf9aecf00af7e353b373478b/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1816 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/0945e908cf9aecf00af7e353b373478b/plot_future_imports.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/19fd12aa0d4382f326db31f16d3d1d1e/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      353 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/19fd12aa0d4382f326db31f16d3d1d1e/plot_command_line_args.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/1ef095bd0669862690bd67d790b94ef7/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      364 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/1ef095bd0669862690bd67d790b94ef7/plot_svg.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2300099a8a72b1f91aa46a11810faaaa/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1194 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2300099a8a72b1f91aa46a11810faaaa/plot_scraper_broken.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2605673e66d2cc847b70bb1bf2d4b939/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      420 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2605673e66d2cc847b70bb1bf2d4b939/plot_log.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2b12073b01b18ea3dc8c5aeafcb7eeb0/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      493 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2b12073b01b18ea3dc8c5aeafcb7eeb0/plot_future_imports_broken.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/3b0b6bf78eb66e43437306cf540227da/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2387 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/3b0b6bf78eb66e43437306cf540227da/plot_numpy_matplotlib.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/411f5bf9287e74d4e2c58e6144219a86/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      596 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/411f5bf9287e74d4e2c58e6144219a86/plot_future_imports.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/454b2c75039cd779f665618ef983be2c/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1315 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/454b2c75039cd779f665618ef983be2c/plot_command_line_args.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/4b57cb1bb48eabbaf6e5f630e7437e3b/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      717 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/4b57cb1bb48eabbaf6e5f630e7437e3b/plot_animation.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    21745 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7525ca7e05c4870d06f1177b4881f139/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      677 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7525ca7e05c4870d06f1177b4881f139/plot_matplotlib_alt.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7c725e874f6ee2b5b1ccc38e70dea163/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      436 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7c725e874f6ee2b5b1ccc38e70dea163/plot_pickle.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7dc32ed5edb2b56d912aa8b53b27e465/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1916 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7dc32ed5edb2b56d912aa8b53b27e465/plot_matplotlib_alt.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/80a6099e54c6c11338620217777d2a02/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1428 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/80a6099e54c6c11338620217777d2a02/plot_pickle.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/875869823209fb298bef99090ff5b596/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      229 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/875869823209fb298bef99090ff5b596/plot_scraper_broken.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/93047193aca007ee7c3b7b968d303020/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1060 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/93047193aca007ee7c3b7b968d303020/local_module.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/936dfa023c8a1fbfaa560a549ee3f458/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1754 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/936dfa023c8a1fbfaa560a549ee3f458/plot_log.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/9395a333d61cc5d8b4a7881c7f3a6185/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1454 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/9395a333d61cc5d8b4a7881c7f3a6185/plot_future_imports_broken.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a12f17d9ba4a6fcbe3f5fc11f7be70c9/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      706 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a12f17d9ba4a6fcbe3f5fc11f7be70c9/plot_second_future_imports.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a3e878cfae7468eb4a033c6a533aca80/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1667 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a3e878cfae7468eb4a033c6a533aca80/plot_second_future_imports.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bb97c554404070d247821825b00698e8/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1413 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bb97c554404070d247821825b00698e8/plot_numpy_matplotlib.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bf7778dabfc4caff452aaed2231aad91/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1107 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bf7778dabfc4caff452aaed2231aad91/plot_repr.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/c97a3031e7cba7452bc30b650a43ec86/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       81 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/c97a3031e7cba7452bc30b650a43ec86/local_module.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/cbb0b98552467a25c4244e5c246fa313/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1321 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/cbb0b98552467a25c4244e5c246fa313/plot_svg.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e43712bb9ad80e85ad20366b3fb3c5dd/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      131 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e43712bb9ad80e85ad20366b3fb3c5dd/plot_repr.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e63e7669ff68ac4d5808e80c4c6bfa47/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1704 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e63e7669ff68ac4d5808e80c4c6bfa47/plot_animation.ipynb
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3380 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/binder_badge_logo.svg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3380 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/binder_badge_logo1.svg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_local_module_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2402 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_001.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     7703 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_003.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)   115993 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_thumb.gif
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4375 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_command_line_args_001.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     5811 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_command_line_args_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    35467 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_future_imports_broken_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_future_imports_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_log_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    28529 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_001.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    18597 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_002.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    22812 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    22555 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_numpy_matplotlib_001.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    13799 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_numpy_matplotlib_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_pickle_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_repr_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    35467 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_scraper_broken_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    34269 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_second_future_imports_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    17208 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_svg_001.svg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    17208 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_svg_thumb.svg
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2442 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/plot_future_imports.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2214 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/plot_future_imports_broken.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      814 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/sg_execution_times.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     6339 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/index.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1612 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/local_module.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)   921291 2020-10-27 22:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_animation.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2148 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_command_line_args.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2290 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_log.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2764 2020-10-27 22:32:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_matplotlib_alt.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3627 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_numpy_matplotlib.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2187 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_pickle.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1809 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_repr.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1828 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_scraper_broken.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2410 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_second_future_imports.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2099 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_svg.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2943 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/sg_execution_times.rst.txt
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/examples/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/examples/future/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       77 2020-04-27 14:13:40.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/examples/future/README.rst.txt
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      920 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.backreferences.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1121 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.docs_resolv.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      873 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.downloads.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3377 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.gen_gallery.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2698 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.gen_rst.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2160 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.notebook.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1189 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.py_source_parser.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1291 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.sorting.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      696 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      816 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/minigallery.rst.txt
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11185 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/alabaster.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12171 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/basic.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3380 2020-09-02 17:13:45.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/binder_badge_logo.svg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    21404 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/broken_example.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    53268 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/broken_stamp.svg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       42 2018-10-08 18:30:38.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/custom.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)   230273 2020-09-09 20:02:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/demo.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     9270 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/doctools.js
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      303 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/documentation_options.js
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      286 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/file.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      101 2020-03-06 11:08:45.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-binder.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      829 2020-03-06 11:08:45.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-dataframe.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3714 2020-10-07 18:28:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-rendered-html.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4071 2020-06-05 19:46:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)   280364 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/jquery-3.4.1.js
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    88145 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/jquery.js
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    10847 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/language_data.js
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       90 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/minus.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4315 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/no_image.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       90 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/plus.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4798 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/pygments.css
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    15987 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/searchtools.js
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    35168 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12140 2019-12-03 16:59:50.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/underscore.js
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11376 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/plot_future_imports.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     9109 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/plot_future_imports_broken.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     5730 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/sg_execution_times.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    16018 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/index.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     7017 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/local_module.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)   820229 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_animation.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12491 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_command_line_args.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    13108 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_log.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    16841 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_matplotlib_alt.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    24703 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_numpy_matplotlib.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12984 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_pickle.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     8727 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_repr.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     9040 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_scraper_broken.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    11603 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_second_future_imports.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    13087 2020-10-27 22:32:57.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_svg.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     8578 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/sg_execution_times.html
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/binder/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      167 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/binder/requirements.txt
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/examples/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/examples/future/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4736 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/examples/future/README.html
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12156 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.backreferences.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    15430 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.docs_resolv.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12443 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.downloads.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26286 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.gen_gallery.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    30339 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.gen_rst.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    21418 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.notebook.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    13207 2020-10-27 22:32:55.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.py_source_parser.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    14992 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.sorting.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    20077 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/genindex.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     9204 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/index.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    12519 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/minigallery.html
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1816 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/plot_future_imports.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1454 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/plot_future_imports_broken.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1060 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/local_module.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1704 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_animation.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1315 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_command_line_args.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1754 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_log.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1916 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_matplotlib_alt.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2387 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_numpy_matplotlib.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1428 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_pickle.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1107 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_repr.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1194 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_scraper_broken.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1667 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_second_future_imports.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1321 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_svg.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3078 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/objects.inv
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     6838 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/py-modindex.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4715 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/search.html
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    16063 2020-10-27 22:32:56.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/searchindex.js
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/sphinx-gallery/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      281 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/sphinx-gallery/junit-results.xml
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_static_nonstandard/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)   230273 2020-09-09 20:02:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_static_nonstandard/demo.png
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_templates/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      992 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_templates/module.rst
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    21745 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/auto_examples_jupyter.zip
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     8160 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/auto_examples_python.zip
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/images/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3380 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/images/binder_badge_logo.svg
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    35467 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/sphx_glr_plot_future_imports_broken_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/sphx_glr_plot_future_imports_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1816 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      596 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     2442 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1454 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      493 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.py
--rw-r--r--   0 lucy      (1000) lucy      (1000)     2214 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      138 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      472 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      814 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/sg_execution_times.rst
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3380 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/binder_badge_logo.svg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2402 2020-10-27 22:32:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_001.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)   115993 2020-10-27 22:32:08.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_002.gif
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     7703 2020-10-27 22:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_003.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4375 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_command_line_args_001.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    28529 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_matplotlib_alt_001.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    18597 2020-10-27 22:32:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_matplotlib_alt_002.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    22555 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_numpy_matplotlib_001.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    17208 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_svg_001.svg
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_local_module_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)   115993 2020-10-27 22:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_animation_thumb.gif
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     5811 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_command_line_args_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_log_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    22812 2020-10-27 22:32:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_matplotlib_alt_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    13799 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_numpy_matplotlib_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_pickle_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    26786 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_repr_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    35467 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_scraper_broken_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    34269 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_second_future_imports_thumb.png
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    17208 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_svg_thumb.svg
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     6339 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/index.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1060 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/local_module.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       81 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/local_module.py
--rw-r--r--   0 lucy      (1000) lucy      (1000)     1612 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/local_module.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1704 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      717 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)   921291 2020-10-27 22:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3797 2020-10-27 22:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1315 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      353 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     2148 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1548 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1754 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      420 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     2290 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      953 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_log_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1916 2020-10-22 02:42:22.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      677 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     2764 2020-10-27 22:32:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      925 2020-10-27 22:32:06.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2387 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1413 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     3627 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     5053 2020-10-27 22:32:10.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1428 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      436 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     2187 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      786 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1107 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      131 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     1809 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      115 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1194 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      229 2020-10-22 02:42:20.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.py
--rw-r--r--   0 lucy      (1000) lucy      (1000)     1828 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      158 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1667 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      706 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     2410 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      492 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1321 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.ipynb
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      364 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       32 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.py.md5
--rw-r--r--   0 lucy      (1000) lucy      (1000)     2099 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      765 2020-10-27 22:32:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg_codeobj.pickle
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      341 2020-10-22 02:42:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/searchindex.bak
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    25916 2020-10-22 02:42:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/searchindex.dat
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      341 2020-10-22 02:42:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/searchindex.dir
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2943 2020-10-27 22:32:54.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/sg_execution_times.rst
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/binder/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      167 2020-09-09 20:02:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/binder/requirements.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3124 2020-09-09 20:02:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/conf.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       56 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/README.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      155 2019-08-12 18:32:09.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/__init__.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/future/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       77 2020-04-27 14:13:40.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/future/README.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      596 2020-04-27 14:13:40.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/future/plot_future_imports.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      493 2020-04-27 14:13:40.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/future/plot_future_imports_broken.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       81 2020-05-05 14:46:33.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/local_module.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      717 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_animation.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      353 2020-08-28 08:44:51.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_command_line_args.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      420 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_log.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      677 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_matplotlib_alt.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1413 2020-04-27 14:13:40.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_numpy_matplotlib.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      436 2020-04-27 14:13:40.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_pickle.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      131 2020-10-07 18:28:05.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_repr.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      229 2020-08-31 19:26:33.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_scraper_broken.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      706 2020-09-09 20:02:30.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_second_future_imports.py
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      364 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_svg.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      559 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      569 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.prop.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      567 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.run.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      599 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.ExplicitOrder.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      589 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      599 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.prop.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      597 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.run.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      582 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.NameFinder.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      597 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.identify_names.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.SphinxDocLinkResolver.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.SphinxDocLinkResolver.resolve.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.embed_code_links.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.get_data.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.parse_sphinx_docopts.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.downloads.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.downloads.generate_zipfiles.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.downloads.list_downloadable_sources.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.downloads.python_zip.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.DefaultResetArgv.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.check_duplicate_filenames.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.check_spaces_in_filenames.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.collect_gallery_files.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.cost_name_key.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.generate_gallery_rst.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.get_default_config_value.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.get_subsections.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.parse_config.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.setup.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.setup_module.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.summarize_failing_examples.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.touch_empty_backreferences.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.write_computation_times.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.write_junit_xml.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.codestr2rst.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.executable_script.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.execute_code_block.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.execute_script.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.extract_intro_and_title.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.generate_dir_rst.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.generate_file_rst.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.handle_exception.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.md5sum_is_current.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.patch_warnings.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.rst_blocks.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.save_rst_example.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.save_thumbnail.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.add_code_cell.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.add_markdown_cell.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.directive_fun.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.fill_notebook.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.generate_image_src.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.jupyter_notebook.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.jupyter_notebook_skeleton.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.python_to_jupyter_cli.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.rst2md.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.save_notebook.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.extract_file_config.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.parse_source_file.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.remove_config_comments.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.split_code_and_text_blocks.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.ExampleTitleSortKey.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      615 2020-10-22 02:42:21.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.ExplicitOrder.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      585 2020-10-22 02:42:27.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.FileNameSortKey.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.FileSizeSortKey.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.NumberOfCodeLinesSortKey.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        0 2020-10-22 02:42:28.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.examples
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      920 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.backreferences.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1121 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.docs_resolv.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      873 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.downloads.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     3377 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.gen_gallery.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2698 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.gen_rst.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2160 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.notebook.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1189 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.py_source_parser.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     1291 2020-10-22 02:42:19.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.sorting.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      696 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/index.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      816 2020-05-24 13:42:13.000000 sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/minigallery.rst
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     5635 2020-07-09 14:10:26.000000 sphinx-gallery-0.8.2/sphinx_gallery/utils.py
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery.egg-info/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     4723 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery.egg-info/PKG-INFO
--rw-rw-r--   0 lucy      (1000) lucy      (1000)    34453 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery.egg-info/SOURCES.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)        1 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery.egg-info/dependency_links.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       14 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery.egg-info/requires.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)       15 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/sphinx_gallery.egg-info/top_level.txt
-drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2020-12-17 21:25:14.000000 sphinx-gallery-0.8.2/tutorials/
--rw-rw-r--   0 lucy      (1000) lucy      (1000)      366 2019-11-18 11:15:18.000000 sphinx-gallery-0.8.2/tutorials/README.txt
--rw-rw-r--   0 lucy      (1000) lucy      (1000)     2890 2020-03-27 12:49:06.000000 sphinx-gallery-0.8.2/tutorials/plot_parse.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)    75429 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/CHANGES.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1486 2021-03-21 23:00:52.000000 sphinx-gallery-0.9.0/LICENSE
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      864 2021-03-21 22:56:48.000000 sphinx-gallery-0.9.0/MANIFEST.in
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)     4848 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/PKG-INFO
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)     3506 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/README.rst
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/bin/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      292 2021-03-21 23:00:52.000000 sphinx-gallery-0.9.0/bin/copy_sphinxgallery.sh
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      460 2021-03-21 23:00:52.000000 sphinx-gallery-0.9.0/bin/sphx_glr_python_to_jupyter.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/examples/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      753 2021-03-21 23:01:28.000000 sphinx-gallery-0.9.0/examples/README.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      199 2021-03-21 23:01:28.000000 sphinx-gallery-0.9.0/examples/local_module.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/examples/no_output/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      250 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/no_output/README.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      423 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/no_output/just_code.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1038 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/no_output/plot_raise.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      414 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/no_output/plot_strings.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      369 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/no_output/plot_syntaxerror.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3368 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_0_sin.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1109 2021-03-21 23:01:28.000000 sphinx-gallery-0.9.0/examples/plot_1_exp.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      942 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_2_seaborn.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4917 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_3_capture_repr.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1122 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_4_choose_thumbnail.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      938 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_4b_provide_thumbnail.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1011 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_5_unicode_everywhere.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1937 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_6_function_identifier.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      760 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_7_sys_argv.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      599 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_8_animations.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2741 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/examples/plot_9_plotly.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/mayavi_examples/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      229 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/mayavi_examples/README.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      844 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/mayavi_examples/plot_3d.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       14 2021-03-21 22:56:50.000000 sphinx-gallery-0.9.0/requirements.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      585 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/setup.cfg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1874 2021-03-21 22:56:48.000000 sphinx-gallery-0.9.0/setup.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)      346 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/__init__.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/_static/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3380 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/_static/binder_badge_logo.svg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    21404 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/_static/broken_example.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      101 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/_static/gallery-binder.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      829 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/_static/gallery-dataframe.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3714 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/_static/gallery-rendered-html.css
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)     4068 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/_static/gallery.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4315 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/_static/no_image.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12437 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/sphinx_gallery/backreferences.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     9758 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/sphinx_gallery/binder.py
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)     3399 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/directives.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    16690 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/sphinx_gallery/docs_resolv.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4044 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/downloads.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    32649 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/sphinx_gallery/gen_gallery.py
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)    38266 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/gen_rst.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      580 2021-03-21 23:02:06.000000 sphinx-gallery-0.9.0/sphinx_gallery/load_style.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    10205 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/sphinx_gallery/notebook.py
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)     6929 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/py_source_parser.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    15061 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/sphinx_gallery/scrapers.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3576 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/sorting.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2140 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/sphinx_compatibility.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/__init__.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     6981 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/conftest.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3395 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/reference_parse.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4551 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_backreferences.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     5273 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_binder.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2807 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_docs_resolv.py
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)    41119 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_full.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    16354 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_gen_gallery.py
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)    29890 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_gen_rst.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      676 2021-03-21 23:02:02.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_load_style.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     9343 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_notebook.py
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)     2767 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_py_source_parser.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     8300 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_scrapers.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1830 2021-03-21 23:01:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_sorting.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2900 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_sphinx_compatibility.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      668 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/test_utils.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/testconfs/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       57 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/testconfs/index.rst
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/testconfs/src/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       34 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/testconfs/src/README.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      112 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/testconfs/src/plot_1.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       84 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/testconfs/src/plot_2.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      319 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/testconfs/src/plot_3.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      501 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/Makefile
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    13025 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/plot_future_imports.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11885 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/plot_future_imports_broken.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     6594 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/sg_execution_times.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    29953 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/index.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    10131 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/local_module.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)  3290349 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_animation.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11643 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_command_line_args.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11908 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_log.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    13094 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_matplotlib_alt.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    16382 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_numpy_matplotlib.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11672 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_pickle.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    10704 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_repr.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11287 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_scraper_broken.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12163 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_second_future_imports.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11617 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_svg.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    17038 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/sg_execution_times.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)  4665324 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/environment.pickle
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/examples/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/examples/future/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2627 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/examples/future/README.doctree
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    24238 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.backreferences.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    27583 2021-03-21 23:01:50.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.docs_resolv.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    23240 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.downloads.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    54703 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.gen_gallery.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    72707 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.gen_rst.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    45530 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.notebook.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    25989 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.py_source_parser.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    30747 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.sorting.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    16862 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/index.doctree
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    32286 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/minigallery.doctree
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      230 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/.buildinfo
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     8160 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/0945e908cf9aecf00af7e353b373478b/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1816 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/0945e908cf9aecf00af7e353b373478b/plot_future_imports.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/19fd12aa0d4382f326db31f16d3d1d1e/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      353 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/19fd12aa0d4382f326db31f16d3d1d1e/plot_command_line_args.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/1ef095bd0669862690bd67d790b94ef7/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      364 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/1ef095bd0669862690bd67d790b94ef7/plot_svg.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2300099a8a72b1f91aa46a11810faaaa/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1194 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2300099a8a72b1f91aa46a11810faaaa/plot_scraper_broken.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2605673e66d2cc847b70bb1bf2d4b939/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      420 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2605673e66d2cc847b70bb1bf2d4b939/plot_log.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2b12073b01b18ea3dc8c5aeafcb7eeb0/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      493 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2b12073b01b18ea3dc8c5aeafcb7eeb0/plot_future_imports_broken.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/3b0b6bf78eb66e43437306cf540227da/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2387 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/3b0b6bf78eb66e43437306cf540227da/plot_numpy_matplotlib.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/411f5bf9287e74d4e2c58e6144219a86/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      596 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/411f5bf9287e74d4e2c58e6144219a86/plot_future_imports.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/454b2c75039cd779f665618ef983be2c/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1315 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/454b2c75039cd779f665618ef983be2c/plot_command_line_args.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/4b57cb1bb48eabbaf6e5f630e7437e3b/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      717 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/4b57cb1bb48eabbaf6e5f630e7437e3b/plot_animation.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    21745 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7525ca7e05c4870d06f1177b4881f139/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      677 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7525ca7e05c4870d06f1177b4881f139/plot_matplotlib_alt.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7c725e874f6ee2b5b1ccc38e70dea163/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      436 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7c725e874f6ee2b5b1ccc38e70dea163/plot_pickle.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7dc32ed5edb2b56d912aa8b53b27e465/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1916 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7dc32ed5edb2b56d912aa8b53b27e465/plot_matplotlib_alt.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/80a6099e54c6c11338620217777d2a02/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1428 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/80a6099e54c6c11338620217777d2a02/plot_pickle.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/875869823209fb298bef99090ff5b596/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      229 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/875869823209fb298bef99090ff5b596/plot_scraper_broken.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/93047193aca007ee7c3b7b968d303020/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1060 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/93047193aca007ee7c3b7b968d303020/local_module.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/936dfa023c8a1fbfaa560a549ee3f458/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1754 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/936dfa023c8a1fbfaa560a549ee3f458/plot_log.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/9395a333d61cc5d8b4a7881c7f3a6185/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1454 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/9395a333d61cc5d8b4a7881c7f3a6185/plot_future_imports_broken.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a12f17d9ba4a6fcbe3f5fc11f7be70c9/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      706 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a12f17d9ba4a6fcbe3f5fc11f7be70c9/plot_second_future_imports.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a3e878cfae7468eb4a033c6a533aca80/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1667 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a3e878cfae7468eb4a033c6a533aca80/plot_second_future_imports.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bb97c554404070d247821825b00698e8/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1413 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bb97c554404070d247821825b00698e8/plot_numpy_matplotlib.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bf7778dabfc4caff452aaed2231aad91/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1107 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bf7778dabfc4caff452aaed2231aad91/plot_repr.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/c97a3031e7cba7452bc30b650a43ec86/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       81 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/c97a3031e7cba7452bc30b650a43ec86/local_module.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/cbb0b98552467a25c4244e5c246fa313/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1321 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/cbb0b98552467a25c4244e5c246fa313/plot_svg.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e43712bb9ad80e85ad20366b3fb3c5dd/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      131 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e43712bb9ad80e85ad20366b3fb3c5dd/plot_repr.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e63e7669ff68ac4d5808e80c4c6bfa47/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1704 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e63e7669ff68ac4d5808e80c4c6bfa47/plot_animation.ipynb
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3380 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/binder_badge_logo.svg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3380 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/binder_badge_logo1.svg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_local_module_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2402 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_001.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     7703 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_003.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   115993 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_thumb.gif
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4375 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_command_line_args_001.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     5811 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_command_line_args_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    35467 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_future_imports_broken_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_future_imports_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_log_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    28529 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_001.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    18597 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_002.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    22812 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    22555 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_numpy_matplotlib_001.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    13799 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_numpy_matplotlib_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_pickle_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_repr_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    35467 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_scraper_broken_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    34269 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_second_future_imports_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    17208 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_svg_001.svg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    17208 2021-03-21 23:01:44.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_svg_thumb.svg
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2442 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/plot_future_imports.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2214 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/plot_future_imports_broken.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      814 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/sg_execution_times.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     6339 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/index.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1612 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/local_module.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   921291 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_animation.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2148 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_command_line_args.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2290 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_log.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2764 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_matplotlib_alt.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3627 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_numpy_matplotlib.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2187 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_pickle.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1809 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_repr.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1828 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_scraper_broken.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2410 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_second_future_imports.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2099 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_svg.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2943 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/sg_execution_times.rst.txt
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/examples/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/examples/future/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       77 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/examples/future/README.rst.txt
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      920 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.backreferences.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1121 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.docs_resolv.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      873 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.downloads.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3377 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.gen_gallery.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2698 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.gen_rst.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2160 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.notebook.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1189 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.py_source_parser.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1291 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.sorting.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      696 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      816 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/minigallery.rst.txt
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11185 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/alabaster.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12171 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/basic.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3380 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/binder_badge_logo.svg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    21404 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/broken_example.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    53268 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/broken_stamp.svg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       42 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/custom.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   230273 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/demo.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     9270 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/doctools.js
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      303 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/documentation_options.js
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      286 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/file.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      101 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-binder.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      829 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-dataframe.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3714 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-rendered-html.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4071 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   280364 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/jquery-3.4.1.js
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    88145 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/jquery.js
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    10847 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/language_data.js
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       90 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/minus.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4315 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/no_image.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       90 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/plus.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4798 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/pygments.css
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    15987 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/searchtools.js
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    35168 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12140 2021-03-21 23:01:46.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/underscore.js
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11376 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/plot_future_imports.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     9109 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/plot_future_imports_broken.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     5730 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/sg_execution_times.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    16018 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/index.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     7017 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/local_module.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   820229 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_animation.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12491 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_command_line_args.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    13108 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_log.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    16841 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_matplotlib_alt.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    24703 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_numpy_matplotlib.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12984 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_pickle.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     8727 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_repr.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     9040 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_scraper_broken.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    11603 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_second_future_imports.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    13087 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_svg.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     8578 2021-03-21 23:01:40.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/sg_execution_times.html
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/binder/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      167 2021-03-21 23:01:48.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/binder/requirements.txt
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/examples/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/examples/future/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4736 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/examples/future/README.html
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12156 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.backreferences.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    15430 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.docs_resolv.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12443 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.downloads.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26286 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.gen_gallery.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    30339 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.gen_rst.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    21418 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.notebook.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    13207 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.py_source_parser.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    14992 2021-03-21 23:01:42.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.sorting.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    20077 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/genindex.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     9204 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/index.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    12519 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/minigallery.html
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1816 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/plot_future_imports.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1454 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/plot_future_imports_broken.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1060 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/local_module.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1704 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_animation.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1315 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_command_line_args.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1754 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_log.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1916 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_matplotlib_alt.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2387 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_numpy_matplotlib.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1428 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_pickle.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1107 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_repr.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1194 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_scraper_broken.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1667 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_second_future_imports.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1321 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_svg.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3078 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/objects.inv
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     6838 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/py-modindex.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4715 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/search.html
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    16063 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/searchindex.js
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/sphinx-gallery/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      281 2021-03-21 23:01:38.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/sphinx-gallery/junit-results.xml
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_static_nonstandard/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   230273 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_static_nonstandard/demo.png
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_templates/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      992 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_templates/module.rst
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    21745 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/auto_examples_jupyter.zip
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     8160 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/auto_examples_python.zip
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/images/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3380 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/images/binder_badge_logo.svg
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    35467 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/sphx_glr_plot_future_imports_broken_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/sphx_glr_plot_future_imports_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1816 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      596 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2442 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1454 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      493 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2214 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      138 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      472 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      814 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/sg_execution_times.rst
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3380 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/binder_badge_logo.svg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2402 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_001.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   115993 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_002.gif
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     7703 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_003.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4375 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_command_line_args_001.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    28529 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_matplotlib_alt_001.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    18597 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_matplotlib_alt_002.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    22555 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_numpy_matplotlib_001.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    17208 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_svg_001.svg
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_local_module_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   115993 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_animation_thumb.gif
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     5811 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_command_line_args_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_log_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    22812 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_matplotlib_alt_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    13799 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_numpy_matplotlib_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_pickle_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    26786 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_repr_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    35467 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_scraper_broken_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    34269 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_second_future_imports_thumb.png
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    17208 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_svg_thumb.svg
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     6339 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/index.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1060 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/local_module.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       81 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/local_module.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1612 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/local_module.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1704 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      717 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)   921291 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3797 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1315 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      353 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2148 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1548 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1754 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      420 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2290 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      953 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_log_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1916 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      677 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2764 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      925 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2387 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1413 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3627 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     5053 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1428 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      436 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2187 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      786 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1107 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      131 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1809 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      115 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1194 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      229 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1828 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      158 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1667 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      706 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2410 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      492 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1321 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.ipynb
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      364 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       32 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.py.md5
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2099 2021-03-21 23:01:56.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      765 2021-03-21 23:01:58.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg_codeobj.pickle
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      341 2021-03-21 23:02:02.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/searchindex.bak
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    25916 2021-03-21 23:02:02.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/searchindex.dat
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      341 2021-03-21 23:02:02.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/searchindex.dir
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2943 2021-03-21 23:02:00.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/sg_execution_times.rst
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/binder/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      167 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/binder/requirements.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3127 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/conf.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       56 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/README.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      155 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/__init__.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/future/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       77 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/future/README.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      596 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/future/plot_future_imports.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      493 2021-03-21 23:01:36.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/future/plot_future_imports_broken.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       81 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/local_module.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      717 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_animation.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      353 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_command_line_args.py
+-rw-rw-r--   0 lucy      (1000) lucy      (1000)      343 2021-04-25 05:36:15.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_defer_figures.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      420 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_log.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      717 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_matplotlib_alt.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1413 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_numpy_matplotlib.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      436 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_pickle.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      131 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_repr.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      229 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_scraper_broken.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      706 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_second_future_imports.py
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      364 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_svg.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      559 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      569 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.prop.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      567 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.run.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      599 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.ExplicitOrder.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      589 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      599 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.prop.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      597 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.run.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      582 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.NameFinder.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      597 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.identify_names.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.SphinxDocLinkResolver.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.SphinxDocLinkResolver.resolve.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.embed_code_links.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.get_data.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.docs_resolv.parse_sphinx_docopts.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.downloads.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.downloads.generate_zipfiles.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.downloads.list_downloadable_sources.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.downloads.python_zip.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.DefaultResetArgv.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.check_duplicate_filenames.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.check_spaces_in_filenames.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.collect_gallery_files.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.cost_name_key.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.generate_gallery_rst.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.get_default_config_value.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.get_subsections.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.parse_config.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.setup.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.setup_module.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.summarize_failing_examples.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.touch_empty_backreferences.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.write_computation_times.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_gallery.write_junit_xml.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.codestr2rst.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.executable_script.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.execute_code_block.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.execute_script.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.extract_intro_and_title.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.generate_dir_rst.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.generate_file_rst.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.handle_exception.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.md5sum_is_current.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.patch_warnings.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.rst_blocks.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.save_rst_example.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.gen_rst.save_thumbnail.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.add_code_cell.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.add_markdown_cell.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.directive_fun.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.fill_notebook.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.generate_image_src.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.jupyter_notebook.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.jupyter_notebook_skeleton.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.python_to_jupyter_cli.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.rst2md.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.notebook.save_notebook.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.extract_file_config.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.parse_source_file.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.remove_config_comments.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.py_source_parser.split_code_and_text_blocks.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.ExampleTitleSortKey.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      615 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.ExplicitOrder.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      585 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.FileNameSortKey.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.FileSizeSortKey.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.NumberOfCodeLinesSortKey.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        0 2021-03-21 23:01:54.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.examples
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      920 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.backreferences.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1121 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.docs_resolv.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      873 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.downloads.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     3377 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.gen_gallery.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2698 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.gen_rst.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2160 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.notebook.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1189 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.py_source_parser.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     1291 2021-03-21 23:01:52.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.sorting.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      696 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/index.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      816 2021-03-21 23:01:34.000000 sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/minigallery.rst
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     5633 2021-03-21 23:01:30.000000 sphinx-gallery-0.9.0/sphinx_gallery/utils.py
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery.egg-info/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     4848 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery.egg-info/PKG-INFO
+-rw-r--r--   0 lucy      (1000) lucy      (1000)    34515 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery.egg-info/SOURCES.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)        1 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery.egg-info/dependency_links.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       14 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery.egg-info/requires.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)       15 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/sphinx_gallery.egg-info/top_level.txt
+drwxrwxr-x   0 lucy      (1000) lucy      (1000)        0 2021-04-25 05:37:32.000000 sphinx-gallery-0.9.0/tutorials/
+-rw-r--r--   0 lucy      (1000) lucy      (1000)      366 2021-03-21 23:02:08.000000 sphinx-gallery-0.9.0/tutorials/README.txt
+-rw-r--r--   0 lucy      (1000) lucy      (1000)     2890 2021-03-21 23:02:08.000000 sphinx-gallery-0.9.0/tutorials/plot_parse.py
```

### Comparing `sphinx-gallery-0.8.2/CHANGES.rst` & `sphinx-gallery-0.9.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,73 @@
 Change Log
 ==========
 
+v0.9.0
+------
+
+Support for Python 3.5 dropped in this release. Requirement is Python >=3.6.
+
+**Implemented enhancements:**
+
+-  Add a mode which “skips” an example if it fails `#789 <https://github.com/sphinx-gallery/sphinx-gallery/issues/789>`__
+-  Can sphinx_gallery_thumbnail_number support negative indexes? `#785 <https://github.com/sphinx-gallery/sphinx-gallery/issues/785>`__
+-  Configure thumbnail style `#780 <https://github.com/sphinx-gallery/sphinx-gallery/issues/780>`__
+-  ENH: Check for invalid sphinx_gallery_conf keys `#774 <https://github.com/sphinx-gallery/sphinx-gallery/issues/774>`__
+-  DOC Document how to hide download link note `#760 <https://github.com/sphinx-gallery/sphinx-gallery/issues/760>`__
+-  DOC use intersphinx references in projects_list.rst `#755 <https://github.com/sphinx-gallery/sphinx-gallery/issues/755>`__
+-  Delay output capturing to a further code block `#363 <https://github.com/sphinx-gallery/sphinx-gallery/issues/363>`__
+-  ENH: Only add minigallery if there’s something to show `#813 <https://github.com/sphinx-gallery/sphinx-gallery/pull/813>`__ (`NicolasHug <https://github.com/NicolasHug>`__)
+-  Optional flag to defer figure scraping to the next code block `#801 <https://github.com/sphinx-gallery/sphinx-gallery/pull/801>`__ (`ayshih <https://github.com/ayshih>`__)
+-  ENH: PyQt5 `#794 <https://github.com/sphinx-gallery/sphinx-gallery/pull/794>`__ (`larsoner <https://github.com/larsoner>`__)
+-  Add a configuration to warn on error not fail `#792 <https://github.com/sphinx-gallery/sphinx-gallery/pull/792>`__ (`Cadair <https://github.com/Cadair>`__)
+-  Let sphinx_gallery_thumbnail_number support negative indexes `#786 <https://github.com/sphinx-gallery/sphinx-gallery/pull/786>`__ (`seisman <https://github.com/seisman>`__)
+-  Make any borders introduced when rescaling images to thumbnails transparent `#781 <https://github.com/sphinx-gallery/sphinx-gallery/pull/781>`__ (`rossbar <https://github.com/rossbar>`__)
+-  MAINT: Move travis CI jobs to Azure `#779 <https://github.com/sphinx-gallery/sphinx-gallery/pull/779>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+-  ENH, DEP: Check for invalid keys, remove ancient key `#775 <https://github.com/sphinx-gallery/sphinx-gallery/pull/775>`__ (`larsoner <https://github.com/larsoner>`__)
+
+**Fixed bugs:**
+
+-  Custom CSS for space above title target conflicts with pydata-sphinx-theme `#815 <https://github.com/sphinx-gallery/sphinx-gallery/issues/815>`__
+-  Minigalleries are generated even for objects without examples `#812 <https://github.com/sphinx-gallery/sphinx-gallery/issues/812>`__
+-  Python nightly failing due to Jinja2 import from collections.abc `#790 <https://github.com/sphinx-gallery/sphinx-gallery/issues/790>`__
+-  test_rebuild and test_error_messages failing on travis `#777 <https://github.com/sphinx-gallery/sphinx-gallery/issues/777>`__
+-  Animation not show on Read the Docs `#772 <https://github.com/sphinx-gallery/sphinx-gallery/issues/772>`__
+-  BUG: Empty code block output `#765 <https://github.com/sphinx-gallery/sphinx-gallery/issues/765>`__
+-  BUG: Fix CSS selector `#816 <https://github.com/sphinx-gallery/sphinx-gallery/pull/816>`__ (`larsoner <https://github.com/larsoner>`__)
+-  MAINT: Fix test for links `#811 <https://github.com/sphinx-gallery/sphinx-gallery/pull/811>`__ (`larsoner <https://github.com/larsoner>`__)
+-  Fix SVG default thumbnail support `#810 <https://github.com/sphinx-gallery/sphinx-gallery/pull/810>`__ (`jacobolofsson <https://github.com/jacobolofsson>`__)
+-  Clarify clean docs for custom gallery_dirs `#798 <https://github.com/sphinx-gallery/sphinx-gallery/pull/798>`__ (`timhoffm <https://github.com/timhoffm>`__)
+-  MAINT Specify Jinja2 version in azure Python nightly `#793 <https://github.com/sphinx-gallery/sphinx-gallery/pull/793>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+-  BUG Remove if final block empty `#791 <https://github.com/sphinx-gallery/sphinx-gallery/pull/791>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+-  Replace Travis CI badge with Azure Badge in README `#783 <https://github.com/sphinx-gallery/sphinx-gallery/pull/783>`__ (`sdhiscocks <https://github.com/sdhiscocks>`__)
+-  Point to up-to-date re documentation `#778 <https://github.com/sphinx-gallery/sphinx-gallery/pull/778>`__ (`dstansby <https://github.com/dstansby>`__)
+
+**Closed issues:**
+
+-  Generating the output notebooks together with data (folders) used for generating… `#809 <https://github.com/sphinx-gallery/sphinx-gallery/issues/809>`__
+-  How to link from one example to another? `#805 <https://github.com/sphinx-gallery/sphinx-gallery/issues/805>`__
+-  Incompatibility with matplotlib 3.4.0 ? `#802 <https://github.com/sphinx-gallery/sphinx-gallery/issues/802>`__
+-  Pandas \_repr_html\_ not captured in PDF output `#799 <https://github.com/sphinx-gallery/sphinx-gallery/issues/799>`__
+-  Optuna project Uses Sphinx-Gallery `#795 <https://github.com/sphinx-gallery/sphinx-gallery/issues/795>`__
+-  Adding an extended README `#771 <https://github.com/sphinx-gallery/sphinx-gallery/issues/771>`__
+
+**Merged pull requests:**
+
+-  DOC Add section on altering CSS `#820 <https://github.com/sphinx-gallery/sphinx-gallery/pull/820>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+-  DOC Use intersphinx references in projects_list.rst `#819 <https://github.com/sphinx-gallery/sphinx-gallery/pull/819>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+-  DOC Update CI badge `#818 <https://github.com/sphinx-gallery/sphinx-gallery/pull/818>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+-  DOC Include SOURCEDIR in Makefile `#814 <https://github.com/sphinx-gallery/sphinx-gallery/pull/814>`__ (`NicolasHug <https://github.com/NicolasHug>`__)
+-  DOC: add 2 projects using sphinx gallery `#807 <https://github.com/sphinx-gallery/sphinx-gallery/pull/807>`__ (`mfeurer <https://github.com/mfeurer>`__)
+-  DOC: clarify advanced doc wrt referencing examples `#806 <https://github.com/sphinx-gallery/sphinx-gallery/pull/806>`__ (`mfeurer <https://github.com/mfeurer>`__)
+-  MAINT: Add link `#800 <https://github.com/sphinx-gallery/sphinx-gallery/pull/800>`__ (`larsoner <https://github.com/larsoner>`__)
+-  Add Optuna to “Who uses Optuna” `#796 <https://github.com/sphinx-gallery/sphinx-gallery/pull/796>`__ (`crcrpar <https://github.com/crcrpar>`__)
+-  DOC Add segment on CSS styling `#788 <https://github.com/sphinx-gallery/sphinx-gallery/pull/788>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+-  DOC minor doc typo fixes `#787 <https://github.com/sphinx-gallery/sphinx-gallery/pull/787>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+-  DOC Update CI links in index.rst `#784 <https://github.com/sphinx-gallery/sphinx-gallery/pull/784>`__ (`lucyleeow <https://github.com/lucyleeow>`__)
+
 v0.8.2
 ------
 
 Enables HTML animations to be rendered on readthedocs.
 
 **Implemented enhancements:**
```

### Comparing `sphinx-gallery-0.8.2/LICENSE` & `sphinx-gallery-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/MANIFEST.in` & `sphinx-gallery-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/PKG-INFO` & `sphinx-gallery-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sphinx-gallery
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Sphinx extension that builds an HTML version of any Python script and puts it into an examples gallery.
 Home-page: https://sphinx-gallery.github.io
 Author: Óscar Nájera
 Author-email: najera.oscar@gmail.com
 License: 3-clause BSD
 Description: ==============
         Sphinx-Gallery
         ==============
         
-        .. image:: https://travis-ci.org/sphinx-gallery/sphinx-gallery.svg?branch=master
-            :target: https://travis-ci.org/sphinx-gallery/sphinx-gallery
+        .. image:: https://dev.azure.com/sphinx-gallery/sphinx-gallery/_apis/build/status/sphinx-gallery.sphinx-gallery?branchName=master
+            :target: https://dev.azure.com/sphinx-gallery/sphinx-gallery/_build/latest?definitionId=1&branchName=master
         
-        .. image::     https://ci.appveyor.com/api/projects/status/github/sphinx-gallery/sphinx-gallery?branch=master&svg=true
-            :target: https://ci.appveyor.com/project/sphinx-gallery/sphinx-gallery/history
+        .. image:: https://circleci.com/gh/sphinx-gallery/sphinx-gallery.svg?style=shield
+            :target: https://circleci.com/gh/sphinx-gallery/sphinx-gallery
         
         .. image:: https://zenodo.org/badge/25860190.svg
             :target: https://zenodo.org/badge/latestdoi/25860190
         
         
         A Sphinx extension that builds an HTML version of any Python
         script and puts it into an examples gallery.
@@ -45,14 +45,15 @@
         * `Matplotlib <https://matplotlib.org/index.html>`_ `Examples <https://matplotlib.org/gallery/index.html>`_ and `Tutorials  <https://matplotlib.org/tutorials/index.html>`__
         * `PyTorch tutorials <http://pytorch.org/tutorials>`_
         * `Cartopy <http://scitools.org.uk/cartopy/docs/latest/gallery/>`_
         * `PyVista <https://docs.pyvista.org/examples/>`_
         * `SimPEG <http://docs.simpeg.xyz/content/examples/>`_
         * `PlasmaPy <http://docs.plasmapy.org/en/latest/auto_examples/>`_
         * `Fury <http://fury.gl/latest/auto_examples/index.html>`_
+        * `Optuna <https://optuna.readthedocs.io/en/stable/tutorial/index.html>`_
         
         .. installation-begin-content
         
         Installation
         ============
         
         Install via ``pip``
@@ -104,9 +105,9 @@
         deposit <https://zenodo.org/record/3838216>`_.
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
```

### Comparing `sphinx-gallery-0.8.2/README.rst` & `sphinx-gallery-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ==============
 Sphinx-Gallery
 ==============
 
-.. image:: https://travis-ci.org/sphinx-gallery/sphinx-gallery.svg?branch=master
-    :target: https://travis-ci.org/sphinx-gallery/sphinx-gallery
+.. image:: https://dev.azure.com/sphinx-gallery/sphinx-gallery/_apis/build/status/sphinx-gallery.sphinx-gallery?branchName=master
+    :target: https://dev.azure.com/sphinx-gallery/sphinx-gallery/_build/latest?definitionId=1&branchName=master
 
-.. image::     https://ci.appveyor.com/api/projects/status/github/sphinx-gallery/sphinx-gallery?branch=master&svg=true
-    :target: https://ci.appveyor.com/project/sphinx-gallery/sphinx-gallery/history
+.. image:: https://circleci.com/gh/sphinx-gallery/sphinx-gallery.svg?style=shield
+    :target: https://circleci.com/gh/sphinx-gallery/sphinx-gallery
 
 .. image:: https://zenodo.org/badge/25860190.svg
     :target: https://zenodo.org/badge/latestdoi/25860190
 
 
 A Sphinx extension that builds an HTML version of any Python
 script and puts it into an examples gallery.
@@ -37,14 +37,15 @@
 * `Matplotlib <https://matplotlib.org/index.html>`_ `Examples <https://matplotlib.org/gallery/index.html>`_ and `Tutorials  <https://matplotlib.org/tutorials/index.html>`__
 * `PyTorch tutorials <http://pytorch.org/tutorials>`_
 * `Cartopy <http://scitools.org.uk/cartopy/docs/latest/gallery/>`_
 * `PyVista <https://docs.pyvista.org/examples/>`_
 * `SimPEG <http://docs.simpeg.xyz/content/examples/>`_
 * `PlasmaPy <http://docs.plasmapy.org/en/latest/auto_examples/>`_
 * `Fury <http://fury.gl/latest/auto_examples/index.html>`_
+* `Optuna <https://optuna.readthedocs.io/en/stable/tutorial/index.html>`_
 
 .. installation-begin-content
 
 Installation
 ============
 
 Install via ``pip``
```

### Comparing `sphinx-gallery-0.8.2/examples/README.txt` & `sphinx-gallery-0.9.0/examples/README.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/no_output/plot_raise.py` & `sphinx-gallery-0.9.0/examples/no_output/plot_raise.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_0_sin.py` & `sphinx-gallery-0.9.0/examples/plot_0_sin.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_1_exp.py` & `sphinx-gallery-0.9.0/examples/plot_1_exp.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_2_seaborn.py` & `sphinx-gallery-0.9.0/examples/plot_2_seaborn.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_3_capture_repr.py` & `sphinx-gallery-0.9.0/examples/plot_3_capture_repr.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_4_choose_thumbnail.py` & `sphinx-gallery-0.9.0/examples/plot_4_choose_thumbnail.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_4b_provide_thumbnail.py` & `sphinx-gallery-0.9.0/examples/plot_4b_provide_thumbnail.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_5_unicode_everywhere.py` & `sphinx-gallery-0.9.0/examples/plot_5_unicode_everywhere.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_6_function_identifier.py` & `sphinx-gallery-0.9.0/examples/plot_6_function_identifier.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_7_sys_argv.py` & `sphinx-gallery-0.9.0/examples/plot_7_sys_argv.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_8_animations.py` & `sphinx-gallery-0.9.0/examples/plot_8_animations.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/examples/plot_9_plotly.py` & `sphinx-gallery-0.9.0/examples/plot_9_plotly.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/mayavi_examples/plot_3d.py` & `sphinx-gallery-0.9.0/mayavi_examples/plot_3d.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/setup.cfg` & `sphinx-gallery-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/setup.py` & `sphinx-gallery-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         '_static/binder_badge_logo.svg'
     ]},
     scripts=['bin/copy_sphinxgallery.sh', 'bin/sphx_glr_python_to_jupyter.py'],
     url="https://sphinx-gallery.github.io",
     author="Óscar Nájera",
     author_email='najera.oscar@gmail.com',
     install_requires=install_requires,
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     license='3-clause BSD',
     classifiers=['Intended Audience :: Developers',
                  'Development Status :: 4 - Beta',
                  'Framework :: Sphinx :: Extension',
                  'Programming Language :: Python',
                  ],
 )
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/_static/binder_badge_logo.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/_static/binder_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/_static/broken_example.png` & `sphinx-gallery-0.9.0/sphinx_gallery/_static/broken_example.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/_static/gallery-dataframe.css` & `sphinx-gallery-0.9.0/sphinx_gallery/_static/gallery-dataframe.css`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/_static/gallery-rendered-html.css` & `sphinx-gallery-0.9.0/sphinx_gallery/_static/gallery-rendered-html.css`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/_static/gallery.css` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery.css`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/_static/no_image.png` & `sphinx-gallery-0.9.0/sphinx_gallery/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/backreferences.py` & `sphinx-gallery-0.9.0/sphinx_gallery/backreferences.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/binder.py` & `sphinx-gallery-0.9.0/sphinx_gallery/binder.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/directives.py` & `sphinx-gallery-0.9.0/sphinx_gallery/directives.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,14 +54,23 @@
                     heading = 'Examples using ``{}``'.format(obj_list[0])
                 else:
                     heading = 'Examples using one of multiple objects'
             lines.append(heading)
             heading_level = self.options.get('heading-level', '^')
             lines.append(heading_level * len(heading))
 
+        def has_backrefs(obj):
+            src_dir = config.sphinx_gallery_conf['src_dir']
+            path = os.path.join(src_dir, backreferences_dir,
+                                '{}.examples'.format(obj))
+            return os.path.isfile(path) and os.path.getsize(path) > 0
+
+        if not any(has_backrefs(obj) for obj in obj_list):
+            return []
+
         # Insert the backreferences file(s) using the `include` directive
         for obj in obj_list:
             path = os.path.join('/',  # Sphinx treats this as the source dir
                                 backreferences_dir,
                                 '{}.examples'.format(obj))
 
             # Always remove the heading (first 5 lines) from the file
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/docs_resolv.py` & `sphinx-gallery-0.9.0/sphinx_gallery/docs_resolv.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/downloads.py` & `sphinx-gallery-0.9.0/sphinx_gallery/downloads.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/gen_gallery.py` & `sphinx-gallery-0.9.0/sphinx_gallery/gen_gallery.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 """
 
 
 from __future__ import division, print_function, absolute_import
 import codecs
 import copy
 from datetime import timedelta, datetime
+from difflib import get_close_matches
 from importlib import import_module
 import re
 import os
 import pathlib
 from xml.sax.saxutils import quoteattr, escape
 
 from sphinx.errors import ConfigError, ExtensionError
@@ -64,14 +65,15 @@
     # -------------
     # We use a string for 'plot_gallery' rather than simply the Python boolean
     # `True` as it avoids a warning about unicode when controlling this value
     # via the command line switches of sphinx-build
     'plot_gallery': 'True',
     'download_all_examples': True,
     'abort_on_example_error': False,
+    'only_warn_on_example_error': False,
     'failing_examples': {},
     'passing_examples': [],
     'stale_examples': [],  # ones that did not need to be run due to md5sum
     'run_stale_examples': False,
     'expected_failing_examples': set(),
     'thumbnail_size': (400, 280),  # Default CSS does 0.4 scaling (160, 112)
     'min_reported_time': 0,
@@ -87,49 +89,65 @@
     'show_memory': False,
     'show_signature': True,
     'junit': '',
     'log_level': {'backreference_missing': 'warning'},
     'inspect_global_variables': True,
     'css': _KNOWN_CSS,
     'matplotlib_animations': False,
+    'default_thumb_file': None,
+    'line_numbers': False,
 }
 
 logger = sphinx_compatibility.getLogger('sphinx-gallery')
 
 
 def _bool_eval(x):
     if isinstance(x, str):
         try:
             x = eval(x)
         except TypeError:
             pass
     return bool(x)
 
 
-def parse_config(app):
+def parse_config(app, check_keys=True):
     """Process the Sphinx Gallery configuration."""
     plot_gallery = _bool_eval(app.builder.config.plot_gallery)
     src_dir = app.builder.srcdir
     abort_on_example_error = _bool_eval(
         app.builder.config.abort_on_example_error)
     lang = app.builder.config.highlight_language
     gallery_conf = _complete_gallery_conf(
         app.config.sphinx_gallery_conf, src_dir, plot_gallery,
-        abort_on_example_error, lang, app.builder.name, app)
+        abort_on_example_error, lang, app.builder.name, app,
+        check_keys)
 
     # this assures I can call the config in other places
     app.config.sphinx_gallery_conf = gallery_conf
     app.config.html_static_path.append(glr_path_static())
     return gallery_conf
 
 
 def _complete_gallery_conf(sphinx_gallery_conf, src_dir, plot_gallery,
                            abort_on_example_error, lang='python',
-                           builder_name='html', app=None):
+                           builder_name='html', app=None, check_keys=True):
     gallery_conf = copy.deepcopy(DEFAULT_GALLERY_CONF)
+    options = sorted(gallery_conf)
+    extra_keys = sorted(set(sphinx_gallery_conf) - set(options))
+    if extra_keys and check_keys:
+        msg = 'Unknown key(s) in sphinx_gallery_conf:\n'
+        for key in extra_keys:
+            options = get_close_matches(key, options, cutoff=0.66)
+            msg += repr(key)
+            if len(options) == 1:
+                msg += ', did you mean %r?' % (options[0],)
+            elif len(options) > 1:
+                msg += ', did you mean one of %r?' % (options,)
+            msg += '\n'
+        raise ConfigError(msg.strip())
     gallery_conf.update(sphinx_gallery_conf)
     if sphinx_gallery_conf.get('find_mayavi_figures', False):
         logger.warning(
             "Deprecated image scraping variable `find_mayavi_figures`\n"
             "detected, use `image_scrapers` instead as:\n\n"
             "   image_scrapers=('matplotlib', 'mayavi')",
             type=DeprecationWarning)
@@ -139,28 +157,14 @@
     # XXX anything that can only be a bool (rather than str) should probably be
     # evaluated this way as it allows setting via -D on the command line
     for key in ('run_stale_examples',):
         gallery_conf[key] = _bool_eval(gallery_conf[key])
     gallery_conf['src_dir'] = src_dir
     gallery_conf['app'] = app
 
-    if gallery_conf.get("mod_example_dir", False):
-        backreferences_warning = """\n========
-        Sphinx-Gallery found the configuration key 'mod_example_dir'. This
-        is deprecated, and you should now use the key 'backreferences_dir'
-        instead. Support for 'mod_example_dir' will be removed in a subsequent
-        version of Sphinx-Gallery. For more details, see the backreferences
-        documentation:
-
-        https://sphinx-gallery.github.io/configuration.html#references-to-examples"""  # noqa: E501
-        gallery_conf['backreferences_dir'] = gallery_conf['mod_example_dir']
-        logger.warning(
-            backreferences_warning,
-            type=DeprecationWarning)
-
     # Check capture_repr
     capture_repr = gallery_conf['capture_repr']
     supported_reprs = ['__repr__', '__str__', '_repr_html_']
     if isinstance(capture_repr, tuple):
         for rep in capture_repr:
             if rep not in supported_reprs:
                 raise ConfigError("All entries in 'capture_repr' must be one "
@@ -705,18 +709,21 @@
                    gallery_conf['filename_pattern'],
                    gallery_conf['ignore_pattern'],
                    n_stale, 's' if n_stale != 1 else '',
                    ),
                 color='brown')
 
     if fail_msgs:
-        raise ExtensionError(
-            "Here is a summary of the problems encountered "
-            "when running the examples\n\n" + "\n".join(fail_msgs) +
-            "\n" + "-" * 79)
+        fail_message = ("Here is a summary of the problems encountered "
+                        "when running the examples\n\n" +
+                        "\n".join(fail_msgs) + "\n" + "-" * 79)
+        if gallery_conf['only_warn_on_example_error']:
+            logger.warning(fail_message)
+        else:
+            raise ExtensionError(fail_message)
 
 
 def collect_gallery_files(examples_dirs, gallery_conf):
     """Collect python files from the gallery example directories."""
     files = []
     for example_dir in examples_dirs:
         for root, dirnames, filenames in os.walk(example_dir):
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/gen_rst.py` & `sphinx-gallery-0.9.0/sphinx_gallery/gen_rst.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,23 +252,29 @@
             ref_md5 = file_checksum.read()
 
         return src_md5 == ref_md5
 
     return False
 
 
-def save_thumbnail(image_path_template, src_file, file_conf, gallery_conf):
+def save_thumbnail(image_path_template, src_file, script_vars, file_conf,
+                   gallery_conf):
     """Generate and Save the thumbnail image
 
     Parameters
     ----------
     image_path_template : str
         holds the template where to save and how to name the image
     src_file : str
         path to source python file
+    script_vars : dict
+        Configuration and run time variables
+    file_conf : dict
+        File-specific settings given in source file comments as:
+        ``# sphinx_gallery_<name> = <value>``
     gallery_conf : dict
         Sphinx-Gallery configuration dictionary
     """
 
     thumb_dir = os.path.join(os.path.dirname(image_path_template), 'thumb')
     if not os.path.exists(thumb_dir):
         os.makedirs(thumb_dir)
@@ -283,32 +289,43 @@
     if thumbnail_number is None:
         image_path = os.path.join(gallery_conf['src_dir'], thumbnail_path)
     else:
         if not isinstance(thumbnail_number, int):
             raise ExtensionError(
                 'sphinx_gallery_thumbnail_number setting is not a number, '
                 'got %r' % (thumbnail_number,))
+        # negative index means counting from the last one
+        if thumbnail_number < 0:
+            thumbnail_number += len(script_vars["image_path_iterator"]) + 1
         image_path = image_path_template.format(thumbnail_number)
     del thumbnail_number, thumbnail_path, image_path_template
     thumbnail_image_path, ext = _find_image_ext(image_path)
 
     base_image_name = os.path.splitext(os.path.basename(src_file))[0]
     thumb_file = os.path.join(thumb_dir,
                               'sphx_glr_%s_thumb.%s' % (base_image_name, ext))
 
     if src_file in gallery_conf['failing_examples']:
         img = os.path.join(glr_path_static(), 'broken_example.png')
     elif os.path.exists(thumbnail_image_path):
         img = thumbnail_image_path
     elif not os.path.exists(thumb_file):
         # create something to replace the thumbnail
-        img = os.path.join(glr_path_static(), 'no_image.png')
-        img = gallery_conf.get("default_thumb_file", img)
+        default_thumb_path = gallery_conf.get("default_thumb_file")
+        if default_thumb_path is None:
+            default_thumb_path = os.path.join(
+                glr_path_static(),
+                'no_image.png',
+            )
+        img, ext = _find_image_ext(default_thumb_path)
     else:
         return
+    # update extension, since gallery_conf setting can be different
+    # from file_conf
+    thumb_file = '%s.%s' % (os.path.splitext(thumb_file)[0], ext)
     if ext in ('svg', 'gif'):
         copyfile(img, thumb_file)
     else:
         scale_image(img, thumb_file, *gallery_conf["thumbnail_size"])
         if 'thumbnails' in gallery_conf['compress_images']:
             optipng(thumb_file, gallery_conf['compress_images_args'])
 
@@ -545,15 +562,20 @@
     # First cd in the original example dir, so that any file
     # created by the example get created in this directory
 
     os.chdir(os.path.dirname(src_file))
 
     sys_path = copy.deepcopy(sys.path)
     sys.path.append(os.getcwd())
-    need_save_figures = True
+
+    # Save figures unless there is a `sphinx_gallery_defer_figures` flag
+    match = re.search(r'^[\ \t]*#\s*sphinx_gallery_defer_figures[\ \t]*\n?',
+                      bcontent, re.MULTILINE)
+    need_save_figures = match is None
+
     try:
         dont_inherit = 1
         if sys.version_info >= (3, 8):
             ast_Module = partial(ast.Module, type_ignores=[])
         else:
             ast_Module = ast.Module
         code_ast = ast_Module([bcontent])
@@ -586,16 +608,19 @@
             mem_max, _ = gallery_conf['call_memory'](
                 _exec_once(
                     compiler(code_ast, src_file, 'exec'),
                     script_vars['fake_main']))
         script_vars['memory_delta'].append(mem_max)
         # This should be inside the try block, e.g., in case of a savefig error
         logging_tee.restore_std()
-        need_save_figures = False
-        images_rst = save_figures(block, script_vars, gallery_conf)
+        if need_save_figures:
+            need_save_figures = False
+            images_rst = save_figures(block, script_vars, gallery_conf)
+        else:
+            images_rst = u''
     except Exception:
         logging_tee.restore_std()
         except_rst = handle_exception(sys.exc_info(), src_file, script_vars,
                                       gallery_conf)
         code_output = u"\n{0}\n\n\n\n".format(except_rst)
         # still call this even though we won't use the images so that
         # figures are closed
@@ -828,37 +853,44 @@
 
     script_vars = {
         'execute_script': executable,
         'image_path_iterator': ImagePathIterator(image_path_template),
         'src_file': src_file,
         'target_file': target_file}
 
-    if gallery_conf['remove_config_comments']:
-        script_blocks = [
-            (label, remove_config_comments(content), line_number)
-            for label, content, line_number in script_blocks
-        ]
-
     if executable:
         clean_modules(gallery_conf, fname)
     output_blocks, time_elapsed = execute_script(script_blocks,
                                                  script_vars,
                                                  gallery_conf)
 
     logger.debug("%s ran in : %.2g seconds\n", src_file, time_elapsed)
 
+    if gallery_conf['remove_config_comments']:
+        script_blocks = [
+            (label, remove_config_comments(content), line_number)
+            for label, content, line_number in script_blocks
+        ]
+
+    # Remove final empty block, which can occur after config comments
+    # are removed
+    if script_blocks[-1][1].isspace():
+        script_blocks = script_blocks[:-1]
+        output_blocks = output_blocks[:-1]
+
     example_rst = rst_blocks(script_blocks, output_blocks,
                              file_conf, gallery_conf)
     memory_used = gallery_conf['memory_base'] + script_vars['memory_delta']
     if not executable:
         time_elapsed = memory_used = 0.  # don't let the output change
     save_rst_example(example_rst, target_file, time_elapsed, memory_used,
                      gallery_conf)
 
-    save_thumbnail(image_path_template, src_file, file_conf, gallery_conf)
+    save_thumbnail(image_path_template, src_file, script_vars, file_conf,
+                   gallery_conf)
 
     example_nb = jupyter_notebook(script_blocks, gallery_conf, target_dir)
     ipy_fname = replace_py_ipynb(target_file) + '.new'
     save_notebook(example_nb, ipy_fname)
     _replace_md5(ipy_fname, mode='t')
 
     # Write names
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/load_style.py` & `sphinx-gallery-0.9.0/sphinx_gallery/load_style.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/notebook.py` & `sphinx-gallery-0.9.0/sphinx_gallery/notebook.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/py_source_parser.py` & `sphinx-gallery-0.9.0/sphinx_gallery/py_source_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 #
 #     a = 1
 #
 #     # sphinx_gallery_thumbnail_number = 2
 #
 #     b = 2
 INFILE_CONFIG_PATTERN = re.compile(
-    r"^[\ \t]*#\s*sphinx_gallery_([A-Za-z0-9_]+)\s*=\s*(.+)[\ \t]*\n?",
+    r"^[\ \t]*#\s*sphinx_gallery_([A-Za-z0-9_]+)(\s*=\s*(.+))?[\ \t]*\n?",
     re.MULTILINE)
 
 
 def parse_source_file(filename):
     """Parse source file into AST node.
 
     Parameters
@@ -133,15 +133,17 @@
 def extract_file_config(content):
     """
     Pull out the file-specific config specified in the docstring.
     """
     file_conf = {}
     for match in re.finditer(INFILE_CONFIG_PATTERN, content):
         name = match.group(1)
-        value = match.group(2)
+        value = match.group(3)
+        if value is None:  # a flag rather than a config setting
+            continue
         try:
             value = ast.literal_eval(value)
         except (SyntaxError, ValueError):
             logger.warning(
                 'Sphinx-gallery option %s was passed invalid value %s',
                 name, value)
         else:
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/scrapers.py` & `sphinx-gallery-0.9.0/sphinx_gallery/scrapers.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/sorting.py` & `sphinx-gallery-0.9.0/sphinx_gallery/sorting.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/sphinx_compatibility.py` & `sphinx-gallery-0.9.0/sphinx_gallery/sphinx_compatibility.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/conftest.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/reference_parse.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/reference_parse.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_backreferences.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_backreferences.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_binder.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_binder.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_docs_resolv.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_docs_resolv.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_full.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_full.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 import os
 import os.path as op
 import re
 import shutil
 import sys
 import time
 
-import numpy as np
-from numpy.testing import assert_allclose
-
 from sphinx.application import Sphinx
 from sphinx.errors import ExtensionError
 from sphinx.util.docutils import docutils_namespace
 from sphinx_gallery.utils import (_get_image, scale_image, _has_optipng,
                                   _has_pypandoc)
 
 import pytest
 
-N_TOT = 12
+N_TOT = 13
 
 N_FAILING = 2
 N_GOOD = N_TOT - N_FAILING
 N_RST = 15 + N_TOT
 N_RST = '(%s|%s)' % (N_RST, N_RST - 1)  # AppVeyor weirdness
 
 
 @pytest.fixture(scope='module')
 def sphinx_app(tmpdir_factory, req_mpl, req_pil):
+    # Skip if numpy not installed
+    pytest.importorskip("numpy")
+
     temp_dir = (tmpdir_factory.getbasetemp() / 'root').strpath
     src_dir = op.join(op.dirname(__file__), 'tinybuild')
 
     def ignore(src, names):
         return ('_build', 'gen_modules', 'auto_examples')
 
     shutil.copytree(src_dir, temp_dir, ignore=ignore)
@@ -158,14 +158,15 @@
     warning = sphinx_app._warning.getvalue()
     want = '.*fetching .*wrong_url.*404.*'
     assert re.match(want, warning, re.DOTALL) is not None, warning
 
 
 def test_thumbnail_path(sphinx_app, tmpdir):
     """Test sphinx_gallery_thumbnail_path."""
+    import numpy as np
     # Make sure our thumbnail matches what it should be
     fname_orig = op.join(
         sphinx_app.srcdir, '_static_nonstandard', 'demo.png')
     fname_thumb = op.join(
         sphinx_app.outdir, '_images',
         'sphx_glr_plot_second_future_imports_thumb.png')
     fname_new = str(tmpdir.join('new.png'))
@@ -176,14 +177,37 @@
     new = np.asarray(Image.open(fname_new))
     assert new.shape[:2] == orig.shape[:2]
     assert new.shape[2] in (3, 4)  # optipng can strip the alpha channel
     corr = np.corrcoef(new[..., :3].ravel(), orig[..., :3].ravel())[0, 1]
     assert corr > 0.99
 
 
+def test_negative_thumbnail_config(sphinx_app, tmpdir):
+    """Test 'sphinx_gallery_thumbnail_number' config works correctly for
+    negative numbers."""
+    import numpy as np
+    # Make sure our thumbnail is the 2nd (last) image
+    fname_orig = op.join(
+        sphinx_app.outdir, '_images',
+        'sphx_glr_plot_matplotlib_alt_002.png')
+    fname_thumb = op.join(
+        sphinx_app.outdir, '_images',
+        'sphx_glr_plot_matplotlib_alt_thumb.png')
+    fname_new = str(tmpdir.join('new.png'))
+    scale_image(fname_orig, fname_new,
+                *sphinx_app.config.sphinx_gallery_conf["thumbnail_size"])
+    Image = _get_image()
+    orig = np.asarray(Image.open(fname_thumb))
+    new = np.asarray(Image.open(fname_new))
+    assert new.shape[:2] == orig.shape[:2]
+    assert new.shape[2] in (3, 4)  # optipng can strip the alpha channel
+    corr = np.corrcoef(new[..., :3].ravel(), orig[..., :3].ravel())[0, 1]
+    assert corr > 0.99
+
+
 def test_command_line_args_img(sphinx_app):
     generated_examples_dir = op.join(sphinx_app.outdir, 'auto_examples')
     thumb_fname = '../_images/sphx_glr_plot_command_line_args_thumb.png'
     file_fname = op.join(generated_examples_dir, thumb_fname)
     assert op.isfile(file_fname), file_fname
 
 
@@ -247,15 +271,15 @@
     assert 'matplotlib.colors.is_color_like' in lines
     assert 'class="sphx-glr-backref-module-matplotlib-colors sphx-glr-backref-type-py-function">' in lines  # noqa: E501
     assert '#module-numpy' in lines
     assert 'numpy.arange.html' in lines
     assert 'class="sphx-glr-backref-module-numpy sphx-glr-backref-type-py-function">' in lines  # noqa: E501
     assert '#module-matplotlib.pyplot' in lines
     assert 'pyplot.html' in lines
-    assert 'matplotlib.figure.Figure.html#matplotlib.figure.Figure.tight_layout' in lines  # noqa: E501
+    assert '.html#matplotlib.figure.Figure.tight_layout' in lines
     assert 'matplotlib.axes.Axes.plot.html#matplotlib.axes.Axes.plot' in lines
     assert 'matplotlib_configuration_api.html#matplotlib.RcParams' in lines
     assert 'stdtypes.html#list' in lines
     assert 'warnings.html#warnings.warn' in lines
     assert 'itertools.html#itertools.compress' in lines
     assert 'numpy.ndarray.html' in lines
     # see issue 617
@@ -292,15 +316,15 @@
     # method
     dummy_class_meth = re.search(
         r'sphinx_gallery.backreferences.html#sphinx[_,-]gallery[.,-]backreferences[.,-][D,d]ummy[C,c]lass[.,-]run" title="sphinx_gallery.backreferences.DummyClass.run" class="sphx-glr-backref-module-sphinx_gallery-backreferences sphx-glr-backref-type-py-method"><span class="n">dc</span><span class="o">.</span><span class="n">run</span>',  # noqa: E501
         lines
     )
     assert dummy_class_meth is not None
     # property (Sphinx 2+ calls it a method rather than attribute, so regex)
-    dummy_class_prop = re.compile(r'sphinx_gallery.backreferences.html#sphinx[_,-]gallery[.,-]backreferences[.,-][D,d]ummy[C,c]lass[.,-]prop" title="sphinx_gallery.backreferences.DummyClass.prop" class="sphx-glr-backref-module-sphinx_gallery-backreferences sphx-glr-backref-type-py-(attribute|method)"><span class="n">dc</span><span class="o">.</span><span class="n">prop</span>')  # noqa: E501
+    dummy_class_prop = re.compile(r'sphinx_gallery.backreferences.html#sphinx[_,-]gallery[.,-]backreferences[.,-][D,d]ummy[C,c]lass[.,-]prop" title="sphinx_gallery.backreferences.DummyClass.prop" class="sphx-glr-backref-module-sphinx_gallery-backreferences sphx-glr-backref-type-py-(attribute|method|property)"><span class="n">dc</span><span class="o">.</span><span class="n">prop</span>')  # noqa: E501
     assert dummy_class_prop.search(lines) is not None
 
     try:
         import memory_profiler  # noqa, analysis:ignore
     except ImportError:
         assert "memory usage" not in lines
     else:
@@ -373,14 +397,17 @@
         lines = fid.read()
     assert '.. code-block:: none\n\n    is in the same cell' in lines
     assert '.. code-block:: none\n\n    is not in the same cell' in lines
 
 
 def _assert_mtimes(list_orig, list_new, different=(), ignore=()):
     """Assert that the correct set of files were changed based on mtime."""
+    import numpy as np
+    from numpy.testing import assert_allclose
+
     assert ([op.basename(x) for x in list_orig] ==
             [op.basename(x) for x in list_new])
     for orig, new in zip(list_orig, list_new):
         check_name = op.splitext(op.basename(orig))[0]
         if check_name.endswith('_codeobj'):
             check_name = check_name[:-8]
         if check_name in different:
@@ -628,15 +655,17 @@
         # get extremely unlucky and have identical run times
         # on the one script above that changes...
         'sg_execution_times',
         # this one will not change even though it was retried
         'plot_future_imports_broken',
         'plot_scraper_broken',
     )
-    if not sys.platform.startswith('win'):  # not reliable on Windows
+    # not reliable on Windows and one Ubuntu run
+    bad = sys.platform.startswith('win') or os.getenv('BAD_MTIME', '0') == '1'
+    if not bad:
         _assert_mtimes(generated_rst_0, generated_rst_1, different, ignore)
 
         # mtimes for pickles
         use_different = () if how == 'run_stale' else different
         _assert_mtimes(generated_pickle_0, generated_pickle_1, ignore=ignore)
 
         # mtimes for .py files (gh-395)
@@ -875,7 +904,21 @@
                     html, re.DOTALL)
     assert path is not None
     path = path.groups()[0]
     img_fname = op.abspath(op.join(root, path))
     assert 'binder_badge_logo' in img_fname  # can have numbers appended
     assert op.isfile(img_fname)
     assert 'https://mybinder.org/v2/gh/sphinx-gallery/sphinx-gallery.github.io/master?urlpath=lab/tree/notebooks/auto_examples/plot_svg.ipynb' in html  # noqa: E501
+
+
+def test_defer_figures(sphinx_app):
+    """Test the deferring of figures."""
+    root = op.join(sphinx_app.outdir, 'auto_examples')
+    fname = op.join(root, 'plot_defer_figures.html')
+    with codecs.open(fname, 'r', 'utf-8') as fid:
+        html = fid.read()
+
+    # The example has two code blocks with plotting commands, but the first
+    # block has the flag ``sphinx_gallery_defer_figures``.  Thus, there should
+    # be only one image, not two, in the output.
+    assert '../_images/sphx_glr_plot_defer_figures_001.png' in html
+    assert '../_images/sphx_glr_plot_defer_figures_002.png' not in html
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_gen_gallery.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_gen_gallery.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # -*- coding: utf-8 -*-
 # Author: Óscar Nájera
 # License: 3-clause BSD
 r"""
 Test Sphinx-Gallery
 """
-
-from __future__ import (division, absolute_import, print_function,
-                        unicode_literals)
 import codecs
 import os
 import re
+from pathlib import Path
 
 import pytest
 
-from sphinx.errors import ConfigError, ExtensionError
-from sphinx_gallery.gen_gallery import (check_duplicate_filenames,
-                                        check_spaces_in_filenames,
-                                        collect_gallery_files,
-                                        write_computation_times)
+from sphinx.errors import ConfigError, ExtensionError, SphinxWarning
+from sphinx_gallery.gen_gallery import (
+    check_duplicate_filenames, check_spaces_in_filenames,
+    collect_gallery_files, write_computation_times, _complete_gallery_conf)
+
+
+def test_bad_config():
+    """Test that bad config values are caught."""
+    sphinx_gallery_conf = dict(example_dir='')
+    with pytest.raises(ConfigError, match="example_dir.*did you mean 'examples_dirs'?.*"):  # noqa: E501
+        _complete_gallery_conf(sphinx_gallery_conf, '', True, False)
+    sphinx_gallery_conf = dict(n_subsection_order='')
+    with pytest.raises(ConfigError, match=r"did you mean one of \['subsection_order', 'within_.*"):  # noqa: E501
+        _complete_gallery_conf(sphinx_gallery_conf, '', True, False)
 
 
 def test_default_config(sphinx_app_wrapper):
     """Test the default Sphinx-Gallery configuration is loaded
 
     if only the extension is added to Sphinx"""
     sphinx_app = sphinx_app_wrapper.create_sphinx_app()
@@ -79,38 +86,14 @@
 def test_bad_css(sphinx_app_wrapper, err_class, err_match):
     with pytest.raises(err_class, match=err_match):
         sphinx_app_wrapper.create_sphinx_app()
 
 
 @pytest.mark.conf_file(content="""
 sphinx_gallery_conf = {
-    'mod_example_dir' : os.path.join('modules', 'gen'),
-    'examples_dirs': 'src',
-    'gallery_dirs': 'ex',
-}""")
-def test_config_old_backreferences_conf(sphinx_app_wrapper):
-    """Testing Deprecation warning message against old backreference config
-
-    In this case the user is required to update the mod_example_dir config
-    variable Sphinx-Gallery should notify the user and also silently update
-    the old config to the new one. """
-    sphinx_app = sphinx_app_wrapper.create_sphinx_app()
-    cfg = sphinx_app.config
-    assert cfg.project == "Sphinx-Gallery <Tests>"
-    assert cfg.sphinx_gallery_conf['backreferences_dir'] == os.path.join(
-        'modules', 'gen')
-    build_warn = sphinx_app._warning.getvalue()
-
-    assert "WARNING:" in build_warn
-    assert "deprecated" in build_warn
-    assert "Support for 'mod_example_dir' will be removed" in build_warn
-
-
-@pytest.mark.conf_file(content="""
-sphinx_gallery_conf = {
     'backreferences_dir': os.path.join('gen_modules', 'backreferences'),
     'examples_dirs': 'src',
     'gallery_dirs': 'ex',
 }""")
 def test_config_backreferences(sphinx_app_wrapper):
     """Test no warning is issued under the new configuration"""
     sphinx_app = sphinx_app_wrapper.create_sphinx_app()
@@ -336,14 +319,53 @@
     sphinx_app_wrapper.build_sphinx_app()
 
 
 @pytest.mark.conf_file(content="""
 sphinx_gallery_conf = {
     'examples_dirs': 'src',
     'gallery_dirs': 'ex',
+    'only_warn_on_example_error': True,
+}""")
+def test_only_warn_on_example_error(sphinx_app_wrapper):
+    """
+    Test behaviour of only_warn_on_example_error flag.
+    """
+    example_dir = Path(sphinx_app_wrapper.srcdir) / 'src'
+    with codecs.open(example_dir / 'plot_3.py', 'a', encoding='utf-8') as fid:
+        fid.write('raise ValueError')
+    sphinx_app = sphinx_app_wrapper.build_sphinx_app()
+
+    build_warn = sphinx_app._warning.getvalue()
+    assert 'plot_3.py failed to execute correctly' in build_warn
+    assert 'WARNING: Here is a summary of the problems' in build_warn
+
+
+@pytest.mark.conf_file(content="""
+sphinx_gallery_conf = {
+    'examples_dirs': 'src',
+    'gallery_dirs': 'ex',
+    'only_warn_on_example_error': True,
+}""")
+def test_only_warn_on_example_error_sphinx_warning(sphinx_app_wrapper):
+    """
+    Test behaviour of only_warn_on_example_error flag.
+    """
+    sphinx_app_wrapper.kwargs['warningiserror'] = True
+    example_dir = Path(sphinx_app_wrapper.srcdir) / 'src'
+    with codecs.open(example_dir / 'plot_3.py', 'a', encoding='utf-8') as fid:
+        fid.write('raise ValueError')
+    with pytest.raises(SphinxWarning) as excinfo:
+        sphinx_app_wrapper.build_sphinx_app()
+    assert "plot_3.py failed to execute" in str(excinfo.value)
+
+
+@pytest.mark.conf_file(content="""
+sphinx_gallery_conf = {
+    'examples_dirs': 'src',
+    'gallery_dirs': 'ex',
     'expected_failing_examples' :['src/plot_2.py'],
 }""")
 def test_examples_not_expected_to_pass(sphinx_app_wrapper):
     with pytest.raises(ExtensionError) as excinfo:
         sphinx_app_wrapper.build_sphinx_app()
     assert "expected to fail, but not failing" in str(excinfo.value)
 
@@ -363,50 +385,50 @@
 sphinx_gallery_conf = {
     'first_notebook_cell': 2,
 }""")
 def test_first_notebook_cell_config(sphinx_app_wrapper):
     from sphinx_gallery.gen_gallery import parse_config
     # First cell must be str
     with pytest.raises(ConfigError):
-        parse_config(sphinx_app_wrapper.create_sphinx_app())
+        parse_config(sphinx_app_wrapper.create_sphinx_app(), False)
 
 
 @pytest.mark.conf_file(content="""
 sphinx_gallery_conf = {
     'last_notebook_cell': 2,
 }""")
 def test_last_notebook_cell_config(sphinx_app_wrapper):
     from sphinx_gallery.gen_gallery import parse_config
     # First cell must be str
     with pytest.raises(ConfigError):
-        parse_config(sphinx_app_wrapper.create_sphinx_app())
+        parse_config(sphinx_app_wrapper.create_sphinx_app(), False)
 
 
 @pytest.mark.conf_file(content="""
 sphinx_gallery_conf = {
     'backreferences_dir': False,
 }""")
 def test_backreferences_dir_config(sphinx_app_wrapper):
     """Tests 'backreferences_dir' type checking."""
     from sphinx_gallery.gen_gallery import parse_config
     with pytest.raises(ConfigError,
                        match="The 'backreferences_dir' parameter must be of"):
-        parse_config(sphinx_app_wrapper.create_sphinx_app())
+        parse_config(sphinx_app_wrapper.create_sphinx_app(), False)
 
 
 @pytest.mark.conf_file(content="""
 import pathlib
 
 sphinx_gallery_conf = {
     'backreferences_dir': pathlib.Path('.'),
 }""")
 def test_backreferences_dir_pathlib_config(sphinx_app_wrapper):
     """Tests pathlib.Path does not raise exception."""
     from sphinx_gallery.gen_gallery import parse_config
-    parse_config(sphinx_app_wrapper.create_sphinx_app())
+    parse_config(sphinx_app_wrapper.create_sphinx_app(), False)
 
 
 def test_write_computation_times_noop():
     write_computation_times(None, None, [[[0]]])
 
 
 @pytest.mark.conf_file(content="""
@@ -415,21 +437,21 @@
 }""")
 def test_pypandoc_config_list(sphinx_app_wrapper):
     """Tests 'pypandoc' type checking."""
     from sphinx_gallery.gen_gallery import parse_config
     with pytest.raises(ConfigError,
                        match="'pypandoc' parameter must be of type bool or "
                              "dict"):
-        parse_config(sphinx_app_wrapper.create_sphinx_app())
+        parse_config(sphinx_app_wrapper.create_sphinx_app(), False)
 
 
 @pytest.mark.conf_file(content="""
 sphinx_gallery_conf = {
     'pypandoc': {'bad key': 1},
 }""")
 def test_pypandoc_config_keys(sphinx_app_wrapper):
     """Tests 'pypandoc' dictonary key checking."""
     from sphinx_gallery.gen_gallery import parse_config
     with pytest.raises(ConfigError,
                        match="'pypandoc' only accepts the following key "
                              "values:"):
-        parse_config(sphinx_app_wrapper.create_sphinx_app())
+        parse_config(sphinx_app_wrapper.create_sphinx_app(), False)
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_gen_rst.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_gen_rst.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     'This is the description of the example',
     'which goes on and on, Óscar',
     '',
     '',
     'And this is a second paragraph',
     '"""',
     '',
-    '# sphinx_gallery_thumbnail_number = 1'
+    '# sphinx_gallery_thumbnail_number = 1',
+    '# sphinx_gallery_defer_figures',
     '# and now comes the module code',
     'import logging',
     'import sys',
     'from warnings import warn',
     'x, y = 1, 2',
     'print(u"Óscar output") # need some code output',
     'logger = logging.getLogger()',
@@ -441,18 +442,32 @@
     assert '.jpg' in rst
 
 
 def test_remove_config_comments(gallery_conf, req_pil):
     """Test the gallery_conf['remove_config_comments'] setting."""
     rst = _generate_rst(gallery_conf, 'test.py', CONTENT)
     assert '# sphinx_gallery_thumbnail_number = 1' in rst
+    assert '# sphinx_gallery_defer_figures' in rst
 
     gallery_conf['remove_config_comments'] = True
     rst = _generate_rst(gallery_conf, 'test.py', CONTENT)
     assert '# sphinx_gallery_thumbnail_number = 1' not in rst
+    assert '# sphinx_gallery_defer_figures' not in rst
+
+
+def test_final_empty_block(gallery_conf, req_pil):
+    """Test empty final block is removed. Empty final block can occur after
+    sole config comment is removed from final block."""
+    CONTENT.extend(
+        ('# %%', '', '# sphinx_gallery_line_numbers = True')
+    )
+    gallery_conf['remove_config_comments'] = True
+    rst = _generate_rst(gallery_conf, 'test.py', CONTENT)
+    want = "RuntimeWarning)\n\n\n.. rst-class:: sphx-glr-timing"
+    assert want in rst
 
 
 def test_download_link_note_only_html(gallery_conf, req_pil):
     """Test html only directive for download_link."""
     rst = _generate_rst(gallery_conf, 'test.py', CONTENT)
     download_link_note = (".. only:: html\n\n"
                           "    .. note::\n"
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_load_style.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_load_style.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_notebook.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_py_source_parser.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_py_source_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,18 @@
      {'line_numbers': True}),
     ("  #   sphinx_gallery_line_numbers   =   True   ",
      {'line_numbers': True}),
     ("#sphinx_gallery_line_numbers=True",
      {'line_numbers': True}),
     ("#sphinx_gallery_thumbnail_number\n=\n5",
      {'thumbnail_number': 5}),
-    ('#sphinx_gallery_thumbnail_number=1foo', None),
+    ("#sphinx_gallery_thumbnail_number=1foo",
+     None),
+    ("# sphinx_gallery_defer_figures",
+     {}),
 ])
 def test_extract_file_config(content, file_conf, log_collector):
     if file_conf is None:
         assert sg.extract_file_config(content) == {}
         assert len(log_collector.calls['warning']) == 1
         assert '1foo' == log_collector.calls['warning'][0].args[2]
     else:
@@ -70,10 +73,12 @@
      ""),
     ("a = 1\n# sphinx_gallery_line_numbers = True\nb = 1",
      "a = 1\nb = 1"),
     ("a = 1\n\n# sphinx_gallery_line_numbers = True\n\nb = 1",
      "a = 1\n\n\nb = 1"),
     ("# comment\n# sphinx_gallery_line_numbers = True\n# commment 2",
      "# comment\n# commment 2"),
+    ("# sphinx_gallery_defer_figures",
+     ""),
 ])
 def test_remove_config_comments(contents, result):
     assert sg.remove_config_comments(contents) == result
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_scrapers.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_scrapers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 
 import pytest
-import numpy as np
 
 from sphinx.errors import ConfigError, ExtensionError
 import sphinx_gallery
 from sphinx_gallery.gen_gallery import _complete_gallery_conf
 from sphinx_gallery.scrapers import (figure_rst, mayavi_scraper, SINGLE_IMAGE,
                                      matplotlib_scraper, ImagePathIterator,
                                      save_figures, _KNOWN_IMG_EXTS)
 from sphinx_gallery.utils import _get_image
 
 
 @pytest.fixture(scope='function')
 def gallery_conf(tmpdir):
     """Sets up a test sphinx-gallery configuration"""
+    # Skip if numpy not installed
+    pytest.importorskip("numpy")
+
     gallery_conf = _complete_gallery_conf({}, str(tmpdir), True, False)
     gallery_conf.update(examples_dir=str(tmpdir), gallery_dir=str(tmpdir))
     return gallery_conf
 
 
 class matplotlib_svg_scraper():
 
@@ -60,14 +62,15 @@
         assert fname in image_rst
         fname = gallery_conf['gallery_dir'] + fname
         assert os.path.isfile(fname)
 
 
 def test_save_mayavi_figures(gallery_conf, req_mpl, req_pil):
     """Test file naming when saving figures. Requires mayavi."""
+    import numpy as np
     Image = _get_image()
     try:
         from mayavi import mlab
     except ImportError:
         raise pytest.skip('Mayavi not installed')
     import matplotlib.pyplot as plt
     mlab.options.offscreen = True
@@ -127,27 +130,28 @@
     # Test the API contract for custom scrapers
     complete_args = (gallery_conf, gallery_conf['gallery_dir'], True, False)
     with monkeypatch.context() as m:
         m.setattr(sphinx_gallery, '_get_sg_image_scraper',
                   lambda: _custom_func, raising=False)
         for cust in (_custom_func, 'sphinx_gallery'):
             gallery_conf.update(image_scrapers=[cust])
-            _complete_gallery_conf(*complete_args)  # smoke test that it works
+            # smoke test that it works
+            _complete_gallery_conf(*complete_args, check_keys=False)
     # degenerate
     # without the monkey patch to add sphinx_gallery._get_sg_image_scraper,
     # we should get an error
     gallery_conf.update(image_scrapers=['sphinx_gallery'])
     with pytest.raises(ConfigError,
                        match="has no attribute '_get_sg_image_scraper'"):
-        _complete_gallery_conf(*complete_args)
+        _complete_gallery_conf(*complete_args, check_keys=False)
 
     # other degenerate conditions
     gallery_conf.update(image_scrapers=['foo'])
     with pytest.raises(ConfigError, match='Unknown image scraper'):
-        _complete_gallery_conf(*complete_args)
+        _complete_gallery_conf(*complete_args, check_keys=False)
     gallery_conf.update(image_scrapers=[_custom_func])
     fname_template = os.path.join(gallery_conf['gallery_dir'],
                                   'image{0}.png')
     image_path_iterator = ImagePathIterator(fname_template)
     block = ('',) * 3
     block_vars = dict(image_path_iterator=image_path_iterator)
     with pytest.raises(ExtensionError, match='did not produce expected image'):
@@ -157,20 +161,20 @@
         save_figures(block, block_vars, gallery_conf)
     # degenerate string interface
     gallery_conf.update(image_scrapers=['sphinx_gallery'])
     with monkeypatch.context() as m:
         m.setattr(sphinx_gallery, '_get_sg_image_scraper', 'foo',
                   raising=False)
         with pytest.raises(ConfigError, match='^Unknown image.*\n.*callable'):
-            _complete_gallery_conf(*complete_args)
+            _complete_gallery_conf(*complete_args, check_keys=False)
     with monkeypatch.context() as m:
         m.setattr(sphinx_gallery, '_get_sg_image_scraper', lambda: 'foo',
                   raising=False)
         with pytest.raises(ConfigError, match='^Scraper.*was not callable'):
-            _complete_gallery_conf(*complete_args)
+            _complete_gallery_conf(*complete_args, check_keys=False)
 
 
 @pytest.mark.parametrize('ext', _KNOWN_IMG_EXTS)
 def test_figure_rst(ext):
     """Testing rst of images"""
     figure_list = ['sphx_glr_plot_1.' + ext]
     image_rst = figure_rst(figure_list, '.')
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_sorting.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_sphinx_compatibility.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_sphinx_compatibility.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/test_utils.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/plot_future_imports.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/plot_future_imports.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/plot_future_imports_broken.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/plot_future_imports_broken.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/sg_execution_times.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/future/sg_execution_times.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/index.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/index.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/local_module.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/local_module.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_animation.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_animation.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_command_line_args.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_command_line_args.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_log.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_log.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_matplotlib_alt.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_matplotlib_alt.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_numpy_matplotlib.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_numpy_matplotlib.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_pickle.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_pickle.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_repr.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_repr.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_scraper_broken.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_scraper_broken.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_second_future_imports.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_second_future_imports.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_svg.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/plot_svg.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/sg_execution_times.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/auto_examples/sg_execution_times.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/environment.pickle` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/examples/future/README.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/examples/future/README.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.backreferences.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.backreferences.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.docs_resolv.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.docs_resolv.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.downloads.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.downloads.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.gen_gallery.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.gen_gallery.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.gen_rst.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.gen_rst.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.notebook.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.notebook.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.py_source_parser.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.py_source_parser.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.sorting.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/gen_modules/sphinx_gallery.sorting.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/index.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/doctrees/minigallery.doctree` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/doctrees/minigallery.doctree`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/0945e908cf9aecf00af7e353b373478b/plot_future_imports.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/0945e908cf9aecf00af7e353b373478b/plot_future_imports.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2300099a8a72b1f91aa46a11810faaaa/plot_scraper_broken.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/2300099a8a72b1f91aa46a11810faaaa/plot_scraper_broken.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/3b0b6bf78eb66e43437306cf540227da/plot_numpy_matplotlib.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/3b0b6bf78eb66e43437306cf540227da/plot_numpy_matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/411f5bf9287e74d4e2c58e6144219a86/plot_future_imports.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/411f5bf9287e74d4e2c58e6144219a86/plot_future_imports.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/454b2c75039cd779f665618ef983be2c/plot_command_line_args.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/454b2c75039cd779f665618ef983be2c/plot_command_line_args.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/4b57cb1bb48eabbaf6e5f630e7437e3b/plot_animation.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/4b57cb1bb48eabbaf6e5f630e7437e3b/plot_animation.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7525ca7e05c4870d06f1177b4881f139/plot_matplotlib_alt.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7525ca7e05c4870d06f1177b4881f139/plot_matplotlib_alt.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7dc32ed5edb2b56d912aa8b53b27e465/plot_matplotlib_alt.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/7dc32ed5edb2b56d912aa8b53b27e465/plot_matplotlib_alt.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/80a6099e54c6c11338620217777d2a02/plot_pickle.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/80a6099e54c6c11338620217777d2a02/plot_pickle.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/93047193aca007ee7c3b7b968d303020/local_module.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/93047193aca007ee7c3b7b968d303020/local_module.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/936dfa023c8a1fbfaa560a549ee3f458/plot_log.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/936dfa023c8a1fbfaa560a549ee3f458/plot_log.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/9395a333d61cc5d8b4a7881c7f3a6185/plot_future_imports_broken.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/9395a333d61cc5d8b4a7881c7f3a6185/plot_future_imports_broken.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a12f17d9ba4a6fcbe3f5fc11f7be70c9/plot_second_future_imports.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a12f17d9ba4a6fcbe3f5fc11f7be70c9/plot_second_future_imports.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a3e878cfae7468eb4a033c6a533aca80/plot_second_future_imports.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/a3e878cfae7468eb4a033c6a533aca80/plot_second_future_imports.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bb97c554404070d247821825b00698e8/plot_numpy_matplotlib.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bb97c554404070d247821825b00698e8/plot_numpy_matplotlib.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bf7778dabfc4caff452aaed2231aad91/plot_repr.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/bf7778dabfc4caff452aaed2231aad91/plot_repr.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/cbb0b98552467a25c4244e5c246fa313/plot_svg.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/cbb0b98552467a25c4244e5c246fa313/plot_svg.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e63e7669ff68ac4d5808e80c4c6bfa47/plot_animation.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_downloads/e63e7669ff68ac4d5808e80c4c6bfa47/plot_animation.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/binder_badge_logo.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/binder_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/binder_badge_logo1.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/binder_badge_logo1.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_local_module_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_local_module_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_001.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_001.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_003.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_003.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_thumb.gif` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_animation_thumb.gif`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_command_line_args_001.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_command_line_args_001.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_command_line_args_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_command_line_args_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_future_imports_broken_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_future_imports_broken_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_future_imports_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_future_imports_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_log_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_log_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_001.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_001.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_002.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_002.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_matplotlib_alt_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_numpy_matplotlib_001.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_numpy_matplotlib_001.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_numpy_matplotlib_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_numpy_matplotlib_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_pickle_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_pickle_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_repr_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_repr_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_scraper_broken_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_scraper_broken_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_second_future_imports_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_second_future_imports_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_svg_001.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_svg_001.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_svg_thumb.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_images/sphx_glr_plot_svg_thumb.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/plot_future_imports.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/plot_future_imports.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/plot_future_imports_broken.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/plot_future_imports_broken.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/sg_execution_times.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/future/sg_execution_times.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/index.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/index.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/local_module.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/local_module.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_animation.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_animation.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_command_line_args.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_command_line_args.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_log.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_log.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_matplotlib_alt.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_matplotlib_alt.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_numpy_matplotlib.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_numpy_matplotlib.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_pickle.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_pickle.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_repr.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_repr.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_scraper_broken.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_scraper_broken.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_second_future_imports.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_second_future_imports.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_svg.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/plot_svg.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/sg_execution_times.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/auto_examples/sg_execution_times.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.backreferences.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.backreferences.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.docs_resolv.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.docs_resolv.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.downloads.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.downloads.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.gen_gallery.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.gen_gallery.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.gen_rst.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.gen_rst.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.notebook.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.notebook.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.py_source_parser.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.py_source_parser.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.sorting.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/gen_modules/sphinx_gallery.sorting.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/index.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_sources/minigallery.rst.txt` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_sources/minigallery.rst.txt`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/alabaster.css` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/basic.css` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/binder_badge_logo.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/binder_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/broken_example.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/broken_example.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/broken_stamp.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/broken_stamp.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/demo.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/demo.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/doctools.js` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-dataframe.css` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-dataframe.css`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-rendered-html.css` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery-rendered-html.css`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/gallery.css` & `sphinx-gallery-0.9.0/sphinx_gallery/_static/gallery.css`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 div.sphx-glr-download a:hover {
   box-shadow: inset 0 1px 0 rgba(255,255,255,.1), 0 1px 5px rgba(0,0,0,.25);
   text-decoration: none;
   background-image: none;
   background-color: #d5d57e;
 }
 
-.sphx-glr-example-title > :target::before {
+.sphx-glr-example-title:target::before {
   display: block;
   content: "";
   margin-top: -50px;
   height: 50px;
   visibility: hidden;
 }
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/jquery-3.4.1.js` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/jquery.js` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/language_data.js` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/no_image.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/pygments.css` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/searchtools.js` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/underscore-1.3.1.js` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/_static/underscore.js` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/plot_future_imports.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/plot_future_imports.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/plot_future_imports_broken.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/plot_future_imports_broken.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/sg_execution_times.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/future/sg_execution_times.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/index.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/index.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/local_module.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/local_module.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_animation.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_animation.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_command_line_args.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_command_line_args.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_log.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_log.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_matplotlib_alt.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_matplotlib_alt.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_numpy_matplotlib.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_numpy_matplotlib.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_pickle.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_pickle.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_repr.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_repr.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_scraper_broken.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_scraper_broken.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_second_future_imports.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_second_future_imports.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_svg.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/plot_svg.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/sg_execution_times.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/auto_examples/sg_execution_times.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/examples/future/README.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/examples/future/README.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.backreferences.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.backreferences.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.docs_resolv.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.docs_resolv.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.downloads.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.downloads.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.gen_gallery.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.gen_gallery.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.gen_rst.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.gen_rst.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.notebook.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.notebook.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.py_source_parser.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.py_source_parser.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.sorting.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/gen_modules/sphinx_gallery.sorting.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/genindex.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/index.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/minigallery.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/minigallery.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/plot_future_imports.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/plot_future_imports.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/plot_future_imports_broken.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/future/plot_future_imports_broken.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/local_module.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/local_module.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_animation.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_animation.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_command_line_args.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_command_line_args.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_log.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_log.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_matplotlib_alt.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_matplotlib_alt.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_numpy_matplotlib.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_numpy_matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_pickle.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_pickle.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_repr.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_repr.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_scraper_broken.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_scraper_broken.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_second_future_imports.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_second_future_imports.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_svg.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/notebooks/auto_examples/plot_svg.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/objects.inv` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/py-modindex.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/search.html` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_build/html/searchindex.js` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_static_nonstandard/demo.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_static_nonstandard/demo.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/_templates/module.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/auto_examples_jupyter.zip` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/auto_examples_jupyter.zip`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/auto_examples_python.zip` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/auto_examples_python.zip`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/images/binder_badge_logo.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/images/binder_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/sphx_glr_plot_future_imports_broken_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/sphx_glr_plot_future_imports_broken_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/sphx_glr_plot_future_imports_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/images/thumb/sphx_glr_plot_future_imports_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/plot_future_imports_broken.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/future/sg_execution_times.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/future/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/binder_badge_logo.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/binder_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_001.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_001.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_002.gif` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_002.gif`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_003.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_animation_003.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_command_line_args_001.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_command_line_args_001.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_matplotlib_alt_001.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_matplotlib_alt_001.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_matplotlib_alt_002.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_matplotlib_alt_002.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_numpy_matplotlib_001.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_numpy_matplotlib_001.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_svg_001.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/sphx_glr_plot_svg_001.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_local_module_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_local_module_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_animation_thumb.gif` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_animation_thumb.gif`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_command_line_args_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_command_line_args_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_log_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_log_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_matplotlib_alt_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_matplotlib_alt_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_numpy_matplotlib_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_numpy_matplotlib_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_pickle_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_pickle_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_repr_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_repr_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_scraper_broken_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_scraper_broken_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_second_future_imports_thumb.png` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_second_future_imports_thumb.png`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_svg_thumb.svg` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_svg_thumb.svg`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/index.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/local_module.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/local_module.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/local_module.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/local_module.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation_codeobj.pickle` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_animation_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args_codeobj.pickle` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_command_line_args_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_log.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_log_codeobj.pickle` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_log_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt_codeobj.pickle` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_matplotlib_alt_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib_codeobj.pickle` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_numpy_matplotlib_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle_codeobj.pickle` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_pickle_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_repr.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_scraper_broken.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_second_future_imports.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.ipynb` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.ipynb`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg_codeobj.pickle` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/plot_svg_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/searchindex.dat` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/searchindex.dat`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/auto_examples/sg_execution_times.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/auto_examples/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/conf.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/conf.py`

 * *Files identical despite different names*

```diff
@@ -78,15 +78,15 @@
                'use_jupyter_lab': True,
                },
     'examples_dirs': ['examples/'],
     'reset_argv': ResetArgv(),
     'reset_modules': (MockScrapeProblem(), 'matplotlib'),
     'gallery_dirs': ['auto_examples'],
     'backreferences_dir': 'gen_modules/backreferences',
-    'within_section_order': FileNameSortKey,
+    'within_subsection_order': FileNameSortKey,
     'image_scrapers': (matplotlib_format_scraper(),),
     'expected_failing_examples': [
         'examples/future/plot_future_imports_broken.py',
         'examples/plot_scraper_broken.py',
     ],
     'show_memory': True,
     'compress_images': ('images', 'thumbnails'),
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/future/plot_future_imports.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/future/plot_future_imports.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_animation.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_animation.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_matplotlib_alt.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_matplotlib_alt.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 plt.show()
 
 
 # %%
 # Several titles.
 
+# sphinx_gallery_thumbnail_number = -1
+
 plt.plot(range(10))
 
 plt.title('Center Title')
 plt.title('Left Title', loc='left')
 plt.title('Right Title', loc='right')
 
 plt.show()
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_numpy_matplotlib.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_numpy_matplotlib.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/examples/plot_second_future_imports.py` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/examples/plot_second_future_imports.py`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.prop.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.prop.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.run.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.DummyClass.run.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.ExplicitOrder.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.ExplicitOrder.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.prop.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.prop.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.run.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.DummyClass.run.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.NameFinder.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.NameFinder.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.identify_names.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.backreferences.identify_names.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.ExplicitOrder.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.ExplicitOrder.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.FileNameSortKey.examples` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/backreferences/sphinx_gallery.sorting.FileNameSortKey.examples`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.backreferences.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.backreferences.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.docs_resolv.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.docs_resolv.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.downloads.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.downloads.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.gen_gallery.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.gen_gallery.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.gen_rst.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.gen_rst.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.notebook.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.notebook.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.py_source_parser.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.py_source_parser.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.sorting.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/gen_modules/sphinx_gallery.sorting.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/index.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/tests/tinybuild/minigallery.rst` & `sphinx-gallery-0.9.0/sphinx_gallery/tests/tinybuild/minigallery.rst`

 * *Files identical despite different names*

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery/utils.py` & `sphinx-gallery-0.9.0/sphinx_gallery/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     # already smaller than max_width, max_height, then this won't scale up
     # at all (maybe could be an option someday...)
     img = img.resize((width_sc, height_sc), Image.BICUBIC)
     # img.thumbnail((width_sc, height_sc), Image.BICUBIC)
     # width_sc, height_sc = img.size  # necessary if using thumbnail
 
     # insert centered
-    thumb = Image.new('RGBA', (max_width, max_height), (255, 255, 255, 255))
+    thumb = Image.new('RGBA', (max_width, max_height), (255, 255, 255, 0))
     pos_insert = ((max_width - width_sc) // 2, (max_height - height_sc) // 2)
     thumb.paste(img, pos_insert)
 
     try:
         thumb.save(out_fname)
     except IOError:
         # try again, without the alpha channel (e.g., for JPEG)
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery.egg-info/PKG-INFO` & `sphinx-gallery-0.9.0/sphinx_gallery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sphinx-gallery
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Sphinx extension that builds an HTML version of any Python script and puts it into an examples gallery.
 Home-page: https://sphinx-gallery.github.io
 Author: Óscar Nájera
 Author-email: najera.oscar@gmail.com
 License: 3-clause BSD
 Description: ==============
         Sphinx-Gallery
         ==============
         
-        .. image:: https://travis-ci.org/sphinx-gallery/sphinx-gallery.svg?branch=master
-            :target: https://travis-ci.org/sphinx-gallery/sphinx-gallery
+        .. image:: https://dev.azure.com/sphinx-gallery/sphinx-gallery/_apis/build/status/sphinx-gallery.sphinx-gallery?branchName=master
+            :target: https://dev.azure.com/sphinx-gallery/sphinx-gallery/_build/latest?definitionId=1&branchName=master
         
-        .. image::     https://ci.appveyor.com/api/projects/status/github/sphinx-gallery/sphinx-gallery?branch=master&svg=true
-            :target: https://ci.appveyor.com/project/sphinx-gallery/sphinx-gallery/history
+        .. image:: https://circleci.com/gh/sphinx-gallery/sphinx-gallery.svg?style=shield
+            :target: https://circleci.com/gh/sphinx-gallery/sphinx-gallery
         
         .. image:: https://zenodo.org/badge/25860190.svg
             :target: https://zenodo.org/badge/latestdoi/25860190
         
         
         A Sphinx extension that builds an HTML version of any Python
         script and puts it into an examples gallery.
@@ -45,14 +45,15 @@
         * `Matplotlib <https://matplotlib.org/index.html>`_ `Examples <https://matplotlib.org/gallery/index.html>`_ and `Tutorials  <https://matplotlib.org/tutorials/index.html>`__
         * `PyTorch tutorials <http://pytorch.org/tutorials>`_
         * `Cartopy <http://scitools.org.uk/cartopy/docs/latest/gallery/>`_
         * `PyVista <https://docs.pyvista.org/examples/>`_
         * `SimPEG <http://docs.simpeg.xyz/content/examples/>`_
         * `PlasmaPy <http://docs.plasmapy.org/en/latest/auto_examples/>`_
         * `Fury <http://fury.gl/latest/auto_examples/index.html>`_
+        * `Optuna <https://optuna.readthedocs.io/en/stable/tutorial/index.html>`_
         
         .. installation-begin-content
         
         Installation
         ============
         
         Install via ``pip``
@@ -104,9 +105,9 @@
         deposit <https://zenodo.org/record/3838216>`_.
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
```

### Comparing `sphinx-gallery-0.8.2/sphinx_gallery.egg-info/SOURCES.txt` & `sphinx-gallery-0.9.0/sphinx_gallery.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -352,14 +352,15 @@
 sphinx_gallery/tests/tinybuild/auto_examples/images/thumb/sphx_glr_plot_svg_thumb.svg
 sphinx_gallery/tests/tinybuild/binder/requirements.txt
 sphinx_gallery/tests/tinybuild/examples/README.txt
 sphinx_gallery/tests/tinybuild/examples/__init__.py
 sphinx_gallery/tests/tinybuild/examples/local_module.py
 sphinx_gallery/tests/tinybuild/examples/plot_animation.py
 sphinx_gallery/tests/tinybuild/examples/plot_command_line_args.py
+sphinx_gallery/tests/tinybuild/examples/plot_defer_figures.py
 sphinx_gallery/tests/tinybuild/examples/plot_log.py
 sphinx_gallery/tests/tinybuild/examples/plot_matplotlib_alt.py
 sphinx_gallery/tests/tinybuild/examples/plot_numpy_matplotlib.py
 sphinx_gallery/tests/tinybuild/examples/plot_pickle.py
 sphinx_gallery/tests/tinybuild/examples/plot_repr.py
 sphinx_gallery/tests/tinybuild/examples/plot_scraper_broken.py
 sphinx_gallery/tests/tinybuild/examples/plot_second_future_imports.py
```

### Comparing `sphinx-gallery-0.8.2/tutorials/plot_parse.py` & `sphinx-gallery-0.9.0/tutorials/plot_parse.py`

 * *Files identical despite different names*

