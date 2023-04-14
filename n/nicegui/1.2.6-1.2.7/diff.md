# Comparing `tmp/nicegui-1.2.6.tar.gz` & `tmp/nicegui-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicegui-1.2.6.tar", max compression
+gzip compressed data, was "nicegui-1.2.7.tar", max compression
```

## Comparing `nicegui-1.2.6.tar` & `nicegui-1.2.7.tar`

### file list

```diff
@@ -1,413 +1,416 @@
--rw-r--r--   0        0        0     1072 2023-04-05 06:49:29.128164 nicegui-1.2.6/LICENSE
--rw-r--r--   0        0        0     5645 2023-04-05 06:49:29.128164 nicegui-1.2.6/README.md
--rw-r--r--   0        0        0      288 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/__init__.py
--rw-r--r--   0        0        0     2978 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/app.py
--rw-r--r--   0        0        0     2056 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/background_tasks.py
--rw-r--r--   0        0        0     4599 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/binding.py
--rw-r--r--   0        0        0     5486 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/client.py
--rw-r--r--   0        0        0     3030 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/dependencies.py
--rw-r--r--   0        0        0      457 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/deprecation.py
--rw-r--r--   0        0        0    10475 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/element.py
--rw-r--r--   0        0        0     2958 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/aggrid.js
--rw-r--r--   0        0        0     2429 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/aggrid.py
--rw-r--r--   0        0        0      212 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/audio.js
--rw-r--r--   0        0        0     1487 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/audio.py
--rw-r--r--   0        0        0     1769 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/avatar.py
--rw-r--r--   0        0        0      904 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/badge.py
--rw-r--r--   0        0        0      727 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/button.py
--rw-r--r--   0        0        0      555 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/card.py
--rw-r--r--   0        0        0      990 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/chart.js
--rw-r--r--   0        0        0     4774 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/chart.py
--rw-r--r--   0        0        0      622 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/checkbox.py
--rw-r--r--   0        0        0     1075 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/choice_element.py
--rw-r--r--   0        0        0     1361 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/color_input.py
--rw-r--r--   0        0        0      915 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/color_picker.py
--rw-r--r--   0        0        0      317 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/colors.js
--rw-r--r--   0        0        0      928 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/colors.py
--rw-r--r--   0        0        0      269 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/column.py
--rw-r--r--   0        0        0     1217 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/date.py
--rw-r--r--   0        0        0     1441 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/dialog.py
--rw-r--r--   0        0        0      782 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/expansion.py
--rw-r--r--   0        0        0      543 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/html.py
--rw-r--r--   0        0        0      907 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/icon.py
--rw-r--r--   0        0        0      321 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/image.py
--rw-r--r--   0        0        0     2830 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/input.py
--rw-r--r--   0        0        0     2004 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/interactive_image.js
--rw-r--r--   0        0        0     2600 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/interactive_image.py
--rw-r--r--   0        0        0     2370 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/joystick.py
--rw-r--r--   0        0        0      622 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/joystick.vue
--rw-r--r--   0        0        0      792 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/keyboard.js
--rw-r--r--   0        0        0     2397 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/keyboard.py
--rw-r--r--   0        0        0     2202 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/knob.py
--rw-r--r--   0        0        0      274 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/label.py
--rw-r--r--   0        0        0     4673 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/lib/CSS2DRenderer.js
--rw-r--r--   0        0        0     8988 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/lib/CSS3DRenderer.js
--rw-r--r--   0        0        0    29354 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/lib/OrbitControls.js
--rw-r--r--   0        0        0    10612 2023-04-05 06:49:29.140164 nicegui-1.2.6/nicegui/elements/lib/STLLoader.js
--rw-r--r--   0        0        0  1570067 2023-04-05 06:49:29.148164 nicegui-1.2.6/nicegui/elements/lib/ag-grid-community.min.js
--rw-r--r--   0        0        0    49248 2023-04-05 06:49:29.148164 nicegui-1.2.6/nicegui/elements/lib/highcharts-3d.js
--rw-r--r--   0        0        0   106326 2023-04-05 06:49:29.148164 nicegui-1.2.6/nicegui/elements/lib/highcharts-more.js
--rw-r--r--   0        0        0   303628 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts.js
--rw-r--r--   0        0        0   130976 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/accessibility.js
--rw-r--r--   0        0        0    98853 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/annotations-advanced.js
--rw-r--r--   0        0        0    65315 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/annotations.js
--rw-r--r--   0        0        0     7406 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/arc-diagram.js
--rw-r--r--   0        0        0     1211 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/arrow-symbols.js
--rw-r--r--   0        0        0    43377 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/boost-canvas.js
--rw-r--r--   0        0        0    47427 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/boost.js
--rw-r--r--   0        0        0     5884 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/broken-axis.js
--rw-r--r--   0        0        0     4029 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/bullet.js
--rw-r--r--   0        0        0    12125 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/coloraxis.js
--rw-r--r--   0        0        0     1770 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/current-date-indicator.js
--rw-r--r--   0        0        0     5056 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/cylinder.js
--rw-r--r--   0        0        0    16507 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/data.js
--rw-r--r--   0        0        0    11360 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/datagrouping.js
--rw-r--r--   0        0        0    15051 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/debugger.js
--rw-r--r--   0        0        0     5733 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/dependency-wheel.js
--rw-r--r--   0        0        0     2652 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/dotplot.js
--rw-r--r--   0        0        0     4560 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/drag-panes.js
--rw-r--r--   0        0        0    17196 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/draggable-points.js
--rw-r--r--   0        0        0    18352 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/drilldown.js
--rw-r--r--   0        0        0     8141 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/dumbbell.js
--rw-r--r--   0        0        0    12791 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/export-data.js
--rw-r--r--   0        0        0    19692 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/exporting.js
--rw-r--r--   0        0        0     3491 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/full-screen.js
--rw-r--r--   0        0        0     5606 2023-04-05 06:49:29.152165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/funnel.js
--rw-r--r--   0        0        0    10167 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/funnel3d.js
--rw-r--r--   0        0        0   112925 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/gantt.js
--rw-r--r--   0        0        0    11206 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/grid-axis.js
--rw-r--r--   0        0        0    19983 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/heatmap.js
--rw-r--r--   0        0        0     3869 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/heikinashi.js
--rw-r--r--   0        0        0     6199 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/histogram-bellcurve.js
--rw-r--r--   0        0        0     3983 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/hollowcandlestick.js
--rw-r--r--   0        0        0     5636 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/item-series.js
--rw-r--r--   0        0        0     3063 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/lollipop.js
--rw-r--r--   0        0        0    17955 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/marker-clusters.js
--rw-r--r--   0        0        0    27952 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/networkgraph.js
--rw-r--r--   0        0        0     1947 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/no-data-to-display.js
--rw-r--r--   0        0        0     9627 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/offline-exporting.js
--rw-r--r--   0        0        0     3042 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/oldie-polyfills.js
--rw-r--r--   0        0        0    14679 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/oldie.js
--rw-r--r--   0        0        0     8553 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/organization.js
--rw-r--r--   0        0        0      741 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/overlapping-datalabels.js
--rw-r--r--   0        0        0     5234 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/parallel-coordinates.js
--rw-r--r--   0        0        0     3180 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/pareto.js
--rw-r--r--   0        0        0    15251 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/pathfinder.js
--rw-r--r--   0        0        0     7026 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/pattern-fill.js
--rw-r--r--   0        0        0     2151 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/price-indicator.js
--rw-r--r--   0        0        0     1640 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/pyramid3d.js
--rw-r--r--   0        0        0    16340 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/sankey.js
--rw-r--r--   0        0        0     9424 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/series-label.js
--rw-r--r--   0        0        0     3792 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/series-on-point.js
--rw-r--r--   0        0        0     4944 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/solid-gauge.js
--rw-r--r--   0        0        0    29682 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/sonification.js
--rw-r--r--   0        0        0     1837 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/static-scale.js
--rw-r--r--   0        0        0    55798 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/stock-tools.js
--rw-r--r--   0        0        0   108215 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/stock.js
--rw-r--r--   0        0        0     1698 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/streamgraph.js
--rw-r--r--   0        0        0    37904 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/sunburst.js
--rw-r--r--   0        0        0     8257 2023-04-05 06:49:29.156165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/tilemap.js
--rw-r--r--   0        0        0     8804 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/timeline.js
--rw-r--r--   0        0        0    18184 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/treegraph.js
--rw-r--r--   0        0        0    28748 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/treegrid.js
--rw-r--r--   0        0        0    27334 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/treemap.js
--rw-r--r--   0        0        0     4254 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/variable-pie.js
--rw-r--r--   0        0        0     5739 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/variwide.js
--rw-r--r--   0        0        0     3265 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/vector.js
--rw-r--r--   0        0        0    15068 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/venn.js
--rw-r--r--   0        0        0     7390 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/windbarb.js
--rw-r--r--   0        0        0    11231 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/wordcloud.js
--rw-r--r--   0        0        0     8508 2023-04-05 06:49:29.160165 nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/xrange.js
--rw-r--r--   0        0        0  2777841 2023-04-05 06:49:29.172165 nicegui-1.2.6/nicegui/elements/lib/mermaid.min.js
--rw-r--r--   0        0        0    20547 2023-04-05 06:49:29.176165 nicegui-1.2.6/nicegui/elements/lib/nipplejs.min.js
--rw-r--r--   0        0        0  3579005 2023-04-05 06:49:29.192165 nicegui-1.2.6/nicegui/elements/lib/plotly.min.js
--rw-r--r--   0        0        0   613740 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/lib/three.min.js
--rw-r--r--   0        0        0    10633 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/lib/tween.umd.min.js
--rw-r--r--   0        0        0     2298 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/line_plot.py
--rw-r--r--   0        0        0     1231 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/link.py
--rw-r--r--   0        0        0      997 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/log.js
--rw-r--r--   0        0        0     1102 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/log.py
--rw-r--r--   0        0        0      933 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/markdown.js
--rw-r--r--   0        0        0     2701 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/markdown.py
--rw-r--r--   0        0        0     1593 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/menu.py
--rw-r--r--   0        0        0      274 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/mermaid.js
--rw-r--r--   0        0        0      861 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/mermaid.py
--rw-r--r--   0        0        0     3327 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/mixins/content_element.py
--rw-r--r--   0        0        0     3131 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/mixins/filter_element.py
--rw-r--r--   0        0        0     3055 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/mixins/source_element.py
--rw-r--r--   0        0        0     3058 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/mixins/text_element.py
--rw-r--r--   0        0        0     4204 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/mixins/value_element.py
--rw-r--r--   0        0        0     3850 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/mixins/visibility.py
--rw-r--r--   0        0        0     2406 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/number.py
--rw-r--r--   0        0        0     2047 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/plotly.py
--rw-r--r--   0        0        0     2622 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/plotly.vue
--rw-r--r--   0        0        0     2109 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/progress.py
--rw-r--r--   0        0        0     1471 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/pyplot.py
--rw-r--r--   0        0        0     1158 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/query.js
--rw-r--r--   0        0        0     2751 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/query.py
--rw-r--r--   0        0        0     1021 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/radio.py
--rw-r--r--   0        0        0      257 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/row.py
--rw-r--r--   0        0        0    13006 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/scene.js
--rw-r--r--   0        0        0     5631 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/scene.py
--rw-r--r--   0        0        0     3894 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/scene_object3d.py
--rw-r--r--   0        0        0     5066 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/scene_objects.py
--rw-r--r--   0        0        0      924 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/select.js
--rw-r--r--   0        0        0     2065 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/select.py
--rw-r--r--   0        0        0      280 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/separator.py
--rw-r--r--   0        0        0      852 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/slider.py
--rw-r--r--   0        0        0     1286 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/spinner.py
--rw-r--r--   0        0        0     1704 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/splitter.py
--rw-r--r--   0        0        0      634 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/switch.py
--rw-r--r--   0        0        0     3281 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/table.py
--rw-r--r--   0        0        0     2867 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/tabs.py
--rw-r--r--   0        0        0     1125 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/textarea.py
--rw-r--r--   0        0        0      813 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/time.py
--rw-r--r--   0        0        0     1019 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/toggle.py
--rw-r--r--   0        0        0      335 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/tooltip.py
--rw-r--r--   0        0        0     2634 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/tree.py
--rw-r--r--   0        0        0     1849 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/upload.py
--rw-r--r--   0        0        0      212 2023-04-05 06:49:29.196165 nicegui-1.2.6/nicegui/elements/video.js
--rw-r--r--   0        0        0     1487 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/elements/video.py
--rw-r--r--   0        0        0     1046 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/error.py
--rw-r--r--   0        0        0      947 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/event_listener.py
--rw-r--r--   0        0        0     6093 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/events.py
--rw-r--r--   0        0        0     1078 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/favicon.py
--rw-r--r--   0        0        0      203 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/functions/html.py
--rw-r--r--   0        0        0     1230 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/functions/javascript.py
--rw-r--r--   0        0        0     1408 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/functions/notify.py
--rw-r--r--   0        0        0      669 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/functions/open.py
--rw-r--r--   0        0        0     3992 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/functions/timer.py
--rw-r--r--   0        0        0      126 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/functions/update.py
--rw-r--r--   0        0        0     2262 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/globals.py
--rw-r--r--   0        0        0     2857 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/helpers.py
--rw-r--r--   0        0        0      387 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/ids.py
--rw-r--r--   0        0        0      788 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/json/__init__.py
--rw-r--r--   0        0        0     1627 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/json/builtin_wrapper.py
--rw-r--r--   0        0        0     1758 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/json/orjson_wrapper.py
--rw-r--r--   0        0        0      220 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/native.py
--rw-r--r--   0        0        0     1902 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/native_mode.py
--rw-r--r--   0        0        0     6390 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/nicegui.py
--rw-r--r--   0        0        0     1609 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/outbox.py
--rw-r--r--   0        0        0     4217 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/page.py
--rw-r--r--   0        0        0     8064 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/page_layout.py
--rw-r--r--   0        0        0     5742 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/run.py
--rw-r--r--   0        0        0      895 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/run_with.py
--rw-r--r--   0        0        0      611 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/slot.py
--rw-r--r--   0        0        0    15086 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/favicon.ico
--rw-r--r--   0        0        0      756 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxEIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0    10144 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxFIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0     7668 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxGIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0     3360 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxHIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0    10972 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxIIzIXKMny.woff2
--rw-r--r--   0        0        0     4960 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxLIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0     6384 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxMIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0     6632 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    11072 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2
--rw-r--r--   0        0        0     4796 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0      768 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10352 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     7676 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     3472 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     6480 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    11160 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2
--rw-r--r--   0        0        0     4928 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0      756 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10412 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     7840 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     3448 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     6620 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    11040 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2
--rw-r--r--   0        0        0     4796 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0      756 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10256 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     7676 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     3468 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     6612 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfABc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10992 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc4AMP6lQ.woff2
--rw-r--r--   0        0        0     4756 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0      772 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCBc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10188 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCRc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     7608 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfChc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     3388 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     4864 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0    11028 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2
--rw-r--r--   0        0        0     6460 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0    10352 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2
--rw-r--r--   0        0        0     7736 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0     3496 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0      748 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0   128616 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0        0        0    11484 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/fonts.css
--rw-r--r--   0        0        0     1913 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/nicegui.css
--rw-r--r--   0        0        0   198973 2023-04-05 06:49:29.200165 nicegui-1.2.6/nicegui/static/quasar.prod.css
--rw-r--r--   0        0        0   509452 2023-04-05 06:49:29.204166 nicegui-1.2.6/nicegui/static/quasar.umd.prod.js
--rw-r--r--   0        0        0     1510 2023-04-05 06:49:29.204166 nicegui-1.2.6/nicegui/static/sad_face.svg
--rw-r--r--   0        0        0    45896 2023-04-05 06:49:29.204166 nicegui-1.2.6/nicegui/static/socket.io.min.js
--rw-r--r--   0        0        0   350399 2023-04-05 06:49:29.204166 nicegui-1.2.6/nicegui/static/tailwindcss.min.js
--rw-r--r--   0        0        0   128872 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/static/vue.global.prod.js
--rw-r--r--   0        0        0   107302 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/static/vue.min.js
--rw-r--r--   0        0        0    44035 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind.py
--rw-r--r--   0        0        0     4232 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/accent_color.py
--rw-r--r--   0        0        0      191 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/align_content.py
--rw-r--r--   0        0        0      132 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/align_items.py
--rw-r--r--   0        0        0      143 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/align_self.py
--rw-r--r--   0        0        0      125 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/animation.py
--rw-r--r--   0        0        0       75 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/appearance.py
--rw-r--r--   0        0        0      103 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/aspect_ratio.py
--rw-r--r--   0        0        0      147 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_blur.py
--rw-r--r--   0        0        0      186 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_brightness.py
--rw-r--r--   0        0        0      142 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_contrast.py
--rw-r--r--   0        0        0       87 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_grayscale.py
--rw-r--r--   0        0        0      130 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_hue_rotate.py
--rw-r--r--   0        0        0       84 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_invert.py
--rw-r--r--   0        0        0      217 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_opacity.py
--rw-r--r--   0        0        0      121 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_saturate.py
--rw-r--r--   0        0        0       83 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/backdrop_sepia.py
--rw-r--r--   0        0        0      113 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_attachment.py
--rw-r--r--   0        0        0      328 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_blend_mode.py
--rw-r--r--   0        0        0      123 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_clip.py
--rw-r--r--   0        0        0     4224 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_color.py
--rw-r--r--   0        0        0      252 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_image.py
--rw-r--r--   0        0        0      113 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_origin.py
--rw-r--r--   0        0        0      207 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_position.py
--rw-r--r--   0        0        0      172 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_repeat.py
--rw-r--r--   0        0        0      107 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/background_size.py
--rw-r--r--   0        0        0      139 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/blur.py
--rw-r--r--   0        0        0       99 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/border_collapse.py
--rw-r--r--   0        0        0    41420 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/border_color.py
--rw-r--r--   0        0        0     1785 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/border_radius.py
--rw-r--r--   0        0        0     1238 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/border_spacing.py
--rw-r--r--   0        0        0      145 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/border_style.py
--rw-r--r--   0        0        0      532 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/border_width.py
--rw-r--r--   0        0        0       97 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/box_decoration_break.py
--rw-r--r--   0        0        0      146 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/box_shadow.py
--rw-r--r--   0        0        0     4223 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/box_shadow_color.py
--rw-r--r--   0        0        0       91 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/box_sizing.py
--rw-r--r--   0        0        0      168 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/break_after.py
--rw-r--r--   0        0        0      169 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/break_before.py
--rw-r--r--   0        0        0      127 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/break_inside.py
--rw-r--r--   0        0        0      178 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/brightness.py
--rw-r--r--   0        0        0       89 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/caption_side.py
--rw-r--r--   0        0        0     4219 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/caret_color.py
--rw-r--r--   0        0        0      107 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/clear.py
--rw-r--r--   0        0        0      321 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/columns.py
--rw-r--r--   0        0        0       72 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/content.py
--rw-r--r--   0        0        0      134 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/contrast.py
--rw-r--r--   0        0        0      623 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/cursor.py
--rw-r--r--   0        0        0      443 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/display.py
--rw-r--r--   0        0        0     4220 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/divide_color.py
--rw-r--r--   0        0        0      131 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/divide_style.py
--rw-r--r--   0        0        0      204 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/divide_width.py
--rw-r--r--   0        0        0      134 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/drop_shadow.py
--rw-r--r--   0        0        0     4225 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/fill.py
--rw-r--r--   0        0        0      105 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/flex.py
--rw-r--r--   0        0        0      729 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/flex_basis.py
--rw-r--r--   0        0        0      126 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/flex_direction.py
--rw-r--r--   0        0        0       78 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/flex_grow.py
--rw-r--r--   0        0        0       80 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/flex_shrink.py
--rw-r--r--   0        0        0      107 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/flex_wrap.py
--rw-r--r--   0        0        0       96 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/floats.py
--rw-r--r--   0        0        0      100 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/font_family.py
--rw-r--r--   0        0        0      201 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/font_size.py
--rw-r--r--   0        0        0      113 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/font_smoothing.py
--rw-r--r--   0        0        0       94 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/font_style.py
--rw-r--r--   0        0        0      261 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/font_variant_numeric.py
--rw-r--r--   0        0        0      192 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/font_weight.py
--rw-r--r--   0        0        0     1228 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/gap.py
--rw-r--r--   0        0        0    16445 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/gradient_color_stops.py
--rw-r--r--   0        0        0       79 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/grayscale.py
--rw-r--r--   0        0        0      112 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/grid_auto_columns.py
--rw-r--r--   0        0        0      134 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/grid_auto_flow.py
--rw-r--r--   0        0        0      109 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/grid_auto_rows.py
--rw-r--r--   0        0        0      677 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/grid_column_start_end.py
--rw-r--r--   0        0        0      411 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/grid_row_start_end.py
--rw-r--r--   0        0        0      195 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/grid_template_columns.py
--rw-r--r--   0        0        0      135 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/grid_template_rows.py
--rw-r--r--   0        0        0      639 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/height.py
--rw-r--r--   0        0        0      122 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/hue_rotate.py
--rw-r--r--   0        0        0       98 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/hyphens.py
--rw-r--r--   0        0        0       76 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/invert.py
--rw-r--r--   0        0        0       99 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/isolation.py
--rw-r--r--   0        0        0      177 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/justify_content.py
--rw-r--r--   0        0        0      118 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/justify_items.py
--rw-r--r--   0        0        0      129 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/justify_self.py
--rw-r--r--   0        0        0      147 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/letter_spacing.py
--rw-r--r--   0        0        0      128 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/line_clamp.py
--rw-r--r--   0        0        0      215 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/line_height.py
--rw-r--r--   0        0        0       79 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/list_style_image.py
--rw-r--r--   0        0        0       99 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/list_style_position.py
--rw-r--r--   0        0        0      105 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/list_style_type.py
--rw-r--r--   0        0        0     4199 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/margin.py
--rw-r--r--   0        0        0      477 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/max_height.py
--rw-r--r--   0        0        0      342 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/max_width.py
--rw-r--r--   0        0        0      130 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/min_height.py
--rw-r--r--   0        0        0      115 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/min_width.py
--rw-r--r--   0        0        0      341 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/mix_blend_mode.py
--rw-r--r--   0        0        0      132 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/object_fit.py
--rw-r--r--   0        0        0      203 2023-04-05 06:49:29.208166 nicegui-1.2.6/nicegui/tailwind_types/object_position.py
--rw-r--r--   0        0        0      209 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/opacity.py
--rw-r--r--   0        0        0      206 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/order.py
--rw-r--r--   0        0        0     4221 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/outline_color.py
--rw-r--r--   0        0        0      111 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/outline_offset.py
--rw-r--r--   0        0        0      127 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/outline_style.py
--rw-r--r--   0        0        0      110 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/outline_width.py
--rw-r--r--   0        0        0      282 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/overflow.py
--rw-r--r--   0        0        0      200 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/overscroll_behavior.py
--rw-r--r--   0        0        0     4066 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/padding.py
--rw-r--r--   0        0        0      177 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/place_content.py
--rw-r--r--   0        0        0      132 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/place_items.py
--rw-r--r--   0        0        0      127 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/place_self.py
--rw-r--r--   0        0        0       90 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/pointer_events.py
--rw-r--r--   0        0        0      134 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/position.py
--rw-r--r--   0        0        0       97 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/resize.py
--rw-r--r--   0        0        0     4218 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/ring_color.py
--rw-r--r--   0        0        0     4224 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/ring_offset_color.py
--rw-r--r--   0        0        0      113 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/ring_offset_width.py
--rw-r--r--   0        0        0      128 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/ring_width.py
--rw-r--r--   0        0        0      145 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/rotate.py
--rw-r--r--   0        0        0      113 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/saturate.py
--rw-r--r--   0        0        0      410 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/scale.py
--rw-r--r--   0        0        0      100 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/screen_readers.py
--rw-r--r--   0        0        0       93 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/scroll_behavior.py
--rw-r--r--   0        0        0     4071 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/scroll_margin.py
--rw-r--r--   0        0        0     4072 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/scroll_padding.py
--rw-r--r--   0        0        0      124 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/scroll_snap_align.py
--rw-r--r--   0        0        0       95 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/scroll_snap_stop.py
--rw-r--r--   0        0        0      143 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/scroll_snap_type.py
--rw-r--r--   0        0        0       75 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/sepia.py
--rw-r--r--   0        0        0      191 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/skew.py
--rw-r--r--   0        0        0      927 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/space_between.py
--rw-r--r--   0        0        0     4227 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/stroke.py
--rw-r--r--   0        0        0       91 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/stroke_width.py
--rw-r--r--   0        0        0       89 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/table_layout.py
--rw-r--r--   0        0        0      140 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_align.py
--rw-r--r--   0        0        0     4218 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_color.py
--rw-r--r--   0        0        0      140 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_decoration.py
--rw-r--r--   0        0        0     4228 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_decoration_color.py
--rw-r--r--   0        0        0      139 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_decoration_style.py
--rw-r--r--   0        0        0      150 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_decoration_thickness.py
--rw-r--r--   0        0        0      407 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_indent.py
--rw-r--r--   0        0        0      119 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_overflow.py
--rw-r--r--   0        0        0      137 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_transform.py
--rw-r--r--   0        0        0      129 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/text_underline_offset.py
--rw-r--r--   0        0        0     6299 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/top_right_bottom_left.py
--rw-r--r--   0        0        0      215 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/touch_action.py
--rw-r--r--   0        0        0      204 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/transform_origin.py
--rw-r--r--   0        0        0      165 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/transition_delay.py
--rw-r--r--   0        0        0      168 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/transition_duration.py
--rw-r--r--   0        0        0      162 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/transition_property.py
--rw-r--r--   0        0        0      126 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/transition_timing_function.py
--rw-r--r--   0        0        0     1074 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/translate.py
--rw-r--r--   0        0        0      110 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/user_select.py
--rw-r--r--   0        0        0      180 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/vertical_align.py
--rw-r--r--   0        0        0      111 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/visibility.py
--rw-r--r--   0        0        0      154 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/whitespace.py
--rw-r--r--   0        0        0      772 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/width.py
--rw-r--r--   0        0        0      122 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/will_change.py
--rw-r--r--   0        0        0      112 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/word_break.py
--rw-r--r--   0        0        0      130 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/tailwind_types/z_index.py
--rw-r--r--   0        0        0     6595 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/templates/index.html
--rw-r--r--   0        0        0     3717 2023-04-05 06:49:29.212166 nicegui-1.2.6/nicegui/ui.py
--rw-r--r--   0        0        0     1542 2023-04-05 06:49:38.644309 nicegui-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     7355 1970-01-01 00:00:00.000000 nicegui-1.2.6/setup.py
--rw-r--r--   0        0        0     7257 1970-01-01 00:00:00.000000 nicegui-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-14 14:12:00.674256 nicegui-1.2.7/LICENSE
+-rw-r--r--   0        0        0     5645 2023-04-14 14:12:00.674256 nicegui-1.2.7/README.md
+-rw-r--r--   0        0        0      288 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/__init__.py
+-rw-r--r--   0        0        0     3118 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/app.py
+-rw-r--r--   0        0        0     2056 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/background_tasks.py
+-rw-r--r--   0        0        0     4599 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/binding.py
+-rw-r--r--   0        0        0     6050 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/client.py
+-rw-r--r--   0        0        0     1291 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/colors.py
+-rw-r--r--   0        0        0     3030 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/dependencies.py
+-rw-r--r--   0        0        0      457 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/deprecation.py
+-rw-r--r--   0        0        0    11039 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/element.py
+-rw-r--r--   0        0        0     2958 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/aggrid.js
+-rw-r--r--   0        0        0     2975 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/aggrid.py
+-rw-r--r--   0        0        0      212 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/audio.js
+-rw-r--r--   0        0        0     1487 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/audio.py
+-rw-r--r--   0        0        0     1827 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/avatar.py
+-rw-r--r--   0        0        0     1095 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/badge.py
+-rw-r--r--   0        0        0     1454 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/button.py
+-rw-r--r--   0        0        0     1124 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/card.py
+-rw-r--r--   0        0        0      990 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/chart.js
+-rw-r--r--   0        0        0     4840 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/chart.py
+-rw-r--r--   0        0        0      622 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/checkbox.py
+-rw-r--r--   0        0        0     1075 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/choice_element.py
+-rw-r--r--   0        0        0     1361 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/color_input.py
+-rw-r--r--   0        0        0      915 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/color_picker.py
+-rw-r--r--   0        0        0      335 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/colors.js
+-rw-r--r--   0        0        0     1062 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/colors.py
+-rw-r--r--   0        0        0      269 2023-04-14 14:12:00.686256 nicegui-1.2.7/nicegui/elements/column.py
+-rw-r--r--   0        0        0     1216 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/date.py
+-rw-r--r--   0        0        0     1441 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/dialog.py
+-rw-r--r--   0        0        0      782 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/expansion.py
+-rw-r--r--   0        0        0      543 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/html.py
+-rw-r--r--   0        0        0      947 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/icon.py
+-rw-r--r--   0        0        0      321 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/image.py
+-rw-r--r--   0        0        0     2830 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/input.py
+-rw-r--r--   0        0        0     2004 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/interactive_image.js
+-rw-r--r--   0        0        0     2600 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/interactive_image.py
+-rw-r--r--   0        0        0     2370 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/joystick.py
+-rw-r--r--   0        0        0      622 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/joystick.vue
+-rw-r--r--   0        0        0      792 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/keyboard.js
+-rw-r--r--   0        0        0     2397 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/keyboard.py
+-rw-r--r--   0        0        0     2246 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/knob.py
+-rw-r--r--   0        0        0      274 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/label.py
+-rw-r--r--   0        0        0     4673 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/lib/CSS2DRenderer.js
+-rw-r--r--   0        0        0     8988 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/lib/CSS3DRenderer.js
+-rw-r--r--   0        0        0    29354 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/lib/OrbitControls.js
+-rw-r--r--   0        0        0    10612 2023-04-14 14:12:00.690256 nicegui-1.2.7/nicegui/elements/lib/STLLoader.js
+-rw-r--r--   0        0        0  1570067 2023-04-14 14:12:00.694256 nicegui-1.2.7/nicegui/elements/lib/ag-grid-community.min.js
+-rw-r--r--   0        0        0    49248 2023-04-14 14:12:00.698256 nicegui-1.2.7/nicegui/elements/lib/highcharts-3d.js
+-rw-r--r--   0        0        0   106326 2023-04-14 14:12:00.698256 nicegui-1.2.7/nicegui/elements/lib/highcharts-more.js
+-rw-r--r--   0        0        0   303628 2023-04-14 14:12:00.698256 nicegui-1.2.7/nicegui/elements/lib/highcharts.js
+-rw-r--r--   0        0        0   130976 2023-04-14 14:12:00.698256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/accessibility.js
+-rw-r--r--   0        0        0    98853 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/annotations-advanced.js
+-rw-r--r--   0        0        0    65315 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/annotations.js
+-rw-r--r--   0        0        0     7406 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/arc-diagram.js
+-rw-r--r--   0        0        0     1211 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/arrow-symbols.js
+-rw-r--r--   0        0        0    43377 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/boost-canvas.js
+-rw-r--r--   0        0        0    47427 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/boost.js
+-rw-r--r--   0        0        0     5884 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/broken-axis.js
+-rw-r--r--   0        0        0     4029 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/bullet.js
+-rw-r--r--   0        0        0    12125 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/coloraxis.js
+-rw-r--r--   0        0        0     1770 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/current-date-indicator.js
+-rw-r--r--   0        0        0     5056 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/cylinder.js
+-rw-r--r--   0        0        0    16507 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/data.js
+-rw-r--r--   0        0        0    11360 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/datagrouping.js
+-rw-r--r--   0        0        0    15051 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/debugger.js
+-rw-r--r--   0        0        0     5733 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/dependency-wheel.js
+-rw-r--r--   0        0        0     2652 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/dotplot.js
+-rw-r--r--   0        0        0     4560 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/drag-panes.js
+-rw-r--r--   0        0        0    17196 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/draggable-points.js
+-rw-r--r--   0        0        0    18352 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/drilldown.js
+-rw-r--r--   0        0        0     8141 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/dumbbell.js
+-rw-r--r--   0        0        0    12791 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/export-data.js
+-rw-r--r--   0        0        0    19692 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/exporting.js
+-rw-r--r--   0        0        0     3491 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/full-screen.js
+-rw-r--r--   0        0        0     5606 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/funnel.js
+-rw-r--r--   0        0        0    10167 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/funnel3d.js
+-rw-r--r--   0        0        0   112925 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/gantt.js
+-rw-r--r--   0        0        0    11206 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/grid-axis.js
+-rw-r--r--   0        0        0    19983 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/heatmap.js
+-rw-r--r--   0        0        0     3869 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/heikinashi.js
+-rw-r--r--   0        0        0     6199 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/histogram-bellcurve.js
+-rw-r--r--   0        0        0     3983 2023-04-14 14:12:00.702256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/hollowcandlestick.js
+-rw-r--r--   0        0        0     5636 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/item-series.js
+-rw-r--r--   0        0        0     3063 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/lollipop.js
+-rw-r--r--   0        0        0    17955 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/marker-clusters.js
+-rw-r--r--   0        0        0    27952 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/networkgraph.js
+-rw-r--r--   0        0        0     1947 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/no-data-to-display.js
+-rw-r--r--   0        0        0     9627 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/offline-exporting.js
+-rw-r--r--   0        0        0     3042 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/oldie-polyfills.js
+-rw-r--r--   0        0        0    14679 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/oldie.js
+-rw-r--r--   0        0        0     8553 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/organization.js
+-rw-r--r--   0        0        0      741 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/overlapping-datalabels.js
+-rw-r--r--   0        0        0     5234 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/parallel-coordinates.js
+-rw-r--r--   0        0        0     3180 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/pareto.js
+-rw-r--r--   0        0        0    15251 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/pathfinder.js
+-rw-r--r--   0        0        0     7026 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/pattern-fill.js
+-rw-r--r--   0        0        0     2151 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/price-indicator.js
+-rw-r--r--   0        0        0     1640 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/pyramid3d.js
+-rw-r--r--   0        0        0    16340 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/sankey.js
+-rw-r--r--   0        0        0     9424 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/series-label.js
+-rw-r--r--   0        0        0     3792 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/series-on-point.js
+-rw-r--r--   0        0        0     4944 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/solid-gauge.js
+-rw-r--r--   0        0        0    29682 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/sonification.js
+-rw-r--r--   0        0        0     1837 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/static-scale.js
+-rw-r--r--   0        0        0    55798 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/stock-tools.js
+-rw-r--r--   0        0        0   108215 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/stock.js
+-rw-r--r--   0        0        0     1698 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/streamgraph.js
+-rw-r--r--   0        0        0    37904 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/sunburst.js
+-rw-r--r--   0        0        0     8257 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/tilemap.js
+-rw-r--r--   0        0        0     8804 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/timeline.js
+-rw-r--r--   0        0        0    18184 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/treegraph.js
+-rw-r--r--   0        0        0    28748 2023-04-14 14:12:00.706256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/treegrid.js
+-rw-r--r--   0        0        0    27334 2023-04-14 14:12:00.710256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/treemap.js
+-rw-r--r--   0        0        0     4254 2023-04-14 14:12:00.710256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/variable-pie.js
+-rw-r--r--   0        0        0     5739 2023-04-14 14:12:00.710256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/variwide.js
+-rw-r--r--   0        0        0     3265 2023-04-14 14:12:00.710256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/vector.js
+-rw-r--r--   0        0        0    15068 2023-04-14 14:12:00.710256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/venn.js
+-rw-r--r--   0        0        0     7390 2023-04-14 14:12:00.710256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/windbarb.js
+-rw-r--r--   0        0        0    11231 2023-04-14 14:12:00.710256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/wordcloud.js
+-rw-r--r--   0        0        0     8508 2023-04-14 14:12:00.710256 nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/xrange.js
+-rw-r--r--   0        0        0  2777841 2023-04-14 14:12:00.726256 nicegui-1.2.7/nicegui/elements/lib/mermaid.min.js
+-rw-r--r--   0        0        0    20547 2023-04-14 14:12:00.726256 nicegui-1.2.7/nicegui/elements/lib/nipplejs.min.js
+-rw-r--r--   0        0        0  3579005 2023-04-14 14:12:00.746256 nicegui-1.2.7/nicegui/elements/lib/plotly.min.js
+-rw-r--r--   0        0        0   613740 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/lib/three.min.js
+-rw-r--r--   0        0        0    10633 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/lib/tween.umd.min.js
+-rw-r--r--   0        0        0     2298 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/line_plot.py
+-rw-r--r--   0        0        0      439 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/link.js
+-rw-r--r--   0        0        0     1329 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/link.py
+-rw-r--r--   0        0        0      997 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/log.js
+-rw-r--r--   0        0        0     1168 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/log.py
+-rw-r--r--   0        0        0      933 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/markdown.js
+-rw-r--r--   0        0        0     2701 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/markdown.py
+-rw-r--r--   0        0        0     1593 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/menu.py
+-rw-r--r--   0        0        0      274 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/mermaid.js
+-rw-r--r--   0        0        0      861 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/mermaid.py
+-rw-r--r--   0        0        0     3327 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/mixins/content_element.py
+-rw-r--r--   0        0        0     3131 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/mixins/filter_element.py
+-rw-r--r--   0        0        0     3055 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/mixins/source_element.py
+-rw-r--r--   0        0        0     3058 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/mixins/text_element.py
+-rw-r--r--   0        0        0     4204 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/mixins/value_element.py
+-rw-r--r--   0        0        0     3850 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/mixins/visibility.py
+-rw-r--r--   0        0        0     2475 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/number.py
+-rw-r--r--   0        0        0     2047 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/plotly.py
+-rw-r--r--   0        0        0     2622 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/plotly.vue
+-rw-r--r--   0        0        0     2741 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/progress.py
+-rw-r--r--   0        0        0     1471 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/pyplot.py
+-rw-r--r--   0        0        0     1158 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/query.js
+-rw-r--r--   0        0        0     2751 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/query.py
+-rw-r--r--   0        0        0     1021 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/radio.py
+-rw-r--r--   0        0        0      257 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/row.py
+-rw-r--r--   0        0        0    13006 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/scene.js
+-rw-r--r--   0        0        0     5765 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/scene.py
+-rw-r--r--   0        0        0     4047 2023-04-14 14:12:00.750256 nicegui-1.2.7/nicegui/elements/scene_object3d.py
+-rw-r--r--   0        0        0     5066 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/scene_objects.py
+-rw-r--r--   0        0        0      924 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/select.js
+-rw-r--r--   0        0        0     2065 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/select.py
+-rw-r--r--   0        0        0      280 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/separator.py
+-rw-r--r--   0        0        0      852 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/slider.py
+-rw-r--r--   0        0        0     1461 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/spinner.py
+-rw-r--r--   0        0        0     1704 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/splitter.py
+-rw-r--r--   0        0        0      634 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/switch.py
+-rw-r--r--   0        0        0     3281 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/table.py
+-rw-r--r--   0        0        0     2867 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/tabs.py
+-rw-r--r--   0        0        0     1125 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/textarea.py
+-rw-r--r--   0        0        0      813 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/time.py
+-rw-r--r--   0        0        0     1019 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/toggle.py
+-rw-r--r--   0        0        0      335 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/tooltip.py
+-rw-r--r--   0        0        0     2634 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/tree.py
+-rw-r--r--   0        0        0     2827 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/upload.py
+-rw-r--r--   0        0        0      212 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/video.js
+-rw-r--r--   0        0        0     1487 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/elements/video.py
+-rw-r--r--   0        0        0     1046 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/error.py
+-rw-r--r--   0        0        0     1102 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/event_listener.py
+-rw-r--r--   0        0        0     6093 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/events.py
+-rw-r--r--   0        0        0     1078 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/favicon.py
+-rw-r--r--   0        0        0      384 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/functions/download.py
+-rw-r--r--   0        0        0      203 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/functions/html.py
+-rw-r--r--   0        0        0     1230 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/functions/javascript.py
+-rw-r--r--   0        0        0     1408 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/functions/notify.py
+-rw-r--r--   0        0        0      669 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/functions/open.py
+-rw-r--r--   0        0        0     3992 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/functions/timer.py
+-rw-r--r--   0        0        0      126 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/functions/update.py
+-rw-r--r--   0        0        0     2262 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/globals.py
+-rw-r--r--   0        0        0     2900 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/helpers.py
+-rw-r--r--   0        0        0      387 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/ids.py
+-rw-r--r--   0        0        0      788 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/json/__init__.py
+-rw-r--r--   0        0        0     1627 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/json/builtin_wrapper.py
+-rw-r--r--   0        0        0     1758 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/json/orjson_wrapper.py
+-rw-r--r--   0        0        0      220 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/native.py
+-rw-r--r--   0        0        0     2074 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/native_mode.py
+-rw-r--r--   0        0        0     6390 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/nicegui.py
+-rw-r--r--   0        0        0     1609 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/outbox.py
+-rw-r--r--   0        0        0     4217 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/page.py
+-rw-r--r--   0        0        0     8064 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/page_layout.py
+-rw-r--r--   0        0        0     5924 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/run.py
+-rw-r--r--   0        0        0      895 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/run_with.py
+-rw-r--r--   0        0        0      611 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/slot.py
+-rw-r--r--   0        0        0    15086 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/favicon.ico
+-rw-r--r--   0        0        0      756 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxEIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0    10144 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxFIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0     7668 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxGIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0     3360 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxHIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0    10972 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxIIzIXKMny.woff2
+-rw-r--r--   0        0        0     4960 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxLIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0     6384 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxMIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0     6632 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    11072 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2
+-rw-r--r--   0        0        0     4796 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0      768 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10352 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     7676 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     3472 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     6480 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    11160 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2
+-rw-r--r--   0        0        0     4928 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0      756 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10412 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     7840 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     3448 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     6620 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    11040 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2
+-rw-r--r--   0        0        0     4796 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0      756 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10256 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     7676 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     3468 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     6612 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfABc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10992 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc4AMP6lQ.woff2
+-rw-r--r--   0        0        0     4756 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0      772 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCBc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10188 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCRc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     7608 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfChc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     3388 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     4864 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0    11028 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2
+-rw-r--r--   0        0        0     6460 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0    10352 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0     7736 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0     3496 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0      748 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0   128616 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0        0        0    11484 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/fonts.css
+-rw-r--r--   0        0        0     1913 2023-04-14 14:12:00.754256 nicegui-1.2.7/nicegui/static/nicegui.css
+-rw-r--r--   0        0        0   198973 2023-04-14 14:12:00.758256 nicegui-1.2.7/nicegui/static/quasar.prod.css
+-rw-r--r--   0        0        0   509631 2023-04-14 14:12:00.758256 nicegui-1.2.7/nicegui/static/quasar.umd.prod.js
+-rw-r--r--   0        0        0     1510 2023-04-14 14:12:00.758256 nicegui-1.2.7/nicegui/static/sad_face.svg
+-rw-r--r--   0        0        0    45896 2023-04-14 14:12:00.758256 nicegui-1.2.7/nicegui/static/socket.io.min.js
+-rw-r--r--   0        0        0   350399 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/static/tailwindcss.min.js
+-rw-r--r--   0        0        0   128872 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/static/vue.global.prod.js
+-rw-r--r--   0        0        0   107302 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/static/vue.min.js
+-rw-r--r--   0        0        0    44035 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/tailwind.py
+-rw-r--r--   0        0        0     4232 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/tailwind_types/accent_color.py
+-rw-r--r--   0        0        0      191 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/tailwind_types/align_content.py
+-rw-r--r--   0        0        0      132 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/tailwind_types/align_items.py
+-rw-r--r--   0        0        0      143 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/tailwind_types/align_self.py
+-rw-r--r--   0        0        0      125 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/tailwind_types/animation.py
+-rw-r--r--   0        0        0       75 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/tailwind_types/appearance.py
+-rw-r--r--   0        0        0      103 2023-04-14 14:12:00.762256 nicegui-1.2.7/nicegui/tailwind_types/aspect_ratio.py
+-rw-r--r--   0        0        0      147 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_blur.py
+-rw-r--r--   0        0        0      186 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_brightness.py
+-rw-r--r--   0        0        0      142 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_contrast.py
+-rw-r--r--   0        0        0       87 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_grayscale.py
+-rw-r--r--   0        0        0      130 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_hue_rotate.py
+-rw-r--r--   0        0        0       84 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_invert.py
+-rw-r--r--   0        0        0      217 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_opacity.py
+-rw-r--r--   0        0        0      121 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_saturate.py
+-rw-r--r--   0        0        0       83 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/backdrop_sepia.py
+-rw-r--r--   0        0        0      113 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_attachment.py
+-rw-r--r--   0        0        0      328 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_blend_mode.py
+-rw-r--r--   0        0        0      123 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_clip.py
+-rw-r--r--   0        0        0     4224 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_color.py
+-rw-r--r--   0        0        0      252 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_image.py
+-rw-r--r--   0        0        0      113 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_origin.py
+-rw-r--r--   0        0        0      207 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_position.py
+-rw-r--r--   0        0        0      172 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_repeat.py
+-rw-r--r--   0        0        0      107 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/background_size.py
+-rw-r--r--   0        0        0      139 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/blur.py
+-rw-r--r--   0        0        0       99 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/border_collapse.py
+-rw-r--r--   0        0        0    41420 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/border_color.py
+-rw-r--r--   0        0        0     1785 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/border_radius.py
+-rw-r--r--   0        0        0     1238 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/border_spacing.py
+-rw-r--r--   0        0        0      145 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/border_style.py
+-rw-r--r--   0        0        0      532 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/border_width.py
+-rw-r--r--   0        0        0       97 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/box_decoration_break.py
+-rw-r--r--   0        0        0      146 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/box_shadow.py
+-rw-r--r--   0        0        0     4223 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/box_shadow_color.py
+-rw-r--r--   0        0        0       91 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/box_sizing.py
+-rw-r--r--   0        0        0      168 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/break_after.py
+-rw-r--r--   0        0        0      169 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/break_before.py
+-rw-r--r--   0        0        0      127 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/break_inside.py
+-rw-r--r--   0        0        0      178 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/brightness.py
+-rw-r--r--   0        0        0       89 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/caption_side.py
+-rw-r--r--   0        0        0     4219 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/caret_color.py
+-rw-r--r--   0        0        0      107 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/clear.py
+-rw-r--r--   0        0        0      321 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/columns.py
+-rw-r--r--   0        0        0       72 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/content.py
+-rw-r--r--   0        0        0      134 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/contrast.py
+-rw-r--r--   0        0        0      623 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/cursor.py
+-rw-r--r--   0        0        0      443 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/display.py
+-rw-r--r--   0        0        0     4220 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/divide_color.py
+-rw-r--r--   0        0        0      131 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/divide_style.py
+-rw-r--r--   0        0        0      204 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/divide_width.py
+-rw-r--r--   0        0        0      134 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/drop_shadow.py
+-rw-r--r--   0        0        0     4225 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/fill.py
+-rw-r--r--   0        0        0      105 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/flex.py
+-rw-r--r--   0        0        0      729 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/flex_basis.py
+-rw-r--r--   0        0        0      126 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/flex_direction.py
+-rw-r--r--   0        0        0       78 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/flex_grow.py
+-rw-r--r--   0        0        0       80 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/flex_shrink.py
+-rw-r--r--   0        0        0      107 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/flex_wrap.py
+-rw-r--r--   0        0        0       96 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/floats.py
+-rw-r--r--   0        0        0      100 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/font_family.py
+-rw-r--r--   0        0        0      201 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/font_size.py
+-rw-r--r--   0        0        0      113 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/font_smoothing.py
+-rw-r--r--   0        0        0       94 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/font_style.py
+-rw-r--r--   0        0        0      261 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/font_variant_numeric.py
+-rw-r--r--   0        0        0      192 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/font_weight.py
+-rw-r--r--   0        0        0     1228 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/gap.py
+-rw-r--r--   0        0        0    16445 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/gradient_color_stops.py
+-rw-r--r--   0        0        0       79 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/grayscale.py
+-rw-r--r--   0        0        0      112 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/grid_auto_columns.py
+-rw-r--r--   0        0        0      134 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/grid_auto_flow.py
+-rw-r--r--   0        0        0      109 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/grid_auto_rows.py
+-rw-r--r--   0        0        0      677 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/grid_column_start_end.py
+-rw-r--r--   0        0        0      411 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/grid_row_start_end.py
+-rw-r--r--   0        0        0      195 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/grid_template_columns.py
+-rw-r--r--   0        0        0      135 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/grid_template_rows.py
+-rw-r--r--   0        0        0      639 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/height.py
+-rw-r--r--   0        0        0      122 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/hue_rotate.py
+-rw-r--r--   0        0        0       98 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/hyphens.py
+-rw-r--r--   0        0        0       76 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/invert.py
+-rw-r--r--   0        0        0       99 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/isolation.py
+-rw-r--r--   0        0        0      177 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/justify_content.py
+-rw-r--r--   0        0        0      118 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/justify_items.py
+-rw-r--r--   0        0        0      129 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/justify_self.py
+-rw-r--r--   0        0        0      147 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/letter_spacing.py
+-rw-r--r--   0        0        0      128 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/line_clamp.py
+-rw-r--r--   0        0        0      215 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/line_height.py
+-rw-r--r--   0        0        0       79 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/list_style_image.py
+-rw-r--r--   0        0        0       99 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/list_style_position.py
+-rw-r--r--   0        0        0      105 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/list_style_type.py
+-rw-r--r--   0        0        0     4199 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/margin.py
+-rw-r--r--   0        0        0      477 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/max_height.py
+-rw-r--r--   0        0        0      342 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/max_width.py
+-rw-r--r--   0        0        0      130 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/min_height.py
+-rw-r--r--   0        0        0      115 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/min_width.py
+-rw-r--r--   0        0        0      341 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/mix_blend_mode.py
+-rw-r--r--   0        0        0      132 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/object_fit.py
+-rw-r--r--   0        0        0      203 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/object_position.py
+-rw-r--r--   0        0        0      209 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/opacity.py
+-rw-r--r--   0        0        0      206 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/order.py
+-rw-r--r--   0        0        0     4221 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/outline_color.py
+-rw-r--r--   0        0        0      111 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/outline_offset.py
+-rw-r--r--   0        0        0      127 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/outline_style.py
+-rw-r--r--   0        0        0      110 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/outline_width.py
+-rw-r--r--   0        0        0      282 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/overflow.py
+-rw-r--r--   0        0        0      200 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/overscroll_behavior.py
+-rw-r--r--   0        0        0     4066 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/padding.py
+-rw-r--r--   0        0        0      177 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/place_content.py
+-rw-r--r--   0        0        0      132 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/place_items.py
+-rw-r--r--   0        0        0      127 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/place_self.py
+-rw-r--r--   0        0        0       90 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/pointer_events.py
+-rw-r--r--   0        0        0      134 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/position.py
+-rw-r--r--   0        0        0       97 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/resize.py
+-rw-r--r--   0        0        0     4218 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/ring_color.py
+-rw-r--r--   0        0        0     4224 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/ring_offset_color.py
+-rw-r--r--   0        0        0      113 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/ring_offset_width.py
+-rw-r--r--   0        0        0      128 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/ring_width.py
+-rw-r--r--   0        0        0      145 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/rotate.py
+-rw-r--r--   0        0        0      113 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/saturate.py
+-rw-r--r--   0        0        0      410 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/scale.py
+-rw-r--r--   0        0        0      100 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/screen_readers.py
+-rw-r--r--   0        0        0       93 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/scroll_behavior.py
+-rw-r--r--   0        0        0     4071 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/scroll_margin.py
+-rw-r--r--   0        0        0     4072 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/scroll_padding.py
+-rw-r--r--   0        0        0      124 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/scroll_snap_align.py
+-rw-r--r--   0        0        0       95 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/scroll_snap_stop.py
+-rw-r--r--   0        0        0      143 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/scroll_snap_type.py
+-rw-r--r--   0        0        0       75 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/sepia.py
+-rw-r--r--   0        0        0      191 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/skew.py
+-rw-r--r--   0        0        0      927 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/space_between.py
+-rw-r--r--   0        0        0     4227 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/stroke.py
+-rw-r--r--   0        0        0       91 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/stroke_width.py
+-rw-r--r--   0        0        0       89 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/table_layout.py
+-rw-r--r--   0        0        0      140 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_align.py
+-rw-r--r--   0        0        0     4218 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_color.py
+-rw-r--r--   0        0        0      140 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_decoration.py
+-rw-r--r--   0        0        0     4228 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_decoration_color.py
+-rw-r--r--   0        0        0      139 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_decoration_style.py
+-rw-r--r--   0        0        0      150 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_decoration_thickness.py
+-rw-r--r--   0        0        0      407 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_indent.py
+-rw-r--r--   0        0        0      119 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_overflow.py
+-rw-r--r--   0        0        0      137 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_transform.py
+-rw-r--r--   0        0        0      129 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/text_underline_offset.py
+-rw-r--r--   0        0        0     6299 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/top_right_bottom_left.py
+-rw-r--r--   0        0        0      215 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/touch_action.py
+-rw-r--r--   0        0        0      204 2023-04-14 14:12:00.766256 nicegui-1.2.7/nicegui/tailwind_types/transform_origin.py
+-rw-r--r--   0        0        0      165 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/transition_delay.py
+-rw-r--r--   0        0        0      168 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/transition_duration.py
+-rw-r--r--   0        0        0      162 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/transition_property.py
+-rw-r--r--   0        0        0      126 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/transition_timing_function.py
+-rw-r--r--   0        0        0     1074 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/translate.py
+-rw-r--r--   0        0        0      110 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/user_select.py
+-rw-r--r--   0        0        0      180 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/vertical_align.py
+-rw-r--r--   0        0        0      111 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/visibility.py
+-rw-r--r--   0        0        0      154 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/whitespace.py
+-rw-r--r--   0        0        0      772 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/width.py
+-rw-r--r--   0        0        0      122 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/will_change.py
+-rw-r--r--   0        0        0      112 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/word_break.py
+-rw-r--r--   0        0        0      130 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/tailwind_types/z_index.py
+-rw-r--r--   0        0        0     7912 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/templates/index.html
+-rw-r--r--   0        0        0     3758 2023-04-14 14:12:00.770256 nicegui-1.2.7/nicegui/ui.py
+-rw-r--r--   0        0        0     1685 2023-04-14 14:12:13.375171 nicegui-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     7355 1970-01-01 00:00:00.000000 nicegui-1.2.7/setup.py
+-rw-r--r--   0        0        0     7257 1970-01-01 00:00:00.000000 nicegui-1.2.7/PKG-INFO
```

### Comparing `nicegui-1.2.6/LICENSE` & `nicegui-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/README.md` & `nicegui-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/app.py` & `nicegui-1.2.7/nicegui/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,12 +67,14 @@
         This is useful for providing local data like images to the frontend.
         Otherwise the browser would not be able to access the files.
         Do only put non-security-critical files in there, as they are accessible to everyone.
 
         :param path: string that starts with a slash "/"
         :param directory: folder with static files to serve under the given path
         """
+        if path == '/':
+            raise ValueError('''Path cannot be "/", because it would hide NiceGUI's internal "/_nicegui" route.''')
         globals.app.mount(path, StaticFiles(directory=directory))
 
     def remove_route(self, path: str) -> None:
         """Remove routes with the given path."""
         self.routes[:] = [r for r in self.routes if getattr(r, 'path', None) != path]
```

### Comparing `nicegui-1.2.6/nicegui/background_tasks.py` & `nicegui-1.2.7/nicegui/background_tasks.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/binding.py` & `nicegui-1.2.7/nicegui/binding.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/client.py` & `nicegui-1.2.7/nicegui/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,18 +48,20 @@
         self.page = page
 
         self.connect_handlers: List[Union[Callable, Awaitable]] = []
         self.disconnect_handlers: List[Union[Callable, Awaitable]] = []
 
     @property
     def ip(self) -> Optional[str]:
+        """Return the IP address of the client, or None if the client is not connected."""
         return self.environ.get('REMOTE_ADDR') if self.environ else None
 
     @property
     def has_socket_connection(self) -> bool:
+        """Return True if the client is connected, False otherwise."""
         return self.environ is not None
 
     def __enter__(self):
         self.content.__enter__()
         return self
 
     def __exit__(self, *_):
@@ -84,37 +86,38 @@
             'dark': str(self.page.resolve_dark()),
             'prefix': prefix,
             'tailwind': globals.tailwind,
             'socket_io_js_extra_headers': globals.socket_io_js_extra_headers,
         }, status_code, {'Cache-Control': 'no-store', 'X-NiceGUI-Content': 'page'})
 
     async def connected(self, timeout: float = 3.0, check_interval: float = 0.1) -> None:
-        '''Blocks execution until the client is connected.'''
+        """Block execution until the client is connected."""
         self.is_waiting_for_connection = True
         deadline = time.time() + timeout
         while not self.environ:
             if time.time() > deadline:
                 raise TimeoutError(f'No connection after {timeout} seconds')
             await asyncio.sleep(check_interval)
         self.is_waiting_for_connection = False
 
     async def disconnected(self, check_interval: float = 0.1) -> None:
-        '''Blocks execution until the client disconnects.'''
+        """Block execution until the client disconnects."""
         self.is_waiting_for_disconnect = True
         while self.id in globals.clients:
             await asyncio.sleep(check_interval)
         self.is_waiting_for_disconnect = False
 
     async def run_javascript(self, code: str, *,
                              respond: bool = True, timeout: float = 1.0, check_interval: float = 0.01) -> Optional[str]:
-        '''Allows execution of javascript on the client.
+        """Execute JavaScript on the client.
 
         The client connection must be established before this method is called.
         You can do this by `await client.connected()` or register a callback with `client.on_connected(...)`.
