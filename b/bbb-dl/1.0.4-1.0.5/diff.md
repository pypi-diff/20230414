# Comparing `tmp/bbb-dl-1.0.4.tar.gz` & `tmp/bbb-dl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbb-dl-1.0.4.tar", last modified: Fri Apr 14 08:50:51 2023, max compression
+gzip compressed data, was "bbb-dl-1.0.5.tar", last modified: Fri Apr 14 10:08:24 2023, max compression
```

## Comparing `bbb-dl-1.0.4.tar` & `bbb-dl-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/bbb_dl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/ffmpeg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58606 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    22273 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/bbb_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:24.344219 bbb-dl-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-14 10:08:24.344219 bbb-dl-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:24.344219 bbb-dl-1.0.5/bbb_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/bbb_dl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/bbb_dl/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/bbb_dl/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/bbb_dl/ffmpeg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58606 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/bbb_dl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22268 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/bbb_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/bbb_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:24.344219 bbb-dl-1.0.5/bbb_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-14 10:08:24.000000 bbb-dl-1.0.5/bbb_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 10:08:24.000000 bbb-dl-1.0.5/bbb_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:08:24.000000 bbb-dl-1.0.5/bbb_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 10:08:24.000000 bbb-dl-1.0.5/bbb_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:08:24.000000 bbb-dl-1.0.5/bbb_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 10:08:24.000000 bbb-dl-1.0.5/bbb_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 10:08:24.000000 bbb-dl-1.0.5/bbb_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:08:24.344219 bbb-dl-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-14 10:08:14.000000 bbb-dl-1.0.5/setup.py
```

### Comparing `bbb-dl-1.0.4/LICENSE` & `bbb-dl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.4/PKG-INFO` & `bbb-dl-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-dl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Big Blue Button Downloader that downloads a BBB lesson as MP4 video
 Home-page: https://github.com/C0D3D3V/bbb-dl
 Author: C0D3D3V
 License: GPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bbb-dl-1.0.4/README.md` & `bbb-dl-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.4/bbb_dl/batch.py` & `bbb-dl-1.0.5/bbb_dl/batch.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.4/bbb_dl/browser.py` & `bbb-dl-1.0.5/bbb_dl/browser.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,16 +34,17 @@
     def __init__(self, args):
         super().__init__()
         self.working_dir = bbb_dl.BBBDL.get_working_dir(args.working_dir)
         self.cookies_path = PT.make_path(self.working_dir, "cookies.txt")
         self.cookie_jar = BBBDLCookieJar(self.cookies_path)
         self.setWindowTitle('BBB Browser')
 
-        web_engine_context_log = QLoggingCategory("qt.webenginecontext")
-        web_engine_context_log.setFilterRules("*.info=false")
+        if args.verbose is None or not args.verbose:
+            web_engine_context_log = QLoggingCategory("qt.webenginecontext")
+            web_engine_context_log.setFilterRules("*.info=false")
 
         self.toolBar = QToolBar()
         self.addToolBar(self.toolBar)
         self.backButton = QPushButton()
         self.backButton.setIcon(self.style().standardIcon(QStyle.StandardPixmap.SP_ArrowBack))
         self.backButton.clicked.connect(self.back)
         self.toolBar.addWidget(self.backButton)
@@ -54,59 +55,62 @@
 
         self.addressLineEdit = QLineEdit()
         self.addressLineEdit.returnPressed.connect(self.load)
         self.toolBar.addWidget(self.addressLineEdit)
 
         self.webEngineView = QWebEngineView()
 
-        self.profile = QWebEngineProfile("storage", self.webEngineView)
+        # We use the off-the-record mode to not use persistent storage
+        self.profile = QWebEngineProfile(self.webEngineView)
         self.cookie_store = self.profile.cookieStore()
         if os.path.isfile(self.cookies_path):
             self.cookie_jar.load(ignore_discard=True, ignore_expires=True)
             load_mozilla_cookies_into_qt_cookie_store(self.cookie_jar, self.cookie_store)
 
         self.cookie_store.cookieAdded.connect(self.handle_cookie_added)
         self.profile.settings().setAttribute(QWebEngineSettings.JavascriptEnabled, True)
 
         webpage = QWebEnginePage(self.profile, self)
         self.webEngineView.setPage(webpage)
 
         self.setCentralWidget(self.webEngineView)
