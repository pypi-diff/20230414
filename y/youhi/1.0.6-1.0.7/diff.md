# Comparing `tmp/youhi-1.0.6.tar.gz` & `tmp/youhi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youhi-1.0.6.tar", last modified: Wed Mar 29 09:35:54 2023, max compression
+gzip compressed data, was "youhi-1.0.7.tar", last modified: Fri Apr 14 07:44:51 2023, max compression
```

## Comparing `youhi-1.0.6.tar` & `youhi-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-29 09:35:54.381003 youhi-1.0.6/
--rw-r--r--   0 eric       (501) staff       (20)     1069 2023-03-29 08:22:05.000000 youhi-1.0.6/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      108 2023-03-29 09:22:12.000000 youhi-1.0.6/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)     1315 2023-03-29 09:35:54.380856 youhi-1.0.6/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1017 2023-03-29 08:22:05.000000 youhi-1.0.6/README.md
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-03-29 09:35:54.381056 youhi-1.0.6/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      783 2023-03-29 08:57:08.000000 youhi-1.0.6/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-29 09:35:54.379799 youhi-1.0.6/youhi/
--rw-r--r--   0 eric       (501) staff       (20)     1341 2023-03-29 09:35:49.000000 youhi-1.0.6/youhi/Button.py
--rw-r--r--   0 eric       (501) staff       (20)      924 2023-03-29 09:35:49.000000 youhi-1.0.6/youhi/Youhi.py
--rw-r--r--   0 eric       (501) staff       (20)     1637 2023-03-29 08:22:05.000000 youhi-1.0.6/youhi/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)       92 2023-03-29 09:35:49.000000 youhi-1.0.6/youhi/_imports_.py
--rw-r--r--   0 eric       (501) staff       (20)     2015 2023-03-29 09:35:49.000000 youhi-1.0.6/youhi/metadata.json
--rw-r--r--   0 eric       (501) staff       (20)     1125 2023-03-29 09:35:48.000000 youhi-1.0.6/youhi/package.json
--rw-r--r--   0 eric       (501) staff       (20)    10156 2023-03-29 09:19:44.000000 youhi-1.0.6/youhi/style.css
--rw-r--r--   0 eric       (501) staff       (20)     1386 2023-03-29 09:19:45.000000 youhi-1.0.6/youhi/youhi.js
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-29 09:35:54.380618 youhi-1.0.6/youhi.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     1315 2023-03-29 09:35:54.000000 youhi-1.0.6/youhi.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      292 2023-03-29 09:35:54.000000 youhi-1.0.6/youhi.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-03-29 09:35:54.000000 youhi-1.0.6/youhi.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)        6 2023-03-29 09:35:54.000000 youhi-1.0.6/youhi.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-14 07:44:51.502147 youhi-1.0.7/
+-rw-r--r--   0 eric       (501) staff       (20)     1069 2023-03-29 08:22:05.000000 youhi-1.0.7/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      108 2023-03-29 09:22:12.000000 youhi-1.0.7/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)     1315 2023-04-14 07:44:51.501911 youhi-1.0.7/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1017 2023-03-29 08:22:05.000000 youhi-1.0.7/README.md
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-04-14 07:44:51.502191 youhi-1.0.7/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      783 2023-04-14 07:42:52.000000 youhi-1.0.7/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-14 07:44:51.501224 youhi-1.0.7/youhi/
+-rw-r--r--   0 eric       (501) staff       (20)     1341 2023-04-14 07:44:45.000000 youhi-1.0.7/youhi/Button.py
+-rw-r--r--   0 eric       (501) staff       (20)     1390 2023-04-14 07:44:45.000000 youhi-1.0.7/youhi/MenuTrigger.py
+-rw-r--r--   0 eric       (501) staff       (20)      924 2023-04-14 07:44:45.000000 youhi-1.0.7/youhi/Youhi.py
+-rw-r--r--   0 eric       (501) staff       (20)     1637 2023-03-29 08:22:05.000000 youhi-1.0.7/youhi/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      148 2023-04-14 07:44:45.000000 youhi-1.0.7/youhi/_imports_.py
+-rw-r--r--   0 eric       (501) staff       (20)     3177 2023-04-14 07:44:45.000000 youhi-1.0.7/youhi/metadata.json
+-rw-r--r--   0 eric       (501) staff       (20)     1125 2023-04-14 07:44:44.000000 youhi-1.0.7/youhi/package.json
+-rw-r--r--   0 eric       (501) staff       (20)    10156 2023-03-29 09:19:44.000000 youhi-1.0.7/youhi/style.css
+-rw-r--r--   0 eric       (501) staff       (20)     1894 2023-04-14 07:33:29.000000 youhi-1.0.7/youhi/youhi.js
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-14 07:44:51.501696 youhi-1.0.7/youhi.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     1315 2023-04-14 07:44:51.000000 youhi-1.0.7/youhi.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      313 2023-04-14 07:44:51.000000 youhi-1.0.7/youhi.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-14 07:44:51.000000 youhi-1.0.7/youhi.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)        6 2023-04-14 07:44:51.000000 youhi-1.0.7/youhi.egg-info/top_level.txt
```

### Comparing `youhi-1.0.6/LICENSE` & `youhi-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `youhi-1.0.6/PKG-INFO` & `youhi-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youhi
-Version: 1.0.6
+Version: 1.0.7
 Summary: Plotly dash React component UI library boilerplate
 Home-page: UNKNOWN
 Author: thesameeric <osivwiokiti@gmail.com>
 License: MIT
 Platform: UNKNOWN
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
```

