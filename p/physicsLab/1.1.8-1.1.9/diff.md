# Comparing `tmp/physicsLab-1.1.8.tar.gz` & `tmp/physicsLab-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\physicsLab-1.1.8.tar", last modified: Sat Apr  8 15:06:30 2023, max compression
+gzip compressed data, was "dist\physicsLab-1.1.9.tar", last modified: Sat Apr  8 15:46:11 2023, max compression
```

## Comparing `physicsLab-1.1.8.tar` & `physicsLab-1.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 15:06:30.000000 physicsLab-1.1.8/
--rw-rw-rw-   0        0        0     1094 2023-04-05 15:16:06.000000 physicsLab-1.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4343 2023-04-08 15:06:30.000000 physicsLab-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3783 2023-04-08 14:49:18.000000 physicsLab-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab/
--rw-rw-rw-   0        0        0      391 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/__init__.py
--rw-rw-rw-   0        0        0      453 2023-04-08 14:49:18.000000 physicsLab-1.1.8/physicsLab/_colorUtils.py
--rw-rw-rw-   0        0        0     3345 2023-04-08 14:49:18.000000 physicsLab-1.1.8/physicsLab/_fileGlobals.py
--rw-rw-rw-   0        0        0      534 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab/astrophysics/
--rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/astrophysics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab/electricity/
--rw-rw-rw-   0        0        0      335 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/element.py
--rw-rw-rw-   0        0        0      478 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/elementPin.py
--rw-rw-rw-   0        0        0     2248 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/elementXYZ.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab/electricity/elementsClass/
--rw-rw-rw-   0        0        0      311 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/elementsClass/__init__.py
--rw-rw-rw-   0        0        0     4321 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/elementsClass/_elementClassHead.py
--rw-rw-rw-   0        0        0     9276 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/elementsClass/artificialCircuit.py
--rw-rw-rw-   0        0        0     8736 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/elementsClass/basicCircuit.py
--rw-rw-rw-   0        0        0    17238 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/elementsClass/logicCircuit.py
--rw-rw-rw-   0        0        0     4599 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/elementsClass/otherCircuit.py
--rw-rw-rw-   0        0        0     3039 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electricity/wire.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab/electromagnetism/
--rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/electromagnetism/__init__.py
--rw-rw-rw-   0        0        0      319 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/errors.py
--rw-rw-rw-   0        0        0    11091 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/experiment.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab/unionElements/
--rw-rw-rw-   0        0        0      137 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/unionElements/__init__.py
--rw-rw-rw-   0        0        0     6894 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/unionElements/unionLogic.py
--rw-rw-rw-   0        0        0       54 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/unionElements/unionPin.py
--rw-rw-rw-   0        0        0     1259 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/unionElements/union_music.py
--rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.8/physicsLab/userlog.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab.egg-info/
--rw-rw-rw-   0        0        0     4343 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1073 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 15:06:30.000000 physicsLab-1.1.8/physicsLab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      581 2023-03-16 14:16:49.000000 physicsLab-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 15:06:30.000000 physicsLab-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-08 15:02:52.000000 physicsLab-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/
+-rw-rw-rw-   0        0        0     1094 2023-04-05 15:16:06.000000 physicsLab-1.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4458 2023-04-08 15:46:11.000000 physicsLab-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3898 2023-04-08 15:42:02.000000 physicsLab-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/
+-rw-rw-rw-   0        0        0      391 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-04-08 15:31:13.000000 physicsLab-1.1.9/physicsLab/_colorUtils.py
+-rw-rw-rw-   0        0        0     3345 2023-04-08 15:31:13.000000 physicsLab-1.1.9/physicsLab/_fileGlobals.py
+-rw-rw-rw-   0        0        0      534 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/astrophysics/
+-rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/astrophysics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/electricity/
+-rw-rw-rw-   0        0        0      335 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/__init__.py
+-rw-rw-rw-   0        0        0     4152 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/element.py
+-rw-rw-rw-   0        0        0      478 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementPin.py
+-rw-rw-rw-   0        0        0     2248 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementXYZ.py
+drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/
+-rw-rw-rw-   0        0        0      311 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/__init__.py
+-rw-rw-rw-   0        0        0     4321 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/_elementClassHead.py
+-rw-rw-rw-   0        0        0     9276 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/artificialCircuit.py
+-rw-rw-rw-   0        0        0     8736 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/basicCircuit.py
+-rw-rw-rw-   0        0        0    17238 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/logicCircuit.py
+-rw-rw-rw-   0        0        0     4599 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/otherCircuit.py
+-rw-rw-rw-   0        0        0     3039 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/wire.py
+drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/electromagnetism/
+-rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electromagnetism/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/errors.py
+-rw-rw-rw-   0        0        0    11091 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/experiment.py
+drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/unionElements/
+-rw-rw-rw-   0        0        0      137 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/unionElements/__init__.py
+-rw-rw-rw-   0        0        0     6894 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/unionElements/unionLogic.py
+-rw-rw-rw-   0        0        0       54 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/unionElements/unionPin.py
+-rw-rw-rw-   0        0        0     1259 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/unionElements/union_music.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/userlog.py
+drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/
+-rw-rw-rw-   0        0        0     4458 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1073 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      581 2023-03-16 14:16:49.000000 physicsLab-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-08 15:46:11.000000 physicsLab-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-04-08 15:33:37.000000 physicsLab-1.1.9/setup.py
```

### Comparing `physicsLab-1.1.8/LICENSE.txt` & `physicsLab-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/PKG-INFO` & `physicsLab-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.1.8
+Version: 1.1.9
 Summary: Doing experiments in the physics lab AR by python
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -74,16 +74,17 @@
 ## 不足
 1. 对逻辑电路元件的支持是最好的，其余电路的部分原件还没有时间封装。但随着时间的推移，这一问题会逐渐消失。
 2. 在物理实验室连接导线只需要点击两下，但用程序连接导线需要指定什么原件的什么引脚，相对麻烦。
 3. 在物理实验室选择原件只需要点击一下，但用程序选择原件需要确定它的位置。（如果有更好的索引原件的方式，欢迎提出）
 4. 作者在接下来很长一段时间内将因为学业没有精力继续维护该仓库，但这并不代表弃坑。
 
 ## 其他
