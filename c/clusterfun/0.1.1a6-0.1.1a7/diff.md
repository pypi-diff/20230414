# Comparing `tmp/clusterfun-0.1.1a6.tar.gz` & `tmp/clusterfun-0.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterfun-0.1.1a6.tar", max compression
+gzip compressed data, was "clusterfun-0.1.1a7.tar", max compression
```

## Comparing `clusterfun-0.1.1a6.tar` & `clusterfun-0.1.1a7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     2124 2023-03-23 23:47:08.757953 clusterfun-0.1.1a6/README.md
--rw-r--r--   0        0        0      479 2023-04-10 13:24:09.476276 clusterfun-0.1.1a6/clusterfun/__init__.py
--rw-r--r--   0        0        0      970 2023-04-12 21:50:47.811062 clusterfun-0.1.1a6/clusterfun/app.py
--rw-r--r--   0        0        0     1898 2023-04-10 15:12:23.404213 clusterfun-0.1.1a6/clusterfun/config.py
--rw-r--r--   0        0        0      715 2023-04-10 13:24:09.475338 clusterfun-0.1.1a6/clusterfun/constants.py
--rw-r--r--   0        0        0     2271 2023-04-12 19:26:39.848095 clusterfun-0.1.1a6/clusterfun/frontend/404/index.html
--rw-r--r--   0        0        0     2271 2023-04-12 19:26:39.828544 clusterfun-0.1.1a6/clusterfun/frontend/404.html
--rw-r--r--   0        0        0      737 2023-04-12 19:26:39.447836 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/1QyiY8tsv4hAH3HR9ReVe/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-04-12 19:26:39.447866 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/1QyiY8tsv4hAH3HR9ReVe/_ssgManifest.js
--rw-r--r--   0        0        0     1719 2023-04-12 19:26:39.448090 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/311.6371271c6213fe76.js
--rw-r--r--   0        0        0     8320 2023-04-12 19:26:39.448238 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/500-fee090358e8ae436.js
--rw-r--r--   0        0        0     8227 2023-04-12 19:26:39.448152 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/660.8e595c259eac1e04.js
--rw-r--r--   0        0        0     1212 2023-04-12 19:26:39.448388 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/811.55af53aff1479292.js
--rw-r--r--   0        0        0    59584 2023-04-12 19:26:39.448663 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/845-6e5cd4484d87bcf7.js
--rw-r--r--   0        0        0  3560332 2023-04-12 19:26:39.454811 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/e48519b3.5f5de64206d77e57.js
--rw-r--r--   0        0        0   141052 2023-04-12 19:26:39.449284 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0        0        0    90774 2023-04-12 19:26:39.449417 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/main-a028e25a41b5197e.js
--rw-r--r--   0        0        0      523 2023-04-12 19:26:39.450545 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/_app-7113ace39c1058aa.js
--rw-r--r--   0        0        0      247 2023-04-12 19:26:39.450636 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/_error-54de1933a164a1ff.js
--rw-r--r--   0        0        0     5571 2023-04-12 19:26:39.450723 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/index-d8c33fb679044d17.js
--rw-r--r--   0        0        0    11447 2023-04-12 19:26:39.451388 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]/grid-1b39229fdd12f891.js
--rw-r--r--   0        0        0     1780 2023-04-12 19:26:39.451594 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]/media/[mediaIndex]-65fd1e6cacd5b598.js
--rw-r--r--   0        0        0     5127 2023-04-12 19:26:39.451068 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]-2ebd00dc8e38d508.js
--rw-r--r--   0        0        0    91460 2023-04-12 19:26:39.449900 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3235 2023-04-12 19:26:39.449802 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/webpack-a45339d45be8fd42.js
--rw-r--r--   0        0        0   275169 2023-04-12 19:26:39.448906 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/css/367d53e6bb6fad91.css
--rw-r--r--   0        0        0   121340 2023-04-12 19:26:39.450114 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/media/bootstrap-icons.02685dab.woff2
--rw-r--r--   0        0        0   164360 2023-04-12 19:26:39.450428 clusterfun-0.1.1a6/clusterfun/frontend/_next/static/media/bootstrap-icons.8463cb1e.woff
--rw-r--r--   0        0        0     2413 2023-04-12 19:26:39.789883 clusterfun-0.1.1a6/clusterfun/frontend/index.html
--rw-r--r--   0        0        0     3006 2023-04-12 22:32:28.951213 clusterfun-0.1.1a6/clusterfun/main.py
--rw-r--r--   0        0        0        0 2023-04-10 13:24:09.484470 clusterfun-0.1.1a6/clusterfun/models/__init__.py
--rw-r--r--   0        0        0     3099 2023-04-12 22:32:29.005237 clusterfun-0.1.1a6/clusterfun/models/filter.py
--rw-r--r--   0        0        0     1034 2023-04-10 13:50:11.406451 clusterfun-0.1.1a6/clusterfun/models/media_indices.py
--rw-r--r--   0        0        0     1207 2023-04-12 22:32:28.996729 clusterfun-0.1.1a6/clusterfun/models/media_item.py
--rw-r--r--   0        0        0     7812 2023-04-12 22:32:28.927076 clusterfun-0.1.1a6/clusterfun/plot.py
--rw-r--r--   0        0        0     1183 2023-04-10 13:24:09.531751 clusterfun-0.1.1a6/clusterfun/plot_types/__init__.py
--rw-r--r--   0        0        0     1146 2023-04-10 13:24:09.530379 clusterfun-0.1.1a6/clusterfun/plot_types/grid.py
--rw-r--r--   0        0        0     4248 2023-04-12 22:32:29.041902 clusterfun-0.1.1a6/clusterfun/plot_types/histogram.py
--rw-r--r--   0        0        0     6119 2023-04-10 13:24:09.532587 clusterfun-0.1.1a6/clusterfun/plot_types/pie_chart.py
--rw-r--r--   0        0        0     1356 2023-04-10 14:24:18.607363 clusterfun-0.1.1a6/clusterfun/plot_types/scatter.py
--rw-r--r--   0        0        0     4277 2023-04-12 22:32:29.051052 clusterfun-0.1.1a6/clusterfun/plot_types/violin.py
--rw-r--r--   0        0        0     2180 2023-04-12 22:30:50.608767 clusterfun-0.1.1a6/clusterfun/serve_cli.py
--rw-r--r--   0        0        0        0 2023-04-10 13:24:09.508798 clusterfun-0.1.1a6/clusterfun/storage/__init__.py
--rw-r--r--   0        0        0     2238 2023-04-12 22:32:29.017793 clusterfun-0.1.1a6/clusterfun/storage/loader.py
--rw-r--r--   0        0        0        0 2023-04-10 13:24:09.517519 clusterfun-0.1.1a6/clusterfun/storage/local/__init__.py
--rw-r--r--   0        0        0     5387 2023-04-12 22:32:29.034368 clusterfun-0.1.1a6/clusterfun/storage/local/data.py
--rw-r--r--   0        0        0     4353 2023-04-12 19:23:39.480104 clusterfun-0.1.1a6/clusterfun/storage/local/helpers.py
--rw-r--r--   0        0        0     4269 2023-04-12 22:32:29.028932 clusterfun-0.1.1a6/clusterfun/storage/local/loader.py
--rw-r--r--   0        0        0     2463 2023-04-12 22:32:29.024185 clusterfun-0.1.1a6/clusterfun/storage/local/storer.py
--rw-r--r--   0        0        0     2753 2023-04-12 22:32:29.014387 clusterfun-0.1.1a6/clusterfun/storage/storer.py
--rw-r--r--   0        0        0        0 2023-04-10 13:24:09.477881 clusterfun-0.1.1a6/clusterfun/utils/__init__.py
--rw-r--r--   0        0        0     1064 2023-04-10 13:24:09.481772 clusterfun-0.1.1a6/clusterfun/utils/s3.py
--rw-r--r--   0        0        0     2258 2023-04-10 13:24:09.546097 clusterfun-0.1.1a6/clusterfun/validation.py
--rw-r--r--   0        0        0      968 2023-04-14 20:25:45.648519 clusterfun-0.1.1a6/pyproject.toml
--rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 clusterfun-0.1.1a6/setup.py
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 clusterfun-0.1.1a6/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-04-14 20:35:58.043163 clusterfun-0.1.1a7/README.md
+-rw-r--r--   0        0        0      479 2023-04-10 13:24:09.476276 clusterfun-0.1.1a7/clusterfun/__init__.py
+-rw-r--r--   0        0        0      970 2023-04-12 21:50:47.811062 clusterfun-0.1.1a7/clusterfun/app.py
+-rw-r--r--   0        0        0     1898 2023-04-10 15:12:23.404213 clusterfun-0.1.1a7/clusterfun/config.py
+-rw-r--r--   0        0        0      715 2023-04-10 13:24:09.475338 clusterfun-0.1.1a7/clusterfun/constants.py
+-rw-r--r--   0        0        0     2271 2023-04-12 19:26:39.848095 clusterfun-0.1.1a7/clusterfun/frontend/404/index.html
+-rw-r--r--   0        0        0     2271 2023-04-12 19:26:39.828544 clusterfun-0.1.1a7/clusterfun/frontend/404.html
+-rw-r--r--   0        0        0      737 2023-04-12 19:26:39.447836 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/1QyiY8tsv4hAH3HR9ReVe/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-04-12 19:26:39.447866 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/1QyiY8tsv4hAH3HR9ReVe/_ssgManifest.js
+-rw-r--r--   0        0        0     1719 2023-04-12 19:26:39.448090 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/311.6371271c6213fe76.js
+-rw-r--r--   0        0        0     8320 2023-04-12 19:26:39.448238 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/500-fee090358e8ae436.js
+-rw-r--r--   0        0        0     8227 2023-04-12 19:26:39.448152 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/660.8e595c259eac1e04.js
+-rw-r--r--   0        0        0     1212 2023-04-12 19:26:39.448388 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/811.55af53aff1479292.js
+-rw-r--r--   0        0        0    59584 2023-04-12 19:26:39.448663 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/845-6e5cd4484d87bcf7.js
+-rw-r--r--   0        0        0  3560332 2023-04-12 19:26:39.454811 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/e48519b3.5f5de64206d77e57.js
+-rw-r--r--   0        0        0   141052 2023-04-12 19:26:39.449284 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0        0        0    90774 2023-04-12 19:26:39.449417 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/main-a028e25a41b5197e.js
+-rw-r--r--   0        0        0      523 2023-04-12 19:26:39.450545 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/_app-7113ace39c1058aa.js
+-rw-r--r--   0        0        0      247 2023-04-12 19:26:39.450636 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+-rw-r--r--   0        0        0     5571 2023-04-12 19:26:39.450723 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/index-d8c33fb679044d17.js
+-rw-r--r--   0        0        0    11447 2023-04-12 19:26:39.451388 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]/grid-1b39229fdd12f891.js
+-rw-r--r--   0        0        0     1780 2023-04-12 19:26:39.451594 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]/media/[mediaIndex]-65fd1e6cacd5b598.js
+-rw-r--r--   0        0        0     5127 2023-04-12 19:26:39.451068 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]-2ebd00dc8e38d508.js
+-rw-r--r--   0        0        0    91460 2023-04-12 19:26:39.449900 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3235 2023-04-12 19:26:39.449802 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/webpack-a45339d45be8fd42.js
+-rw-r--r--   0        0        0   275169 2023-04-12 19:26:39.448906 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/css/367d53e6bb6fad91.css
+-rw-r--r--   0        0        0   121340 2023-04-12 19:26:39.450114 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/media/bootstrap-icons.02685dab.woff2
+-rw-r--r--   0        0        0   164360 2023-04-12 19:26:39.450428 clusterfun-0.1.1a7/clusterfun/frontend/_next/static/media/bootstrap-icons.8463cb1e.woff
+-rw-r--r--   0        0        0     2413 2023-04-12 19:26:39.789883 clusterfun-0.1.1a7/clusterfun/frontend/index.html
+-rw-r--r--   0        0        0     3006 2023-04-12 22:32:28.951213 clusterfun-0.1.1a7/clusterfun/main.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:24:09.484470 clusterfun-0.1.1a7/clusterfun/models/__init__.py
+-rw-r--r--   0        0        0     3099 2023-04-12 22:32:29.005237 clusterfun-0.1.1a7/clusterfun/models/filter.py
+-rw-r--r--   0        0        0     1034 2023-04-10 13:50:11.406451 clusterfun-0.1.1a7/clusterfun/models/media_indices.py
+-rw-r--r--   0        0        0     1207 2023-04-12 22:32:28.996729 clusterfun-0.1.1a7/clusterfun/models/media_item.py
+-rw-r--r--   0        0        0     7812 2023-04-12 22:32:28.927076 clusterfun-0.1.1a7/clusterfun/plot.py
+-rw-r--r--   0        0        0     1183 2023-04-10 13:24:09.531751 clusterfun-0.1.1a7/clusterfun/plot_types/__init__.py
+-rw-r--r--   0        0        0     1146 2023-04-10 13:24:09.530379 clusterfun-0.1.1a7/clusterfun/plot_types/grid.py
+-rw-r--r--   0        0        0     4248 2023-04-12 22:32:29.041902 clusterfun-0.1.1a7/clusterfun/plot_types/histogram.py
+-rw-r--r--   0        0        0     6119 2023-04-10 13:24:09.532587 clusterfun-0.1.1a7/clusterfun/plot_types/pie_chart.py
+-rw-r--r--   0        0        0     1356 2023-04-10 14:24:18.607363 clusterfun-0.1.1a7/clusterfun/plot_types/scatter.py
+-rw-r--r--   0        0        0     4277 2023-04-12 22:32:29.051052 clusterfun-0.1.1a7/clusterfun/plot_types/violin.py
+-rw-r--r--   0        0        0     2180 2023-04-12 22:30:50.608767 clusterfun-0.1.1a7/clusterfun/serve_cli.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:24:09.508798 clusterfun-0.1.1a7/clusterfun/storage/__init__.py
+-rw-r--r--   0        0        0     2238 2023-04-12 22:32:29.017793 clusterfun-0.1.1a7/clusterfun/storage/loader.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:24:09.517519 clusterfun-0.1.1a7/clusterfun/storage/local/__init__.py
+-rw-r--r--   0        0        0     5387 2023-04-12 22:32:29.034368 clusterfun-0.1.1a7/clusterfun/storage/local/data.py
+-rw-r--r--   0        0        0     4353 2023-04-12 19:23:39.480104 clusterfun-0.1.1a7/clusterfun/storage/local/helpers.py
+-rw-r--r--   0        0        0     4269 2023-04-12 22:32:29.028932 clusterfun-0.1.1a7/clusterfun/storage/local/loader.py
+-rw-r--r--   0        0        0     2463 2023-04-12 22:32:29.024185 clusterfun-0.1.1a7/clusterfun/storage/local/storer.py
+-rw-r--r--   0        0        0     2753 2023-04-12 22:32:29.014387 clusterfun-0.1.1a7/clusterfun/storage/storer.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:24:09.477881 clusterfun-0.1.1a7/clusterfun/utils/__init__.py
+-rw-r--r--   0        0        0     1064 2023-04-10 13:24:09.481772 clusterfun-0.1.1a7/clusterfun/utils/s3.py
+-rw-r--r--   0        0        0     2258 2023-04-10 13:24:09.546097 clusterfun-0.1.1a7/clusterfun/validation.py
+-rw-r--r--   0        0        0      968 2023-04-14 20:36:02.831704 clusterfun-0.1.1a7/pyproject.toml
+-rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 clusterfun-0.1.1a7/setup.py
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 clusterfun-0.1.1a7/PKG-INFO
```

### Comparing `clusterfun-0.1.1a6/clusterfun/app.py` & `clusterfun-0.1.1a7/clusterfun/app.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/config.py` & `clusterfun-0.1.1a7/clusterfun/config.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/constants.py` & `clusterfun-0.1.1a7/clusterfun/constants.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/404/index.html` & `clusterfun-0.1.1a7/clusterfun/frontend/404/index.html`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/404.html` & `clusterfun-0.1.1a7/clusterfun/frontend/404.html`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/1QyiY8tsv4hAH3HR9ReVe/_buildManifest.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/1QyiY8tsv4hAH3HR9ReVe/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/311.6371271c6213fe76.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/311.6371271c6213fe76.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/500-fee090358e8ae436.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/500-fee090358e8ae436.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/660.8e595c259eac1e04.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/660.8e595c259eac1e04.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/811.55af53aff1479292.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/811.55af53aff1479292.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/845-6e5cd4484d87bcf7.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/845-6e5cd4484d87bcf7.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/e48519b3.5f5de64206d77e57.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/e48519b3.5f5de64206d77e57.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/main-a028e25a41b5197e.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/main-a028e25a41b5197e.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/_app-7113ace39c1058aa.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/_app-7113ace39c1058aa.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/index-d8c33fb679044d17.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/index-d8c33fb679044d17.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]/grid-1b39229fdd12f891.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]/grid-1b39229fdd12f891.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]/media/[mediaIndex]-65fd1e6cacd5b598.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]/media/[mediaIndex]-65fd1e6cacd5b598.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]-2ebd00dc8e38d508.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/pages/plots/[uuid]-2ebd00dc8e38d508.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/chunks/webpack-a45339d45be8fd42.js` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/chunks/webpack-a45339d45be8fd42.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/css/367d53e6bb6fad91.css` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/css/367d53e6bb6fad91.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/media/bootstrap-icons.02685dab.woff2` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/media/bootstrap-icons.02685dab.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/_next/static/media/bootstrap-icons.8463cb1e.woff` & `clusterfun-0.1.1a7/clusterfun/frontend/_next/static/media/bootstrap-icons.8463cb1e.woff`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/frontend/index.html` & `clusterfun-0.1.1a7/clusterfun/frontend/index.html`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/main.py` & `clusterfun-0.1.1a7/clusterfun/main.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/models/filter.py` & `clusterfun-0.1.1a7/clusterfun/models/filter.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/models/media_indices.py` & `clusterfun-0.1.1a7/clusterfun/models/media_indices.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/models/media_item.py` & `clusterfun-0.1.1a7/clusterfun/models/media_item.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/plot.py` & `clusterfun-0.1.1a7/clusterfun/plot.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/plot_types/__init__.py` & `clusterfun-0.1.1a7/clusterfun/plot_types/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/plot_types/grid.py` & `clusterfun-0.1.1a7/clusterfun/plot_types/grid.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/plot_types/histogram.py` & `clusterfun-0.1.1a7/clusterfun/plot_types/histogram.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/plot_types/pie_chart.py` & `clusterfun-0.1.1a7/clusterfun/plot_types/pie_chart.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/plot_types/scatter.py` & `clusterfun-0.1.1a7/clusterfun/plot_types/scatter.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/plot_types/violin.py` & `clusterfun-0.1.1a7/clusterfun/plot_types/violin.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/serve_cli.py` & `clusterfun-0.1.1a7/clusterfun/serve_cli.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/storage/loader.py` & `clusterfun-0.1.1a7/clusterfun/storage/loader.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/storage/local/data.py` & `clusterfun-0.1.1a7/clusterfun/storage/local/data.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/storage/local/helpers.py` & `clusterfun-0.1.1a7/clusterfun/storage/local/helpers.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/storage/local/loader.py` & `clusterfun-0.1.1a7/clusterfun/storage/local/loader.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/storage/local/storer.py` & `clusterfun-0.1.1a7/clusterfun/storage/local/storer.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/storage/storer.py` & `clusterfun-0.1.1a7/clusterfun/storage/storer.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/utils/s3.py` & `clusterfun-0.1.1a7/clusterfun/utils/s3.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/clusterfun/validation.py` & `clusterfun-0.1.1a7/clusterfun/validation.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.1.1a6/pyproject.toml` & `clusterfun-0.1.1a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clusterfun"
-version = "0.1.1a6"
+version = "0.1.1a7"
 description = "Clusterfun - a plotting library to inspect data"
 authors = ["Jochem Gietema <jochem@giete.ma>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 pandas = "*"
```