-        initialUrl = 'https://www.ecosia.org'
+        initialUrl = 'https://www.startpage.com/'
         self.addressLineEdit.setText(initialUrl)
         self.webEngineView.load(QUrl(initialUrl))
         self.webEngineView.page().titleChanged.connect(self.setWindowTitle)
         self.webEngineView.page().urlChanged.connect(self.urlChanged)
 
     def closeEvent(self, event):
         self.cookie_jar.save(ignore_discard=True, ignore_expires=True)
 
     def handle_cookie_added(self, qt_cookie: QNetworkCookie):
         # print("added {name} : {value}".format(name=qt_cookie.name(), value=qt_cookie.value()))
-        self.cookie_jar.set_cookie(
-            Cookie(
-                version=None,
-                name=qt_cookie.name().data().decode('utf-8'),
-                value=qt_cookie.value().data().decode('utf-8'),
-                port=None,
-                port_specified=False,
-                domain=qt_cookie.domain(),
-                domain_specified=True,
-                domain_initial_dot=qt_cookie.domain().startswith("."),  # should be always true
-                path=qt_cookie.path(),
-                path_specified=True,
-                secure=qt_cookie.isSecure(),
-                expires=qt_cookie.expirationDate().toSecsSinceEpoch(),
-                discard=False,
-                comment=None,
-                comment_url=None,
-                rest=None,
-                rfc2109=False,
-            )
+        exp = qt_cookie.expirationDate().toSecsSinceEpoch()
+        if exp <= 0:
+            exp = 2147483647
+        new_cookie = Cookie(
+            version=None,
+            name=qt_cookie.name().data().decode('utf-8'),
+            value=qt_cookie.value().data().decode('utf-8'),
+            port=None,
+            port_specified=False,
+            domain=qt_cookie.domain(),
+            domain_specified=True,
+            domain_initial_dot=qt_cookie.domain().startswith("."),  # should be always true
+            path=qt_cookie.path(),
+            path_specified=True,
+            secure=qt_cookie.isSecure(),
+            expires=exp,
+            discard=False,
+            comment=None,
+            comment_url=None,
+            rest=None,
+            rfc2109=False,
         )
+        self.cookie_jar.set_cookie(new_cookie)
 
     @Slot()
     def load(self):
         url = QUrl.fromUserInput(self.addressLineEdit.text())
         if url.isValid():
             self.webEngineView.load(url)
 
@@ -129,14 +133,20 @@
         '-wd',
         '--working-dir',
         type=str,
         default=None,
         help='Optional output directory for all temporary directories/files',
     )
 
+    parser.add_argument(
+        '-v',
+        '--verbose',
+        action='store_true',
+        help=('Print more verbose debug information'),
+    )
     return parser
 
 
 # --- called at the program invocation: -------------------------------------
 def main(args=None):
     args, _ = get_parser().parse_known_args(args)
     app = QApplication(sys.argv)
```

### Comparing `bbb-dl-1.0.4/bbb_dl/ffmpeg.py` & `bbb-dl-1.0.5/bbb_dl/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.4/bbb_dl/main.py` & `bbb-dl-1.0.5/bbb_dl/main.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.4/bbb_dl/utils.py` & `bbb-dl-1.0.5/bbb_dl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
                     cf.write(prepare_line(line))
                 except http.cookiejar.LoadError as cookie_err:
                     if f'{line.strip()} '[0] in '[{"':
                         raise http.cookiejar.LoadError(
                             'Cookies file must be Netscape formatted, not JSON. See  '
                             'https://github.com/C0D3D3V/Moodle-DL/wiki/Use-cookies-when-downloading'
                         )
-                    logging.info('WARNING: Skipping cookie file entry due to %s: %r', cookie_err, line)
+                    Log.info(f'WARNING: Skipping cookie file entry due to {cookie_err}: {line!r}')
                     continue
         cf.seek(0)
         self._really_load(cf, filename, ignore_discard, ignore_expires)
         # Session cookies are denoted by either `expires` field set to
         # an empty string or 0. MozillaCookieJar only recognizes the former
         # (see [1]). So we need force the latter to be recognized as session
         # cookies on our own.
```

### Comparing `bbb-dl-1.0.4/bbb_dl.egg-info/PKG-INFO` & `bbb-dl-1.0.5/bbb_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-dl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Big Blue Button Downloader that downloads a BBB lesson as MP4 video
 Home-page: https://github.com/C0D3D3V/bbb-dl
 Author: C0D3D3V
 License: GPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bbb-dl-1.0.4/setup.py` & `bbb-dl-1.0.5/setup.py`

 * *Files identical despite different names*

