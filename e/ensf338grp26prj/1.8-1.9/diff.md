# Comparing `tmp/ensf338grp26prj-1.8.tar.gz` & `tmp/ensf338grp26prj-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensf338grp26prj-1.8.tar", last modified: Thu Apr 13 21:17:30 2023, max compression
+gzip compressed data, was "ensf338grp26prj-1.9.tar", last modified: Thu Apr 13 21:21:56 2023, max compression
```

## Comparing `ensf338grp26prj-1.8.tar` & `ensf338grp26prj-1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.613416 ensf338grp26prj-1.8/
--rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 21:17:30.613200 ensf338grp26prj-1.8/PKG-INFO
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.609265 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/
--rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 21:17:30.000000 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/PKG-INFO
--rw-r--r--   0 tonytran   (501) staff       (20)      729 2023-04-13 21:17:30.000000 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/SOURCES.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 21:17:30.000000 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/dependency_links.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 21:17:30.000000 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/top_level.txt
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.609490 ensf338grp26prj-1.8/myLib/
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:23.000000 ensf338grp26prj-1.8/myLib/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.609649 ensf338grp26prj-1.8/myLib/datastructures/
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-13 19:59:57.000000 ensf338grp26prj-1.8/myLib/datastructures/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.610909 ensf338grp26prj-1.8/myLib/datastructures/linear/
--rw-r--r--   0 tonytran   (501) staff       (20)     6679 2023-04-13 21:11:41.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/CDLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8319 2023-04-13 21:13:01.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/CSLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8984 2023-04-13 21:12:57.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/DLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/QueueLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8110 2023-04-13 21:12:49.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/SLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1952 2023-04-13 21:12:22.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/StackLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)      145 2023-04-13 19:45:04.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.611928 ensf338grp26prj-1.8/myLib/datastructures/nodes/
--rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 ensf338grp26prj-1.8/myLib/datastructures/nodes/DNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 ensf338grp26prj-1.8/myLib/datastructures/nodes/SNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 ensf338grp26prj-1.8/myLib/datastructures/nodes/TNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)       74 2023-04-13 19:45:09.000000 ensf338grp26prj-1.8/myLib/datastructures/nodes/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.612685 ensf338grp26prj-1.8/myLib/datastructures/trees/
--rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 ensf338grp26prj-1.8/myLib/datastructures/trees/AVL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 ensf338grp26prj-1.8/myLib/datastructures/trees/BST.py
--rw-r--r--   0 tonytran   (501) staff       (20)       62 2023-04-13 21:16:26.000000 ensf338grp26prj-1.8/myLib/datastructures/trees/__init__.py
--rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 21:17:30.613482 ensf338grp26prj-1.8/setup.cfg
--rw-r--r--   0 tonytran   (501) staff       (20)      222 2023-04-13 21:16:32.000000 ensf338grp26prj-1.8/setup.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:21:56.075837 ensf338grp26prj-1.9/
+-rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 21:21:56.075668 ensf338grp26prj-1.9/PKG-INFO
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:21:56.072157 ensf338grp26prj-1.9/ensf338grp26prj.egg-info/
+-rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 21:21:56.000000 ensf338grp26prj-1.9/ensf338grp26prj.egg-info/PKG-INFO
+-rw-r--r--   0 tonytran   (501) staff       (20)      729 2023-04-13 21:21:56.000000 ensf338grp26prj-1.9/ensf338grp26prj.egg-info/SOURCES.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 21:21:56.000000 ensf338grp26prj-1.9/ensf338grp26prj.egg-info/dependency_links.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 21:21:56.000000 ensf338grp26prj-1.9/ensf338grp26prj.egg-info/top_level.txt
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:21:56.072357 ensf338grp26prj-1.9/myLib/
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-13 21:21:23.000000 ensf338grp26prj-1.9/myLib/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:21:56.072501 ensf338grp26prj-1.9/myLib/datastructures/
+-rw-r--r--   0 tonytran   (501) staff       (20)       28 2023-04-13 21:21:28.000000 ensf338grp26prj-1.9/myLib/datastructures/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:21:56.073989 ensf338grp26prj-1.9/myLib/datastructures/linear/
+-rw-r--r--   0 tonytran   (501) staff       (20)     6679 2023-04-13 21:11:41.000000 ensf338grp26prj-1.9/myLib/datastructures/linear/CDLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8319 2023-04-13 21:13:01.000000 ensf338grp26prj-1.9/myLib/datastructures/linear/CSLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8984 2023-04-13 21:12:57.000000 ensf338grp26prj-1.9/myLib/datastructures/linear/DLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 ensf338grp26prj-1.9/myLib/datastructures/linear/QueueLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8110 2023-04-13 21:12:49.000000 ensf338grp26prj-1.9/myLib/datastructures/linear/SLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1952 2023-04-13 21:12:22.000000 ensf338grp26prj-1.9/myLib/datastructures/linear/StackLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      167 2023-04-13 21:20:21.000000 ensf338grp26prj-1.9/myLib/datastructures/linear/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:21:56.074847 ensf338grp26prj-1.9/myLib/datastructures/nodes/
+-rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 ensf338grp26prj-1.9/myLib/datastructures/nodes/DNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 ensf338grp26prj-1.9/myLib/datastructures/nodes/SNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 ensf338grp26prj-1.9/myLib/datastructures/nodes/TNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       95 2023-04-13 21:20:02.000000 ensf338grp26prj-1.9/myLib/datastructures/nodes/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:21:56.075418 ensf338grp26prj-1.9/myLib/datastructures/trees/
+-rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 ensf338grp26prj-1.9/myLib/datastructures/trees/AVL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 ensf338grp26prj-1.9/myLib/datastructures/trees/BST.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       62 2023-04-13 21:16:26.000000 ensf338grp26prj-1.9/myLib/datastructures/trees/__init__.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 21:21:56.075905 ensf338grp26prj-1.9/setup.cfg
+-rw-r--r--   0 tonytran   (501) staff       (20)      222 2023-04-13 21:21:52.000000 ensf338grp26prj-1.9/setup.py
```

### Comparing `ensf338grp26prj-1.8/ensf338grp26prj.egg-info/SOURCES.txt` & `ensf338grp26prj-1.9/ensf338grp26prj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/linear/CDLL.py` & `ensf338grp26prj-1.9/myLib/datastructures/linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/linear/CSLL.py` & `ensf338grp26prj-1.9/myLib/datastructures/linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/linear/DLL.py` & `ensf338grp26prj-1.9/myLib/datastructures/linear/DLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/linear/QueueLL.py` & `ensf338grp26prj-1.9/myLib/datastructures/linear/QueueLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/linear/SLL.py` & `ensf338grp26prj-1.9/myLib/datastructures/linear/SLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/linear/StackLL.py` & `ensf338grp26prj-1.9/myLib/datastructures/linear/StackLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/nodes/DNode.py` & `ensf338grp26prj-1.9/myLib/datastructures/nodes/DNode.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/nodes/TNode.py` & `ensf338grp26prj-1.9/myLib/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/trees/AVL.py` & `ensf338grp26prj-1.9/myLib/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.8/myLib/datastructures/trees/BST.py` & `ensf338grp26prj-1.9/myLib/datastructures/trees/BST.py`

 * *Files identical despite different names*