-更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
-
+1. 更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
+2. github: https://github.com/GoodenoughPhysicsLab/physicsLab
+3. gitee: https://gitee.com/script2000/physicsLab
 
 ## 参与贡献
 1.  Fork 本仓库
 2.  新建 Feat_xxx 分支
 3.  提交代码
 4.  新建 Pull Request
 5.  补充readme
```

### Comparing `physicsLab-1.1.8/README.md` & `physicsLab-1.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 ## 不足
 1. 对逻辑电路元件的支持是最好的，其余电路的部分原件还没有时间封装。但随着时间的推移，这一问题会逐渐消失。
 2. 在物理实验室连接导线只需要点击两下，但用程序连接导线需要指定什么原件的什么引脚，相对麻烦。
 3. 在物理实验室选择原件只需要点击一下，但用程序选择原件需要确定它的位置。（如果有更好的索引原件的方式，欢迎提出）
 4. 作者在接下来很长一段时间内将因为学业没有精力继续维护该仓库，但这并不代表弃坑。
 
 ## 其他
-更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
-
+1. 更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
+2. github: https://github.com/GoodenoughPhysicsLab/physicsLab
+3. gitee: https://gitee.com/script2000/physicsLab
 
 ## 参与贡献
 1.  Fork 本仓库
 2.  新建 Feat_xxx 分支
 3.  提交代码
 4.  新建 Pull Request
 5.  补充readme
```

### Comparing `physicsLab-1.1.8/physicsLab/_fileGlobals.py` & `physicsLab-1.1.9/physicsLab/_fileGlobals.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/_tools.py` & `physicsLab-1.1.9/physicsLab/_tools.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/electricity/element.py` & `physicsLab-1.1.9/physicsLab/electricity/element.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/electricity/elementXYZ.py` & `physicsLab-1.1.9/physicsLab/electricity/elementXYZ.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/electricity/elementsClass/_elementClassHead.py` & `physicsLab-1.1.9/physicsLab/electricity/elementsClass/_elementClassHead.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/electricity/elementsClass/artificialCircuit.py` & `physicsLab-1.1.9/physicsLab/electricity/elementsClass/artificialCircuit.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/electricity/elementsClass/basicCircuit.py` & `physicsLab-1.1.9/physicsLab/electricity/elementsClass/basicCircuit.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/electricity/elementsClass/logicCircuit.py` & `physicsLab-1.1.9/physicsLab/electricity/elementsClass/logicCircuit.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/electricity/elementsClass/otherCircuit.py` & `physicsLab-1.1.9/physicsLab/electricity/elementsClass/otherCircuit.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/electricity/wire.py` & `physicsLab-1.1.9/physicsLab/electricity/wire.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/experiment.py` & `physicsLab-1.1.9/physicsLab/experiment.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/unionElements/unionLogic.py` & `physicsLab-1.1.9/physicsLab/unionElements/unionLogic.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab/unionElements/union_music.py` & `physicsLab-1.1.9/physicsLab/unionElements/union_music.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/physicsLab.egg-info/PKG-INFO` & `physicsLab-1.1.9/physicsLab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.1.8
+Version: 1.1.9
 Summary: Doing experiments in the physics lab AR by python
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -74,16 +74,17 @@
 ## 不足
 1. 对逻辑电路元件的支持是最好的，其余电路的部分原件还没有时间封装。但随着时间的推移，这一问题会逐渐消失。
 2. 在物理实验室连接导线只需要点击两下，但用程序连接导线需要指定什么原件的什么引脚，相对麻烦。
 3. 在物理实验室选择原件只需要点击一下，但用程序选择原件需要确定它的位置。（如果有更好的索引原件的方式，欢迎提出）
 4. 作者在接下来很长一段时间内将因为学业没有精力继续维护该仓库，但这并不代表弃坑。
 
 ## 其他
-更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
-
+1. 更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
+2. github: https://github.com/GoodenoughPhysicsLab/physicsLab
+3. gitee: https://gitee.com/script2000/physicsLab
 
 ## 参与贡献
 1.  Fork 本仓库
 2.  新建 Feat_xxx 分支
 3.  提交代码
 4.  新建 Pull Request
 5.  补充readme
```

### Comparing `physicsLab-1.1.8/physicsLab.egg-info/SOURCES.txt` & `physicsLab-1.1.9/physicsLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/pyproject.toml` & `physicsLab-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.8/setup.py` & `physicsLab-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("D:/program physicsLab/hub/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="physicsLab",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.1.8",  # 包版本号，便于维护版本
+    version="1.1.9",  # 包版本号，便于维护版本
     author="Goodenough",  # 作者，可以写自己的姓名
     author_email="2381642961@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="Doing experiments in the physics lab AR by python",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://gitee.com/script2000/physicsLab",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