### Comparing `youhi-1.0.6/README.md` & `youhi-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `youhi-1.0.6/setup.py` & `youhi-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `youhi-1.0.6/youhi/Button.py` & `youhi-1.0.7/youhi/Button.py`

 * *Files identical despite different names*

### Comparing `youhi-1.0.6/youhi/Youhi.py` & `youhi-1.0.7/youhi/Youhi.py`

 * *Files identical despite different names*

### Comparing `youhi-1.0.6/youhi/__init__.py` & `youhi-1.0.7/youhi/__init__.py`

 * *Files identical despite different names*

### Comparing `youhi-1.0.6/youhi/metadata.json` & `youhi-1.0.7/youhi/metadata.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'src/ts/components/MenuTrigger.tsx'": "OrderedDict([('displayName', 'MenuTrigger'), "*

 * *                                        "('description', ''), ('props', OrderedDict([('className', "*

 * *                                        "OrderedDict([('description', ''), ('required', False), "*

 * *                                        "('type', OrderedDict([('name', 'string'), ('raw', "*

 * *                                        "'string')]))])), ('type', OrderedDict([('description', "*

 * *                                   […]*

```diff
@@ -58,14 +58,65 @@
                 "type": {
                     "name": "any",
                     "raw": "any"
                 }
             }
         }
     },
+    "src/ts/components/MenuTrigger.tsx": {
+        "description": "",
+        "displayName": "MenuTrigger",
+        "isContext": false,
+        "props": {
+            "children": {
+                "description": "",
+                "required": true,
+                "type": {
+                    "name": "any",
+                    "raw": "any"
+                }
+            },
+            "className": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string",
+                    "raw": "string"
+                }
+            },
+            "id": {
+                "description": "Unique ID to identify this component in Dash callbacks.",
+                "required": false,
+                "type": {
+                    "name": "string",
+                    "raw": "string"
+                }
+            },
+            "setProps": {
+                "description": "Update props to trigger callbacks.",
+                "required": true,
+                "type": {
+                    "name": "func",
+                    "raw": "(props: Record<string, any>) => void"
+                }
+            },
+            "type": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'button'"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "any",
+                    "raw": "any"
+                }
+            }
+        }
+    },
     "src/ts/components/Youhi.tsx": {
         "description": "Component description",
         "displayName": "Youhi",
         "isContext": false,
         "props": {
             "id": {
                 "description": "Unique ID to identify this component in Dash callbacks.",
```

### Comparing `youhi-1.0.6/youhi/package.json` & `youhi-1.0.7/youhi/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'1.0.7'"}*

```diff
@@ -27,9 +27,9 @@
         "build": "npm run build:css && npm run build:js && npm run build:backends",
         "build:backends": "dash-generate-components ./src/ts/components youhi -p package.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:css": "npx tailwindcss -i ./src/input.css -o ./youhi/style.css",
         "build:js": "webpack",
         "build:js::dev": "webpack --mode development",
         "watch": "npm run build:js::dev -- --watch"
     },
-    "version": "1.0.6"
+    "version": "1.0.7"
 }
```

### Comparing `youhi-1.0.6/youhi/style.css` & `youhi-1.0.7/youhi/style.css`

 * *Files identical despite different names*