-        If respond is True, the javascript code must return a string.'''
+        If respond is True, the javascript code must return a string.
+        """
         request_id = str(uuid.uuid4())
         command = {
             'code': code,
             'request_id': request_id if respond else None,
         }
         outbox.enqueue_message('run_javascript', command, self.id)
         if not respond:
@@ -123,15 +126,22 @@
         while request_id not in self.waiting_javascript_commands:
             if time.time() > deadline:
                 raise TimeoutError('JavaScript did not respond in time')
             await asyncio.sleep(check_interval)
         return self.waiting_javascript_commands.pop(request_id)
 
     def open(self, target: Union[Callable, str]) -> None:
+        """Open a new page in the client."""
         path = target if isinstance(target, str) else globals.page_routes[target]
         outbox.enqueue_message('open', path, self.id)
 
+    def download(self, url: str, filename: Optional[str] = None) -> None:
+        """Download a file from the given URL."""
+        outbox.enqueue_message('download', {'url': url, 'filename': filename}, self.id)
+
     def on_connect(self, handler: Union[Callable, Awaitable]) -> None:
+        """Register a callback to be called when the client connects."""
         self.connect_handlers.append(handler)
 
     def on_disconnect(self, handler: Union[Callable, Awaitable]) -> None:
+        """Register a callback to be called when the client disconnects."""
         self.disconnect_handlers.append(handler)
```

### Comparing `nicegui-1.2.6/nicegui/dependencies.py` & `nicegui-1.2.7/nicegui/dependencies.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/element.py` & `nicegui-1.2.7/nicegui/element.py`

 * *Files 7% similar despite different names*

```diff
@@ -191,29 +191,45 @@
         :param text: text of the tooltip
         """
         with self:
             tooltip = Element('q-tooltip')
             tooltip._text = text
         return self
 
-    def on(self, type: str, handler: Optional[Callable], args: Optional[List[str]] = None, *, throttle: float = 0.0) \
-            -> Self:
+    def on(self,
+           type: str,
+           handler: Optional[Callable],
+           args: Optional[List[str]] = None, *,
+           throttle: float = 0.0,
+           leading_events: bool = True,
+           trailing_events: bool = True,
+           ) -> Self:
         """Subscribe to an event.
 
         :param type: name of the event (e.g. "click", "mousedown", or "update:model-value")
         :param handler: callback that is called upon occurrence of the event
         :param args: arguments included in the event message sent to the event handler (default: `None` meaning all)
         :param throttle: minimum time (in seconds) between event occurrences (default: 0.0)
+        :param leading_events: whether to trigger the event handler immediately upon the first event occurrence (default: `True`)
+        :param trailing_events: whether to trigger the event handler after the last event occurrence (default: `True`)
         """
         if handler:
             if args and '*' in args:
                 url = f'https://github.com/zauberzeug/nicegui/issues/644'
                 warnings.warn(DeprecationWarning(f'Event args "*" is deprecated, omit this parameter instead ({url})'))
                 args = None
-            listener = EventListener(element_id=self.id, type=type, args=args, handler=handler, throttle=throttle)
+            listener = EventListener(
+                element_id=self.id,
+                type=type,
+                args=args,
+                handler=handler,
+                throttle=throttle,
+                leading_events=leading_events,
+                trailing_events=trailing_events,
+            )
             self._event_listeners[listener.id] = listener
         return self
 
     def _handle_event(self, msg: Dict) -> None:
         listener = self._event_listeners[msg['listener_id']]
         events.handle_event(listener.handler, msg, sender=self)
```

### Comparing `nicegui-1.2.6/nicegui/elements/aggrid.js` & `nicegui-1.2.7/nicegui/elements/aggrid.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/audio.py` & `nicegui-1.2.7/nicegui/elements/audio.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/avatar.py` & `nicegui-1.2.7/nicegui/elements/avatar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Optional
 
+from ..colors import set_background_color, set_text_color
 from ..element import Element
 
 
 class Avatar(Element):
 
     def __init__(self,
                  icon: str = 'none', *,
-                 color: str = 'primary',
+                 color: Optional[str] = 'primary',
                  text_color: Optional[str] = None,
                  size: Optional[str] = None,
                  font_size: Optional[str] = None,
                  square: bool = False,
                  rounded: bool = False,
                  ) -> None:
         """Avatar
 
         A avatar element wrapping Quasar's
         `QAvatar <https://quasar.dev/vue-components/avatar>`_ component.
 
         :param icon: name of the icon or image path with "img:" prefix (e.g. "map", "img:path/to/image.png")
-        :param color: color name for component from the Quasar Color Palette (e.g. "primary", "teal-10")
+        :param color: background color (either a Quasar, Tailwind, or CSS color or `None`, default: "primary")
         :param text_color: color name from the Quasar Color Palette (e.g. "primary", "teal-10")
         :param size: size in CSS units, including unit name or standard size name (xs|sm|md|lg|xl) (e.g. "16px", "2rem")
         :param font_size: size in CSS units, including unit name, of the content (icon, text) (e.g. "18px", "2rem")
         :param square: removes border-radius so borders are squared (default: False)
         :param rounded: applies a small standard border-radius for a squared shape of the component (default: False)
         """
         super().__init__('q-avatar')
 
         self._props['icon'] = icon
-        self._props['color'] = color
         self._props['square'] = square
         self._props['rounded'] = rounded
 
-        if text_color is not None:
-            self._props['text-color'] = text_color
+        set_background_color(self, color)
+        set_text_color(self, text_color, prop_name='text-color')
 
         if size is not None:
             self._props['size'] = size
 
         if font_size is not None:
             self._props['font-size'] = font_size
```

### Comparing `nicegui-1.2.6/nicegui/elements/badge.py` & `nicegui-1.2.7/nicegui/elements/badge.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from typing import Optional
+
+from ..colors import set_background_color, set_text_color
 from .mixins.text_element import TextElement
 
 
 class Badge(TextElement):
 
-    def __init__(self, text: str = '', *,
-                 color: str = 'blue', text_color: str = 'white', outline: bool = False) -> None:
+    def __init__(self,
+                 text: str = '', *,
+                 color: Optional[str] = 'primary',
+                 text_color: Optional[str] = None,
+                 outline: bool = False) -> None:
         """Badge
 
         A badge element wrapping Quasar's
         `QBadge <https://quasar.dev/vue-components/badge>`_ component.
 
         :param text: the initial value of the text field
-        :param color: the color name for component from the Quasar Color Palette (default: "blue")
-        :param text_color: overrides text color (if needed); color name from the Quasar Color Palette (default: "white")
+        :param color: the color name for component (either a Quasar, Tailwind, or CSS color or `None`, default: "primary")
+        :param text_color: text color (either a Quasar, Tailwind, or CSS color or `None`, default: `None`)
         :param outline: use 'outline' design (colored text and borders only) (default: False)
         """
         super().__init__(tag='q-badge', text=text)
-        self._props['color'] = color
-        self._props['text_color'] = text_color
+        set_background_color(self, color)
+        set_text_color(self, text_color, prop_name='text-color')
         self._props['outline'] = outline
```

### Comparing `nicegui-1.2.6/nicegui/elements/chart.js` & `nicegui-1.2.7/nicegui/elements/chart.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/chart.py` & `nicegui-1.2.7/nicegui/elements/chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         self._props['type'] = type
         self._props['options'] = options
         self._props['extras'] = [
             dependency.import_path
             for dependency in js_dependencies.values()
             if dependency.optional and dependency.path.stem in extras and 'chart' in dependency.dependents
         ]
+        self._props['key'] = self.id  # HACK: workaround for #600
 
     @property
     def options(self) -> Dict:
         return self._props['options']
 
     def update(self) -> None:
         super().update()
```

### Comparing `nicegui-1.2.6/nicegui/elements/checkbox.py` & `nicegui-1.2.7/nicegui/elements/checkbox.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/choice_element.py` & `nicegui-1.2.7/nicegui/elements/choice_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/color_input.py` & `nicegui-1.2.7/nicegui/elements/color_input.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/color_picker.py` & `nicegui-1.2.7/nicegui/elements/color_picker.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/colors.py` & `nicegui-1.2.7/nicegui/elements/colors.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 
 class Colors(Element):
 
     def __init__(self, *,
                  primary='#5898d4',
                  secondary='#26a69a',
                  accent='#9c27b0',
+                 dark='#1d1d1d',
                  positive='#21ba45',
                  negative='#c10015',
                  info='#31ccec',
                  warning='#f2c037') -> None:
         """Color Theming
 
         Sets the main colors (primary, secondary, accent, ...) used by `Quasar <https://quasar.dev/>`_.
         """
         super().__init__('colors')
         self._props['primary'] = primary
         self._props['secondary'] = secondary
         self._props['accent'] = accent
+        self._props['dark'] = dark
         self._props['positive'] = positive
         self._props['negative'] = negative
         self._props['info'] = info
         self._props['warning'] = warning
+        self._props['key'] = self.id  # HACK: workaround for #600
         self.update()
```

### Comparing `nicegui-1.2.6/nicegui/elements/date.py` & `nicegui-1.2.7/nicegui/elements/date.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Optional
 
 from .mixins.value_element import ValueElement
 
 
 class Date(ValueElement):
-    EVENT_ARGS = ['*']
+    EVENT_ARGS = None
 
     def __init__(self,
                  value: Optional[str] = None,
                  *,
                  mask: str = 'YYYY-MM-DD',
                  on_change: Optional[Callable] = None) -> None:
         """Date Input
```

### Comparing `nicegui-1.2.6/nicegui/elements/dialog.py` & `nicegui-1.2.7/nicegui/elements/dialog.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/expansion.py` & `nicegui-1.2.7/nicegui/elements/expansion.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/html.py` & `nicegui-1.2.7/nicegui/elements/html.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/icon.py` & `nicegui-1.2.7/nicegui/elements/icon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 
+from ..colors import set_text_color
 from ..element import Element
 
 
 class Icon(Element):
 
     def __init__(self,
                  name: str,
@@ -15,17 +16,16 @@
 
         This element is based on Quasar's `QIcon <https://quasar.dev/vue-components/icon>`_ component.
 
         `Here <https://material.io/icons/>`_ is a reference of possible names.
 
         :param name: name of the icon
         :param size: size in CSS units, including unit name or standard size name (xs|sm|md|lg|xl), examples: 16px, 2rem
-        :param color: color name for component, examples: primary, teal-10
+        :param color: icon color (either a Quasar, Tailwind, or CSS color or `None`, default: `None`)
         """
         super().__init__('q-icon')
         self._props['name'] = name
 
         if size:
             self._props['size'] = size
 
-        if color:
-            self._props['color'] = color
+        set_text_color(self, color)
```

### Comparing `nicegui-1.2.6/nicegui/elements/input.py` & `nicegui-1.2.7/nicegui/elements/input.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/interactive_image.js` & `nicegui-1.2.7/nicegui/elements/interactive_image.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/interactive_image.py` & `nicegui-1.2.7/nicegui/elements/interactive_image.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/joystick.py` & `nicegui-1.2.7/nicegui/elements/joystick.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/joystick.vue` & `nicegui-1.2.7/nicegui/elements/joystick.vue`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/keyboard.js` & `nicegui-1.2.7/nicegui/elements/keyboard.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/keyboard.py` & `nicegui-1.2.7/nicegui/elements/keyboard.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/knob.py` & `nicegui-1.2.7/nicegui/elements/knob.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 
+from ..colors import set_text_color
 from .label import Label
 from .mixins.value_element import ValueElement
 
 
 class Knob(ValueElement):
 
     def __init__(self,
@@ -23,26 +24,26 @@
         This element is based on Quasar's `QKnob <https://quasar.dev/vue-components/knob>`_ component.
         The element is used to take a number input from the user through mouse/touch panning.
 
         :param value: the initial value (default: 0.0)
         :param min: the minimum value (default: 0.0)
         :param max: the maximum value (default: 1.0)
         :param step: the step size (default: 0.01)
-        :param color: color name for component, examples: primary, teal-10 (default: "primary")
+        :param color: knob color (either a Quasar, Tailwind, or CSS color or `None`, default: "primary")
         :param center_color: color name for the center part of the component, examples: primary, teal-10
         :param track_color: color name for the track of the component, examples: primary, teal-10
         :param size: size in CSS units, including unit name or standard size name (xs|sm|md|lg|xl), examples: 16px, 2rem
         :param show_value: whether to show the value as text
         """
         super().__init__(tag='q-knob', value=value, on_value_change=None, throttle=0.05)
 
         self._props['min'] = min
         self._props['max'] = max
         self._props['step'] = step
-        self._props['color'] = color
+        set_text_color(self, color)
         self._props['show-value'] = True  # NOTE: enable default slot, e.g. for nested icon
 
         if center_color:
             self._props['center-color'] = center_color
 
         if track_color:
             self._props['track-color'] = track_color
```

### Comparing `nicegui-1.2.6/nicegui/elements/lib/CSS2DRenderer.js` & `nicegui-1.2.7/nicegui/elements/lib/CSS2DRenderer.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/CSS3DRenderer.js` & `nicegui-1.2.7/nicegui/elements/lib/CSS3DRenderer.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/OrbitControls.js` & `nicegui-1.2.7/nicegui/elements/lib/OrbitControls.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/STLLoader.js` & `nicegui-1.2.7/nicegui/elements/lib/STLLoader.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/ag-grid-community.min.js` & `nicegui-1.2.7/nicegui/elements/lib/ag-grid-community.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts-3d.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts-3d.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts-more.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts-more.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/accessibility.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/accessibility.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/annotations-advanced.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/annotations-advanced.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/annotations.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/annotations.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/arc-diagram.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/arc-diagram.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/arrow-symbols.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/arrow-symbols.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/boost-canvas.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/boost-canvas.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/boost.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/boost.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/broken-axis.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/broken-axis.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/bullet.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/bullet.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/coloraxis.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/coloraxis.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/current-date-indicator.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/current-date-indicator.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/cylinder.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/cylinder.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/data.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/data.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/datagrouping.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/datagrouping.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/debugger.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/debugger.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/dependency-wheel.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/dependency-wheel.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/dotplot.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/dotplot.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/drag-panes.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/drag-panes.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/draggable-points.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/draggable-points.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/drilldown.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/drilldown.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/dumbbell.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/dumbbell.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/export-data.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/export-data.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/exporting.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/exporting.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/full-screen.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/full-screen.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/funnel.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/funnel.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/funnel3d.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/funnel3d.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/gantt.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/gantt.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/grid-axis.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/grid-axis.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/heatmap.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/heatmap.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/heikinashi.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/heikinashi.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/histogram-bellcurve.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/histogram-bellcurve.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/hollowcandlestick.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/hollowcandlestick.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/item-series.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/item-series.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/lollipop.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/lollipop.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/marker-clusters.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/marker-clusters.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/networkgraph.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/networkgraph.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/no-data-to-display.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/no-data-to-display.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/offline-exporting.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/offline-exporting.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/oldie-polyfills.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/oldie-polyfills.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/oldie.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/oldie.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/organization.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/organization.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/overlapping-datalabels.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/overlapping-datalabels.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/parallel-coordinates.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/parallel-coordinates.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/pareto.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/pareto.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/pathfinder.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/pathfinder.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/pattern-fill.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/pattern-fill.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/price-indicator.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/price-indicator.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/pyramid3d.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/pyramid3d.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/sankey.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/sankey.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/series-label.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/series-label.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/series-on-point.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/series-on-point.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/solid-gauge.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/solid-gauge.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/sonification.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/sonification.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/static-scale.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/static-scale.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/stock-tools.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/stock-tools.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/stock.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/stock.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/streamgraph.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/streamgraph.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/sunburst.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/sunburst.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/tilemap.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/tilemap.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/timeline.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/timeline.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/treegraph.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/treegraph.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/treegrid.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/treegrid.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/treemap.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/treemap.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/variable-pie.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/variable-pie.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/variwide.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/variwide.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/vector.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/vector.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/venn.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/venn.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/windbarb.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/windbarb.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/wordcloud.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/wordcloud.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/highcharts_modules/xrange.js` & `nicegui-1.2.7/nicegui/elements/lib/highcharts_modules/xrange.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/mermaid.min.js` & `nicegui-1.2.7/nicegui/elements/lib/mermaid.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/nipplejs.min.js` & `nicegui-1.2.7/nicegui/elements/lib/nipplejs.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/plotly.min.js` & `nicegui-1.2.7/nicegui/elements/lib/plotly.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/three.min.js` & `nicegui-1.2.7/nicegui/elements/lib/three.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/lib/tween.umd.min.js` & `nicegui-1.2.7/nicegui/elements/lib/tween.umd.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/line_plot.py` & `nicegui-1.2.7/nicegui/elements/line_plot.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/link.py` & `nicegui-1.2.7/nicegui/elements/link.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Callable, Union
 
 from .. import globals
+from ..dependencies import register_component
 from ..element import Element
 from .mixins.text_element import TextElement
 
+register_component('link', __file__, 'link.js')
+
 
 class Link(TextElement):
 
     def __init__(self, text: str = '', target: Union[Callable, str] = '#', new_tab: bool = False) -> None:
         """Link
 
         Create a hyperlink.
@@ -15,15 +18,15 @@
         To jump to a specific location within a page you can place linkable anchors with `ui.link_target("name")`
         and link to it with `ui.link(target="#name")`.
 
         :param text: display text
         :param target: page function or string that is a an absolute URL or relative path from base URL
         :param new_tab: open link in new tab (default: False)
         """
-        super().__init__(tag='a', text=text)
+        super().__init__(tag='link', text=text)
         self._props['href'] = target if isinstance(target, str) else globals.page_routes[target]
         self._props['target'] = '_blank' if new_tab else '_self'
         self._classes = ['nicegui-link']
 
 
 class LinkTarget(Element):
```

### Comparing `nicegui-1.2.6/nicegui/elements/log.js` & `nicegui-1.2.7/nicegui/elements/log.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/log.py` & `nicegui-1.2.7/nicegui/elements/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         Create a log view that allows to add new lines without re-transmitting the whole history to the client.
 
         :param max_lines: maximum number of lines before dropping oldest ones (default: `None`)
         """
         super().__init__('log')
         self._props['max_lines'] = max_lines
         self._props['lines'] = ''
+        self._props['key'] = self.id  # HACK: workaround for #600
         self._classes = ['nicegui-log']
         self.lines: deque[str] = deque(maxlen=max_lines)
 
     def push(self, line: Any) -> None:
         line = str(line)
         self.lines.extend(line.splitlines())
         self._props['lines'] = '\n'.join(self.lines)
```

### Comparing `nicegui-1.2.6/nicegui/elements/markdown.js` & `nicegui-1.2.7/nicegui/elements/markdown.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/markdown.py` & `nicegui-1.2.7/nicegui/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/menu.py` & `nicegui-1.2.7/nicegui/elements/menu.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/mermaid.py` & `nicegui-1.2.7/nicegui/elements/mermaid.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/mixins/content_element.py` & `nicegui-1.2.7/nicegui/elements/mixins/content_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/mixins/filter_element.py` & `nicegui-1.2.7/nicegui/elements/mixins/filter_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/mixins/source_element.py` & `nicegui-1.2.7/nicegui/elements/mixins/source_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/mixins/text_element.py` & `nicegui-1.2.7/nicegui/elements/mixins/text_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/mixins/value_element.py` & `nicegui-1.2.7/nicegui/elements/mixins/value_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/mixins/visibility.py` & `nicegui-1.2.7/nicegui/elements/mixins/visibility.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/number.py` & `nicegui-1.2.7/nicegui/elements/number.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         super().__init__(tag='q-input', value=value, on_value_change=on_change)
         self._props['type'] = 'number'
         if label is not None:
             self._props['label'] = label
         if placeholder is not None:
             self._props['placeholder'] = placeholder
         self.validation = validation
+        self.on('blur', self.update)  # NOTE: to apply format (#736)
 
     def on_value_change(self, value: Any) -> None:
         super().on_value_change(value)
         for message, check in self.validation.items():
             if not check(value):
                 self.props(f'error error-message="{message}"')
                 break
```

### Comparing `nicegui-1.2.6/nicegui/elements/plotly.py` & `nicegui-1.2.7/nicegui/elements/plotly.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/plotly.vue` & `nicegui-1.2.7/nicegui/elements/plotly.vue`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/progress.py` & `nicegui-1.2.7/nicegui/elements/progress.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,70 @@
 from typing import Optional
 
 from nicegui import ui
 
+from ..colors import set_text_color
 from .mixins.value_element import ValueElement
 
 
 class LinearProgress(ValueElement):
     VALUE_PROP = 'value'
 
-    def __init__(self, value: float = 0.0, *, size: Optional[str] = None, show_value: bool = True) -> None:
+    def __init__(self,
+                 value: float = 0.0, *,
+                 size: Optional[str] = None,
+                 show_value: bool = True,
+                 color: Optional[str] = 'primary',
+                 ) -> None:
         """Linear Progress
 
         A linear progress bar wrapping Quasar's
         `QLinearProgress <https://quasar.dev/vue-components/linear-progress>`_ component.
 
         :param value: the initial value of the field (from 0.0 to 1.0)
         :param size: the height of the progress bar (default: "20px" with value label and "4px" without)
         :param show_value: whether to show a value label in the center (default: `True`)
+        :param color: color (either a Quasar, Tailwind, or CSS color or `None`, default: "primary")
         """
         super().__init__(tag='q-linear-progress', value=value, on_value_change=None)
         self._props['size'] = size if size is not None else '20px' if show_value else '4px'
+        set_text_color(self, color)
 
         if show_value:
             with self:
                 ui.label().classes('absolute-center text-sm text-white').bind_text_from(self, 'value')
 
 
 class CircularProgress(ValueElement):
     VALUE_PROP = 'value'
 
-    def __init__(self, value: float = 0.0, *,
-                 min: float = 0.0, max: float = 1.0, size: str = 'xl', show_value: bool = True) -> None:
+    def __init__(self,
+                 value: float = 0.0, *,
+                 min: float = 0.0,
+                 max: float = 1.0,
+                 size: str = 'xl',
+                 show_value: bool = True,
+                 color: Optional[str] = 'primary',
+                 ) -> None:
         """Circular Progress
 
         A circular progress bar wrapping Quasar's
         `QCircularProgress <https://quasar.dev/vue-components/circular-progress>`_.
 
         :param value: the initial value of the field
+        :param min: the minimum value (default: 0.0)
+        :param max: the maximum value (default: 1.0)
         :param size: the size of the progress circle (default: "xl")
         :param show_value: whether to show a value label in the center (default: `True`)
+        :param color: color (either a Quasar, Tailwind, or CSS color or `None`, default: "primary")
         """
         super().__init__(tag='q-circular-progress', value=value, on_value_change=None)
         self._props['min'] = min
         self._props['max'] = max
         self._props['size'] = size
         self._props['show-value'] = show_value
-        self._props['color'] = 'primary'
+        set_text_color(self, color)
         self._props['track-color'] = 'grey-4'
 
         if show_value:
             with self:
                 ui.label().classes('absolute-center text-xs').bind_text_from(self, 'value')
```

### Comparing `nicegui-1.2.6/nicegui/elements/pyplot.py` & `nicegui-1.2.7/nicegui/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/query.js` & `nicegui-1.2.7/nicegui/elements/query.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/query.py` & `nicegui-1.2.7/nicegui/elements/query.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/radio.py` & `nicegui-1.2.7/nicegui/elements/radio.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/scene.js` & `nicegui-1.2.7/nicegui/elements/scene.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/scene.py` & `nicegui-1.2.7/nicegui/elements/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,19 @@
     from .scene_objects import Sphere as sphere
     from .scene_objects import SpotLight as spot_light
     from .scene_objects import Stl as stl
     from .scene_objects import Text as text
     from .scene_objects import Text3d as text3d
     from .scene_objects import Texture as texture
 
-    def __init__(self, width: int = 400, height: int = 300, grid: bool = True, on_click: Optional[Callable] = None) -> None:
+    def __init__(self,
+                 width: int = 400,
+                 height: int = 300,
+                 grid: bool = True,
+                 on_click: Optional[Callable] = None) -> None:
         """3D Scene
 
         Display a 3d scene using `three.js <https://threejs.org/>`_.
         Currently NiceGUI supports boxes, spheres, cylinders/cones, extrusions, straight lines, curves and textured meshes.
         Objects can be translated, rotated and displayed with different color, opacity or as wireframes.
         They can also be grouped to apply joint movements.
 
@@ -66,14 +70,15 @@
         :param grid: whether to display a grid
         :param on_click: callback to execute when a 3d object is clicked
         """
         super().__init__('scene')
         self._props['width'] = width
         self._props['height'] = height
         self._props['grid'] = grid
+        self._props['key'] = self.id  # HACK: workaround for #600
         self.objects: Dict[str, Object3D] = {}
         self.stack: List[Union[Object3D, SceneObject]] = [SceneObject()]
         self.camera: SceneCamera = SceneCamera()
         self.on_click = on_click
         self.is_initialized = False
         self.on('init', self.handle_init)
         self.on('click3d', self.handle_click)
```

### Comparing `nicegui-1.2.6/nicegui/elements/scene_object3d.py` & `nicegui-1.2.7/nicegui/elements/scene_object3d.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,9 +120,12 @@
     def visible(self, value: bool = True):
         if self.visible_ != value:
             self.visible_ = value
             self._visible()
         return self
 
     def delete(self) -> None:
+        children = [object for object in self.scene.objects.values() if object.parent == self]
+        for child in children:
+            child.delete()
         del self.scene.objects[self.id]
         self._delete()
```

### Comparing `nicegui-1.2.6/nicegui/elements/scene_objects.py` & `nicegui-1.2.7/nicegui/elements/scene_objects.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/select.js` & `nicegui-1.2.7/nicegui/elements/select.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/select.py` & `nicegui-1.2.7/nicegui/elements/select.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/slider.py` & `nicegui-1.2.7/nicegui/elements/slider.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/spinner.py` & `nicegui-1.2.7/nicegui/elements/spinner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 from typing_extensions import Literal
 
+from ..colors import set_text_color
 from ..element import Element
 
 SpinnerTypes = Literal[
     'default',
     'audio',
     'ball',
     'bars',
@@ -29,22 +30,26 @@
     'rings',
     'tail',
 ]
 
 
 class Spinner(Element):
 
-    def __init__(self, type: Optional[SpinnerTypes] = 'default', *,
-                 size: str = '1em', color: str = 'primary', thickness: float = 5.0):
+    def __init__(self,
+                 type: Optional[SpinnerTypes] = 'default', *,
+                 size: str = '1em',
+                 color: Optional[str] = 'primary',
+                 thickness: float = 5.0,
+                 ) -> None:
         """Spinner
 
-        See `Quasar Spinner <https://quasar.dev/vue-components/spinner>`_ for more information.
+        See `Quasar Spinner <https://quasar.dev/vue-components/spinners>`_ for more information.
 
         :param type: type of spinner (e.g. "audio", "ball", "bars", ..., default: "default")
         :param size: size of the spinner (e.g. "3em", "10px", "xl", ..., default: "1em")
-        :param color: color of the spinner (default: "primary")
+        :param color: color of the spinner (either a Quasar, Tailwind, or CSS color or `None`, default: "primary")
         :param thickness: thickness of the spinner (applies to the "default" spinner only, default: 5.0)
         """
         super().__init__('q-spinner' if type == 'default' else f'q-spinner-{type}')
         self._props['size'] = size
-        self._props['color'] = color
+        set_text_color(self, color)
         self._props['thickness'] = thickness
```

### Comparing `nicegui-1.2.6/nicegui/elements/splitter.py` & `nicegui-1.2.7/nicegui/elements/splitter.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/switch.py` & `nicegui-1.2.7/nicegui/elements/switch.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/table.py` & `nicegui-1.2.7/nicegui/elements/table.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/tabs.py` & `nicegui-1.2.7/nicegui/elements/tabs.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/textarea.py` & `nicegui-1.2.7/nicegui/elements/textarea.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/time.py` & `nicegui-1.2.7/nicegui/elements/time.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/toggle.py` & `nicegui-1.2.7/nicegui/elements/toggle.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/tree.py` & `nicegui-1.2.7/nicegui/elements/tree.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/elements/upload.py` & `nicegui-1.2.7/nicegui/elements/upload.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,72 @@
 from typing import Callable, Optional
 
 from fastapi import Request, Response
 
 from ..element import Element
-from ..events import UploadEventArguments, handle_event
+from ..events import EventArguments, UploadEventArguments, handle_event
 from ..nicegui import app
 
 
 class Upload(Element):
 
     def __init__(self, *,
                  multiple: bool = False,
+                 max_file_size: Optional[int] = None,
+                 max_total_size: Optional[int] = None,
+                 max_files: Optional[int] = None,
                  on_upload: Optional[Callable] = None,
+                 on_rejected: Optional[Callable] = None,
                  label: str = '',
                  auto_upload: bool = False,
                  ) -> None:
         """File Upload
 
         Based on Quasar's `QUploader <https://quasar.dev/vue-components/uploader>`_ component.
 
         :param multiple: allow uploading multiple files at once (default: `False`)
+        :param max_file_size: maximum file size in bytes (default: `0`)
+        :param max_total_size: maximum total size of all files in bytes (default: `0`)
+        :param max_files: maximum number of files (default: `0`)
         :param on_upload: callback to execute for each uploaded file (type: nicegui.events.UploadEventArguments)
+        :param on_rejected: callback to execute for each rejected file
         :param label: label for the uploader (default: `''`)
         :param auto_upload: automatically upload files when they are selected (default: `False`)
         """
         super().__init__('q-uploader')
         self._props['multiple'] = multiple
         self._props['label'] = label
         self._props['auto-upload'] = auto_upload
         self._props['url'] = f'/_nicegui/client/{self.client.id}/upload/{self.id}'
 
+        if max_file_size is not None:
+            self._props['max-file-size'] = max_file_size
+
+        if max_total_size is not None:
+            self._props['max-total-size'] = max_total_size
+
+        if max_files is not None:
+            self._props['max-files'] = max_files
+
         @app.post(self._props['url'])
         async def upload_route(request: Request) -> Response:
             for data in (await request.form()).values():
                 args = UploadEventArguments(
                     sender=self,
                     client=self.client,
                     content=data.file,
                     name=data.filename,
                     type=data.content_type,
                 )
                 handle_event(on_upload, args)
             return {'upload': 'success'}
 
+        if on_rejected:
+            self.on('rejected', lambda _: handle_event(on_rejected, EventArguments(sender=self, client=self.client)),
+                    args=[])
+
     def reset(self) -> None:
         self.run_method('reset')
 
     def delete(self) -> None:
         app.remove_route(self._props['url'])
         super().delete()
```

### Comparing `nicegui-1.2.6/nicegui/elements/video.py` & `nicegui-1.2.7/nicegui/elements/video.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/error.py` & `nicegui-1.2.7/nicegui/error.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/event_listener.py` & `nicegui-1.2.7/nicegui/event_listener.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 class EventListener:
     id: str = field(init=False)
     element_id: int
     type: str
     args: List[str]
     handler: Callable
     throttle: float
+    leading_events: bool
+    trailing_events: bool
 
     def __post_init__(self) -> None:
         self.id = str(uuid.uuid4())
 
     def to_dict(self) -> Dict[str, Any]:
         words = self.type.split('.')
         type = words.pop(0)
@@ -25,8 +27,10 @@
             'listener_id': self.id,
             'type': type,
             'specials': specials,
             'modifiers': modifiers,
             'keys': keys,
             'args': self.args,
             'throttle': self.throttle,
+            'leading_events': self.leading_events,
+            'trailing_events': self.trailing_events,
         }
```

### Comparing `nicegui-1.2.6/nicegui/events.py` & `nicegui-1.2.7/nicegui/events.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/favicon.py` & `nicegui-1.2.7/nicegui/favicon.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/functions/javascript.py` & `nicegui-1.2.7/nicegui/functions/javascript.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/functions/notify.py` & `nicegui-1.2.7/nicegui/functions/notify.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/functions/open.py` & `nicegui-1.2.7/nicegui/functions/open.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/functions/timer.py` & `nicegui-1.2.7/nicegui/functions/timer.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/globals.py` & `nicegui-1.2.7/nicegui/globals.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/helpers.py` & `nicegui-1.2.7/nicegui/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 def is_port_open(host: str, port: int) -> bool:
     """Check if the port is open by checking if a TCP connection can be established."""
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
         sock.connect((host, port))
     except (ConnectionRefusedError, TimeoutError):
         return False
+    except Exception:
+        return False
     else:
         return True
     finally:
         sock.close()
 
 
 def schedule_browser(host: str, port: int) -> Tuple[threading.Thread, threading.Event]:
```

### Comparing `nicegui-1.2.6/nicegui/json/__init__.py` & `nicegui-1.2.7/nicegui/json/__init__.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/json/builtin_wrapper.py` & `nicegui-1.2.7/nicegui/json/builtin_wrapper.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/json/orjson_wrapper.py` & `nicegui-1.2.7/nicegui/json/orjson_wrapper.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/native_mode.py` & `nicegui-1.2.7/nicegui/native_mode.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,50 +2,55 @@
 import multiprocessing
 import socket
 import tempfile
 import time
 import warnings
 from threading import Thread
 
-from . import globals
+from . import globals, helpers
 
 with warnings.catch_warnings():
     # webview depends on bottle which uses the deprecated CGI function (https://github.com/bottlepy/bottle/issues/1403)
     warnings.filterwarnings('ignore', category=DeprecationWarning)
     import webview
 
 
-def open_window(url: str, title: str, width: int, height: int, fullscreen: bool) -> None:
-    window_kwargs = dict(url=url, title=title, width=width, height=height, fullscreen=fullscreen)
+def open_window(host: str, port: int, title: str, width: int, height: int, fullscreen: bool) -> None:
+    while not helpers.is_port_open(host, port):
+        time.sleep(0.1)
+
+    window_kwargs = dict(url=f'http://{host}:{port}', title=title, width=width, height=height, fullscreen=fullscreen)
     window_kwargs.update(globals.app.native.window_args)
+
     webview.create_window(**window_kwargs)
     webview.start(storage_path=tempfile.mkdtemp(), **globals.app.native.start_args)
 
 
-def activate(url: str, title: str, width: int, height: int, fullscreen: bool) -> None:
+def activate(host: str, port: int, title: str, width: int, height: int, fullscreen: bool) -> None:
     def check_shutdown() -> None:
         while process.is_alive():
             time.sleep(0.1)
         globals.server.should_exit = True
         while globals.state != globals.State.STOPPED:
             time.sleep(0.1)
         _thread.interrupt_main()
 
     multiprocessing.freeze_support()
-    process = multiprocessing.Process(target=open_window, args=(url, title, width, height, fullscreen), daemon=False)
+    process = multiprocessing.Process(target=open_window, args=(host, port, title, width, height, fullscreen),
+                                      daemon=False)
     process.start()
     Thread(target=check_shutdown, daemon=True).start()
 
 
 def find_open_port(start_port: int = 8000, end_port: int = 8999) -> int:
-    '''Reliably find an open port in a given range.
+    """Reliably find an open port in a given range.
 
     This function will actually try to open the port to ensure no firewall blocks it.
     This is better than, e.g., passing port=0 to uvicorn.
-    '''
+    """
     for port in range(start_port, end_port + 1):
         try:
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 s.bind(('localhost', port))
                 return port
         except OSError:
             pass
