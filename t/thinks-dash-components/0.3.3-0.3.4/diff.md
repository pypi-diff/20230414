# Comparing `tmp/thinks_dash_components-0.3.3.tar.gz` & `tmp/thinks_dash_components-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.3.3.tar", last modified: Fri Apr 14 07:30:41 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.3.4.tar", last modified: Fri Apr 14 08:37:02 2023, max compression
```

## Comparing `thinks_dash_components-0.3.3.tar` & `thinks_dash_components-0.3.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 07:30:41.012270 thinks_dash_components-0.3.3/
--rw-rw-rw-   0        0        0        0 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.3/LICENSE
--rw-rw-rw-   0        0        0      464 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-04-14 07:30:41.012270 thinks_dash_components-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.3/README.md
--rw-rw-rw-   0        0        0     2320 2023-04-14 07:29:26.000000 thinks_dash_components-0.3.3/package.json
--rw-rw-rw-   0        0        0       42 2023-04-14 07:30:41.012270 thinks_dash_components-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-02-22 05:19:29.000000 thinks_dash_components-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:30:41.006286 thinks_dash_components-0.3.3/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1343 2023-04-06 01:49:20.000000 thinks_dash_components-0.3.3/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2360 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.3/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44306 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2320 2023-04-14 07:29:37.000000 thinks_dash_components-0.3.3/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   124228 2023-04-14 07:29:35.000000 thinks_dash_components-0.3.3/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-04-14 07:29:35.000000 thinks_dash_components-0.3.3/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-14 07:30:41.010275 thinks_dash_components-0.3.3/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-04-14 07:30:40.000000 thinks_dash_components-0.3.3/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-14 07:30:40.000000 thinks_dash_components-0.3.3/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 07:30:40.000000 thinks_dash_components-0.3.3/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-14 07:30:40.000000 thinks_dash_components-0.3.3/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 08:37:02.236989 thinks_dash_components-0.3.4/
+-rw-rw-rw-   0        0        0        0 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0      464 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-04-14 08:37:02.236989 thinks_dash_components-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3802 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.4/README.md
+-rw-rw-rw-   0        0        0     2320 2023-04-14 08:36:38.000000 thinks_dash_components-0.3.4/package.json
+-rw-rw-rw-   0        0        0       42 2023-04-14 08:37:02.236989 thinks_dash_components-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-02-22 05:19:29.000000 thinks_dash_components-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:37:02.232001 thinks_dash_components-0.3.4/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1343 2023-04-06 01:49:20.000000 thinks_dash_components-0.3.4/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2360 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.4/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44306 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2320 2023-04-14 08:36:51.000000 thinks_dash_components-0.3.4/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   124231 2023-04-14 08:36:50.000000 thinks_dash_components-0.3.4/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-04-14 08:36:50.000000 thinks_dash_components-0.3.4/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-14 08:37:02.235992 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-04-14 08:37:02.000000 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-04-14 08:37:02.000000 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:37:02.000000 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-14 08:37:02.000000 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.3.3/PKG-INFO` & `thinks_dash_components-0.3.4/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thinks_dash_components
-Version: 0.3.3
+Name: thinks-dash-components
+Version: 0.3.4
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.3/README.md` & `thinks_dash_components-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/package.json` & `thinks_dash_components-0.3.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.3.4'"}*

```diff
@@ -54,9 +54,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.3"
+    "version": "0.3.4"
 }
```

### Comparing `thinks_dash_components-0.3.3/setup.py` & `thinks_dash_components-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/Alert.py` & `thinks_dash_components-0.3.4/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.3.4/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.3.4/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.3.4/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.3.4/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.3.4/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.3.4/thinks_dash_components/MobileDropdown.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/Notice.py` & `thinks_dash_components-0.3.4/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.3.4/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.3.4/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.3.4/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.3.4/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.3.4/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.3.4/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.3.4/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/__init__.py` & `thinks_dash_components-0.3.4/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.3.4/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/metadata.json` & `thinks_dash_components-0.3.4/thinks_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/package-info.json` & `thinks_dash_components-0.3.4/thinks_dash_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.3.4'"}*