### Comparing `youhi-1.0.6/youhi/youhi.js` & `youhi-1.0.7/youhi/youhi.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,73 +1,102 @@
 ! function(e, t) {
     "object" == typeof exports && "object" == typeof module ? module.exports = t(require("react")) : "function" == typeof define && define.amd ? define(["react"], t) : "object" == typeof exports ? exports.youhi = t(require("react")) : e.youhi = t(e.React)
 }(self, (e => (() => {
     "use strict";
     var t = {
             570: function(e, t, u) {
-                var o = this && this.__importDefault || function(e) {
+                var r = this && this.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
                 t.__esModule = !0;
-                var r = o(u(812)),
-                    a = function(e) {
+                var o = r(u(812)),
+                    n = function(e) {
                         var t = e.id,
                             u = e.type,
-                            o = e.text,
-                            a = e.className;
-                        return r.default.createElement("button", {
+                            r = e.text,
+                            n = e.className;
+                        return o.default.createElement("button", {
                             id: t,
                             type: u,
-                            className: "flex bg-blue-500 text-white rounded-md hover:bg-blue-300 py-2 px-5 ".concat(a)
-                        }, o)
+                            className: "flex bg-blue-500 text-white rounded-md hover:bg-blue-300 py-2 px-5 ".concat(n)
+                        }, r)
                     };
-                a.defaultProps = {
+                n.defaultProps = {
                     type: "button",
                     text: "Submit"
-                }, t.default = a
+                }, t.default = n
+            },
+            518: function(e, t, u) {
+                var r = this && this.__importDefault || function(e) {
+                    return e && e.__esModule ? e : {
+                        default: e
+                    }
+                };
+                t.__esModule = !0;
+                var o = r(u(812)),
+                    n = function(e) {
+                        var t = e.id,
+                            u = e.type,
+                            r = e.className;
+                        return o.default.createElement("button", {
+                            onClick: function(e) {
+                                e.preventDefault();
+                                var t = document.getElementById("youhi-sidebar");
+                                t && t.classList.toggle("open")
+                            },
+                            id: t,
+                            type: u,
+                            className: "youhi_menu_trigger ".concat(r)
+                        }, e.children)
+                    };
+                n.defaultProps = {
+                    type: "button"
+                }, t.default = n
             },
             955: function(e, t, u) {
-                var o = this && this.__importDefault || function(e) {
+                var r = this && this.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
                 t.__esModule = !0;
-                var r = o(u(812)),
-                    a = function(e) {
+                var o = r(u(812)),
+                    n = function(e) {
                         var t = e.id;
-                        return r.default.createElement("div", {
+                        return o.default.createElement("div", {
                             id: t
-                        }, r.default.createElement("h1", {
+                        }, o.default.createElement("h1", {
                             className: "font-bold text-5xl text-blue-600"
                         }, "YouHi"))
                     };
-                a.defaultProps = {}, t.default = a
+                n.defaultProps = {}, t.default = n
             },
             294: function(e, t, u) {
-                var o = this && this.__importDefault || function(e) {
+                var r = this && this.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
-                t.__esModule = !0, t.Button = t.Youhi = void 0;
-                var r = o(u(955));
-                t.Youhi = r.default;
-                var a = o(u(570));
-                t.Button = a.default
+                t.__esModule = !0, t.MenuTrigger = t.Button = t.Youhi = void 0;
+                var o = r(u(955));
+                t.Youhi = o.default;
+                var n = r(u(570));
+                t.Button = n.default;
+                var a = r(u(518));
+                t.MenuTrigger = a.default
             },
             812: t => {
                 t.exports = e
             }
         },
         u = {};
-    return function e(o) {
-        var r = u[o];
-        if (void 0 !== r) return r.exports;
-        var a = u[o] = {
+    return function e(r) {
+        var o = u[r];
+        if (void 0 !== o) return o.exports;
+        var n = u[r] = {
             exports: {}
         };
-        return t[o].call(a.exports, a, a.exports, e), a.exports
+        return t[r].call(n.exports, n, n.exports, e), n.exports
     }(294)
 })()));
```

### Comparing `youhi-1.0.6/youhi.egg-info/PKG-INFO` & `youhi-1.0.7/youhi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youhi
-Version: 1.0.6
+Version: 1.0.7
 Summary: Plotly dash React component UI library boilerplate
 Home-page: UNKNOWN
 Author: thesameeric <osivwiokiti@gmail.com>
 License: MIT
 Platform: UNKNOWN
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
```