```

### Comparing `nicegui-1.2.6/nicegui/nicegui.py` & `nicegui-1.2.7/nicegui/nicegui.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/outbox.py` & `nicegui-1.2.7/nicegui/outbox.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/page.py` & `nicegui-1.2.7/nicegui/page.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/page_layout.py` & `nicegui-1.2.7/nicegui/page_layout.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/run.py` & `nicegui-1.2.7/nicegui/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import multiprocessing
 import os
 import sys
 from typing import List, Optional, Tuple
 
+import __main__
 import uvicorn
 from uvicorn.main import STARTUP_FAILURE
 from uvicorn.supervisors import ChangeReload, Multiprocess
 
 from . import globals, helpers, native_mode
 
 
@@ -66,24 +67,28 @@
     globals.binding_refresh_interval = binding_refresh_interval
     globals.excludes = [e.strip() for e in exclude.split(',')]
     globals.tailwind = tailwind
 
     if multiprocessing.current_process().name != 'MainProcess':
         return
 
+    if reload and not hasattr(__main__, '__file__'):
+        logging.warning('auto-reloading is only supported when running from a file')
+        globals.reload = reload = False
+
     if fullscreen:
         native = True
     if window_size:
         native = True
     if native:
         show = False
         host = host or '127.0.0.1'
         port = native_mode.find_open_port()
         width, height = window_size or (800, 600)
