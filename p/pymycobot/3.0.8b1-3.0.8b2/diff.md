# Comparing `tmp/pymycobot-3.0.8b1.tar.gz` & `tmp/pymycobot-3.0.8b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.0.8b1.tar", last modified: Mon Mar 13 09:10:56 2023, max compression
+gzip compressed data, was "pymycobot-3.0.8b2.tar", last modified: Thu Apr 13 10:06:11 2023, max compression
```

## Comparing `pymycobot-3.0.8b1.tar` & `pymycobot-3.0.8b2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 09:10:56.821991 pymycobot-3.0.8b1/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.0.8b1/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.0.8b1/MANIFEST.in
--rw-rw-rw-   0        0        0    55520 2023-03-13 09:10:56.820493 pymycobot-3.0.8b1/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.0.8b1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 09:10:56.788219 pymycobot-3.0.8b1/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.0.8b1/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1562 2023-03-13 09:10:36.000000 pymycobot-3.0.8b1/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2022-07-18 09:51:08.000000 pymycobot-3.0.8b1/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    12065 2023-03-06 07:56:35.000000 pymycobot-3.0.8b1/pymycobot/common.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.0.8b1/pymycobot/error.py
--rw-rw-rw-   0        0        0    32911 2023-03-13 09:04:37.000000 pymycobot-3.0.8b1/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.0.8b1/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.0.8b1/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.0.8b1/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8869 2023-01-10 08:08:44.000000 pymycobot-3.0.8b1/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13361 2022-12-20 11:11:52.000000 pymycobot-3.0.8b1/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.0.8b1/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.0.8b1/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.0.8b1/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7351 2022-11-29 03:08:51.000000 pymycobot-3.0.8b1/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7441 2022-06-28 10:56:36.000000 pymycobot-3.0.8b1/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8420 2022-11-14 07:30:15.000000 pymycobot-3.0.8b1/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7445 2022-10-20 05:52:29.000000 pymycobot-3.0.8b1/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19564 2023-03-06 07:56:35.000000 pymycobot-3.0.8b1/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.0.8b1/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-13 09:10:56.819041 pymycobot-3.0.8b1/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    55520 2023-03-13 09:10:56.000000 pymycobot-3.0.8b1/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-03-13 09:10:56.000000 pymycobot-3.0.8b1/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 09:10:56.000000 pymycobot-3.0.8b1/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-13 09:10:56.000000 pymycobot-3.0.8b1/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-13 09:10:56.000000 pymycobot-3.0.8b1/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.0.8b1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-13 09:10:56.821991 pymycobot-3.0.8b1/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.0.8b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:06:11.282403 pymycobot-3.0.8b2/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.0.8b2/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.0.8b2/MANIFEST.in
+-rw-rw-rw-   0        0        0    55520 2023-04-13 10:06:11.281400 pymycobot-3.0.8b2/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.0.8b2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 10:06:11.245615 pymycobot-3.0.8b2/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.0.8b2/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1562 2023-04-13 10:05:43.000000 pymycobot-3.0.8b2/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2022-07-18 09:51:08.000000 pymycobot-3.0.8b2/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    12065 2023-03-06 07:56:35.000000 pymycobot-3.0.8b2/pymycobot/common.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.0.8b2/pymycobot/error.py
+-rw-rw-rw-   0        0        0    32911 2023-03-13 09:04:37.000000 pymycobot-3.0.8b2/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.0.8b2/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.0.8b2/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.0.8b2/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     8869 2023-01-10 08:08:44.000000 pymycobot-3.0.8b2/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13308 2023-04-13 10:04:38.000000 pymycobot-3.0.8b2/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.0.8b2/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.0.8b2/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.0.8b2/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     7351 2022-11-29 03:08:51.000000 pymycobot-3.0.8b2/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7441 2022-06-28 10:56:36.000000 pymycobot-3.0.8b2/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     8420 2022-11-14 07:30:15.000000 pymycobot-3.0.8b2/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7445 2022-10-20 05:52:29.000000 pymycobot-3.0.8b2/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19564 2023-03-06 07:56:35.000000 pymycobot-3.0.8b2/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.0.8b2/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:06:11.279405 pymycobot-3.0.8b2/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    55520 2023-04-13 10:06:10.000000 pymycobot-3.0.8b2/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-04-13 10:06:11.000000 pymycobot-3.0.8b2/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 10:06:10.000000 pymycobot-3.0.8b2/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 10:06:10.000000 pymycobot-3.0.8b2/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 10:06:10.000000 pymycobot-3.0.8b2/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.0.8b2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 10:06:11.283406 pymycobot-3.0.8b2/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.0.8b2/setup.py
```

### Comparing `pymycobot-3.0.8b1/LICENSE` & `pymycobot-3.0.8b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/PKG-INFO` & `pymycobot-3.0.8b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.0.8b1
+Version: 3.0.8b2
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `pymycobot-3.0.8b1/README.md` & `pymycobot-3.0.8b2/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/Interface.py` & `pymycobot-3.0.8b2/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/__init__.py` & `pymycobot-3.0.8b2/pymycobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.0.8b1"
+__version__ = "3.0.8b2"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.0.8b1/pymycobot/bluet.py` & `pymycobot-3.0.8b2/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/common.py` & `pymycobot-3.0.8b2/pymycobot/common.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/error.py` & `pymycobot-3.0.8b2/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/generate.py` & `pymycobot-3.0.8b2/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/log.py` & `pymycobot-3.0.8b2/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/myarm.py` & `pymycobot-3.0.8b2/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/mybuddy.py` & `pymycobot-3.0.8b2/pymycobot/mybuddy.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,17 +259,17 @@
                 0 - input
                     define: pull_up_down = DOWN
                 1 - output
                      define: initial = HIGH
         """
         pin_no = self.base_io_to_gpio(pin_no)       
         if mode == 1:
-            self.gpio.setup(pin_no, self.gpio.OUT, initial=self.gpio.HIGH)
+            self.gpio.setup(pin_no, self.gpio.OUT)
         else:
-            self.gpio.setup(pin_no, self.gpio.IN, pull_up_down=self.gpio.DOWN)
+            self.gpio.setup(pin_no, self.gpio.IN)
             
     def set_gpio_output(self, pin_no, v):
         """Set GPIO output value.
 
         Args:
             pin_no: (int)pin number 1-16.
             v: (int) 0 / 1
```

### Comparing `pymycobot-3.0.8b1/pymycobot/mybuddybluetooth.py` & `pymycobot-3.0.8b2/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/mybuddyemoticon.py` & `pymycobot-3.0.8b2/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/mybuddysocket.py` & `pymycobot-3.0.8b2/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/mycobot.py` & `pymycobot-3.0.8b2/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/mycobotsocket.py` & `pymycobot-3.0.8b2/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/mypalletizer.py` & `pymycobot-3.0.8b2/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/mypalletizersocket.py` & `pymycobot-3.0.8b2/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/ultraArm.py` & `pymycobot-3.0.8b2/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot/utils.py` & `pymycobot-3.0.8b2/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.0.8b2/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.0.8b1
+Version: 3.0.8b2
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `pymycobot-3.0.8b1/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.0.8b2/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.0.8b1/setup.py` & `pymycobot-3.0.8b2/setup.py`

 * *Files identical despite different names*

