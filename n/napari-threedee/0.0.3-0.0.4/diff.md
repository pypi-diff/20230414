# Comparing `tmp/napari-threedee-0.0.3.tar.gz` & `tmp/napari-threedee-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-threedee-0.0.3.tar", last modified: Tue Feb 28 14:39:43 2023, max compression
+gzip compressed data, was "napari-threedee-0.0.4.tar", last modified: Fri Apr 14 19:26:21 2023, max compression
```

## Comparing `napari-threedee-0.0.3.tar` & `napari-threedee-0.0.4.tar`

### file list

```diff
@@ -1,175 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.474111 napari-threedee-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.442112 napari-threedee-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.450111 napari-threedee-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/.github/workflows/test-docs-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.450111 napari-threedee-0.0.3/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-02-28 14:39:43.474111 napari-threedee-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.450111 napari-threedee-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.450111 napari-threedee-0.0.3/docs/API/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/API/geometry_utilities.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/API/napari_utilities.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/API/selection_utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.450111 napari-threedee-0.0.3/docs/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/annotations/io.md
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/annotations/point_spec.md
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/annotations/specifications.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/annotations/sphere_spec.md
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/annotations/spline_spec.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.454111 napari-threedee-0.0.3/docs/dev_guides/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/dev_guides/core_concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/dev_guides/manipulators.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.454111 napari-threedee-0.0.3/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/getting_started/developers.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/getting_started/users.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.454111 napari-threedee-0.0.3/docs/how_to/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/how_to/layer_manipulator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/how_to/point_manipulator.md
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/how_to/render_plane_manipulator.md
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.454111 napari-threedee-0.0.3/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.454111 napari-threedee-0.0.3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/docs/tutorials/tutorials.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.454111 napari-threedee-0.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/empty_surface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.454111 napari-threedee-0.0.3/examples/library/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/library/camera_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/library/layer_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/library/mesh_headlight.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/library/point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/library/render_plane_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/library/sphere_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/library/spline_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/library/surface_annotator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.458111 napari-threedee-0.0.3/examples/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/plugin/camera_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/plugin/layer_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/plugin/mesh_headlight.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/plugin/plane_point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/plugin/points_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/plugin/render_plane_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/examples/plugin/spline_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-02-28 14:39:43.478111 napari-threedee-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.446112 napari-threedee-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.458111 napari-threedee-0.0.3/src/napari_threedee/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.458111 napari-threedee-0.0.3/src/napari_threedee/_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.462112 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.462112 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_axis_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_central_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_drag_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_rotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/axis_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/central_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/drag_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/manipulator_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/napari_manipulator_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/rotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/vispy_manipulator_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/vispy_visual_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/threedee_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_backend/threedee_widget_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.462112 napari-threedee-0.0.3/src/napari_threedee/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/_tests/test_mouse_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-28 14:39:43.000000 napari-threedee-0.0.3/src/napari_threedee/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.466112 napari-threedee-0.0.3/src/napari_threedee/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.466112 napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/qt_plane_point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/qt_point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/qt_sphere_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/qt_spline_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/qt_surface_annotator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.466112 napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/test_plane_point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/test_sphere_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/test_spline_annotator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.470111 napari-threedee-0.0.3/src/napari_threedee/annotators/io/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.470111 napari-threedee-0.0.3/src/napari_threedee/annotators/io/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/_tests/test_napari.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/_tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/_tests/test_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/_tests/test_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/io/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/sphere_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/spline_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/annotators/surface_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/dock_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/geometry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.470111 napari-threedee-0.0.3/src/napari_threedee/manipulators/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.470111 napari-threedee-0.0.3/src/napari_threedee/manipulators/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/_qt/qt_layer_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/_qt/qt_point_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/_qt/qt_render_plane_manipulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.474111 napari-threedee-0.0.3/src/napari_threedee/manipulators/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/_tests/test_manipulator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/base_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/layer_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/manipulator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/point_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/manipulators/render_plane_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/mouse_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.474111 napari-threedee-0.0.3/src/napari_threedee/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.474111 napari-threedee-0.0.3/src/napari_threedee/utils/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/utils/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/utils/_tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/utils/napari_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/utils/selection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/vispy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.474111 napari-threedee-0.0.3/src/napari_threedee/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.474111 napari-threedee-0.0.3/src/napari_threedee/visualization/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/visualization/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/visualization/_qt/qt_camera_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/visualization/_qt/qt_lighting_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.474111 napari-threedee-0.0.3/src/napari_threedee/visualization/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/visualization/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/visualization/_tests/test_camera_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/visualization/camera_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/src/napari_threedee/visualization/lighting_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:43.458111 napari-threedee-0.0.3/src/napari_threedee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-02-28 14:39:43.000000 napari-threedee-0.0.3/src/napari_threedee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-02-28 14:39:43.000000 napari-threedee-0.0.3/src/napari_threedee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:39:43.000000 napari-threedee-0.0.3/src/napari_threedee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-28 14:39:43.000000 napari-threedee-0.0.3/src/napari_threedee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-28 14:39:43.000000 napari-threedee-0.0.3/src/napari_threedee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-28 14:39:43.000000 napari-threedee-0.0.3/src/napari_threedee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-28 14:39:33.000000 napari-threedee-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.034209 napari-threedee-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.014209 napari-threedee-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-14 19:26:21.034209 napari-threedee-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/docs/API/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/API/geometry_utilities.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/API/napari_utilities.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/API/selection_utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/docs/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/annotations/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/annotations/point_spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/annotations/specifications.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/annotations/sphere_spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/annotations/spline_spec.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/docs/dev_guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/dev_guides/core_concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/dev_guides/manipulators.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/docs/examples/library/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/camera_spline_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/layer_manipulator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/mesh_headlight_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/path_annotator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/point_annotator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/render_plane_manipulator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/sphere_annotator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/library/surface_annotator_library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.018209 napari-threedee-0.0.4/docs/examples/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/camera_spline_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/layer_manipulator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/mesh_headlight_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/path_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/point_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/points_manipulator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/render_plane_manipulator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/sphere_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/spline_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/examples/plugin/surface_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/gallery_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.022209 napari-threedee-0.0.4/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/getting_started/developers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/getting_started/users.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.022209 napari-threedee-0.0.4/docs/how_to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/how_to/layer_manipulator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/how_to/point_annotator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/how_to/point_manipulator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/how_to/render_plane_manipulator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/how_to/sphere_annotator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/how_to/spline_annotator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.022209 napari-threedee-0.0.4/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.022209 napari-threedee-0.0.4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/docs/tutorials/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-14 19:26:21.034209 napari-threedee-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.014209 napari-threedee-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.022209 napari-threedee-0.0.4/src/napari_threedee/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.022209 napari-threedee-0.0.4/src/napari_threedee/_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.022209 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_axis_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_central_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_drag_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_rotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/axis_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/central_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/drag_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/manipulator_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/napari_manipulator_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/rotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/vispy_manipulator_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/vispy_visual_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/threedee_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_backend/threedee_widget_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/_tests/test_mouse_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 19:26:20.000000 napari-threedee-0.0.4/src/napari_threedee/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/qt_path_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/qt_plane_point_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/qt_point_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/qt_sphere_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/qt_surface_annotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/test_point_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/test_sphere_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/test_spline_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/annotators/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/paths/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/paths/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/paths/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/annotators/points/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/points/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/annotators/points/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/points/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/points/_tests/test_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/points/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/points/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/points/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.026209 napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/_tests/test_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/_tests/test_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/data_models/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/data_models/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/data_models/_tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/data_models/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/data_models/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/data_models/spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/data_models/spline_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/data_models/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/dock_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/manipulators/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/manipulators/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/_qt/qt_layer_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/_qt/qt_point_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/_qt/qt_render_plane_manipulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/manipulators/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/_tests/test_manipulator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/base_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/layer_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/manipulator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/point_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/manipulators/render_plane_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/utils/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/utils/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/utils/_tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/utils/mouse_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/utils/napari_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/utils/selection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/vispy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.030209 napari-threedee-0.0.4/src/napari_threedee/visualization/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/_qt/qt_camera_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/_qt/qt_lighting_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.034209 napari-threedee-0.0.4/src/napari_threedee/visualization/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/_tests/test_camera_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/_tests/test_lighting_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/camera_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/src/napari_threedee/visualization/lighting_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:26:21.022209 napari-threedee-0.0.4/src/napari_threedee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-14 19:26:20.000000 napari-threedee-0.0.4/src/napari_threedee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-14 19:26:20.000000 napari-threedee-0.0.4/src/napari_threedee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:26:20.000000 napari-threedee-0.0.4/src/napari_threedee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 19:26:20.000000 napari-threedee-0.0.4/src/napari_threedee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 19:26:20.000000 napari-threedee-0.0.4/src/napari_threedee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 19:26:20.000000 napari-threedee-0.0.4/src/napari_threedee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 19:26:12.000000 napari-threedee-0.0.4/tox.ini
```

### Comparing `napari-threedee-0.0.3/.github/workflows/test_and_deploy.yml` & `napari-threedee-0.0.4/.github/workflows/test_and_deploy.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # This workflows will upload a Python Package using Twine when a release is created
 # For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
 
-name: tests
+name: test_and_deploy
 
-on: 
+on:
   push:
     branches:
       - main
-      - main
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
     branches:
       - main
-      - main
   workflow_dispatch:
 
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
@@ -59,14 +57,43 @@
           run: python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
         uses: codecov/codecov-action@v2
 
+  docs:
+    needs: [test]  # runs only after the other CI tests pass
+    runs-on: ubuntu-latest
+    steps:
+    - uses: actions/checkout@v2
+    - uses: tlambert03/setup-qt-libs@v1
+    # Install dependencies
+    - name: Set up Python 3.8
+      uses: actions/setup-python@v2
+      with:
+        python-version: 3.8
+    - name: Install dependencies
+      run: |
+        pip install -r requirements.txt
+        pip list
+    # Build the book
+    - name: Build the book
+      uses: aganders3/headless-gui@v1
+      with:
+        run: mkdocs build --strict
+    # Push the book's HTML to github-pages whenever the main repo branch changes
+    - name: GitHub Pages action
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      uses: peaceiris/actions-gh-pages@v3.8.0
+      with:
+        deploy_key: ${{ secrets.DOCS_DEPLOY_TOKEN }}
+        external_repository: napari-threedee/napari-threedee.github.io
+        publish_dir: ./site
+
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your 
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
```

### Comparing `napari-threedee-0.0.3/.gitignore` & `napari-threedee-0.0.4/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 instance/
 
 # Sphinx documentation
 docs/_build/
 
 # MkDocs documentation
 /site/
+/docs/generated/
 
 # PyBuilder
 target/
 
 # Pycharm and VSCode
 .idea/
 venv/
```

### Comparing `napari-threedee-0.0.3/LICENSE` & `napari-threedee-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/PKG-INFO` & `napari-threedee-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-threedee
-Version: 0.0.3
+Version: 0.0.4
 Summary: A suite of useful tools based on 3D interactivity in napari
 Home-page: https://github.com/alisterburt/napari-threedee
 Author: napari team
 Author-email: napari-steering-council@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/napari-threedee/napari-threedee/issues
 Project-URL: Documentation, https://github.com/napari-threedee/napari-threedee#README.md
@@ -57,14 +57,17 @@
 
 
 To install latest development version :
 
     pip install git+https://github.com/alisterburt/napari-threedee.git
 
 ## Example applications