```diff
@@ -54,9 +54,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.3"
+    "version": "0.3.4"
 }
```

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.3.4/thinks_dash_components/thinks_dash_components.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(o()),
                 r = i(e);
             if (!t) return r;
             var n = r.split("/"),
                 a = n.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_3_3m1681457373"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_3_4m1681461408"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -173,27 +173,27 @@
             C = function(e) {
                 return j.get(e)
             },
             A = function(e, t) {
                 t >= T && (T = t + 1), k.set(e, t), j.set(t, e)
             },
             R = "style[" + S + '][data-styled-version="5.3.9"]',
-            L = new RegExp("^" + S + '\\.g(\\d+)\\[id="([\\w\\d-]+)"\\].*?"([^"]*)'),
-            I = function(e, t, r) {
+            I = new RegExp("^" + S + '\\.g(\\d+)\\[id="([\\w\\d-]+)"\\].*?"([^"]*)'),
+            L = function(e, t, r) {
                 for (var n, o = r.split(","), i = 0, a = o.length; i < a; i++)(n = o[i]) && e.registerName(t, n)
             },
             D = function(e, t) {
                 for (var r = (t.textContent || "").split("/*!sc*/\n"), n = [], o = 0, i = r.length; o < i; o++) {
                     var a = r[o].trim();
                     if (a) {
-                        var s = a.match(L);
+                        var s = a.match(I);
                         if (s) {
                             var c = 0 | parseInt(s[1], 10),
                                 u = s[2];
-                            0 !== c && (A(u, c), I(e, u, s[3]), e.getTag().insertRules(c, n)), n.length = 0
+                            0 !== c && (A(u, c), L(e, u, s[3]), e.getTag().insertRules(c, n)), n.length = 0
                         } else n.push(a)
                     }
                 }
             },
             N = function() {
                 return r.nc
             },
@@ -1000,15 +1000,15 @@
             }
             return a
         }
 
         function o(e, t) {
             var r = e.indexOf(1 === t ? ":" : "{"),
                 n = e.substring(0, 3 !== t ? r : 10);
-            return r = e.substring(r + 1, e.length - 1), L(2 !== t ? n : n.replace(E, "$1"), r, t)
+            return r = e.substring(r + 1, e.length - 1), I(2 !== t ? n : n.replace(E, "$1"), r, t)
         }
 
         function i(e, t) {
             var r = n(t, t.charCodeAt(0), t.charCodeAt(1), t.charCodeAt(2));
             return r !== t + ";" ? r.replace(S, " or ($1)").substring(4) : "(" + t + ")"
         }
 