-        native_mode.activate(f'http://{host}:{port}', title, width, height, fullscreen)
+        native_mode.activate(host, port, title, width, height, fullscreen)
     else:
         host = host or '0.0.0.0'
 
     # NOTE: We save the URL in an environment variable so the subprocess started in reload mode can access it.
     os.environ['NICEGUI_URL'] = f'http://{host}:{port}'
 
     if show:
```

### Comparing `nicegui-1.2.6/nicegui/run_with.py` & `nicegui-1.2.7/nicegui/run_with.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/slot.py` & `nicegui-1.2.7/nicegui/slot.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/favicon.ico` & `nicegui-1.2.7/nicegui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxEIzIXKMnyrYk.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxEIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxFIzIXKMnyrYk.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxFIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxGIzIXKMnyrYk.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxGIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxHIzIXKMnyrYk.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxHIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxIIzIXKMny.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxIIzIXKMny.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxLIzIXKMnyrYk.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxLIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxMIzIXKMnyrYk.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxMIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfABc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfABc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc4AMP6lQ.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc4AMP6lQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBxc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCBc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCBc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCRc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCRc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfChc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfChc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCxc4AMP6lbBP.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2` & `nicegui-1.2.7/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `nicegui-1.2.7/nicegui/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/fonts.css` & `nicegui-1.2.7/nicegui/static/fonts.css`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/nicegui.css` & `nicegui-1.2.7/nicegui/static/nicegui.css`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/quasar.prod.css` & `nicegui-1.2.7/nicegui/static/quasar.prod.css`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/quasar.umd.prod.js` & `nicegui-1.2.7/nicegui/static/quasar.umd.prod.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 /*!
- * Quasar Framework v2.11.8
+ * Quasar Framework v2.11.10
  * (c) 2015-present Razvan Stoenescu
  * Released under the MIT License.
  */
 (function(e, t) {
     "object" === typeof exports && "undefined" !== typeof module ? module.exports = t(require("vue")) : "function" === typeof define && define.amd ? define(["vue"], t) : (e = "undefined" !== typeof globalThis ? globalThis : e || self, e.Quasar = t(e.Vue))
 })(this, function(e) {
     "use strict";
@@ -873,15 +873,15 @@
             o.onSSRHydrated.forEach(e => {
                 e()
             }), o.$q.onSSRHydrated = (() => {})
         }))
     }
     var qe = function(e, t = {}) {
         const o = {
-            version: "2.11.8"
+            version: "2.11.10"
         };
         !1 === me ? (void 0 !== t.config && Object.assign(pe, t.config), o.config = {
             ...pe
         }, fe()) : o.config = t.config || {}, Ce(e, t, {
             parentApp: e,
             $q: o,
             lang: t.lang,
@@ -1144,15 +1144,15 @@
         it = new RegExp("^(" + Object.keys(nt).join("|") + ")"),
         rt = new RegExp("^(" + Object.keys(at).join("|") + ")"),
         st = new RegExp("^(" + Object.keys(lt).join("|") + ")"),
         ut = /^[Mm]\s?[-+]?\.?\d/,
         ct = /^img:/,
         dt = /^svguse:/,
         vt = /^ion-/,
-        pt = /^(fa-(solid|regular|light|brands|duotone|thin)|[lf]a[srlbdk]?) /;
+        pt = /^(fa-(sharp|solid|regular|light|brands|duotone|thin)|[lf]a[srlbdk]?) /;
     var mt = $e({
             name: "QIcon",
             props: {
                 ...We,
                 tag: {
                     type: String,
                     default: "i"
@@ -9672,15 +9672,15 @@
                 },
                 contentStyle: Object,
                 contentClass: [Object, Array, String],
                 square: Boolean,
                 flat: Boolean,
                 dense: Boolean
             },
-            emits: [..._a, "update:modelValue", "keydown", "click", "mouseup", "keyup", "touchend", "focus", "blur", "dropdownShow", "dropdownHide", "dropdownBeforeShow", "dropdownBeforeHide"],
+            emits: [..._a, "update:modelValue", "keydown", "click", "mouseup", "keyup", "touchend", "focus", "blur", "dropdownShow", "dropdownHide", "dropdownBeforeShow", "dropdownBeforeHide", "linkShow", "linkHide"],
             setup(t, {
                 slots: o,
                 emit: n,
                 attrs: a
             }) {
                 const {
                     proxy: l,
@@ -9995,14 +9995,16 @@
                         buttonProps: x,
                         contentRef: p,
                         buttons: S,
                         setContent: N
                     };
                 e.watch(() => t.modelValue, e => {
                     y !== e && (y = e, N(e, !0))
+                }), e.watch(m, e => {
+                    n(`link-${e?"Show":"Hide"}`)
                 });
                 const C = e.computed(() => t.toolbar && t.toolbar.length > 0),
                     q = e.computed(() => {
                         const e = {},
                             t = t => {
                                 t.key && (e[t.key] = {
                                     cmd: t.cmd,
@@ -12415,15 +12417,15 @@
             if (e.shiftKey || (c = void 0), 37 === e.keyCode || 39 === e.keyCode) {
                 e.shiftKey && void 0 === c && (c = "forward" === n.selectionDirection ? l : i);
                 const o = y[(39 === e.keyCode ? "right" : "left") + (!0 === t.reverseFillMask ? "Reverse" : "")];
                 if (e.preventDefault(), o(n, c === l ? i : l), e.shiftKey) {
                     const e = n.selectionStart;
                     n.setSelectionRange(Math.min(c, e), Math.max(c, e), "forward")
                 }
-            } else 8 === e.keyCode && !0 !== t.reverseFillMask && l === i ? y.left(n, l) : 46 === e.keyCode && !0 === t.reverseFillMask && l === i && y.rightReverse(n, i)
+            } else 8 === e.keyCode && !0 !== t.reverseFillMask && l === i ? (y.left(n, l), n.setSelectionRange(n.selectionStart, i, "backward")) : 46 === e.keyCode && !0 === t.reverseFillMask && l === i && (y.rightReverse(n, i), n.setSelectionRange(l, n.selectionEnd, "forward"))
         }
 
         function _(e) {
             if (void 0 === e || null === e || "" === e) return "";
             if (!0 === t.reverseFillMask) return S(e);
             const o = r;
             let n = 0,
@@ -23689,15 +23691,15 @@
             __proto__: null,
             useDialogPluginComponent: Xm,
             useFormChild: ds,
             useMeta: Gm,
             useQuasar: Jm
         }),
         tf = {
-            version: "2.11.8",
+            version: "2.11.10",
             install(e, t) {
                 qe(e, {
                     components: wv,
                     directives: cp,
                     plugins: Pm,
                     ...t
                 })
```

### Comparing `nicegui-1.2.6/nicegui/static/sad_face.svg` & `nicegui-1.2.7/nicegui/static/sad_face.svg`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/socket.io.min.js` & `nicegui-1.2.7/nicegui/static/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/tailwindcss.min.js` & `nicegui-1.2.7/nicegui/static/tailwindcss.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/vue.global.prod.js` & `nicegui-1.2.7/nicegui/static/vue.global.prod.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/static/vue.min.js` & `nicegui-1.2.7/nicegui/static/vue.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind.py` & `nicegui-1.2.7/nicegui/tailwind.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/accent_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/accent_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/background_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/background_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/border_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/border_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/border_radius.py` & `nicegui-1.2.7/nicegui/tailwind_types/border_radius.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/border_spacing.py` & `nicegui-1.2.7/nicegui/tailwind_types/border_spacing.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/border_width.py` & `nicegui-1.2.7/nicegui/tailwind_types/border_width.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/box_shadow_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/box_shadow_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/caret_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/caret_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/cursor.py` & `nicegui-1.2.7/nicegui/tailwind_types/cursor.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/divide_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/divide_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/fill.py` & `nicegui-1.2.7/nicegui/tailwind_types/fill.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/flex_basis.py` & `nicegui-1.2.7/nicegui/tailwind_types/flex_basis.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/gap.py` & `nicegui-1.2.7/nicegui/tailwind_types/gap.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/gradient_color_stops.py` & `nicegui-1.2.7/nicegui/tailwind_types/gradient_color_stops.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/grid_column_start_end.py` & `nicegui-1.2.7/nicegui/tailwind_types/grid_column_start_end.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/height.py` & `nicegui-1.2.7/nicegui/tailwind_types/height.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/margin.py` & `nicegui-1.2.7/nicegui/tailwind_types/margin.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/outline_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/outline_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/padding.py` & `nicegui-1.2.7/nicegui/tailwind_types/padding.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/ring_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/ring_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/ring_offset_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/ring_offset_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/scroll_margin.py` & `nicegui-1.2.7/nicegui/tailwind_types/scroll_margin.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/scroll_padding.py` & `nicegui-1.2.7/nicegui/tailwind_types/scroll_padding.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/space_between.py` & `nicegui-1.2.7/nicegui/tailwind_types/space_between.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/stroke.py` & `nicegui-1.2.7/nicegui/tailwind_types/stroke.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/text_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/text_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/text_decoration_color.py` & `nicegui-1.2.7/nicegui/tailwind_types/text_decoration_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/top_right_bottom_left.py` & `nicegui-1.2.7/nicegui/tailwind_types/top_right_bottom_left.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/translate.py` & `nicegui-1.2.7/nicegui/tailwind_types/translate.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/tailwind_types/width.py` & `nicegui-1.2.7/nicegui/tailwind_types/width.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.6/nicegui/templates/index.html` & `nicegui-1.2.7/nicegui/templates/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -26,26 +26,46 @@
     <script type="module">
       const True = true;
       const False = false;
       const None = undefined;
 
       const elements = {{ elements | safe }};
 
-      const throttles = new Set();
-      function throttle(callback, time, id) {
+      const waitingCallbacks = new Map();
+      function throttle(callback, time, leading, trailing, id) {
         if (time <= 0) {
+          // execute callback immediately and return
           callback();
           return;
         }
-        if (throttles.has(id)) return;
-        throttles.add(id);
-        callback();
-        setTimeout(() => throttles.delete(id), 1000 * time);
+        if (waitingCallbacks.has(id)) {
+          if (trailing) {
+            // update trailing callback
+            waitingCallbacks.set(id, callback);
+          }
+        } else {
+          if (leading) {
+            // execute leading callback and set timeout to block more leading callbacks
+            callback();
+            waitingCallbacks.set(id, null);
+          }
+          else if (trailing) {
+            // set trailing callback and set timeout to execute it
+            waitingCallbacks.set(id, callback);
+          }
+          if (leading || trailing) {
+            // set timeout to remove block and to execute trailing callback
+            setTimeout(() => {
+              const trailingCallback = waitingCallbacks.get(id);
+              if (trailingCallback) trailingCallback();
+              waitingCallbacks.delete(id)
+            }, 1000 * time);
+          }
+        }
       }
-
       function renderRecursively(elements, id) {
         const element = elements[id];
         const props = {
           id: element.id,
           ref: 'r' + element.id,
           class: element.class.join(' ') || undefined,
           style: Object.entries(element.style).reduce((str, [p, val]) => `${str}${p}:${val};`, '') || undefined,
@@ -54,15 +74,15 @@
         element.events.forEach((event) => {
           let event_name = 'on' + event.type[0].toLocaleUpperCase() + event.type.substring(1);
           event.specials.forEach(s => event_name += s[0].toLocaleUpperCase() + s.substring(1));
           let handler = (e) => {
             const all = typeof e !== 'object' || !event.args;
             const args = all ? e : Object.fromEntries(event.args.map(a => [a, e[a]]));
             const emitter = () => window.socket.emit("event", {id: element.id, listener_id: event.listener_id, args});
-            throttle(emitter, event.throttle, event.listener_id);
+            throttle(emitter, event.throttle, event.leading_events, event.trailing_events, event.listener_id);
             if (element.props["loopback"] === False && event.type == "update:model-value") {
               element.props["model-value"] = args;
             }
           };
           handler = Vue.withModifiers(handler, event.modifiers);
           handler = event.keys.length ? Vue.withKeys(handler, event.keys) : handler;
           if (props[event_name]) {
@@ -106,14 +126,24 @@
         }).then((result) => {
           if (request_id) {
             window.socket.emit("javascript_response", {request_id, result});
           }
         });
       }
 
+      function download(url, filename) {
+        const anchor = document.createElement("a");
+        anchor.href = url;
+        anchor.target = "_blank";
+        anchor.download = filename || "";
+        document.body.appendChild(anchor);
+        anchor.click();
+        document.body.removeChild(anchor);
+      }
+
       const app = Vue.createApp({
         data() {
           return {
             elements,
           };
         },
         render() {
@@ -137,15 +167,16 @@
           });
           window.socket.on("disconnect", () => {
             document.getElementById('popup').style.opacity = 1;
           });
           window.socket.on("update", (msg) => Object.entries(msg).forEach(([id, el]) => this.elements[el.id] = el));
           window.socket.on("run_method", (msg) => getElement(msg.id)?.[msg.name](...msg.args));
           window.socket.on("run_javascript", (msg) => runJavascript(msg['code'], msg['request_id']));
-          window.socket.on("open", (msg) => (location.href = msg));
+          window.socket.on("open", (msg) => (location.href = msg.startsWith('/') ? "{{ prefix | safe }}" + msg : msg));
+          window.socket.on("download", (msg) => download(msg.url, msg.filename));
           window.socket.on("notify", (msg) => Quasar.Notify.create(msg));
         },
       }).use(Quasar, {
         config: {
           brand: {
             primary: '#5898d4',
           },
```

### Comparing `nicegui-1.2.6/nicegui/ui.py` & `nicegui-1.2.7/nicegui/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 from .elements.textarea import Textarea as textarea
 from .elements.time import Time as time
 from .elements.toggle import Toggle as toggle
 from .elements.tooltip import Tooltip as tooltip
 from .elements.tree import Tree as tree
 from .elements.upload import Upload as upload
 from .elements.video import Video as video
+from .functions.download import download
 from .functions.html import add_body_html, add_head_html
 from .functions.javascript import run_javascript
 from .functions.notify import notify
 from .functions.open import open
 from .functions.timer import Timer as timer
 from .functions.update import update
 from .page import page
```

### Comparing `nicegui-1.2.6/pyproject.toml` & `nicegui-1.2.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nicegui"
-version = "v1.2.6"
+version = "v1.2.7"
 description = "Web User Interface with Buttons, Dialogs, Markdown, 3D Scences and Plots"
 authors = ["Zauberzeug GmbH <info@zauberzeug.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/zauberzeug/nicegui"
 keywords = ["gui", "ui", "web", "interface", "live"]
 
@@ -35,14 +35,18 @@
 debugpy = "^1.3.0"
 pytest-selenium = "^4.0.0"
 pytest-asyncio = "^0.19.0"
 pytest = "6.2.5"
 itsdangerous = "^2.1.2" # required by SessionMiddleware (see https://fastapi.tiangolo.com/?h=itsdangerous#optional-dependencies)
 isort = "^5.11.4"
 docutils = "^0.19"
+pandas = [
+    { version = "^1.0.0", markers = "python_version == '3.7'" },
+    { version = "^2.0.0", markers = "python_version >= '3.8'" },
+]
 
 [build-system]
 requires = [
     "setuptools>=30.3.0,<50",
     "poetry-core>=1.0.0"
 ]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nicegui-1.2.6/setup.py` & `nicegui-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 {':platform_machine != "i386" and platform_machine != "i686"': ['orjson>=3.8.6,<4.0.0'],
  ':python_version ~= "3.11.0"': ['matplotlib>=3.6.0,<4.0.0'],
  ':python_version ~= "3.7"': ['matplotlib>=3.5.0,<4.0.0',
                               'importlib_metadata>=6.0.0,<7.0.0']}
 
 setup_kwargs = {
     'name': 'nicegui',
-    'version': '1.2.6',
+    'version': '1.2.7',
     'description': 'Web User Interface with Buttons, Dialogs, Markdown, 3D Scences and Plots',
     'long_description': '<a href="http://nicegui.io/#about">\n  <img src="https://raw.githubusercontent.com/zauberzeug/nicegui/main/sceenshots/ui-elements-narrow.png"\n    width="200" align="right" alt="Try online!" />\n</a>\n\n# NiceGUI\n\nNiceGUI is an easy-to-use, Python-based UI framework, which shows up in your web browser.\nYou can create buttons, dialogs, Markdown, 3D scenes, plots and much more.\n\nIt is great for micro web apps, dashboards, robotics projects, smart home solutions and similar use cases.\nYou can also use it in development, for example when tweaking/configuring a machine learning algorithm or tuning motor controllers.\n\nNiceGUI is available as [PyPI package](https://pypi.org/project/nicegui/), [Docker image](https://hub.docker.com/r/zauberzeug/nicegui) and on [GitHub](https://github.com/zauberzeug/nicegui).\n\n[![PyPI version](https://badge.fury.io/py/nicegui.svg)](https://pypi.org/project/nicegui/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/nicegui)](https://pypi.org/project/nicegui/)\n[![Docker Pulls](https://img.shields.io/docker/pulls/zauberzeug/nicegui)](https://hub.docker.com/r/zauberzeug/nicegui)<br />\n[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/graphs/commit-activity)\n[![GitHub issues](https://img.shields.io/github/issues/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/issues)\n[![GitHub forks](https://img.shields.io/github/forks/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/network)\n[![GitHub stars](https://img.shields.io/github/stars/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/stargazers)\n[![GitHub license](https://img.shields.io/github/license/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/blob/main/LICENSE)\n\n## Features\n\n- browser-based graphical user interface\n- implicit reload on code change\n- standard GUI elements like label, button, checkbox, switch, slider, input, file upload, ...\n- simple grouping with rows, columns, cards and dialogs\n- general-purpose HTML and Markdown elements\n- powerful high-level elements to\n  - plot graphs and charts,\n  - render 3D scenes,\n  - get steering events via virtual joysticks\n  - annotate and overlay images\n  - interact with tables\n  - navigate foldable tree structures\n- built-in timer to refresh data in intervals (even every 10 ms)\n- straight-forward data binding to write even less code\n- notifications, dialogs and menus to provide state of the art user interaction\n- shared and individual web pages\n- ability to add custom routes and data responses\n- capture keyboard input for global shortcuts etc.\n- customize look by defining primary, secondary and accent colors\n- live-cycle events and session data\n\n## Installation\n\n```bash\npython3 -m pip install nicegui\n```\n\n## Usage\n\nWrite your nice GUI in a file `main.py`:\n\n```python\nfrom nicegui import ui\n\nui.label(\'Hello NiceGUI!\')\nui.button(\'BUTTON\', on_click=lambda: ui.notify(\'button was pressed\'))\n\nui.run()\n```\n\nLaunch it with:\n\n```bash\npython3 main.py\n```\n\nThe GUI is now available through http://localhost:8080/ in your browser.\nNote: NiceGUI will automatically reload the page when you modify the code.\n\n## Documentation and Examples\n\nThe documentation is hosted at [https://nicegui.io/documentation](https://nicegui.io/documentation) and provides plenty of live demos.\nThe whole content of [https://nicegui.io](https://nicegui.io) is [implemented with NiceGUI itself](https://github.com/zauberzeug/nicegui/blob/main/main.py).\n\nYou may also have a look at our [in-depth examples](https://github.com/zauberzeug/nicegui/tree/main/examples) of what you can do with NiceGUI.\n\n## Why?\n\nWe at [Zauberzeug](https://zauberzeug.com) like [Streamlit](https://streamlit.io/)\nbut find it does [too much magic](https://github.com/zauberzeug/nicegui/issues/1#issuecomment-847413651) when it comes to state handling.\nIn search for an alternative nice library to write simple graphical user interfaces in Python we discovered [JustPy](https://justpy.io/).\nAlthough we liked the approach, it is too "low-level HTML" for our daily usage.\nBut it inspired us to use [Vue](https://vuejs.org/) and [Quasar](https://quasar.dev/) for the frontend.\n\nWe have built on top of [FastAPI](https://fastapi.tiangolo.com/),\nwhich itself is based on the ASGI framework [Starlette](https://www.starlette.io/)\nand the ASGI webserver [Uvicorn](https://www.uvicorn.org/)\nbecause of their great performance and ease of use.\n\n## Contributing\n\nThank you for your interest in contributing to NiceGUI! We are thrilled to have you on board and appreciate your efforts to make this project even better.\n\nAs a growing open-source project, we understand that it takes a community effort to achieve our goals. That\'s why we welcome all kinds of contributions, no matter how small or big they are. Whether it\'s adding new features, fixing bugs, improving documentation, or suggesting new ideas, we believe that every contribution counts and adds value to our project.\n\nWe have provided a detailed guide on how to contribute to NiceGUI in our [CONTRIBUTING.md](https://github.com/zauberzeug/nicegui/blob/main/CONTRIBUTING.md) file. We encourage you to read it carefully before making any contributions to ensure that your work aligns with the project\'s goals and standards.\n\nIf you have any questions or need help with anything, please don\'t hesitate to reach out to us. We are always here to support and guide you through the contribution process.\n\n### Included Web Dependencies\n\nSee [DEPENDENCIES.md](https://github.com/zauberzeug/nicegui/blob/main/DEPENDENCIES.md) for a list of web frameworks NiceGUI depends on.\n',
     'author': 'Zauberzeug GmbH',
     'author_email': 'info@zauberzeug.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zauberzeug/nicegui',
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 'plotly>=5.13.0,<6.0.0', 'python-multipart>=0.0.6,<0.0.7',
 'pywebview>=4.0.2,<5.0.0', 'typing-extensions>=3.10.0', 'uvicorn
 [standard]>=0.20.0,<0.21.0', 'vbuild>=0.8.1,<0.9.0',
 'watchfiles>=0.18.1,<0.19.0'] extras_require = \ {':platform_machine != "i386"
 and platform_machine != "i686"': ['orjson>=3.8.6,<4.0.0'], ':python_version ~=
 "3.11.0"': ['matplotlib>=3.6.0,<4.0.0'], ':python_version ~= "3.7"':
 ['matplotlib>=3.5.0,<4.0.0', 'importlib_metadata>=6.0.0,<7.0.0']} setup_kwargs
-= { 'name': 'nicegui', 'version': '1.2.6', 'description': 'Web User Interface
+= { 'name': 'nicegui', 'version': '1.2.7', 'description': 'Web User Interface
 with Buttons, Dialogs, Markdown, 3D Scences and Plots', 'long_description': '\n
 n_width="200"_align="right"_alt="Try_online!"_/>\n\n\n# NiceGUI\n\nNiceGUI is
 an easy-to-use, Python-based UI framework, which shows up in your web
 browser.\nYou can create buttons, dialogs, Markdown, 3D scenes, plots and much
 more.\n\nIt is great for micro web apps, dashboards, robotics projects, smart
 home solutions and similar use cases.\nYou can also use it in development, for
 example when tweaking/configuring a machine learning algorithm or tuning motor
```

### Comparing `nicegui-1.2.6/PKG-INFO` & `nicegui-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegui
-Version: 1.2.6
+Version: 1.2.7
 Summary: Web User Interface with Buttons, Dialogs, Markdown, 3D Scences and Plots
 Home-page: https://github.com/zauberzeug/nicegui
 License: MIT
 Keywords: gui,ui,web,interface,live
 Author: Zauberzeug GmbH
 Author-email: info@zauberzeug.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nicegui Version: 1.2.6 Summary: Web User Interface
+Metadata-Version: 2.1 Name: nicegui Version: 1.2.7 Summary: Web User Interface
 with Buttons, Dialogs, Markdown, 3D Scences and Plots Home-page: https://
 github.com/zauberzeug/nicegui License: MIT Keywords: gui,ui,web,interface,live
 Author: Zauberzeug GmbH Author-email: info@zauberzeug.com Requires-Python:
 >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