+
+See the full list of [example gallery scripts here on our website](https://napari-threedee.github.io/generated/gallery/).
+
 <table border="0">
 <tr><td>
 
 
 <img src="https://user-images.githubusercontent.com/1120672/173021751-9206de7d-5675-4aac-aa9e-8585457a7799.gif"
 width="300"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-threedee Version: 0.0.3 Summary: A suite of
+Metadata-Version: 2.1 Name: napari-threedee Version: 0.0.4 Summary: A suite of
 useful tools based on 3D interactivity in napari Home-page: https://github.com/
 alisterburt/napari-threedee Author: napari team Author-email: napari-steering-
 council@googlegroups.com License: BSD-3-Clause Project-URL: Bug Tracker, https:
 //github.com/napari-threedee/napari-threedee/issues Project-URL: Documentation,
 https://github.com/napari-threedee/napari-threedee#README.md Project-URL:
 Source Code, https://github.com/napari-threedee/napari-threedee Project-URL:
 User Support, https://github.com/napari-threedee/napari-threedee/issues
@@ -26,15 +26,17 @@
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-
 threedee)](https://napari-hub.org/plugins/napari-threedee) A suite of useful
 tools based on 3D interactivity in napari ---------------------------------
 - This [napari] plugin was generated with [Cookiecutter] using [@napari]'s
 [cookiecutter-napari-plugin] template.  ## Installation You can install
 `napari-threedee` via [pip]: pip install napari-threedee To install latest
 development version : pip install git+https://github.com/alisterburt/napari-
-threedee.git ## Example applications
+threedee.git ## Example applications See the full list of [example gallery
+scripts here on our website](https://napari-threedee.github.io/generated/
+gallery/).
 [https://user-                        [mesh lighting control](https://
 images.githubusercontent.com/1120672/ github.com/napari-threedee/napari-
 173021751-9206de7d-5675-4aac-aa9e-    threedee/blob/main/examples/plugin/
 8585457a7799.gif]                     mesh_headlight.py)
 [https://user-                        [annotate points on planes](https://
 images.githubusercontent.com/1120672/ github.com/napari-threedee/napari-
 173022286-2473b6b2-a20e-4514-88a4-    threedee/blob/main/examples/plugin/
```

### Comparing `napari-threedee-0.0.3/README.md` & `napari-threedee-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
 
 To install latest development version :
 
     pip install git+https://github.com/alisterburt/napari-threedee.git
 
 ## Example applications
+
+See the full list of [example gallery scripts here on our website](https://napari-threedee.github.io/generated/gallery/).
+
 <table border="0">
 <tr><td>
 
 
 <img src="https://user-images.githubusercontent.com/1120672/173021751-9206de7d-5675-4aac-aa9e-8585457a7799.gif"
 width="300"/>
```

#### html2text {}

```diff
@@ -11,15 +11,17 @@
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-
 threedee)](https://napari-hub.org/plugins/napari-threedee) A suite of useful
 tools based on 3D interactivity in napari ---------------------------------
 - This [napari] plugin was generated with [Cookiecutter] using [@napari]'s
 [cookiecutter-napari-plugin] template.  ## Installation You can install
 `napari-threedee` via [pip]: pip install napari-threedee To install latest
 development version : pip install git+https://github.com/alisterburt/napari-
-threedee.git ## Example applications
+threedee.git ## Example applications See the full list of [example gallery
+scripts here on our website](https://napari-threedee.github.io/generated/
+gallery/).
 [https://user-                        [mesh lighting control](https://
 images.githubusercontent.com/1120672/ github.com/napari-threedee/napari-
 173021751-9206de7d-5675-4aac-aa9e-    threedee/blob/main/examples/plugin/
 8585457a7799.gif]                     mesh_headlight.py)
 [https://user-                        [annotate points on planes](https://
 images.githubusercontent.com/1120672/ github.com/napari-threedee/napari-
 173022286-2473b6b2-a20e-4514-88a4-    threedee/blob/main/examples/plugin/
```

### Comparing `napari-threedee-0.0.3/docs/annotations/io.md` & `napari-threedee-0.0.4/docs/annotations/io.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/annotations/point_spec.md` & `napari-threedee-0.0.4/docs/annotations/point_spec.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/annotations/sphere_spec.md` & `napari-threedee-0.0.4/docs/annotations/sphere_spec.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/annotations/spline_spec.md` & `napari-threedee-0.0.4/docs/annotations/spline_spec.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/dev_guides/core_concepts.md` & `napari-threedee-0.0.4/docs/dev_guides/core_concepts.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/dev_guides/manipulators.md` & `napari-threedee-0.0.4/docs/dev_guides/manipulators.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/how_to/layer_manipulator.md` & `napari-threedee-0.0.4/docs/how_to/layer_manipulator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/how_to/point_manipulator.md` & `napari-threedee-0.0.4/docs/how_to/point_manipulator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/how_to/render_plane_manipulator.md` & `napari-threedee-0.0.4/docs/how_to/render_plane_manipulator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/index.md` & `napari-threedee-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/docs/stylesheets/extra.css` & `napari-threedee-0.0.4/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/examples/library/camera_spline.py` & `napari-threedee-0.0.4/docs/examples/library/camera_spline_library.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Camera spline (library)
+===============================
+
+An example controlling the camera spline,
+using napari-threedee as a library.
+"""
 import napari
 import skimage
 
 from napari_threedee.visualization._qt.qt_camera_spline import QtCameraSpline
 
 viewer = napari.Viewer(ndisplay=3)
 blobs = skimage.data.binary_blobs(
```

### Comparing `napari-threedee-0.0.3/examples/library/point_annotator.py` & `napari-threedee-0.0.4/docs/examples/plugin/path_annotator_plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,58 @@
-from napari_threedee.annotators import PointAnnotator
-
+"""
+Path point annotator (plugin)
+==============================
+
+An example controlling the path annotator,
+using napari-threedee as a napari plugin.
+"""
 import napari
 from skimage import data
 
+# create napari viewer
 viewer = napari.Viewer(ndisplay=3)
-blobs = data.binary_blobs(length=64, volume_fraction=0.1, n_dim=3).astype(float)
 
-# add a volume and render as plane
-plane_parameters = {
-    'position': (32, 32, 32),
-    'normal': (1, 0, 0),
-    'thickness': 10,
-}
+# generate image data
+blobs = data.binary_blobs(length=64, volume_fraction=0.1, n_dim=4).astype(float)
 
-plane_layer = viewer.add_image(
+# add two image layers to viewer
+viewer.add_image(
     blobs,
+    name='orange plane',
     rendering='average',
-    name='plane',
     colormap='bop orange',
     blending='translucent',
     opacity=0.5,
     depiction='plane',
-    plane=plane_parameters,
+    plane={
+        'position': (32, 32, 32),
+        'normal': (1, 0, 0),
+        'thickness': 10,
+    }
 )
 
-points_layer = viewer.add_points(
-    data=[],
-    size=5,
-    face_color='cornflowerblue',
-    ndim=3
+viewer.add_image(
+    blobs,
+    name='blue plane',
+    rendering='average',
+    colormap='bop blue',
+    blending='additive',
+    opacity=0.5,
+    depiction='plane',
+    plane={
+        'position': (32, 32, 32),
+        'normal': (0, 1, 0),
+        'thickness': 10,
+    }
 )
 
-annotator = PointAnnotator(
-    viewer=viewer,
-    image_layer=plane_layer,
-    points_layer=points_layer,
-    enabled=True,
+# add plugin dock widget to viewer
+viewer.window.add_plugin_dock_widget(
+    plugin_name="napari-threedee", widget_name="path annotator"
 )
-viewer.layers.selection = [plane_layer]
-viewer.camera.set_view_direction([-1, -1, 1])
-napari.run()
+
+# run napari
+viewer.layers.selection = [viewer.layers[0]]
+viewer.axes.visible = True
+viewer.camera.angles = (-15, 25, -30)
+viewer.camera.zoom *= 0.5
+napari.run()
```

### Comparing `napari-threedee-0.0.3/examples/library/spline_annotator.py` & `napari-threedee-0.0.4/docs/examples/plugin/spline_annotator_plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,56 @@
+"""
+Spline annotator (plugin)
+=================================
+
+An example controlling the spline annotator,
+using napari-threedee as a napari plugin.
+"""
 import napari
-import skimage
-
-from napari_threedee.annotators._qt import QtSplineAnnotatorWidget
-
+from skimage import data
 
+# create napari viewer
 viewer = napari.Viewer(ndisplay=3)
-blobs = skimage.data.binary_blobs(
-    length=64,
-    volume_fraction=0.1,
-    n_dim=4
-).astype(float)
 
-plane_parameters_z = {
-    'position': (32, 32, 32),
-    'normal': (1, 0, 0),
-    'thickness': 10,
-}
-
-plane_parameters_y = {
-    'position': (32, 32, 32),
-    'normal': (0, 1, 0),
-    'thickness': 10,
-}
+# generate image data
+blobs = data.binary_blobs(length=64, volume_fraction=0.1, n_dim=3).astype(float)
 
+# add two image layers to viewer
 viewer.add_image(
     blobs,
     name='orange plane',
     rendering='average',
     colormap='bop orange',
     blending='translucent',
     opacity=0.5,
     depiction='plane',
-    plane=plane_parameters_z)
+    plane={
+    'position': (32, 32, 32),
+    'normal': (1, 0, 0),
+    'thickness': 10,
+})
 
 viewer.add_image(
     blobs,
     name='blue plane',
     rendering='average',
     colormap='bop blue',
     blending='additive',
     opacity=0.5,
     depiction='plane',
-    plane=plane_parameters_y)
-
-spline_annotator = QtSplineAnnotatorWidget(viewer=viewer)
-viewer.window.add_dock_widget(spline_annotator)
-
+    plane={
+    'position': (32, 32, 32),
+    'normal': (0, 1, 0),
+    'thickness': 10,
+})
 
-viewer.camera.angles = (60, 60, 60)
-napari.run()
+# add plugin dock widget to viewer
+viewer.window.add_plugin_dock_widget(
+    plugin_name="napari-threedee", widget_name="sphere annotator"
+)
+
+# run napari
+viewer.layers.selection = [viewer.layers[0]]
+viewer.axes.visible = True
+viewer.camera.angles = (-15, 25, -30)
+viewer.camera.zoom *= 0.5
+napari.run()
```

### Comparing `napari-threedee-0.0.3/examples/library/surface_annotator.py` & `napari-threedee-0.0.4/docs/examples/plugin/point_annotator_plugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,56 @@
+"""
+Plane point annotator (plugin)
+==============================
+
+An example controlling the point annotator,
+using napari-threedee as a napari plugin.
+"""
 import napari
-import skimage
-
-from napari_threedee.annotators._qt import QtSurfaceAnnotatorWidget
-
+from skimage import data
 
+# create napari viewer
 viewer = napari.Viewer(ndisplay=3)
-blobs = skimage.data.binary_blobs(
-    length=64,
-    volume_fraction=0.1,
-    n_dim=3
-).astype(float)
 
-plane_parameters_z = {
-    'position': (32, 32, 32),
-    'normal': (1, 0, 0),
-    'thickness': 10,
-}
-
-plane_parameters_y = {
-    'position': (32, 32, 32),
-    'normal': (0, 1, 0),
-    'thickness': 10,
-}
+# generate image data
+blobs = data.binary_blobs(length=64, volume_fraction=0.1, n_dim=4).astype(float)
 
+# add two image layers to viewer
 viewer.add_image(
     blobs,
     name='orange plane',
     rendering='average',
     colormap='bop orange',
     blending='translucent',
     opacity=0.5,
     depiction='plane',
-    plane=plane_parameters_z)
+    plane={
+    'position': (32, 32, 32),
+    'normal': (1, 0, 0),
+    'thickness': 10,
+})
 
 viewer.add_image(
     blobs,
     name='blue plane',
     rendering='average',
     colormap='bop blue',
     blending='additive',
     opacity=0.5,
     depiction='plane',
-    plane=plane_parameters_y)
-
-spline_annotator = QtSurfaceAnnotatorWidget(viewer=viewer)
-viewer.window.add_dock_widget(spline_annotator)
-
+    plane={
+    'position': (32, 32, 32),
+    'normal': (0, 1, 0),
+    'thickness': 10,
+})
 
-viewer.camera.angles = (60, 60, 60)
-napari.run()
+# add plugin dock widget to viewer
+viewer.window.add_plugin_dock_widget(
+    plugin_name="napari-threedee", widget_name="point annotator"
+)
+
+# run napari
+viewer.layers.selection = [viewer.layers[0]]
+viewer.axes.visible = True
+viewer.camera.angles = (-15, 25, -30)
+viewer.camera.zoom *= 0.5
+napari.run()
```

### Comparing `napari-threedee-0.0.3/examples/plugin/camera_spline.py` & `napari-threedee-0.0.4/docs/examples/library/render_plane_manipulator_library.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,40 @@
-import napari
-import skimage
+"""
+Render plane manipulator (library)
+==========================================
+
+An example controlling the render plane manipulator,
+using napari-threedee as a library.
+"""
+from napari_threedee.manipulators._qt import QtRenderPlaneManipulatorWidget
 
+import napari
+from skimage import data
 
 viewer = napari.Viewer(ndisplay=3)
-blobs = skimage.data.binary_blobs(
-    length=64,
-    volume_fraction=0.1,
-    n_dim=4
+blobs = data.binary_blobs(
+    length=64, volume_fraction=0.1, n_dim=3
 ).astype(float)
 
-plane_parameters_z = {
+plane_parameters = {
     'position': (32, 32, 32),
     'normal': (1, 0, 0),
     'thickness': 10,
 }
 
-plane_parameters_y = {
-    'position': (32, 32, 32),
-    'normal': (0, 1, 0),
-    'thickness': 10,
-}
-
-viewer.add_image(
+plane_layer = viewer.add_image(
     blobs,
-    name='orange plane',
     rendering='average',
+    name='plane',
     colormap='bop orange',
     blending='additive',
     opacity=0.5,
     depiction='plane',
-    plane=plane_parameters_z)
-
-viewer.add_image(
-    blobs,
-    name='blue plane',
-    rendering='average',
-    colormap='bop blue',
-    blending='additive',
-    opacity=0.5,
-    depiction='plane',
-    plane=plane_parameters_y)
-
-
-viewer.window.add_plugin_dock_widget(
-    plugin_name="napari-threedee", widget_name="camera spline control"
+    plane=plane_parameters
+)
+volume_layer = viewer.add_image(
+    blobs, rendering='mip', name='volume', blending='additive', opacity=0.25
 )
 
-viewer.camera.angles = (60, 60, 60)
-napari.run()
+widget = QtRenderPlaneManipulatorWidget(viewer)
+viewer.window.add_dock_widget(widget)
+napari.run()
```

### Comparing `napari-threedee-0.0.3/examples/plugin/layer_manipulator.py` & `napari-threedee-0.0.4/docs/examples/plugin/layer_manipulator_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Layer manipulator (plugin)
+==================================
+
+An example controlling the layer manipulator,
+using napari-threedee as a napari plugin.
+"""
 import napari
 
 try:
     from skimage.data import binary_blobs
 except ImportError:
     raise ImportError("This example requires scikit-image. pip install scikit-image")
```

### Comparing `napari-threedee-0.0.3/examples/plugin/plane_point_annotator.py` & `napari-threedee-0.0.4/docs/examples/plugin/camera_spline_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Camera spline (plugin)
+==============================
+
+An example controlling the camera spline,
+using napari-threedee as a napari plugin.
+"""
 import napari
 import skimage
 
 
 viewer = napari.Viewer(ndisplay=3)
 blobs = skimage.data.binary_blobs(
     length=64,
@@ -37,15 +44,14 @@
     rendering='average',
     colormap='bop blue',
     blending='additive',
     opacity=0.5,
     depiction='plane',
     plane=plane_parameters_y)
 
-viewer.add_points([], ndim=4, face_color='cornflowerblue')
 
 viewer.window.add_plugin_dock_widget(
-    plugin_name="napari-threedee", widget_name="plane point annotator"
+    plugin_name="napari-threedee", widget_name="camera spline control"
 )
 
 viewer.camera.angles = (60, 60, 60)
-napari.run()
+napari.run()
```

### Comparing `napari-threedee-0.0.3/examples/plugin/spline_annotator.py` & `napari-threedee-0.0.4/docs/examples/plugin/sphere_annotator_plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,56 @@
+"""
+Sphere annotator (plugin)
+=================================
+
+An example controlling the sphere annotator,
+using napari-threedee as a napari plugin.
+"""
 import napari
-import skimage
-
+from skimage import data
 
+# create napari viewer
 viewer = napari.Viewer(ndisplay=3)
-blobs = skimage.data.binary_blobs(
-    length=64,
-    volume_fraction=0.1,
-    n_dim=4
-).astype(float)
-
-plane_parameters_z = {
-    'position': (32, 32, 32),
-    'normal': (1, 0, 0),
-    'thickness': 10,
-}
 
-plane_parameters_y = {
-    'position': (32, 32, 32),
-    'normal': (0, 1, 0),
-    'thickness': 10,
-}
+# generate image data
+blobs = data.binary_blobs(length=64, volume_fraction=0.1, n_dim=3).astype(float)
 
+# add two image layers to viewer
 viewer.add_image(
     blobs,
     name='orange plane',
     rendering='average',
     colormap='bop orange',
-    blending='additive',
+    blending='translucent',
     opacity=0.5,
     depiction='plane',
-    plane=plane_parameters_z)
+    plane={
+    'position': (32, 32, 32),
+    'normal': (1, 0, 0),
+    'thickness': 10,
+})
 
 viewer.add_image(
     blobs,
     name='blue plane',
     rendering='average',
     colormap='bop blue',
     blending='additive',
     opacity=0.5,
     depiction='plane',
-    plane=plane_parameters_y)
-
+    plane={
+    'position': (32, 32, 32),
+    'normal': (0, 1, 0),
+    'thickness': 10,
+})
 
+# add plugin dock widget to viewer
 viewer.window.add_plugin_dock_widget(
-    plugin_name="napari-threedee", widget_name="spline annotator"
+    plugin_name="napari-threedee", widget_name="sphere annotator"
 )
 
-viewer.camera.angles = (60, 60, 60)
-napari.run()
+# run napari
+viewer.layers.selection = [viewer.layers[0]]
+viewer.axes.visible = True
+viewer.camera.angles = (-15, 25, -30)
+viewer.camera.zoom *= 0.5
+napari.run()
```

### Comparing `napari-threedee-0.0.3/setup.cfg` & `napari-threedee-0.0.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -46,20 +46,23 @@
 
 [options.entry_points]
 napari.manifest = 
 	napari-threedee = napari_threedee:napari.yaml
 
 [options.extras_require]
 dev = 
-	mkdocs
+	mkdocs==1.2.4 # Pinned due to issue https://github.com/smarie/mkdocs-gallery/issues/57
+	mkdocs-gallery
 	mkdocs-material
 	mkdocstrings[python]
 	mkdocs-video
+	napari[all]
 	pytest
 	pytest-qt
+	qtgallery
 
 [options.package_data]
 napari_threedee = napari.yaml
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_axis_model.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_axis_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_drag_manager.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_drag_manager.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_manipulator.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/axis_model.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/axis_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/central_axis.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/central_axis.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/drag_managers.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/drag_managers.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/manipulator_model.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/manipulator_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/napari_manipulator_backend.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/napari_manipulator_backend.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/rotator.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/rotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/translator.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/translator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/utils.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/vispy_manipulator_visual.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/vispy_manipulator_visual.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/manipulator/vispy_visual_data.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/manipulator/vispy_visual_data.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/threedee_model.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/threedee_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 
 
-class ThreeDeeModel(ABC):
+class N3dComponent(ABC):
     """Base class for manipulators and annotators.
 
     By adhering to the interface defined by this class, widgets can be automatically generated for
     manipulators and annotators.
 
     To implement:
         - the __init__() should take the viewer as the first argument and all
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_backend/threedee_widget_base.py` & `napari-threedee-0.0.4/src/napari_threedee/_backend/threedee_widget_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Type
 
 import napari
 from PyQt5.QtWidgets import QWidget, QPushButton, QVBoxLayout
 from napari.utils.events import Event
 
-from napari_threedee._backend.threedee_model import ThreeDeeModel
+from napari_threedee._backend.threedee_model import N3dComponent
 from ..utils.napari_utils import generate_populated_layer_selection_widget
 
 
 class QtThreeDeeWidgetBase(QWidget):
     """Base class for GUI elements in napari-threedee."""
 
-    def __init__(self, model_class: Type[ThreeDeeModel], viewer: napari.Viewer, flags=None, *args,
+    def __init__(self, model_class: Type[N3dComponent], viewer: napari.Viewer, flags=None, *args,
                  **kwargs):
         super().__init__(flags, *args, **kwargs)
-        self.model: ThreeDeeModel = model_class(viewer)
+        self.model: N3dComponent = model_class(viewer)
         self.viewer = viewer
 
         self._layer_selection_widget = generate_populated_layer_selection_widget(
             func=self.model.set_layers, viewer=viewer
         )
         self._layer_selection_widget()
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_tests/test_dock_widget.py` & `napari-threedee-0.0.4/src/napari_threedee/_tests/test_dock_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 MY_PLUGIN_NAME = "napari-threedee"
 MY_WIDGET_NAMES = [
     "render plane manipulator",
     "point manipulator",
     "layer manipulator",
     "point annotator",
-    "spline annotator",
+    "path annotator",
     "mesh lighting controls",
     "camera spline control"
 ]
 
 
 @pytest.mark.parametrize("widget_name", MY_WIDGET_NAMES)
 def test_something_with_viewer(
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/_tests/test_mouse_callbacks.py` & `napari-threedee-0.0.4/src/napari_threedee/_tests/test_mouse_callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from napari_threedee.mouse_callbacks import add_point_on_plane
+from napari_threedee.utils.mouse_callbacks import add_point_on_plane
 
 
 def test_add_point_on_plane_3d(viewer_with_plane_and_points_3d):
     viewer = viewer_with_plane_and_points_3d
     points_layer = viewer.layers['Points']
     plane_layer = viewer.layers['blobs_3d']
 
@@ -13,15 +13,15 @@
         view_direction = np.array((1, 0, 0))
         modifiers = ['Alt']
 
     add_point_on_plane(
         viewer=viewer_with_plane_and_points_3d,
         event=DummyMouseEvent,
         points_layer=points_layer,
-        plane_layer=plane_layer,
+        image_layer=plane_layer,
     )
     assert len(points_layer.data) == 1
     np.testing.assert_array_almost_equal(points_layer.data[0], (14, 14, 14))
 
 
 def test_add_point_on_plane_4d(viewer_with_plane_and_points_4d):
     viewer = viewer_with_plane_and_points_4d
@@ -33,11 +33,11 @@
         view_direction = np.array((0, 1, 0, 0))
         modifiers = ['Alt']
 
     add_point_on_plane(
         viewer=viewer_with_plane_and_points_4d,
         event=DummyMouseEvent,
         points_layer=points_layer,
-        plane_layer=plane_layer,
+        image_layer=plane_layer,
     )
     assert len(points_layer.data) == 1
     np.testing.assert_array_almost_equal(points_layer.data[0], (14, 14, 14, 14))
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/qt_spline_annotator.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/qt_path_annotator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import napari
 from napari.utils.events import Event
 from qtpy.QtWidgets import QPushButton, QGroupBox, QVBoxLayout, QCheckBox, QSpinBox, QLabel, QHBoxLayout
 
 from napari_threedee._backend.threedee_widget_base import QtThreeDeeWidgetBase
 
-from napari_threedee.annotators.spline_annotator import SplineAnnotator
+from napari_threedee.annotators.paths import PathAnnotator
 
 
-class QtSplineAnnotatorWidget(QtThreeDeeWidgetBase):
+class QtPathAnnotatorWidget(QtThreeDeeWidgetBase):
     def __init__(self, viewer: napari.Viewer):
-        super().__init__(model_class=SplineAnnotator, viewer=viewer)
+        super().__init__(model_class=PathAnnotator, viewer=viewer)
 
         self.auto_fit_checkbox = QCheckBox("automatically fit spline")
         self.auto_fit_checkbox.clicked.connect(self._on_auto_fit)
         self.auto_fit_checkbox.setChecked(self.model.auto_fit_spline)
         self.fit_spline_button = QPushButton("fit spline")
         self.fit_spline_button.pressed.connect(self._on_spline_fit)
 
@@ -40,18 +40,18 @@
         # add the widget to the layout
         self.layout().addWidget(self.fitting_group_box)
 
         # connect events to sync changes in the model to the UI
         self.model.events.active_spline_id.connect(self._update_active_spline_id)
 
     def _on_spline_fit(self):
-        # update splines from points
+        # update data from points
         self.model._update_spheres()
 
-        # draw splines
+        # draw data
         self.model._draw_splines()
 
     def _on_auto_fit(self):
         """Callback function when the autofit """
         self.model.auto_fit_spline = self.auto_fit_checkbox.isChecked()
 
     def _on_current_filament_id_changed(self, event: Event):
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/_qt/qt_surface_annotator.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/_qt/qt_surface_annotator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,85 @@
 import napari
 from napari.utils.events import Event
 from qtpy.QtWidgets import QPushButton, QGroupBox, QVBoxLayout, QSpinBox, QLabel, QHBoxLayout
 
 from napari_threedee._backend.threedee_widget_base import QtThreeDeeWidgetBase
 
-from napari_threedee.annotators.surface_annotator import SurfaceAnnotator
+from napari_threedee.annotators.surfaces.annotator import SurfaceAnnotator
 
 
 
 class QtSurfaceAnnotatorWidget(QtThreeDeeWidgetBase):
     def __init__(self, viewer: napari.Viewer):
         super().__init__(model_class=SurfaceAnnotator, viewer=viewer)
 
-        self.update_surface_button = QPushButton("fit surface")
-        self.update_surface_button.pressed.connect(self._draw_surface)
-
-        spinbox_layout = QHBoxLayout()
-        self.active_level_index_spinbox = QSpinBox()
-        self.active_level_index_spinbox.setMinimum(0)
-        self.active_level_index_spinbox.setValue(self.model.active_spline_id)
-        self.active_level_index_spinbox.valueChanged.connect(self._on_current_filament_id_changed)
-        spinbox_layout.addWidget(QLabel("active surface level:"))
-        spinbox_layout.addWidget(self.active_level_index_spinbox)
+        surface_layout = QHBoxLayout()
+        self.active_surface_spinbox = QSpinBox()
+        self.active_surface_spinbox.setMinimum(0)
+        self.active_surface_spinbox.setValue(self.model.active_surface_id)
+        self.active_surface_spinbox.valueChanged.connect(
+            self._on_current_surface_changed
+        )
+
+        surface_layout.addWidget(QLabel("surface:"))
+        surface_layout.addWidget(self.active_surface_spinbox)
+
+        level_layout = QHBoxLayout()
+        self.active_level_spinbox = QSpinBox()
+        self.active_level_spinbox.setMinimum(0)
+        self.active_level_spinbox.setValue(self.model.active_level_id)
+        self.active_level_spinbox.valueChanged.connect(
+            self._on_current_level_changed
+        )
 
+        level_layout.addWidget(QLabel("level:"))
+        level_layout.addWidget(self.active_level_spinbox)
 
         # add the fitting UI to the group_box
+        self.update_surface_button = QPushButton("fit surface")
+        self.update_surface_button.pressed.connect(self._draw_surface)
+
         self.fitting_group_box = QGroupBox("fit surface")
         group_box_layout = QVBoxLayout()
-        group_box_layout.addLayout(spinbox_layout)
+        group_box_layout.addLayout(surface_layout)
+        group_box_layout.addLayout(level_layout)
         group_box_layout.addWidget(self.update_surface_button)
         self.fitting_group_box.setLayout(group_box_layout)
         self.fitting_group_box.setVisible(False)
 
         # add the widget to the layout
         self.layout().addWidget(self.fitting_group_box)
 
         # connect events to sync changes in the model to the UI
-        self.model.events.active_spline_id.connect(self._update_active_level_id)
+        self.model.events.active_surface_id.connect(self._update_active_surface)
+        self.model.events.active_level_id.connect(self._update_active_level)
 
     def _draw_surface(self):
-        self.model._update_splines()
         self.model._draw_splines()
         self.model._draw_surface()
 
-    def _on_current_filament_id_changed(self, event: Event):
-        self.model.active_spline_id = self.active_level_index_spinbox.value()
+    def _on_current_surface_changed(self, event: Event):
+        self.model.active_surface_id = self.active_surface_spinbox.value()
+
+    def _on_current_level_changed(self, event: Event):
+        self.model.active_spline_id = self.active_level_spinbox.value()
 
     def on_activate_button_click(self, event: Event):
         """Callback function when the activate button is clicked"""
         if self.activate_button.isChecked() is True:
             self.model.enabled = True
             self.activate_button.setText('deactivate')
             self.fitting_group_box.setVisible(True)
         else:
             self.model.enabled = False
             self.activate_button.setText('activate')
             self.fitting_group_box.setVisible(False)
 
-    def _update_active_level_id(self):
-        """Update the spline id spinbox when the model has changed value"""
-        self.active_level_index_spinbox.setValue(self.model.active_spline_id)
+    def _update_active_surface(self):
+        """Update surface spinbox when surface id has changed on the model."""
+        self.active_surface_spinbox.setValue(self.model.active_surface_id)
+
+    def _update_active_level(self):
+        """Update the spline id spinbox when the model has changed value."""
+        self.active_level_spinbox.setValue(self.model.active_level_id)
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/conftest.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from napari_threedee.annotators import PointAnnotator, SplineAnnotator, \
+from napari_threedee.annotators import PointAnnotator, PathAnnotator, \
     SphereAnnotator
 
 
 @pytest.fixture
 def point_annotator(make_napari_viewer, points_layer_4d, blobs_layer_4d_plane):
     viewer = make_napari_viewer(ndisplay=3)
     points_layer = viewer.add_layer(points_layer_4d)
@@ -15,15 +15,15 @@
     return annotator
 
 
 @pytest.fixture
 def spline_annotator(make_napari_viewer, blobs_layer_4d_plane):
     viewer = make_napari_viewer(ndisplay=3)
     plane_layer = viewer.add_layer(blobs_layer_4d_plane)
-    annotator = SplineAnnotator(viewer=viewer, image_layer=plane_layer)
+    annotator = PathAnnotator(viewer=viewer, image_layer=plane_layer)
     return annotator
 
 
 @pytest.fixture
 def sphere_annotator(viewer_with_plane_3d):
     viewer = viewer_with_plane_3d
     plane_layer = viewer.layers['blobs_3d']
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/test_plane_point_annotator.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/test_point_annotator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from napari.layers import Points
 
-from napari_threedee.annotators.point_annotator import PointAnnotator
+from napari_threedee.annotators.points import PointAnnotator
 
 
 def test_plane_point_annotator_instantiation(viewer_with_plane_and_points_3d):
     viewer = viewer_with_plane_and_points_3d
     plane_layer = viewer.layers['blobs_3d']
     points_layer = viewer.layers['Points']
     annotator = PointAnnotator(
@@ -20,8 +20,8 @@
     plane_layer = viewer.layers['blobs_3d']
     annotator = PointAnnotator(
         viewer=viewer,
         image_layer=plane_layer,
         points_layer=None
     )
     assert isinstance(annotator.points_layer, Points)
-    assert annotator.points_layer.ndim == 3
+    assert annotator.points_layer.ndim == 3   # matches ndim of image layer
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/test_sphere_annotator.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/test_sphere_annotator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from napari_threedee.annotators import SphereAnnotator
-from napari_threedee.annotators.sphere_annotator import SphereAnnotatorMode
+from napari_threedee.annotators.spheres import SphereAnnotatorMode, \
+    SPHERE_ID_FEATURES_KEY, SPHERE_RADIUS_FEATURES_KEY
 
 
 def test_sphere_annotator_instantiation(viewer_with_plane_and_points_3d):
     viewer = viewer_with_plane_and_points_3d
     plane_layer = viewer.layers['blobs_3d']
     annotator = SphereAnnotator(
         viewer=viewer,
@@ -15,34 +16,32 @@
 def test_sphere_annotator_layer_creation(sphere_annotator):
     assert sphere_annotator.points_layer is not None
     assert sphere_annotator.surface_layer is not None
 
 
 def test_sphere_annotator_update_current_properties(sphere_annotator):
     sphere_annotator._update_current_properties(sphere_id=1, radius=None)
-    assert sphere_annotator.points_layer.current_properties[SphereAnnotator.SPHERE_ID_FEATURES_KEY] == 1
+    assert sphere_annotator.points_layer.current_properties[SPHERE_ID_FEATURES_KEY] == 1
 
     sphere_annotator._update_current_properties(sphere_id=0, radius=1)
-    assert sphere_annotator.points_layer.current_properties[SphereAnnotator.SPHERE_ID_FEATURES_KEY] == 0
-    assert sphere_annotator.points_layer.current_properties[
-               SphereAnnotator.SPHERE_RADIUS_FEATURES_KEY] == 1
+    assert sphere_annotator.points_layer.current_properties[SPHERE_ID_FEATURES_KEY] == 0
+    assert sphere_annotator.points_layer.current_properties[SPHERE_RADIUS_FEATURES_KEY] == 1
 
     # passing none should have no effect
     sphere_annotator._update_current_properties(sphere_id=None, radius=None)
-    assert sphere_annotator.points_layer.current_properties[SphereAnnotator.SPHERE_ID_FEATURES_KEY] == 0
-    assert sphere_annotator.points_layer.current_properties[
-               SphereAnnotator.SPHERE_RADIUS_FEATURES_KEY] == 1
+    assert sphere_annotator.points_layer.current_properties[SPHERE_ID_FEATURES_KEY] == 0
+    assert sphere_annotator.points_layer.current_properties[SPHERE_RADIUS_FEATURES_KEY] == 1
 
 
 def test_sphere_annotator_enable_add_mode_side_effects(sphere_annotator):
     # add some data
     sphere_annotator.points_layer.add([1, 2, 3])
     assert sphere_annotator.points_layer.selected_data == {0}
 
     # change to add mode
     sphere_annotator.mode = SphereAnnotatorMode.ADD
 
     # check no point selected
     assert sphere_annotator.points_layer.selected_data == set()
 
     # check sphere id for next point updated
-    assert sphere_annotator.points_layer.current_properties[sphere_annotator.SPHERE_ID_FEATURES_KEY] == 1
+    assert sphere_annotator.points_layer.current_properties[SPHERE_ID_FEATURES_KEY] == 1
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/_tests/test_spline_annotator.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/_tests/test_spline_annotator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from napari.layers import Points
 
-from napari_threedee.annotators.spline_annotator import SplineAnnotator
+import napari_threedee.annotators.paths.constants
+from napari_threedee.annotators.paths import PathAnnotator
 
 
 def test_spline_annotator_instantiation(make_napari_viewer, blobs_layer_4d_plane):
     viewer = make_napari_viewer(ndisplay=3)
     plane_layer = viewer.add_layer(blobs_layer_4d_plane)
-    annotator = SplineAnnotator(
+    annotator = PathAnnotator(
         viewer=viewer,
         image_layer=plane_layer,
     )
     assert isinstance(annotator.points_layer, Points)
-    assert annotator.SPLINE_ID_FEATURES_KEY in annotator.points_layer.features
+    assert napari_threedee.annotators.paths.constants.PATH_ID_FEATURES_KEY in annotator.points_layer.features
     assert len(annotator.points_layer.data) == 0
 
 
 def test_add_point(spline_annotator):
     points_layer = spline_annotator.points_layer
-    label = spline_annotator.SPLINE_ID_FEATURES_KEY
+    label = napari_threedee.annotators.paths.constants.PATH_ID_FEATURES_KEY
 
     # start empty
     assert len(points_layer.data) == 0
 
     # add points, make sure filament id in feature table matches the annotator
     points_layer.add([1, 2, 3, 4])
     assert len(points_layer.data) == 1
     assert points_layer.features[label][0] == spline_annotator.active_spline_id
 
     # change filemanet_id in annotator, add point, check matches
-    spline_annotator.active_spline_id = 534
+    spline_annotator.active_level_id = 534
     points_layer.add([2, 3, 4, 5])
     assert points_layer.features[label][1] == spline_annotator.active_spline_id
 
 
 def test_get_colors(spline_annotator):
     """Test getting spline colors from the annotator."""
     points_layer = spline_annotator.points_layer
     spline_annotator.active_spline_id = 0
     points_layer.add([1, 2, 3, 4])
     spline_annotator.active_spline_id = 1
     points_layer.add([2, 3, 4, 5])
 
-    spline_colors = spline_annotator._get_spline_colors()
+    spline_colors = spline_annotator._get_path_colors()
     for spline_id in (0, 1):
         assert spline_id in spline_colors
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/io/point.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/paths/validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,28 @@
-import os
-
 import napari
-import numpy as np
 import zarr
-from napari.types import LayerDataTuple
 
-from napari_threedee.annotators import PointAnnotator
-from napari_threedee.annotators.io import ANNOTATION_TYPE_KEY, N3D_METADATA_KEY
+from napari_threedee.annotators.paths.constants import N3D_METADATA_KEY, \
+    ANNOTATION_TYPE_KEY, PATH_ANNOTATION_TYPE_KEY, PATH_ID_FEATURES_KEY
 
 
 def validate_layer(layer: napari.layers.Points):
-    """Ensure a sphere layer matches the specification."""
+    """Ensure a spline layer matches the spline layer specification."""
     if N3D_METADATA_KEY not in layer.metadata:
-        raise ValueError(f"{N3D_METADATA_KEY} not found")
+        raise ValueError(f"{N3D_METADATA_KEY} not in layer metadata.")
     n3d_metadata = layer.metadata[N3D_METADATA_KEY]
-    if n3d_metadata[ANNOTATION_TYPE_KEY] != PointAnnotator.ANNOTATION_TYPE:
-        raise ValueError("Cannot read as n3d points layer.")
+    if n3d_metadata[ANNOTATION_TYPE_KEY] != PATH_ANNOTATION_TYPE_KEY:
+        error = f"Annotation type is not {PATH_ANNOTATION_TYPE_KEY}"
+        raise ValueError(error)
+    elif PATH_ID_FEATURES_KEY not in layer.features:
+        error = f"{PATH_ID_FEATURES_KEY} not in layer features."
+        raise ValueError(error)
 
 
-def validate_zarr(n3d_zarr: zarr.Array):
-    """Ensure an n3d zarr array contains data for n3d points layer."""
+def validate_n3d_zarr(n3d_zarr: zarr.Array):
+    """Ensure an n3d zarr array can be converted to a n3d spline points layer."""
     if ANNOTATION_TYPE_KEY not in n3d_zarr.attrs:
-        raise ValueError("cannot read as n3d sphere.")
-    if n3d_zarr.attrs[ANNOTATION_TYPE_KEY] != PointAnnotator.ANNOTATION_TYPE:
-        raise ValueError("cannot read as n3d sphere.")
-
-
-def layer_to_n3d_zarr(layer: napari.layers.Points, path: os.PathLike) -> zarr.Array:
-    """Convert an n3d sphere points layer into an n3d zarr array."""
-    validate_layer(layer)
-    n3d_zarr = zarr.open_array(
-        store=path,
-        shape=layer.data.shape,
-        dtype=layer.data.dtype,
-        mode="w"
-    )
-    n3d_zarr[...] = layer.data
-    n3d_zarr.attrs[ANNOTATION_TYPE_KEY] = PointAnnotator.ANNOTATION_TYPE
-    return n3d_zarr
-
-
-def n3d_zarr_to_layer_data_tuple(n3d_zarr: zarr.Array) -> LayerDataTuple:
-    """Convert an n3d zarr array into an n3d sphere points layer data tuple."""
-    validate_zarr(n3d_zarr)
-    layer_kwargs = {
-        "metadata": {N3D_METADATA_KEY: {
-            ANNOTATION_TYPE_KEY: PointAnnotator.ANNOTATION_TYPE,
-        }},
-    }
-    return (np.array(n3d_zarr), layer_kwargs, "points")
+        raise ValueError("cannot read as n3d paths.")
+    elif n3d_zarr.attrs[ANNOTATION_TYPE_KEY] != PATH_ANNOTATION_TYPE_KEY:
+        raise ValueError("cannot read as n3d paths.")
+    elif PATH_ID_FEATURES_KEY not in n3d_zarr.attrs:
+        raise ValueError(f"{PATH_ID_FEATURES_KEY} not found.")
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/point_annotator.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/points/annotator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from typing import Optional
 
-import napari
-from napari.layers import Image, Points
+import napari.layers
+import napari.types
+import numpy as np
+
+from napari_threedee._backend.threedee_model import N3dComponent
+from napari_threedee.annotators.points.validation import validate_layer
+from napari_threedee.utils.mouse_callbacks import add_point_on_plane
+from napari_threedee.utils.napari_utils import add_mouse_callback_safe, \
+    remove_mouse_callback_safe
 
-from napari_threedee._backend.threedee_model import ThreeDeeModel
-from ..mouse_callbacks import add_point_on_plane
-from napari_threedee.utils.napari_utils import add_mouse_callback_safe, remove_mouse_callback_safe
-
-
-class PointAnnotator(ThreeDeeModel):
-    ANNOTATION_TYPE: str = "point"
 
+class PointAnnotator(N3dComponent):
     def __init__(
-            self,
-            viewer: napari.Viewer,
-            image_layer: Optional[Image] = None,
-            points_layer: Optional[Points] = None,
-            enabled: bool = False
+        self,
+        viewer: napari.Viewer,
+        image_layer: Optional[napari.layers.Image] = None,
+        points_layer: Optional[napari.layers.Points] = None,
+        enabled: bool = False
     ):
         self.viewer = viewer
         self.image_layer = image_layer
+        if points_layer is None:
+            points_layer = self._create_points_layer()
         self.points_layer = points_layer
-        if points_layer is None and image_layer is not None:
-            self.points_layer = Points(data=[], ndim=image_layer.data.ndim)
-            self.viewer.add_layer(self.points_layer)
         self.enabled = enabled
 
     def _mouse_callback(self, viewer, event):
         if (self.image_layer is None) or (self.points_layer is None):
             return
         add_point_on_plane(
             viewer=viewer,
             event=event,
             points_layer=self.points_layer,
-            plane_layer=self.image_layer
+            image_layer=self.image_layer
         )
 
+    def _create_points_layer(self) -> napari.layers.Points:
+        from napari_threedee.data_models import N3dPoints
+        ndim = self.image_layer.ndim if self.image_layer is not None else 3
+        return N3dPoints(data=np.empty(shape=(0, ndim))).as_layer()
+
     def set_layers(
-            self,
-            image_layer: napari.layers.Image,
-            points_layer: napari.layers.Points
+        self,
+        image_layer: napari.layers.Image,
+        points_layer: napari.layers.Points
     ):
         self.image_layer = image_layer
         self.points_layer = points_layer
 
     def _on_enable(self):
         add_mouse_callback_safe(
             self.viewer.mouse_drag_callbacks, self._mouse_callback
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/sphere_annotator.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/spheres/annotator.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,138 +3,119 @@
 from typing import Optional, Union
 
 import napari
 import numpy as np
 from napari.layers import Image, Points, Surface
 from napari.utils.events import EmitterGroup, Event
 from napari.layers.utils.layer_utils import features_to_pandas_dataframe
-from vispy.geometry import create_sphere
 
-from .._backend import ThreeDeeModel
-from ..mouse_callbacks import add_point_on_plane
-from ..utils.napari_utils import add_mouse_callback_safe, \
+from napari_threedee._backend import N3dComponent
+from napari_threedee.annotators.spheres.constants import SPHERE_ID_FEATURES_KEY, \
+    SPHERE_RADIUS_FEATURES_KEY, SPHERE_MESH_METADATA_KEY
+from napari_threedee.utils.mouse_callbacks import add_point_on_plane
+from napari_threedee.utils.napari_utils import add_mouse_callback_safe, \
     remove_mouse_callback_safe
-from .io import N3D_METADATA_KEY, ANNOTATION_TYPE_KEY
+from napari_threedee.annotators.constants import N3D_METADATA_KEY
 
 
 class SphereAnnotatorMode(Enum):
     ADD = auto()
     EDIT = auto()
 
 
-class SphereAnnotator(ThreeDeeModel):
-    COLOR_CYCLE = [
-        '#1f77b4',
-        '#ff7f0e',
-        '#2ca02c',
-        '#d62728',
-        '#9467bd',
-        '#8c564b',
-        '#e377c2',
-        '#7f7f7f',
-        '#bcbd22',
-        '#17becf',
-    ]
-    ANNOTATION_TYPE: str = "sphere"
-
-    # column names in points layer features
-    SPHERE_ID_FEATURES_KEY: str = "sphere_id"
-    SPHERE_RADIUS_FEATURES_KEY: str = "radius"
-
-    # metadata
-    SPHERE_MESH_METADATA_KEY: str = "mesh_data"
-
-    # parameter defaults
-    DEFAULT_SPHERE_RADIUS = 5
-
+class SphereAnnotator(N3dComponent):
     def __init__(
         self,
         viewer: napari.Viewer,
         image_layer: Optional[Image] = None,
+        points_layer: Optional[Points] = None,
         enabled: bool = False
     ):
         self.events = EmitterGroup(
             source=self,
             current_sphere_id=Event
         )
 
         self.viewer = viewer
         self.image_layer = image_layer
-        self.points_layer = None
+        self.points_layer = points_layer
+        self.surface_layer = None
+        if self.points_layer is not None:
+            self._update_spheres()
         self.enabled = enabled
         self.mode = SphereAnnotatorMode.ADD
 
         if image_layer is not None:
             self.set_layers(self.image_layer)
 
     @property
     def active_sphere_id(self) -> Union[int, None]:
         if self.points_layer is None:
             return None
-        elif self.points_layer.selected_data != {}:
+        elif list(self.points_layer.selected_data) != []:
             return int(list(self.points_layer.selected_data)[0])
         else:
             return None
 
     @property
     def active_sphere_center(self) -> np.ndarray:
         return self.points_layer.data[self._active_sphere_index]
 
     @property
     def active_sphere_radius(self) -> Union[float, None]:
         df = features_to_pandas_dataframe(self.points_layer.features)
         if len(df) == 0:
             return None
         else:
-            return float(df[self.SPHERE_RADIUS_FEATURES_KEY].iloc[self._active_sphere_index])
+            return float(
+                df[SPHERE_RADIUS_FEATURES_KEY].iloc[self._active_sphere_index])
 
     @property
     def _active_sphere_index(self) -> Union[int, None]:
         """index into data/features of current sphere"""
         if self.active_sphere_id is None:
             return None
         df = features_to_pandas_dataframe(self.points_layer.features)
-        idx = df[self.SPHERE_ID_FEATURES_KEY] == self.active_sphere_id
+        idx = df[SPHERE_ID_FEATURES_KEY] == self.active_sphere_id
         df = df.loc[idx, :]
         return df.index.values[0]
 
     @property
     def mode(self) -> SphereAnnotatorMode:
         return self._mode
 
     @mode.setter
     def mode(self, value: SphereAnnotatorMode):
         self._mode = value
         if self._mode == SphereAnnotatorMode.ADD:
             if self.points_layer is None:
                 sphere_ids = []
             else:
-                sphere_ids = self.points_layer.features[self.SPHERE_ID_FEATURES_KEY]
+                sphere_ids = self.points_layer.features[SPHERE_ID_FEATURES_KEY]
                 self.points_layer.selected_data = {}
             if len(sphere_ids) == 0:
                 new_sphere_id = 1
             else:
                 new_sphere_id = np.max(sphere_ids) + 1
             self._update_current_properties(sphere_id=new_sphere_id)
 
-    def _enable_add_mode(self, event=None):
-        """Callback for enabling add mode."""
-        self.mode = SphereAnnotatorMode.ADD
-
     def _mouse_callback(self, viewer, event):
         if (self.image_layer is None) or (self.points_layer is None):
             return
+        if ('Alt' not in event.modifiers):
+            return
         replace_selected = True if self.mode == SphereAnnotatorMode.EDIT else False
-        add_point_on_plane(
-            viewer=viewer,
-            event=event,
-            points_layer=self.points_layer,
-            plane_layer=self.image_layer,
-            replace_selected=replace_selected,
-        )
+        with self.points_layer.events.highlight.blocker():
+            add_point_on_plane(
+                viewer=viewer,
+                event=event,
+                points_layer=self.points_layer,
+                image_layer=self.image_layer,
+                replace_selected=replace_selected,
+            )
         self.mode = SphereAnnotatorMode.EDIT
 
     def _set_radius_from_mouse_event(self, event: Event = None):
         # early exits
         if (self.image_layer is None) or (self.points_layer is None):
             return
         if not self.image_layer.visible or self.active_sphere_center is None:
@@ -155,59 +136,48 @@
         self._update_active_sphere_radius(radius=radius)
         self._update_current_properties(radius=radius)
         self._update_spheres()
 
     def _update_active_sphere_radius(self, radius: float):
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore")
-            self.points_layer.features[self.SPHERE_RADIUS_FEATURES_KEY].iloc[self._active_sphere_index] = radius
+            self.points_layer.features[SPHERE_RADIUS_FEATURES_KEY].iloc[
+                self._active_sphere_index
+            ] = radius
 
     def _update_current_properties(
         self,
         sphere_id: Optional[int] = None,
         radius: Optional[float] = None
     ):
         if self.points_layer is None:
             return
         if sphere_id is None:
-            sphere_id = self.points_layer.current_properties[self.SPHERE_ID_FEATURES_KEY][0]
+            sphere_id = self.points_layer.current_properties[SPHERE_ID_FEATURES_KEY][0]
         if radius is None:
-            radius = self.points_layer.current_properties[self.SPHERE_RADIUS_FEATURES_KEY][0]
+            radius = self.points_layer.current_properties[SPHERE_RADIUS_FEATURES_KEY][0]
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore")
             self.points_layer.current_properties = {
-                self.SPHERE_ID_FEATURES_KEY: [sphere_id],
-                self.SPHERE_RADIUS_FEATURES_KEY: [radius]
+                SPHERE_ID_FEATURES_KEY: [sphere_id],
+                SPHERE_RADIUS_FEATURES_KEY: [radius]
             }
 
     def _create_points_layer(self) -> Optional[Points]:
-        layer = Points(
-            data=[0] * self.image_layer.data.ndim,
-            ndim=self.image_layer.data.ndim,
-            name="sphere centers",
-            size=7,
-            features={
-                self.SPHERE_ID_FEATURES_KEY: [0],
-                self.SPHERE_RADIUS_FEATURES_KEY: [self.DEFAULT_SPHERE_RADIUS]},
-            face_color=self.SPHERE_ID_FEATURES_KEY,
-            face_color_cycle=self.COLOR_CYCLE,
-            metadata={
-                N3D_METADATA_KEY: {
-                    ANNOTATION_TYPE_KEY: self.ANNOTATION_TYPE,
-                    self.SPHERE_MESH_METADATA_KEY: None}
-            }
-        )
+        from napari_threedee.data_models.spheres import N3dSpheres
+        ndim = self.image_layer.data.ndim if self.image_layer is not None else 3
+        layer = N3dSpheres(centers=[0] * ndim, radii=[0]).as_layer()
         layer.selected_data = {0}
         layer.remove_selected()
         return layer
 
     def _create_surface_layer(self) -> Surface:
         return Surface(
             data=(np.array([[0, 0, 0]]), np.array([[0, 0, 0]])),
-            name="spheres",
+            name="sphere meshes",
             opacity=0.7,
         )
 
     def set_layers(self, image_layer: napari.layers.Image):
         self.image_layer = image_layer
         if self.points_layer is None and self.image_layer is not None:
             self.points_layer = self._create_points_layer()
@@ -219,56 +189,55 @@
     def _on_enable(self):
         if self.points_layer is not None:
             add_mouse_callback_safe(
                 callback_list=self.viewer.mouse_drag_callbacks,
                 callback=self._mouse_callback
             )
             self.points_layer.events.data.connect(self._on_point_data_changed)
-            self.viewer.bind_key('r', self._set_radius_from_mouse_event)
-            self.viewer.bind_key('n', self._enable_add_mode)
+            self.points_layer.events.highlight.connect(self._on_highlight_change)
+            self.viewer.bind_key(
+                'r', self._set_radius_from_mouse_event, overwrite=True
+            )
+            self.viewer.bind_key(
+                'n', self._enable_add_mode, overwrite=True
+            )
             self.viewer.layers.selection.active = self.image_layer
 
     def _on_disable(self):
         remove_mouse_callback_safe(
             callback_list=self.viewer.mouse_drag_callbacks,
             callback=self._mouse_callback
         )
         if self.points_layer is not None:
             self.points_layer.events.data.disconnect(self._on_point_data_changed)
-        self.viewer.bind_key('n', None)
+        self.viewer.bind_key('n', None, overwrite=True)
+        self.viewer.bind_key('r', None, overwrite=True)
 
     def _on_point_data_changed(self, event=None):
         self._update_spheres()
 
     def _update_spheres(self):
+        from napari_threedee.data_models import N3dSpheres
+        vertices, faces = N3dSpheres.from_layer(self.points_layer).to_mesh()
         n3d_metadata = self.points_layer.metadata[N3D_METADATA_KEY]
-        n3d_metadata[self.SPHERE_MESH_METADATA_KEY] = None
-        grouped_points_features = self.points_layer.features.groupby(self.SPHERE_ID_FEATURES_KEY)
-        sphere_vertices = []
-        sphere_faces = []
-        face_index_offset = 0
-        for sphere_id, sphere_df in grouped_points_features:
-            point_index = int(sphere_df.index.values[0])
-            position = self.points_layer.data[point_index]
-            radius = float(sphere_df[self.SPHERE_RADIUS_FEATURES_KEY].iloc[0])
-            mesh_data = create_sphere(radius=radius, rows=20, cols=20)
-            vertex_data = mesh_data.get_vertices() + position
-            sphere_vertices.append(vertex_data)
-            sphere_faces.append(mesh_data.get_faces() + face_index_offset)
-            face_index_offset += len(vertex_data)
-        if len(sphere_vertices) > 0:
-            sphere_vertices = np.concatenate(sphere_vertices, axis=0)
-            sphere_faces = np.concatenate(sphere_faces, axis=0)
-            n3d_metadata[self.SPHERE_MESH_METADATA_KEY] = (
-                sphere_vertices, sphere_faces
-            )
+        if len(vertices) > 0:
+            n3d_metadata[SPHERE_MESH_METADATA_KEY] = (vertices, faces)
             self._draw_spheres()
         else:
-            n3d_metadata[self.SPHERE_MESH_METADATA_KEY] = None
+            n3d_metadata[SPHERE_MESH_METADATA_KEY] = None
 
     def _draw_spheres(self):
         n3d_metadata = self.points_layer.metadata[N3D_METADATA_KEY]
-        sphere_data = n3d_metadata[self.SPHERE_MESH_METADATA_KEY]
-        if sphere_data is None:
+        if self.surface_layer is None:
             self.surface_layer = self._create_surface_layer()
-        else:
-            self.surface_layer.data = n3d_metadata[self.SPHERE_MESH_METADATA_KEY]
+        if self.surface_layer not in self.viewer.layers:
+            self.viewer.layers.append(self.surface_layer)
+        self.surface_layer.data = n3d_metadata[SPHERE_MESH_METADATA_KEY]
+
+    def _enable_add_mode(self, event=None):
+        """Callback for enabling add mode."""
+        self.mode = SphereAnnotatorMode.ADD
+
+    def _on_highlight_change(self, event=None):
+        """Callback for enabling edit mode."""
+        self.mode = SphereAnnotatorMode.EDIT
+
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/annotators/spline_annotator.py` & `napari-threedee-0.0.4/src/napari_threedee/annotators/surfaces/annotator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-
 import einops
 
 import napari
 from napari.layers import Image, Points, Shapes
 from napari.utils.events.event import EmitterGroup, Event
 import numpy as np
 from psygnal import EventedModel
 from pydantic import validator, PrivateAttr
 from scipy.interpolate import splprep, splev
 from typing import Tuple, Union, Optional, Dict
 
-from napari_threedee._backend.threedee_model import ThreeDeeModel
-from ..mouse_callbacks import add_point_on_plane
+from morphosamplers.surface_spline import GriddedSplineSurface
+
+from napari_threedee._backend.threedee_model import N3dComponent
+from napari_threedee.utils.mouse_callbacks import add_point_on_plane
 from napari_threedee.utils.napari_utils import add_mouse_callback_safe, \
     remove_mouse_callback_safe
-from .io import N3D_METADATA_KEY, ANNOTATION_TYPE_KEY
+from .constants import (
+    N3D_METADATA_KEY,
+    ANNOTATION_TYPE_KEY,
+    SURFACE_ANNOTATION_TYPE_KEY,
+    SURFACE_ID_FEATURES_KEY,
+    LEVEL_ID_FEATURES_KEY,
+    SPLINES_METADATA_KEY,
+    SPLINE_COLOR_FEATURES_KEY,
+    COLOR_CYCLE,
+)
 
 
 class _NDimensionalFilament(EventedModel):
     points: np.ndarray
     _n_spline_samples = 10000
     _raw_spline_tck = PrivateAttr(Tuple)
     _equidistant_spline_tck = PrivateAttr(Tuple)
@@ -40,15 +50,15 @@
         points = np.atleast_2d(np.array(v))
         if points.ndim != 2:
             raise ValueError('must be an (n, d) array')
         return points
 
     def __setattr__(self, name, value):
         super().__setattr__(name, value)
-        if name == 'points':  # ensure splines stay in sync
+        if name == 'points':  # ensure paths stay in sync
             self._prepare_splines()
 
     def _prepare_splines(self):
         self._calculate_filament_spline_parameters()
         self._calculate_equidistant_spline_parameters()
 
     def _calculate_filament_spline_parameters(self):
@@ -110,195 +120,207 @@
         self, separation: float, calculate_derivative: bool = False
     ) -> np.ndarray:
         """Calculate equidistant backbone samples with a defined separation in Euclidean space."""
         u = self._get_equidistant_u(separation)
         return self._sample_backbone(u, derivative=calculate_derivative)
 
 
-class SplineAnnotator(ThreeDeeModel):
-    COLOR_CYCLE = [
-        '#1f77b4',
-        '#ff7f0e',
-        '#2ca02c',
-        '#d62728',
-        '#9467bd',
-        '#8c564b',
-        '#e377c2',
-        '#7f7f7f',
-        '#bcbd22',
-        '#17becf',
-    ]
-    ANNOTATION_TYPE = "spline"
-    # keys for data stored in features table
-    SPLINE_ID_FEATURES_KEY = "spline_id"
-    SPLINE_COLOR_FEATURES_KEY = "spline_color"
-
-    # metadata and associated keys
-    SPLINES_KEY = "splines"
-    SPLINE_ORDER = 3
-
+class SurfaceAnnotator(N3dComponent):
     def __init__(
         self,
         viewer: napari.Viewer,
         image_layer: Optional[Image] = None,
-        enabled: bool = False
+        enabled: bool = True
     ):
         self.events = EmitterGroup(
             source=self,
-            active_spline_id=Event,
-            splines_updated=Event,
+            active_surface_id=Event,
+            active_level_id=Event,
         )
 
         self.viewer = viewer
         self.image_layer = image_layer
         self.points_layer = None
         self.shapes_layer = None
+        self.surface_layer = None
         self.auto_fit_spline = True
         self.enabled = enabled
 
-        self.active_spline_id: int = 0
+        self.active_surface_id: int = 0
+        self.active_level_id: int = 0
 
         # storage for the spline objects
         # each spline is in its own object
         self._splines = dict()
 
         if image_layer is not None:
             self.set_layers(self.image_layer)
 
     @property
-    def active_spline_id(self):
+    def active_surface_id(self):
+        return self._active_surface_id
+
+    @active_surface_id.setter
+    def active_surface_id(self, id: int):
+        self._active_surface_id = np.clip(id, 0, None)
+        if self.points_layer is not None:
+            self.points_layer.selected_data = {}
+            self.points_layer.current_properties = {
+                SURFACE_ID_FEATURES_KEY: self.active_surface_id,
+                LEVEL_ID_FEATURES_KEY: self.active_level_id,
+            }
+        self.events.active_surface_id()
+
+    @property
+    def active_level_id(self):
         return self._active_spline_id
 
-    @active_spline_id.setter
-    def active_spline_id(self, id: int):
+    @active_level_id.setter
+    def active_level_id(self, id: int):
         self._active_spline_id = np.clip(id, 0, None)
         if self.points_layer is not None:
             self.points_layer.selected_data = {}
             self.points_layer.current_properties = {
-                self.SPLINE_ID_FEATURES_KEY: self.active_spline_id
+                SURFACE_ID_FEATURES_KEY: self.active_surface_id,
+                LEVEL_ID_FEATURES_KEY: self.active_level_id,
             }
-        self.events.active_spline_id()
+        self.events.active_level_id()
 
     def next_spline(self, event=None):
-        self.active_spline_id += 1
+        self.active_level_id += 1
 
     def previous_spline(self, event=None):
-        self.active_spline_id -= 1
+        self.active_level_id -= 1
+
+    def next_surface(self, event=None):
+        self.active_surface_id += 1
+
+    def previous_surface(self, event=None):
+        self.active_surface_id -= 1
 
     def _mouse_callback(self, viewer, event):
         if (self.image_layer is None) or (self.points_layer is None):
             return
         add_point_on_plane(
             viewer=viewer,
             event=event,
             points_layer=self.points_layer,
-            plane_layer=self.image_layer
+            image_layer=self.image_layer
         )
 
     def _create_points_layer(self) -> Optional[Points]:
         layer = Points(
             data=[0] * self.image_layer.data.ndim,
             ndim=self.image_layer.data.ndim,
-            name="spline control points",
-            size=3,
-            features={self.SPLINE_ID_FEATURES_KEY: [0]},
-            face_color=self.SPLINE_ID_FEATURES_KEY,
-            face_color_cycle=self.COLOR_CYCLE,
+            name="n3d surfaces",
+            size=10,
+            features={
+                SURFACE_ID_FEATURES_KEY: [0],
+                LEVEL_ID_FEATURES_KEY: [0],
+            },
+            face_color=SURFACE_ID_FEATURES_KEY,
+            face_color_cycle=COLOR_CYCLE,
             metadata={
                 N3D_METADATA_KEY: {
-                    ANNOTATION_TYPE_KEY: self.ANNOTATION_TYPE,
-                    self.SPLINES_KEY: dict,
+                    ANNOTATION_TYPE_KEY: SURFACE_ANNOTATION_TYPE_KEY,
+                    SPLINES_METADATA_KEY: dict,
                 }
             }
         )
         layer.selected_data = {0}
         layer.remove_selected()
-        self.active_spline_id = self.active_spline_id
+        self.active_level_id = self.active_level_id
         return layer
 
     def _create_shapes_layer(self) -> Shapes:
         return Shapes(
             ndim=self.image_layer.data.ndim,
-            name="splines",
+            name="n3d surfaces (paths)",
             edge_color="green"
         )
 
     def set_layers(self, image_layer: napari.layers.Image):
+        original_enabled_state = self.enabled
+        self.enabled = False
         self.image_layer = image_layer
         if self.points_layer is None and self.image_layer is not None:
             self.points_layer = self._create_points_layer()
             self.viewer.add_layer(self.points_layer)
             self.shapes_layer = self._create_shapes_layer()
             self.viewer.add_layer(self.shapes_layer)
+        self.enabled = original_enabled_state
 
     def _on_enable(self):
         if self.points_layer is not None:
             add_mouse_callback_safe(
                 self.viewer.mouse_drag_callbacks, self._mouse_callback
             )
             self.points_layer.events.data.connect(self._on_point_data_changed)
-            self.viewer.bind_key('n', self.next_spline)
+            self.viewer.bind_key('n', self.next_spline, overwrite=True)
             self.viewer.layers.selection.active = self.image_layer
 
     def _on_disable(self):
         remove_mouse_callback_safe(
             self.viewer.mouse_drag_callbacks, self._mouse_callback
         )
         if self.points_layer is not None:
             self.points_layer.events.data.disconnect(
                 self._on_point_data_changed
             )
-        self.viewer.bind_key('n', None)
+        self.viewer.bind_key('n', None, overwrite=True)
 
     def _on_point_data_changed(self, event=None):
         if self.auto_fit_spline is True:
-            self._update_splines()
             self._draw_splines()
 
-    def _update_splines(self):
-        grouped_points_features = self.points_layer.features.groupby(
-            self.SPLINE_ID_FEATURES_KEY
-        )
-        splines = dict()
-        for spline_name, spline_df in grouped_points_features:
-            point_indices = spline_df.index.tolist()
-            if len(point_indices) > self.SPLINE_ORDER:
-                # the number of points must be greater than the spline order to properly fit
-                spline_coordinates = self.points_layer.data[point_indices]
-                splines[spline_name] = _NDimensionalFilament(
-                    points=spline_coordinates, k=self.SPLINE_ORDER
-                )
-        metadata = {
-            self.SPLINES_KEY: splines
-        }
-        self.points_layer.metadata[N3D_METADATA_KEY].update(metadata)
-        self.events.splines_updated()
-
-    def _get_spline_colors(self) -> Dict[int, np.ndarray]:
-        self.points_layer.features[self.SPLINE_COLOR_FEATURES_KEY] = \
+    def _get_path_colors(self) -> Dict[int, np.ndarray]:
+        self.points_layer.features[SPLINE_COLOR_FEATURES_KEY] = \
             list(self.points_layer.face_color)
         grouped_points_features = self.points_layer.features.groupby(
-            self.SPLINE_ID_FEATURES_KEY
+            LEVEL_ID_FEATURES_KEY
         )
         spline_colors = dict()
         for spline_id, spline_df in grouped_points_features:
-            spline_colors[spline_id] = spline_df[self.SPLINE_COLOR_FEATURES_KEY].iloc[0]
+            spline_colors[spline_id] = spline_df[SPLINE_COLOR_FEATURES_KEY].iloc[0]
         return spline_colors
 
     def _clear_shapes_layer(self):
         """Delete all shapes in the shapes layer."""
         if self.shapes_layer is None:
             return
         n_shapes = len(self.shapes_layer.data)
         self.shapes_layer.selected_data = set(np.arange(n_shapes))
         self.shapes_layer.remove_selected()
 
     def _draw_splines(self):
+        from napari_threedee.data_models import N3dSurfaces, N3dPath
+        surfaces = N3dSurfaces.from_layer(self.points_layer)
         self._clear_shapes_layer()
-        splines = self.points_layer.metadata[N3D_METADATA_KEY][self.SPLINES_KEY]
-        spline_colors = self._get_spline_colors()
-        for spline_id, spline_object in splines.items():
-            spline_points = spline_object._sample_backbone(
-                u=np.linspace(0, 1, 1000)
+        path_colors = self._get_path_colors()
+        for idx, surface in enumerate(surfaces):
+            for level_points in surface:
+                if len(level_points) >= 2:
+                    path = N3dPath(data=level_points).sample(n=1000)
+                    path_color = path_colors[idx]
+                    self.shapes_layer.add_paths(path, edge_color=path_color)
+
+    def _draw_surface(self):
+        grouped_features = self.points_layer.features.groupby(
+            LEVEL_ID_FEATURES_KEY
+        )
+        surface_levels = [
+            self.points_layer.data[df.index]
+            for _, df in grouped_features
+        ]
+        surface = GriddedSplineSurface(points=surface_levels, separation=3)
+        surface_points, triangle_idx = surface.mesh()
+        valid_triangle_idx = np.all(np.isin(triangle_idx, np.argwhere(surface.mask)),
+                                    axis=1)
+        triangle_idx = triangle_idx[valid_triangle_idx]
+
+        if self.surface_layer is None:
+            self.surface_layer = self.viewer.add_surface(
+                data=(surface_points, triangle_idx),
+                shading='flat'
             )
-            spline_color = spline_colors[spline_id]
-            self.shapes_layer.add_paths(spline_points, edge_color=spline_color)
+        else:
+            self.surface_layer.data = surface.mesh()
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/conftest.py` & `napari-threedee-0.0.4/src/napari_threedee/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/manipulators/_tests/test_manipulator_utils.py` & `napari-threedee-0.0.4/src/napari_threedee/manipulators/_tests/test_manipulator_utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/manipulators/base_manipulator.py` & `napari-threedee-0.0.4/src/napari_threedee/manipulators/base_manipulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Type
 
 import napari
 import numpy as np
 from napari.viewer import Viewer
 
-from napari_threedee._backend.threedee_model import ThreeDeeModel
+from napari_threedee._backend.threedee_model import N3dComponent
 from .._backend.manipulator.axis_model import AxisModel
 from .._backend.manipulator.napari_manipulator_backend import \
     NapariManipulatorBackend
 from napari_threedee.utils.napari_utils import add_mouse_callback_safe, \
     remove_mouse_callback_safe
 
 
-class BaseManipulator(ThreeDeeModel, ABC):
+class BaseManipulator(N3dComponent, ABC):
     """Base class for manipulator implementations.
 
     To implement:
         - the __init__() should take the viewer as the first argument, the layer
             as the second argument followed by any keyword arguments.
             Keyword arguments should have default values.
         - The __init__() should call the super.__init__().
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/manipulators/layer_manipulator.py` & `napari-threedee-0.0.4/src/napari_threedee/manipulators/layer_manipulator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import napari
 import numpy as np
 
 from napari_threedee.manipulators.base_manipulator import BaseManipulator
+from napari_threedee.utils.napari_utils import get_dims_displayed
 
 
 class LayerManipulator(BaseManipulator):
     """A manipulator for translating a layer."""
 
     def __init__(self, viewer, layer=None):
         super().__init__(viewer, layer, rotator_axes=None, translator_axes='xyz')
@@ -14,15 +15,16 @@
         super().set_layers(layer)
 
     def _initialize_transform(self):
         # self.origin = self.layer.translate[self.layer._dims_displayed]
         self.origin = np.asarray((0, 0, 0))
 
     def _pre_drag(self):
-        self.translate_start = self.layer.translate[self.layer._dims_displayed].copy()
+        dims_displayed = get_dims_displayed(self.layer)
+        self.translate_start = self.layer.translate[dims_displayed].copy()
 
     def _while_dragging_translator(self):
         new_translate = self.translate_start + self.origin
         self.layer.translate = new_translate
         # origin is relative to the layer transform so needs
         # to be reset after updating the transform
         self.origin = np.asarray((0, 0, 0))
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/manipulators/manipulator_utils.py` & `napari-threedee-0.0.4/src/napari_threedee/manipulators/manipulator_utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/manipulators/point_manipulator.py` & `napari-threedee-0.0.4/src/napari_threedee/manipulators/point_manipulator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/manipulators/render_plane_manipulator.py` & `napari-threedee-0.0.4/src/napari_threedee/manipulators/render_plane_manipulator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/mouse_callbacks.py` & `napari-threedee-0.0.4/src/napari_threedee/utils/mouse_callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from napari.layers.utils.interactivity_utils import drag_data_to_projected_distance
 import numpy as np
 
-from .geometry_utils import point_in_bounding_box
+from napari_threedee.utils.geometry import point_in_bounding_box
 
 if TYPE_CHECKING:
     import napari
     import napari.layers
     from napari.utils.events import Event
 
 
 def add_point_on_plane(
         viewer: napari.viewer.Viewer,
         event: Event,
         points_layer: napari.layers.Points = None,
-        plane_layer: napari.layers.Image = None,
+        image_layer: napari.layers.Image = None,
         replace_selected: bool = False,
 ):
     # Early exit if not alt-clicked
     if 'Alt' not in event.modifiers:
         return
 
-    # Early exit if plane_layer isn't visible
-    if not plane_layer.visible:
+    # Early exit if image_layer isn't visible
+    if image_layer.visible is False or image_layer.depiction != 'plane':
         return
 
     # Calculate intersection of click with plane through data in displayed data (scene) coordinates
     displayed_dims = np.asarray(viewer.dims.displayed)[list(viewer.dims.displayed_order)]
     cursor_position_3d = np.asarray(event.position)[displayed_dims]
-    intersection_3d = plane_layer.plane.intersect_with_line(
+    intersection_3d = image_layer.plane.intersect_with_line(
         line_position=cursor_position_3d,
         line_direction=event.view_direction[displayed_dims]
     )
     intersection_nd = np.asarray(viewer.dims.point)
     intersection_nd[displayed_dims] = intersection_3d
 
     # Check if click was on plane by checking if intersection occurs within
     # data bounding box. If not, exit early.
-    if not point_in_bounding_box(intersection_nd, plane_layer.extent.data):
+    if not point_in_bounding_box(intersection_nd, image_layer.extent.data):
         return
 
     if replace_selected:
         points_layer.remove_selected()
+    if points_layer.data.shape[-1] < len(intersection_nd):
+        intersection_nd = intersection_3d
     points_layer.add(intersection_nd)
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/napari.yaml` & `napari-threedee-0.0.4/src/napari_threedee/napari.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,25 @@
 contributions:
   commands:
     # Annotators
     - id: napari-threedee.QtPointAnnotatorWidget
       title: Create point annotator
       python_name: napari_threedee.dock_widgets:QtPointAnnotatorWidget
 
-    - id: napari-threedee.QtSplineAnnotatorWidget
-      title: Create filament annotator
-      python_name: napari_threedee.dock_widgets:QtSplineAnnotatorWidget
+    - id: napari-threedee.QtPathAnnotatorWidget
+      title: Create path annotator
+      python_name: napari_threedee.dock_widgets:QtPathAnnotatorWidget
+
+    - id: napari-threedee.QtSphereAnnotatorWidget
+      title: Create sphere annotator
+      python_name: napari_threedee.dock_widgets:QtSphereAnnotatorWidget
+
+    - id: napari-threedee.QtSurfaceAnnotatorWidget
+      title: Create surface annotator
+      python_name: napari_threedee.dock_widgets:QtSurfaceAnnotatorWidget
 
     # Manipulators
     - id: napari-threedee.QtRenderPlaneManipulatorWidget
       title: Create render plane manipulator
       python_name: napari_threedee.dock_widgets:QtRenderPlaneManipulatorWidget
 
     - id: napari-threedee.QtPointManipulatorWidget
@@ -46,16 +54,22 @@
 
 
   widgets:
     # Annotators
     - command: napari-threedee.QtPointAnnotatorWidget
       display_name: point annotator
 
-    - command: napari-threedee.QtSplineAnnotatorWidget
-      display_name: spline annotator
+    - command: napari-threedee.QtPathAnnotatorWidget
+      display_name: path annotator
+
+    - command: napari-threedee.QtSphereAnnotatorWidget
+      display_name: sphere annotator
+
+    - command: napari-threedee.QtSurfaceAnnotatorWidget
+      display_name: surface annotator
 
     # Manipulators
     - command: napari-threedee.QtRenderPlaneManipulatorWidget
       display_name: render plane manipulator
 
     - command: napari-threedee.QtPointManipulatorWidget
       display_name: point manipulator
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/utils/_tests/test_geometry.py` & `napari-threedee-0.0.4/src/napari_threedee/utils/_tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/utils/geometry.py` & `napari-threedee-0.0.4/src/napari_threedee/utils/geometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import numpy as np
 
+from napari_threedee.utils.napari_utils import get_dims_displayed
 
-def signed_angle_between_vectors(vector_0, vector_1, rotation_axis: np.ndarray) -> float:
+
+def signed_angle_between_vectors(vector_0, vector_1,
+                                 rotation_axis: np.ndarray) -> float:
     """ Returns the angle in radians between vectors 'v1' and 'v2'.
 
     Parameters
     ----------
     vector_0 : np.ndarray
         The vector to start the rotation at.
     vector_1 : np.ndarray
@@ -52,20 +55,44 @@
     u_1 = vector_u[1]
     u_2 = vector_u[2]
 
     cos_term = 1 - np.cos(angle)
     sine_term = np.sin(angle)
 
     rotation_matrix = np.zeros((3, 3))
-    rotation_matrix[0, 0] = np.cos(angle) + (u_0**2) * cos_term
+    rotation_matrix[0, 0] = np.cos(angle) + (u_0 ** 2) * cos_term
     rotation_matrix[0, 1] = (u_0 * u_1 * cos_term) - u_2 * sine_term
     rotation_matrix[0, 2] = (u_0 * u_2 * cos_term) + u_1 * sine_term
 
     rotation_matrix[1, 0] = (u_1 * u_0 * cos_term) + u_2 * sine_term
-    rotation_matrix[1, 1] = np.cos(angle) + (u_1**2) * cos_term
+    rotation_matrix[1, 1] = np.cos(angle) + (u_1 ** 2) * cos_term
     rotation_matrix[1, 2] = (u_1 * u_2 * cos_term) - u_0 * sine_term
 
     rotation_matrix[2, 0] = (u_0 * u_2 * cos_term) - u_1 * sine_term
     rotation_matrix[2, 1] = u_1 * u_2 * cos_term + u_0 * sine_term
-    rotation_matrix[2, 2] = np.cos(angle) + (u_2**2) * cos_term
+    rotation_matrix[2, 2] = np.cos(angle) + (u_2 ** 2) * cos_term
 
     return rotation_matrix
+
+
+def point_in_bounding_box(point: np.ndarray, bounding_box: np.ndarray) -> bool:
+    """Determine whether an nD point is inside an nD bounding box.
+    Parameters
+    ----------
+    point : np.ndarray
+        (n,) array containing nD point coordinates to check.
+    bounding_box : np.ndarray
+        (2, n) array containing the min and max of the nD bounding box.
+        As returned by `Layer._extent_data`.
+    """
+    if np.all(point > bounding_box[0]) and np.all(point < bounding_box[1]):
+        return True
+    return False
+
+
+def point_in_layer_bounding_box(point, layer):
+    dims_displayed = get_dims_displayed(layer)
+    bbox = layer._display_bounding_box(dims_displayed).T
+    if np.any(point < bbox[0]) or np.any(point > bbox[1]):
+        return False
+    else:
+        return True
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/utils/napari_utils.py` & `napari-threedee-0.0.4/src/napari_threedee/utils/napari_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,22 @@
             callback_list.append(callback)
 
 
 def get_layers_of_type(*args, viewer: napari.Viewer, layer_type):
     return [layer for layer in viewer.layers if isinstance(layer, layer_type)]
 
 
+def get_dims_displayed(layer):
+    # layer._dims_displayed was removed in
+    # https://github.com/napari/napari/pull/5003
+    if hasattr(layer, "_slice_input"):
+        return layer._slice_input.displayed
+    return layer._dims_displayed
+
+
 def generate_populated_layer_selection_widget(func, viewer) -> FunctionGui:
     parameters = inspect.signature(func).parameters
     magicgui_parameter_arguments = {
         parameter_name: {
             'choices': partial(get_layers_of_type, viewer=viewer, layer_type=parameter.annotation)
         }
         for parameter_name, parameter
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/utils/selection_utils.py` & `napari-threedee-0.0.4/src/napari_threedee/utils/selection_utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.3/src/napari_threedee/visualization/_qt/qt_camera_spline.py` & `napari-threedee-0.0.4/src/napari_threedee/visualization/_qt/qt_camera_spline.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,17 +162,27 @@
         super().__init__(model_class=CameraSpline, viewer=viewer)
 
         # create and add the spline widget
         self.spline_widget = QtCameraSplineControls(viewer=viewer, model=self.model, parent=self)
         self.spline_widget.setVisible(False)
         self.layout().addWidget(self.spline_widget)
 
+    def activate(self):
+        """Activate the spline widget"""
+        self.model.enabled = True
+        self.activate_button.setChecked(True)
+        self.activate_button.setText(self.DISABLE_STRING)
+        self.spline_widget.setVisible(True)
+
+    def deactivate(self):
+        """Deactivate the spline widget"""
+        self.model.enabled = False
+        self.activate_button.setChecked(False)
+        self.activate_button.setText(self.ENABLE_STRING)
+        self.spline_widget.setVisible(False)
+
     def on_activate_button_click(self, event: Event):
         """Callback function when the activate button is clicked"""
         if self.activate_button.isChecked() is True:
-            self.model.enabled = True
-            self.activate_button.setText(self.DISABLE_STRING)
-            self.spline_widget.setVisible(True)
+            self.activate()
         else:
-            self.model.enabled = False
-            self.activate_button.setText(self.ENABLE_STRING)
-            self.spline_widget.setVisible(False)
+            self.deactivate()
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/visualization/_qt/qt_lighting_control.py` & `napari-threedee-0.0.4/src/napari_threedee/visualization/_qt/qt_lighting_control.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from napari_threedee.visualization.lighting_control import LightingControl
 
 
 class QtLightingControlWidget(QWidget):
     _ENABLE_TEXT = 'start following camera'
     _DISABLE_TEXT = 'stop following camera'
+    _TOOLTIP = 'viewer must be in 3D mode'
 
     def __init__(self, viewer: napari.Viewer):
         super().__init__()
         self._viewer = viewer
         self.model = LightingControl(viewer=viewer)
 
         # create layer selection widget
@@ -20,27 +21,47 @@
             layers={
                 'widget_type': 'Select',
                 'choices': self._get_layers
             },
             auto_call=True
         )
 
+        self._viewer.dims.events.ndisplay.connect(self._on_ndisplay_change)
+        self._viewer.layers.events.inserted.connect(
+            self._layer_selection_widget.reset_choices
+        )
+        self._viewer.layers.events.removed.connect(
+            self._layer_selection_widget.reset_choices
+        )
+
         # create set lighing widget
         self._lighting_button = QPushButton(self._ENABLE_TEXT, self)
-        self._lighting_button.setCheckable(True)
         self._lighting_button.setChecked(False)
         self._lighting_button.clicked.connect(self._on_lighting_clicked)
+        self._update_lighting_button()
 
         self.setLayout(QVBoxLayout())
         self.layout().addWidget(self._layer_selection_widget.native)
         self.layout().addWidget(self._lighting_button)
 
+    def _update_lighting_button(self):
+        viewer_is_3d = self._viewer.dims.ndisplay == 3
+        self._lighting_button.setCheckable(viewer_is_3d)
+        self._lighting_button.setEnabled(viewer_is_3d)
+        self._lighting_button.setToolTip("" if viewer_is_3d else self._TOOLTIP)
+
     def _on_lighting_clicked(self, event):
         if self._lighting_button.isChecked() is True:
             self.model.enabled = True
             self._lighting_button.setText(self._DISABLE_TEXT)
         else:
             self.model.enabled = False
             self._lighting_button.setText(self._ENABLE_TEXT)
 
+    def _on_ndisplay_change(self, event):
+        ndisplay = event.value
+        if ndisplay == 2 and self._lighting_button.isChecked() is True:
+            self._lighting_button.click()
+        self._update_lighting_button()
+
     def _get_layers(self, widget):
         return [layer for layer in self._viewer.layers if isinstance(layer, napari.layers.Surface)]
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/visualization/_tests/test_camera_spline.py` & `napari-threedee-0.0.4/src/napari_threedee/visualization/_tests/test_camera_spline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-import platform
+import napari
 from typing import Tuple
 
-import napari
 import numpy as np
-import pytest
 
-from napari_threedee.annotators import SplineAnnotator
-from napari_threedee.annotators.io import N3D_METADATA_KEY
+from napari_threedee.annotators import PathAnnotator
+from napari_threedee.annotators.constants import N3D_METADATA_KEY
+from napari_threedee.data_models import N3dPaths
 from napari_threedee.visualization.camera_spline import CameraSpline, CameraSplineMode
 
 
-def test_initialize_camera_spline():
+def test_initialize_camera_spline(make_napari_viewer):
     """Test creation of an empty CameraSpline model."""
-    viewer = napari.Viewer()
+    viewer = make_napari_viewer()
     camera_spline = CameraSpline(viewer=viewer)
 
     assert camera_spline.image_layer is None
     assert camera_spline.enabled is False
 
 
-def test_setting_camera_spline_mode():
+def test_setting_camera_spline_mode(make_napari_viewer):
     """Test setting camera spline mode with strings and Enum"""
-    viewer = napari.Viewer()
+    viewer = make_napari_viewer()
     camera_spline = CameraSpline(viewer=viewer)
 
     # default mode
     assert camera_spline.mode == CameraSplineMode.PAN_ZOOM
 
     # with strings
     camera_spline.mode = "explore"
@@ -43,18 +42,17 @@
 class FakeMouseEvent:
     position: Tuple[float, float, float]
     view_direction: Tuple[float, float, float] = (1, 0, 0)
     dims_displayed: Tuple[int, int, int] = (0, 1, 2)
     modifiers: Tuple[str] = ("Alt",)
 
 
-@pytest.mark.skipif(platform.system() == 'Windows', reason="fails on CI")
-def test_annotate_spline():
+def test_annotate_spline(make_napari_viewer):
     """Test annotating a spline in the CameraSpline model."""
-    viewer = napari.Viewer()
+    viewer = make_napari_viewer()
     camera_spline = CameraSpline(viewer=viewer)
 
     # add an image layer to the viewer
     plane_parameters_z = {
         'position': (15, 15, 15),
         'normal': (1, 0, 0),
         'thickness': 10,
@@ -71,22 +69,22 @@
     # get the points layer
     points_layer = camera_spline.spline_annotator_model.points_layer
     assert isinstance(points_layer, napari.layers.Points)
 
     # add 4 points and check that the spline was created
     points_layer.add(np.random.random((4, 3)))
     assert camera_spline.spline_valid is True
-    n3d_metadata = points_layer.metadata[N3D_METADATA_KEY]
-    assert len(n3d_metadata[SplineAnnotator.SPLINES_KEY]) == 1
+
+    paths = N3dPaths.from_layer(points_layer)
+    assert len(paths.data) == 1
 
 
-@pytest.mark.skipif(platform.system() == 'Windows', reason="fails on CI")
-def test_spline_explore():
+def test_spline_explore(make_napari_viewer):
     """Test moving the camera along the spline"""
-    viewer = napari.Viewer()
+    viewer = make_napari_viewer()
     viewer.dims.ndisplay = 3
     camera_spline = CameraSpline(viewer=viewer)
 
     # add an image layer to the viewer
     plane_parameters_z = {
         'position': (15, 15, 15),
         'normal': (1, 0, 0),
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/visualization/camera_spline.py` & `napari-threedee-0.0.4/src/napari_threedee/visualization/camera_spline.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 
 import napari
 from napari.layers import Image
 from napari.utils.events.event import EmitterGroup, Event
 from napari.utils.geometry import rotation_matrix_from_vectors_3d
 import numpy as np
 
-from .._backend.threedee_model import ThreeDeeModel
-from ..annotators.spline_annotator import SplineAnnotator
-from ..annotators.io import N3D_METADATA_KEY
+from .._backend.threedee_model import N3dComponent
+from ..annotators.paths import PathAnnotator
+from ..annotators.constants import N3D_METADATA_KEY
+from ..data_models import N3dPaths
+from ..data_models.spline_sampler import SplineSampler
 
 
 class CameraSplineMode(Enum):
     PAN_ZOOM = "pan_zoom"
     EXPLORE = "explore"
     ANNOTATE = "annotate"
 
 
-class CameraSpline(ThreeDeeModel):
+class CameraSpline(N3dComponent):
     """Model for a spline that is used to direct the camera path."""
     COLOR_CYCLE = [
         '#1f77b4',
         '#ff7f0e',
         '#2ca02c',
         '#d62728',
         '#9467bd',
@@ -52,16 +54,16 @@
         self._image_layer = image_layer
         self._mode = CameraSplineMode("pan_zoom")
         self._spline_valid = False
         self._up_direction = (1, 0, 0)
         self._view_direction_transformation = np.eye(3)
         self._current_spline_coordinate = 0
 
-        self.spline_annotator_model = SplineAnnotator(viewer=viewer, image_layer=None, enabled=False)
-        self.spline_annotator_model.events.splines_updated.connect(self._check_if_spline_valid)
+        self.spline_annotator_model = PathAnnotator(viewer=viewer, image_layer=None, enabled=False)
+        self.spline_annotator_model.events.paths_updated.connect(self._check_if_spline_valid)
 
         self._check_if_spline_valid()
         self.enabled = enabled
 
     @property
     def mode(self) -> CameraSplineMode:
         """The current mode for interaction.
@@ -184,15 +186,15 @@
     def current_spline_coordinate(self, current_spline_coordinate: float):
         self._current_spline_coordinate = current_spline_coordinate
         self.set_camera_position(self.current_spline_coordinate)
 
     def calculate_transform_from_spline_tangent_to_view_direction(self):
         current_view_direction = self.viewer.camera.view_direction
         n3d_metadata = self.spline_annotator_model.points_layer.metadata[N3D_METADATA_KEY]
-        spline_dict = n3d_metadata[SplineAnnotator.SPLINES_KEY]
+        spline_dict = n3d_metadata[PathAnnotator.SPLINES_KEY]
 
         # only one spline
         spline_object = spline_dict[0]
         spline_tangent = np.squeeze(spline_object._sample_backbone(u=[self.current_spline_coordinate], derivative=1))
         spline_tangent_displayed = spline_tangent[list(self.viewer.dims.displayed)]
 
         self.view_direction_transformation = rotation_matrix_from_vectors_3d(
@@ -200,25 +202,27 @@
         )
 
         # get the current up direction
         self.up_direction = self.viewer.camera.up_direction
 
     def _check_if_spline_valid(self, event=None):
         """Check if there is a valid spline to slice along"""
+        from napari_threedee.data_models import N3dPaths
         spline_points_layer = self.spline_annotator_model.points_layer
+
         if spline_points_layer is None:
+            # if the points layer isn't set, the path can't be valid
             self.spline_valid = False
             return
-        n3d_metadata = spline_points_layer.metadata[N3D_METADATA_KEY]
-        spline_dict = n3d_metadata[SplineAnnotator.SPLINES_KEY]
-        spline_object = spline_dict.get(0, None)
-        if spline_object is None:
-            self.spline_valid = False
-        else:
+
+        paths = N3dPaths.from_layer(spline_points_layer)
+        if len(paths.data) > 0:
             self.spline_valid = True
+        else:
+            self.spline_valid = False
 
     @property
     def image_layer(self) -> Image:
         """The image layer to set the spline points on.
 
         The visualization plane for the image layer is used to set
         the plane the spline points are added on.
@@ -254,23 +258,23 @@
         if self.image_layer is None:
             # do not do anything if the image layer hasn't been set
             return
 
         if self.spline_valid is False:
             # do not do anything if there isn't a valid spline
             return
-        n3d_metadata = self.spline_annotator_model.points_layer.metadata[N3D_METADATA_KEY]
-        spline_dict = n3d_metadata[SplineAnnotator.SPLINES_KEY]
+        paths = N3dPaths.from_layer(self.spline_annotator_model.points_layer)
 
         # only one spline
-        spline_object = spline_dict[0]
-        spline_point = spline_object._sample_backbone(u=[spline_coordinate])
+        spline_object = paths[0]
+        spline_sampler = SplineSampler(points=spline_object.data)
+        spline_point = spline_sampler(u=[spline_coordinate], derivative=0)
         self.viewer.camera.center = np.squeeze(spline_point)
 
-        view_direction = np.squeeze(spline_object._sample_backbone(u=[spline_coordinate], derivative=1))
+        view_direction = np.squeeze(spline_sampler(u=[spline_coordinate], derivative=1))
         view_direction_displayed = view_direction[list(self.viewer.dims.displayed)]
 
         view_direction_transformed = tuple(self._transform_view_direction(view_direction_displayed))
 
         self.viewer.camera.set_view_direction(
             view_direction=view_direction_transformed, up_direction=self.up_direction
         )
@@ -294,15 +298,15 @@
         return self.view_direction_transformation.dot(view_direction)
 
     def start_spline_annotation(self):
         """Callback called when entering ANNOTATION mode."""
         self.spline_annotator_model.enabled = True
 
         # disable the key binding to switch to the next spline index
-        self.viewer.bind_key('n', None)
+        self.viewer.bind_key('n', None, overwrite=True)
 
     def stop_spline_annotation(self):
         """Callback called when exiting ANNOTATION mode."""
         self.spline_annotator_model.enabled = False
 
     def start_spline_exploration(self):
         """Setup up the exploration mode.
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee/visualization/lighting_control.py` & `napari-threedee-0.0.4/src/napari_threedee/visualization/lighting_control.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import List
 
 import numpy as np
 import napari
 
-from napari_threedee._backend.threedee_model import ThreeDeeModel
-from napari_threedee.utils.napari_utils import get_napari_visual
+from napari_threedee._backend.threedee_model import N3dComponent
+from napari_threedee.utils.napari_utils import (
+    get_napari_visual,
+    get_dims_displayed,
+)
 
 
-class LightingControl(ThreeDeeModel):
+class LightingControl(N3dComponent):
     def __init__(self, viewer: napari.Viewer):
         self._viewer = viewer
         self._selected_layers = []
         self._selected_layer_visuals = []
         self.enabled = False
 
     def set_layers(self, layers: List[napari.layers.Surface]):
@@ -48,15 +51,15 @@
     def _on_camera_change(self, event=None):
         if self.enabled is False:
             # only update lighting direction if enabled
             return
         view_direction = np.asarray(self._viewer.camera.view_direction)
 
         for layer, visual in zip(self.selected_layers, self.selected_layer_visuals):
-            dims_displayed = layer._dims_displayed
+            dims_displayed = get_dims_displayed(layer)
             layer_view_direction = np.asarray(layer._world_to_data_ray(view_direction))[dims_displayed]
             visual.node.shading_filter.light_dir = layer_view_direction[::-1]
 
     def _connect_events(self):
         self._viewer.camera.events.angles.connect(self._on_camera_change)
 
     def _disconnect_events(self):
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee.egg-info/PKG-INFO` & `napari-threedee-0.0.4/src/napari_threedee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-threedee
-Version: 0.0.3
+Version: 0.0.4
 Summary: A suite of useful tools based on 3D interactivity in napari
 Home-page: https://github.com/alisterburt/napari-threedee
 Author: napari team
 Author-email: napari-steering-council@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/napari-threedee/napari-threedee/issues
 Project-URL: Documentation, https://github.com/napari-threedee/napari-threedee#README.md
@@ -57,14 +57,17 @@
 
 
 To install latest development version :
 
     pip install git+https://github.com/alisterburt/napari-threedee.git
 
 ## Example applications
+
+See the full list of [example gallery scripts here on our website](https://napari-threedee.github.io/generated/gallery/).
+
 <table border="0">
 <tr><td>
 
 
 <img src="https://user-images.githubusercontent.com/1120672/173021751-9206de7d-5675-4aac-aa9e-8585457a7799.gif"
 width="300"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-threedee Version: 0.0.3 Summary: A suite of
+Metadata-Version: 2.1 Name: napari-threedee Version: 0.0.4 Summary: A suite of
 useful tools based on 3D interactivity in napari Home-page: https://github.com/
 alisterburt/napari-threedee Author: napari team Author-email: napari-steering-
 council@googlegroups.com License: BSD-3-Clause Project-URL: Bug Tracker, https:
 //github.com/napari-threedee/napari-threedee/issues Project-URL: Documentation,
 https://github.com/napari-threedee/napari-threedee#README.md Project-URL:
 Source Code, https://github.com/napari-threedee/napari-threedee Project-URL:
 User Support, https://github.com/napari-threedee/napari-threedee/issues
@@ -26,15 +26,17 @@
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-
 threedee)](https://napari-hub.org/plugins/napari-threedee) A suite of useful
 tools based on 3D interactivity in napari ---------------------------------
 - This [napari] plugin was generated with [Cookiecutter] using [@napari]'s
 [cookiecutter-napari-plugin] template.  ## Installation You can install
 `napari-threedee` via [pip]: pip install napari-threedee To install latest
 development version : pip install git+https://github.com/alisterburt/napari-
-threedee.git ## Example applications
+threedee.git ## Example applications See the full list of [example gallery
+scripts here on our website](https://napari-threedee.github.io/generated/
+gallery/).
 [https://user-                        [mesh lighting control](https://
 images.githubusercontent.com/1120672/ github.com/napari-threedee/napari-
 173021751-9206de7d-5675-4aac-aa9e-    threedee/blob/main/examples/plugin/
 8585457a7799.gif]                     mesh_headlight.py)
 [https://user-                        [annotate points on planes](https://
 images.githubusercontent.com/1120672/ github.com/napari-threedee/napari-
 173022286-2473b6b2-a20e-4514-88a4-    threedee/blob/main/examples/plugin/
```

### Comparing `napari-threedee-0.0.3/src/napari_threedee.egg-info/SOURCES.txt` & `napari-threedee-0.0.4/src/napari_threedee.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,58 +3,63 @@
 MANIFEST.in
 README.md
 mkdocs.yml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
-.github/workflows/build-and-deploy-docs.yml
-.github/workflows/test-docs-pr.yml
 .github/workflows/test_and_deploy.yml
 .napari-hub/config.yml
+docs/gallery_conf.py
 docs/index.md
 docs/API/geometry_utilities.md
 docs/API/napari_utilities.md
 docs/API/selection_utilities.md
 docs/annotations/io.md
 docs/annotations/point_spec.md
 docs/annotations/specifications.md
 docs/annotations/sphere_spec.md
 docs/annotations/spline_spec.md
 docs/dev_guides/core_concepts.md
 docs/dev_guides/manipulators.md
+docs/examples/README.md
+docs/examples/library/README.md
+docs/examples/library/camera_spline_library.py
+docs/examples/library/layer_manipulator_library.py
+docs/examples/library/mesh_headlight_library.py
+docs/examples/library/path_annotator_library.py
+docs/examples/library/point_annotator_library.py
+docs/examples/library/render_plane_manipulator_library.py
+docs/examples/library/sphere_annotator_library.py
+docs/examples/library/surface_annotator_library.py
+docs/examples/plugin/README.md
+docs/examples/plugin/camera_spline_plugin.py
+docs/examples/plugin/layer_manipulator_plugin.py
+docs/examples/plugin/mesh_headlight_plugin.py
+docs/examples/plugin/path_annotator_plugin.py
+docs/examples/plugin/point_annotator_plugin.py
+docs/examples/plugin/points_manipulator_plugin.py
+docs/examples/plugin/render_plane_manipulator_plugin.py
+docs/examples/plugin/sphere_annotator_plugin.py
+docs/examples/plugin/spline_annotator_plugin.py
+docs/examples/plugin/surface_annotator_plugin.py
 docs/getting_started/developers.md
 docs/getting_started/users.md
 docs/how_to/layer_manipulator.md
+docs/how_to/point_annotator.md
 docs/how_to/point_manipulator.md
 docs/how_to/render_plane_manipulator.md
+docs/how_to/sphere_annotator.md
+docs/how_to/spline_annotator.md
 docs/stylesheets/extra.css
 docs/tutorials/tutorials.md
-examples/empty_surface.py
-examples/library/camera_spline.py
-examples/library/layer_manipulator.py
-examples/library/mesh_headlight.py
-examples/library/point_annotator.py
-examples/library/render_plane_manipulator.py
-examples/library/sphere_annotator.py
-examples/library/spline_annotator.py
-examples/library/surface_annotator.py
-examples/plugin/camera_spline.py
-examples/plugin/layer_manipulator.py
-examples/plugin/mesh_headlight.py
-examples/plugin/plane_point_annotator.py
-examples/plugin/points_manipulator.py
-examples/plugin/render_plane_manipulator.py
-examples/plugin/spline_annotator.py
 src/napari_threedee/__init__.py
 src/napari_threedee/_version.py
 src/napari_threedee/conftest.py
 src/napari_threedee/dock_widgets.py
-src/napari_threedee/geometry_utils.py
-src/napari_threedee/mouse_callbacks.py
 src/napari_threedee/napari.yaml
 src/napari_threedee/vispy.py
 src/napari_threedee.egg-info/PKG-INFO
 src/napari_threedee.egg-info/SOURCES.txt
 src/napari_threedee.egg-info/dependency_links.txt
 src/napari_threedee.egg-info/entry_points.txt
 src/napari_threedee.egg-info/requires.txt
@@ -82,58 +87,78 @@
 src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py
 src/napari_threedee/_backend/manipulator/_tests/test_rotator.py
 src/napari_threedee/_backend/manipulator/_tests/test_translator.py
 src/napari_threedee/_tests/__init__.py
 src/napari_threedee/_tests/test_dock_widget.py
 src/napari_threedee/_tests/test_mouse_callbacks.py
 src/napari_threedee/annotators/__init__.py
-src/napari_threedee/annotators/point_annotator.py
-src/napari_threedee/annotators/sphere_annotator.py
-src/napari_threedee/annotators/spline_annotator.py
-src/napari_threedee/annotators/surface_annotator.py
+src/napari_threedee/annotators/base.py
+src/napari_threedee/annotators/constants.py
 src/napari_threedee/annotators/_qt/__init__.py
+src/napari_threedee/annotators/_qt/qt_path_annotator.py
 src/napari_threedee/annotators/_qt/qt_plane_point_annotator.py
 src/napari_threedee/annotators/_qt/qt_point_annotator.py
 src/napari_threedee/annotators/_qt/qt_sphere_annotator.py
-src/napari_threedee/annotators/_qt/qt_spline_annotator.py
 src/napari_threedee/annotators/_qt/qt_surface_annotator.py
+src/napari_threedee/annotators/_tests/__init__.py
 src/napari_threedee/annotators/_tests/conftest.py
-src/napari_threedee/annotators/_tests/test_plane_point_annotator.py
+src/napari_threedee/annotators/_tests/test_point_annotator.py
 src/napari_threedee/annotators/_tests/test_sphere_annotator.py
 src/napari_threedee/annotators/_tests/test_spline_annotator.py
-src/napari_threedee/annotators/io/__init__.py
-src/napari_threedee/annotators/io/_napari.py
-src/napari_threedee/annotators/io/constants.py
-src/napari_threedee/annotators/io/point.py
-src/napari_threedee/annotators/io/sphere.py
-src/napari_threedee/annotators/io/spline.py
-src/napari_threedee/annotators/io/_tests/conftest.py
-src/napari_threedee/annotators/io/_tests/test_napari.py
-src/napari_threedee/annotators/io/_tests/test_point.py
-src/napari_threedee/annotators/io/_tests/test_sphere.py
-src/napari_threedee/annotators/io/_tests/test_spline.py
+src/napari_threedee/annotators/paths/__init__.py
+src/napari_threedee/annotators/paths/annotator.py
+src/napari_threedee/annotators/paths/constants.py
+src/napari_threedee/annotators/paths/validation.py
+src/napari_threedee/annotators/points/__init__.py
+src/napari_threedee/annotators/points/annotator.py
+src/napari_threedee/annotators/points/constants.py
+src/napari_threedee/annotators/points/validation.py
+src/napari_threedee/annotators/points/_tests/__init__.py
+src/napari_threedee/annotators/points/_tests/test_data_model.py
+src/napari_threedee/annotators/spheres/__init__.py
+src/napari_threedee/annotators/spheres/annotator.py
+src/napari_threedee/annotators/spheres/constants.py
+src/napari_threedee/annotators/spheres/validation.py
+src/napari_threedee/annotators/spheres/_tests/__init__.py
+src/napari_threedee/annotators/spheres/_tests/test_data_model.py
+src/napari_threedee/annotators/surfaces/__init__.py
+src/napari_threedee/annotators/surfaces/annotator.py
+src/napari_threedee/annotators/surfaces/constants.py
+src/napari_threedee/annotators/surfaces/validation.py
+src/napari_threedee/annotators/surfaces/_tests/__init__.py
+src/napari_threedee/annotators/surfaces/_tests/test_data_model.py
+src/napari_threedee/data_models/__init__.py
+src/napari_threedee/data_models/paths.py
+src/napari_threedee/data_models/points.py
+src/napari_threedee/data_models/spheres.py
+src/napari_threedee/data_models/spline_sampler.py
+src/napari_threedee/data_models/surfaces.py
+src/napari_threedee/data_models/_tests/__init__.py
+src/napari_threedee/data_models/_tests/test_paths.py
 src/napari_threedee/manipulators/__init__.py
 src/napari_threedee/manipulators/base_manipulator.py
 src/napari_threedee/manipulators/layer_manipulator.py
 src/napari_threedee/manipulators/manipulator_utils.py
 src/napari_threedee/manipulators/point_manipulator.py
 src/napari_threedee/manipulators/render_plane_manipulator.py
 src/napari_threedee/manipulators/_qt/__init__.py
 src/napari_threedee/manipulators/_qt/qt_layer_manipulator.py
 src/napari_threedee/manipulators/_qt/qt_point_manipulator.py
 src/napari_threedee/manipulators/_qt/qt_render_plane_manipulator.py
 src/napari_threedee/manipulators/_tests/__init__.py
 src/napari_threedee/manipulators/_tests/test_manipulator_utils.py
 src/napari_threedee/utils/__init__.py
 src/napari_threedee/utils/geometry.py
+src/napari_threedee/utils/mouse_callbacks.py
 src/napari_threedee/utils/napari_utils.py
 src/napari_threedee/utils/selection_utils.py
 src/napari_threedee/utils/_tests/__init__.py
 src/napari_threedee/utils/_tests/test_geometry.py
 src/napari_threedee/visualization/__init__.py
 src/napari_threedee/visualization/camera_spline.py
 src/napari_threedee/visualization/lighting_control.py
 src/napari_threedee/visualization/_qt/__init__.py
 src/napari_threedee/visualization/_qt/qt_camera_spline.py
 src/napari_threedee/visualization/_qt/qt_lighting_control.py
 src/napari_threedee/visualization/_tests/__init__.py
-src/napari_threedee/visualization/_tests/test_camera_spline.py
+src/napari_threedee/visualization/_tests/test_camera_spline.py
+src/napari_threedee/visualization/_tests/test_lighting_control.py
```

### Comparing `napari-threedee-0.0.3/tox.ini` & `napari-threedee-0.0.4/tox.ini`

 * *Files identical despite different names*