@@ -1022,25 +1022,25 @@
                 default:
                     d = f
             }
             if (d !== t) return d
         }
 
         function s(e) {
-            return void 0 !== (e = e.prefix) && (L = null, e ? "function" != typeof e ? _ = 1 : (_ = 2, L = e) : _ = 0), s
+            return void 0 !== (e = e.prefix) && (I = null, e ? "function" != typeof e ? _ = 1 : (_ = 2, I = e) : _ = 0), s
         }
 
         function c(e, r) {
             var s = e;
             if (33 > s.charCodeAt(0) && (s = s.trim()), s = [s], 0 < R) {
                 var c = a(-1, r, s, s, j, k, 0, 0, 0, 0);
                 void 0 !== c && "string" == typeof c && (r = c)
             }
             var f = function e(r, s, c, f, p) {
-                for (var d, h, y, g, S, O = 0, E = 0, P = 0, x = 0, A = 0, L = 0, D = y = d = 0, N = 0, M = 0, B = 0, $ = 0, z = c.length, F = z - 1, U = "", G = "", W = "", X = ""; N < z;) {
+                for (var d, h, y, g, S, O = 0, E = 0, P = 0, x = 0, A = 0, I = 0, D = y = d = 0, N = 0, M = 0, B = 0, $ = 0, z = c.length, F = z - 1, U = "", G = "", W = "", X = ""; N < z;) {
                     if (h = c.charCodeAt(N), N === F && 0 !== E + x + P + O && (0 !== E && (h = 47 === E ? 10 : 47), x = P = O = 0, z++, F++), 0 === E + x + P + O) {
                         if (N === F && (0 < M && (U = U.replace(l, "")), 0 < U.trim().length)) {
                             switch (h) {
                                 case 32:
                                 case 9:
                                 case 59:
                                 case 13:
@@ -1141,15 +1141,15 @@
                                 }
                                 B = M = D = d = 0, U = "", h = c.charCodeAt(++N)
                         }
                     }
                     switch (h) {
                         case 13:
                         case 10:
-                            47 === E ? E = 0 : 0 === 1 + d && 107 !== f && 0 < U.length && (M = 1, U += "\0"), 0 < R * I && a(0, U, s, r, j, k, G.length, f, p, f), k = 1, j++;
+                            47 === E ? E = 0 : 0 === 1 + d && 107 !== f && 0 < U.length && (M = 1, U += "\0"), 0 < R * L && a(0, U, s, r, j, k, G.length, f, p, f), k = 1, j++;
                             break;
                         case 59:
                         case 125:
                             if (0 === E + x + P + O) {
                                 k++;
                                 break
                             }
@@ -1181,15 +1181,15 @@
                                     0 === x + E + O && (M = B = 1, g = "\f" + g);
                                     break;
                                 case 108:
                                     if (0 === x + E + O + T && 0 < D) switch (N - D) {
                                         case 2:
                                             112 === A && 58 === c.charCodeAt(N - 3) && (T = A);
                                         case 8:
-                                            111 === L && (T = L)
+                                            111 === I && (T = I)
                                     }
                                     break;
                                 case 58:
                                     0 === x + E + O && (D = N);
                                     break;
                                 case 44:
                                     0 === E + P + x + O && (M = 1, g += "\r");
@@ -1205,15 +1205,15 @@
                                     0 === x + E + P && O--;
                                     break;
                                 case 41:
                                     0 === x + E + O && P--;
                                     break;
                                 case 40:
                                     if (0 === x + E + O) {
-                                        if (0 === d) switch (2 * A + 3 * L) {
+                                        if (0 === d) switch (2 * A + 3 * I) {
                                             case 533:
                                                 break;
                                             default:
                                                 d = 1
                                         }
                                         P++
                                     }
@@ -1235,15 +1235,15 @@
                                             break;
                                         case 42:
                                             47 === h && 42 === A && $ + 2 !== N && (33 === c.charCodeAt($ + 2) && (G += c.substring($, N + 1)), g = "", E = 0)
                                     }
                             }
                             0 === E && (U += g)
                     }
-                    L = A, A = h, N++
+                    I = A, A = h, N++
                 }
                 if (0 < ($ = G.length)) {
                     if (M = s, 0 < R && (void 0 !== (S = a(2, G, M, r, j, k, $, f, p, f)) && 0 === (G = S).length)) return X + G + W;
                     if (G = M.join(",") + "{" + G + "}", 0 != _ * T) {
                         switch (2 !== _ || o(G, 2) || (T = 0), T) {
                             case 111:
                                 G = G.replace(b, ":-moz-$1") + G;
@@ -1278,27 +1278,27 @@
             k = 1,
             j = 1,
             T = 0,
             _ = 1,
             C = [],
             A = [],
             R = 0,
-            L = null,
-            I = 0;
+            I = null,
+            L = 0;
         return c.use = function e(t) {
             switch (t) {
                 case void 0:
                 case null:
                     R = A.length = 0;
                     break;
                 default:
                     if ("function" == typeof t) A[R++] = t;
                     else if ("object" == typeof t)
                         for (var r = 0, n = t.length; r < n; ++r) e(t[r]);
-                    else I = 0 | !!t
+                    else L = 0 | !!t
             }
             return e
         }, c.set = s, void 0 !== e && s(e), c
     }
 }, function(e, t, r) {
     "use strict";
     t.a = {
@@ -1760,15 +1760,15 @@
             return e.duration
         })),
         T = y.a.div(a || (a = P(["\n    padding: 15px 0 20px;\n    background-color: white;\n    border-radius: 10px;\n    display: flex;\n    flex-direction: column;\n    width: 100%;\n"]))),
         _ = y.a.div(s || (s = P(["\n    border-bottom: solid thin black;\n    padding: 5px 30px;\n"]))),
         C = y.a.div(c || (c = P(["\n    padding: 10px 30px;\n"]))),
         A = y.a.div(u || (u = P(["\n    display: flex;\n    justify-content: flex-end;\n    gap: 10px;\n    padding: 0 30px;\n    box-sizing: content-box;\n"]))),
         R = y.a.button(l || (l = P(["\n    flex: 1;\n    padding: 3px 0;\n    background-color: ", ";\n    border-radius: 9999px;\n    border: solid thin ", ";\n    color: white;\n"])), "#00000099", "#00000099"),
-        L = function(e) {
+        I = function(e) {
             ! function(e, t) {
                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                 e.prototype = Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
@@ -1885,16 +1885,16 @@
                     }, c)))
                 }
             }]) && g(t.prototype, r), n && g(t, n), Object.defineProperty(t, "prototype", {
                 writable: !1
             }), i
         }(d.Component);
 
