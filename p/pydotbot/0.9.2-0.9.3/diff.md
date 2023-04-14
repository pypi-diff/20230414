# Comparing `tmp/pydotbot-0.9.2.tar.gz` & `tmp/pydotbot-0.9.3.tar.gz`

## Comparing `pydotbot-0.9.2.tar` & `pydotbot-0.9.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/__init__.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/controller.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/hdlc.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/joystick.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/keyboard.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/lighthouse2.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/main.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/models.py
--rw-r--r--   0        0        0     9043 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/protocol.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/serial_interface.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/server.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/.env
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/.env.test
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/.gitignore
--rw-r--r--   0        0        0  1237202 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/package-lock.json
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/package.json
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/index.html
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/manifest.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/robots.txt
--rw-r--r--   0        0        0   275084 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/static/css/main.ab17a09a.css
--rw-r--r--   0        0        0   721359 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/static/css/main.ab17a09a.css.map
--rw-r--r--   0        0        0   392296 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/static/js/main.eb59a3ba.js
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/static/js/main.eb59a3ba.js.LICENSE.txt
--rw-r--r--   0        0        0  1268701 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/static/js/main.eb59a3ba.js.map
--rw-r--r--   0        0        0   150592 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/static/media/bootstrap-icons.e559bf06bc84fd9525e6.woff
--rw-r--r--   0        0        0   112440 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/build/static/media/bootstrap-icons.ea98e12d2d58747f9fc5.woff2
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/public/index.html
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/public/manifest.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/public/robots.txt
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/src/DotBots.js
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/src/DotBots.test.js
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/src/DotBotsMap.js
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/src/Joystick.js
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/src/Joystick.test.js
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/src/index.js
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/frontend/src/rest.js
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/lib/.gitignore
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/lib/CMakeLists.txt
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/lib/lh2.c
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/tests/test_controller.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/tests/test_hdlc_handler.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/tests/test_lighthouse2.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/tests/test_main.py
--rw-r--r--   0        0        0    10899 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/tests/test_protocol.py
--rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 pydotbot-0.9.2/dotbot/tests/test_server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydotbot-0.9.2/utils/hooks/__init__.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pydotbot-0.9.2/utils/hooks/pydotbot_utils.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydotbot-0.9.2/utils/hooks/sdist.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydotbot-0.9.2/utils/hooks/wheel.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pydotbot-0.9.2/.gitignore
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 pydotbot-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 pydotbot-0.9.2/README.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pydotbot-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 pydotbot-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/__init__.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/controller.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/hdlc.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/joystick.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/keyboard.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/lighthouse2.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/main.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/models.py
+-rw-r--r--   0        0        0     9043 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/protocol.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/serial_interface.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/server.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/.env
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/.env.test
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/.gitignore
+-rw-r--r--   0        0        0  1237202 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/package-lock.json
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/package.json
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/index.html
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/manifest.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/robots.txt
+-rw-r--r--   0        0        0   275084 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/static/css/main.ab17a09a.css
+-rw-r--r--   0        0        0   721359 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/static/css/main.ab17a09a.css.map
+-rw-r--r--   0        0        0   392296 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/static/js/main.eb59a3ba.js
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/static/js/main.eb59a3ba.js.LICENSE.txt
+-rw-r--r--   0        0        0  1268701 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/static/js/main.eb59a3ba.js.map
+-rw-r--r--   0        0        0   150592 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/static/media/bootstrap-icons.e559bf06bc84fd9525e6.woff
+-rw-r--r--   0        0        0   112440 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/build/static/media/bootstrap-icons.ea98e12d2d58747f9fc5.woff2
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/public/index.html
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/public/manifest.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/public/robots.txt
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/src/DotBots.js
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/src/DotBots.test.js
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/src/DotBotsMap.js
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/src/Joystick.js
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/src/Joystick.test.js
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/src/index.js
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/frontend/src/rest.js
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/lib/.gitignore
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/lib/CMakeLists.txt
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/lib/lh2.c
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/tests/test_controller.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/tests/test_hdlc_handler.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/tests/test_lighthouse2.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/tests/test_main.py
+-rw-r--r--   0        0        0    10899 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/tests/test_protocol.py
+-rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 pydotbot-0.9.3/dotbot/tests/test_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydotbot-0.9.3/utils/hooks/__init__.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pydotbot-0.9.3/utils/hooks/pydotbot_utils.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydotbot-0.9.3/utils/hooks/sdist.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydotbot-0.9.3/utils/hooks/wheel.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pydotbot-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 pydotbot-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 pydotbot-0.9.3/README.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pydotbot-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 pydotbot-0.9.3/PKG-INFO
```

### Comparing `pydotbot-0.9.2/dotbot/controller.py` & `pydotbot-0.9.3/dotbot/controller.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/hdlc.py` & `pydotbot-0.9.3/dotbot/hdlc.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/joystick.py` & `pydotbot-0.9.3/dotbot/joystick.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/keyboard.py` & `pydotbot-0.9.3/dotbot/keyboard.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/lighthouse2.py` & `pydotbot-0.9.3/dotbot/lighthouse2.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/main.py` & `pydotbot-0.9.3/dotbot/main.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/models.py` & `pydotbot-0.9.3/dotbot/models.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/protocol.py` & `pydotbot-0.9.3/dotbot/protocol.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/serial_interface.py` & `pydotbot-0.9.3/dotbot/serial_interface.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/server.py` & `pydotbot-0.9.3/dotbot/server.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/package-lock.json` & `pydotbot-0.9.3/dotbot/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/package.json` & `pydotbot-0.9.3/dotbot/frontend/package.json`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/asset-manifest.json` & `pydotbot-0.9.3/dotbot/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/index.html` & `pydotbot-0.9.3/dotbot/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/static/css/main.ab17a09a.css` & `pydotbot-0.9.3/dotbot/frontend/build/static/css/main.ab17a09a.css`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/static/css/main.ab17a09a.css.map` & `pydotbot-0.9.3/dotbot/frontend/build/static/css/main.ab17a09a.css.map`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/static/js/main.eb59a3ba.js` & `pydotbot-0.9.3/dotbot/frontend/build/static/js/main.eb59a3ba.js`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/static/js/main.eb59a3ba.js.LICENSE.txt` & `pydotbot-0.9.3/dotbot/frontend/build/static/js/main.eb59a3ba.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/static/js/main.eb59a3ba.js.map` & `pydotbot-0.9.3/dotbot/frontend/build/static/js/main.eb59a3ba.js.map`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/static/media/bootstrap-icons.e559bf06bc84fd9525e6.woff` & `pydotbot-0.9.3/dotbot/frontend/build/static/media/bootstrap-icons.e559bf06bc84fd9525e6.woff`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/build/static/media/bootstrap-icons.ea98e12d2d58747f9fc5.woff2` & `pydotbot-0.9.3/dotbot/frontend/build/static/media/bootstrap-icons.ea98e12d2d58747f9fc5.woff2`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/src/DotBots.js` & `pydotbot-0.9.3/dotbot/frontend/src/DotBots.js`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/src/DotBots.test.js` & `pydotbot-0.9.3/dotbot/frontend/src/DotBots.test.js`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/src/DotBotsMap.js` & `pydotbot-0.9.3/dotbot/frontend/src/DotBotsMap.js`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/src/Joystick.js` & `pydotbot-0.9.3/dotbot/frontend/src/Joystick.js`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/src/Joystick.test.js` & `pydotbot-0.9.3/dotbot/frontend/src/Joystick.test.js`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/frontend/src/rest.js` & `pydotbot-0.9.3/dotbot/frontend/src/rest.js`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/lib/lh2.c` & `pydotbot-0.9.3/dotbot/lib/lh2.c`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/tests/test_controller.py` & `pydotbot-0.9.3/dotbot/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/tests/test_hdlc_handler.py` & `pydotbot-0.9.3/dotbot/tests/test_hdlc_handler.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/tests/test_lighthouse2.py` & `pydotbot-0.9.3/dotbot/tests/test_lighthouse2.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/tests/test_main.py` & `pydotbot-0.9.3/dotbot/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/tests/test_protocol.py` & `pydotbot-0.9.3/dotbot/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/dotbot/tests/test_server.py` & `pydotbot-0.9.3/dotbot/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/utils/hooks/pydotbot_utils.py` & `pydotbot-0.9.3/utils/hooks/pydotbot_utils.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/utils/hooks/sdist.py` & `pydotbot-0.9.3/utils/hooks/sdist.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/utils/hooks/wheel.py` & `pydotbot-0.9.3/utils/hooks/wheel.py`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/LICENSE.txt` & `pydotbot-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/README.md` & `pydotbot-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pydotbot-0.9.2/pyproject.toml` & `pydotbot-0.9.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 path = "utils/hooks/sdist.py"
 
 [tool.hatch.build.targets.wheel.hooks.custom]
 path = "utils/hooks/wheel.py"
 
 [project]
 name = "pydotbot"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
     { name="Alexandre Abadie", email="alexandre.abadie@inria.fr" },
     { name="Theo Akbas", email="theo.akbas@inria.fr" },
 ]
 dependencies = [
     "click          == 8.1.3",
     "fastapi        == 0.85.1",
```

### Comparing `pydotbot-0.9.2/PKG-INFO` & `pydotbot-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydotbot
-Version: 0.9.2
+Version: 0.9.3
 Summary: Package to easily control your DotBots and SailBots.
 Project-URL: Homepage, https://github.com/DotBots/PyDotBot
 Project-URL: Bug Tracker, https://github.com/DotBots/PyDotBot/issues
 Author-email: Alexandre Abadie <alexandre.abadie@inria.fr>, Theo Akbas <theo.akbas@inria.fr>
 License: BSD
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: BSD License
```