-    function I(e) {
-        return (I = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function L(e) {
+        return (L = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function D(e, t) {
@@ -1958,23 +1958,23 @@
         return n
     }
 
     function M(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, (o = n.key, i = void 0, i = function(e, t) {
-                if ("object" !== I(e) || null === e) return e;
+                if ("object" !== L(e) || null === e) return e;
                 var r = e[Symbol.toPrimitive];
                 if (void 0 !== r) {
                     var n = r.call(e, t || "default");
-                    if ("object" !== I(n)) return n;
+                    if ("object" !== L(n)) return n;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
-            }(o, "string"), "symbol" === I(i) ? i : String(i)), n)
+            }(o, "string"), "symbol" === L(i) ? i : String(i)), n)
         }
         var o, i
     }
 
     function B(e, t) {
         return (B = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
@@ -1999,31 +1999,31 @@
                 r = Reflect.construct(n, arguments, o)
             } else r = n.apply(this, arguments);
             return z(this, r)
         }
     }
 
     function z(e, t) {
-        if (t && ("object" === I(t) || "function" == typeof t)) return t;
+        if (t && ("object" === L(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
     function F(e) {
         return (F = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
-    L.defaultProps = {
+    I.defaultProps = {
         is_open: !1,
         duration: 150
-    }, L.propTypes = {
+    }, I.propTypes = {
         id: p.a.string,
         message: p.a.node.isRequired,
         title: p.a.node,
         buttons: p.a.arrayOf(p.a.object).isRequired,
         value: p.a.oneOfType([p.a.string, p.a.number]),
         is_open: p.a.bool,
         duration: p.a.number,
@@ -3497,22 +3497,22 @@
         delay: p.a.number,
         interval: p.a.number,
         ignores: p.a.arrayOf(p.a.string),
         is_loading: p.a.bool,
         is_stop: p.a.bool,
         setProps: p.a.func
     };
-    var ke, je, Te, _e, Ce, Ae, Re, Le = {
+    var ke, je, Te, _e, Ce, Ae, Re, Ie = {
             color: void 0,
             size: void 0,
             className: void 0,
             style: void 0,
             attr: void 0
         },
-        Ie = h.a.createContext && h.a.createContext(Le),
+        Le = h.a.createContext && h.a.createContext(Ie),
         De = function() {
             return (De = Object.assign || function(e) {
                 for (var t, r = 1, n = arguments.length; r < n; r++)
                     for (var o in t = arguments[r]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
             }).apply(this, arguments)
         },
@@ -3557,17 +3557,17 @@
                     color: e.color || t.color
                 }, t.style), e.style),
                 height: s,
                 width: s,
                 xmlns: "http://www.w3.org/2000/svg"
             }), i && h.a.createElement("title", null, i), e.children)
         };
-        return void 0 !== Ie ? h.a.createElement(Ie.Consumer, null, (function(e) {
+        return void 0 !== Le ? h.a.createElement(Le.Consumer, null, (function(e) {
             return t(e)
-        })) : t(Le)
+        })) : t(Ie)
     }
 
     function $e(e) {
         return Me({
             tag: "svg",
             attr: {
                 viewBox: "0 0 16 16",
@@ -4387,15 +4387,15 @@
         return (Rt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function Lt(e, t) {
+    function It(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, (o = n.key, i = void 0, i = function(e, t) {
                 if ("object" !== Rt(e) || null === e) return e;
                 var r = e[Symbol.toPrimitive];
                 if (void 0 !== r) {
                     var n = r.call(e, t || "default");
@@ -4404,16 +4404,16 @@
                 }
                 return ("string" === t ? String : Number)(e)
             }(o, "string"), "symbol" === Rt(i) ? i : String(i)), n)
         }
         var o, i
     }
 
-    function It(e, t) {
-        return (It = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+    function Lt(e, t) {
+        return (Lt = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
     function Dt(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
@@ -4486,33 +4486,33 @@
                 constructor: {
                     value: e,
                     writable: !0,
                     configurable: !0
                 }
             }), Object.defineProperty(e, "prototype", {
                 writable: !1
-            }), t && It(e, t)
+            }), t && Lt(e, t)
         }(i, e);
         var t, r, n, o = Dt(i);
 
         function i(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
             }(this, i), (t = o.call(this, e)).state = {
                 clear: !1
-            }, t.LAST_OPERATE_KEY = "last_operate", t.interval = null, t.setLastOperate = t.saveLastOperate.bind(Mt(t)), t
+            }, t.LAST_OPERATE_KEY = "last_operate", t.interval = null, t.saveLastOperate = t.saveLastOperate.bind(Mt(t)), t
         }
         return t = i, (r = [{
             key: "componentDidMount",
             value: function() {
                 var e = this;
                 this.saveLastOperate(), window.addEventListener("touchstart", this.saveLastOperate), window.addEventListener("touchend", this.saveLastOperate), window.addEventListener("touchmove", this.saveLastOperate), this.interval = setInterval((function() {
                     var t = sessionStorage.getItem(e.LAST_OPERATE_KEY);
-                    sessionStorage.length > 1 && Date.now() - Number(t) > e.props.limit && (sessionStorage.clear(), console.log("-- STORAGE OBSERVER CLEAR"), e.props.setProps({
+                    sessionStorage.length > 1 && Date.now() - Number(t) > e.props.limit && (sessionStorage.clear(), console.log("-- OPERATION OBSERVER CLEAR"), e.props.setProps({
                         clear: !0
                     }))
                 }), this.props.interval)
             }
         }, {
             key: "componentWillUnmount",
             value: function() {
@@ -4529,15 +4529,15 @@
             key: "render",
             value: function() {
                 var e = this.props.id;
                 return h.a.createElement("div", {
                     id: e
                 })
             }
-        }]) && Lt(t.prototype, r), n && Lt(t, n), Object.defineProperty(t, "prototype", {
+        }]) && It(t.prototype, r), n && It(t, n), Object.defineProperty(t, "prototype", {
             writable: !1
         }), i
     }(d.Component);
 
     function Ft(e) {
         return (Ft = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
@@ -5413,15 +5413,15 @@
         value: 0
     }, jr.propTypes = {
         id: p.a.string,
         value: p.a.oneOfType([p.a.number, p.a.string]),
         className: p.a.string,
         setProps: p.a.func
     }, r.d(t, "Alert", (function() {
-        return L
+        return I
     })), r.d(t, "DesignableRadioItems", (function() {
         return U
     })), r.d(t, "IndexedDB", (function() {
         return ie
     })), r.d(t, "InputNumber", (function() {
         return jr
     })), r.d(t, "IosScrollWrapper", (function() {
```

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thinks-dash-components
-Version: 0.3.3
+Name: thinks_dash_components
+Version: 0.3.4
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.3/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.3.4/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

