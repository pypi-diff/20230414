# Comparing `tmp/neworder-1.2.1.tar.gz` & `tmp/neworder-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neworder-1.2.1.tar", last modified: Fri Apr 14 17:28:59 2023, max compression
+gzip compressed data, was "neworder-1.3.0.tar", last modified: Sun Apr  2 07:35:49 2023, max compression
```

## Comparing `neworder-1.2.1.tar` & `neworder-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-14 17:28:59.526253 neworder-1.2.1/
--rw-rw-r--   0 az        (1000) az        (1000)     1085 2023-01-06 19:30:47.000000 neworder-1.2.1/LICENCE.md
--rw-rw-r--   0 az        (1000) az        (1000)      107 2023-04-02 07:19:22.000000 neworder-1.2.1/MANIFEST.in
--rw-rw-r--   0 az        (1000) az        (1000)     4947 2023-04-14 17:28:59.526253 neworder-1.2.1/PKG-INFO
--rw-rw-r--   0 az        (1000) az        (1000)     4499 2023-04-14 07:57:06.000000 neworder-1.2.1/README.md
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-14 17:28:59.526253 neworder-1.2.1/neworder/
--rw-rw-r--   0 az        (1000) az        (1000)      299 2023-04-13 08:16:28.000000 neworder-1.2.1/neworder/__init__.py
--rw-rw-r--   0 az        (1000) az        (1000)    15890 2023-04-13 09:19:53.000000 neworder-1.2.1/neworder/__init__.pyi
--rw-rw-r--   0 az        (1000) az        (1000)     1290 2022-08-17 09:35:42.000000 neworder-1.2.1/neworder/df.pyi
--rw-rw-r--   0 az        (1000) az        (1000)     8827 2023-04-13 09:29:41.000000 neworder-1.2.1/neworder/domain.py
--rw-rw-r--   0 az        (1000) az        (1000)      383 2022-08-17 19:43:06.000000 neworder-1.2.1/neworder/mc.py
--rw-rw-r--   0 az        (1000) az        (1000)      298 2022-08-17 09:36:56.000000 neworder-1.2.1/neworder/mpi.pyi
--rw-rw-r--   0 az        (1000) az        (1000)        0 2022-03-13 13:41:33.000000 neworder-1.2.1/neworder/py.typed
--rw-rw-r--   0 az        (1000) az        (1000)     1328 2022-08-17 09:36:56.000000 neworder-1.2.1/neworder/stats.pyi
--rw-rw-r--   0 az        (1000) az        (1000)     1164 2022-08-17 09:36:56.000000 neworder-1.2.1/neworder/time.pyi
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-14 17:28:59.526253 neworder-1.2.1/neworder.egg-info/
--rw-rw-r--   0 az        (1000) az        (1000)     4947 2023-04-14 17:28:59.000000 neworder-1.2.1/neworder.egg-info/PKG-INFO
--rw-rw-r--   0 az        (1000) az        (1000)      723 2023-04-14 17:28:59.000000 neworder-1.2.1/neworder.egg-info/SOURCES.txt
--rw-rw-r--   0 az        (1000) az        (1000)        1 2023-04-14 17:28:59.000000 neworder-1.2.1/neworder.egg-info/dependency_links.txt
--rw-rw-r--   0 az        (1000) az        (1000)        1 2022-03-13 10:10:41.000000 neworder-1.2.1/neworder.egg-info/not-zip-safe
--rw-rw-r--   0 az        (1000) az        (1000)       20 2023-04-14 17:28:59.000000 neworder-1.2.1/neworder.egg-info/requires.txt
--rw-rw-r--   0 az        (1000) az        (1000)       24 2023-04-14 17:28:59.000000 neworder-1.2.1/neworder.egg-info/top_level.txt
--rw-rw-r--   0 az        (1000) az        (1000)      228 2023-03-13 18:45:48.000000 neworder-1.2.1/pyproject.toml
--rw-rw-r--   0 az        (1000) az        (1000)      290 2023-04-14 17:28:59.530253 neworder-1.2.1/setup.cfg
--rwxrwxr-x   0 az        (1000) az        (1000)     1591 2023-04-14 17:18:46.000000 neworder-1.2.1/setup.py
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-14 17:28:59.526253 neworder-1.2.1/src/
--rw-rw-r--   0 az        (1000) az        (1000)     4097 2022-01-15 09:49:56.000000 neworder-1.2.1/src/ArrayHelpers.h
--rw-rw-r--   0 az        (1000) az        (1000)     5789 2021-06-27 21:14:58.000000 neworder-1.2.1/src/DataFrame.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      633 2020-09-18 10:07:40.000000 neworder-1.2.1/src/DataFrame.h
--rw-rw-r--   0 az        (1000) az        (1000)      410 2020-10-21 18:49:46.000000 neworder-1.2.1/src/Error.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      547 2020-09-07 20:08:04.000000 neworder-1.2.1/src/Error.h
--rw-rw-r--   0 az        (1000) az        (1000)      577 2021-11-13 15:52:34.000000 neworder-1.2.1/src/Log.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     2313 2021-11-13 15:46:23.000000 neworder-1.2.1/src/Log.h
--rw-rw-r--   0 az        (1000) az        (1000)     3232 2021-11-13 15:53:53.000000 neworder-1.2.1/src/Model.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      893 2021-06-29 19:32:00.000000 neworder-1.2.1/src/Model.h
--rw-rw-r--   0 az        (1000) az        (1000)    12404 2022-08-17 19:54:21.000000 neworder-1.2.1/src/Module.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      662 2021-03-21 12:01:03.000000 neworder-1.2.1/src/Module.h
--rw-rw-r--   0 az        (1000) az        (1000)    14430 2022-03-13 13:41:33.000000 neworder-1.2.1/src/Module_docstr.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     9890 2023-01-07 19:45:30.000000 neworder-1.2.1/src/MonteCarlo.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     2949 2022-08-17 19:43:06.000000 neworder-1.2.1/src/MonteCarlo.h
--rw-rw-r--   0 az        (1000) az        (1000)      643 2021-07-05 18:31:34.000000 neworder-1.2.1/src/NPArray.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      526 2021-07-05 18:32:01.000000 neworder-1.2.1/src/NPArray.h
--rw-rw-r--   0 az        (1000) az        (1000)      393 2020-10-22 08:16:54.000000 neworder-1.2.1/src/NewOrder.h
--rw-rw-r--   0 az        (1000) az        (1000)    11492 2021-06-29 19:31:41.000000 neworder-1.2.1/src/Timeline.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     5911 2021-06-29 19:31:41.000000 neworder-1.2.1/src/Timeline.h
--rw-rw-r--   0 az        (1000) az        (1000)      550 2022-01-14 19:17:46.000000 neworder-1.2.1/src/Timer.h
+drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-02 07:35:49.854714 neworder-1.3.0/
+-rw-rw-r--   0 az        (1000) az        (1000)     1085 2023-01-06 19:30:47.000000 neworder-1.3.0/LICENCE.md
+-rw-rw-r--   0 az        (1000) az        (1000)      107 2023-04-02 07:19:22.000000 neworder-1.3.0/MANIFEST.in
+-rw-rw-r--   0 az        (1000) az        (1000)     4957 2023-04-02 07:35:49.854714 neworder-1.3.0/PKG-INFO
+-rw-rw-r--   0 az        (1000) az        (1000)     4509 2023-03-14 08:06:56.000000 neworder-1.3.0/README.md
+drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-02 07:35:49.850714 neworder-1.3.0/neworder/
+-rw-rw-r--   0 az        (1000) az        (1000)      334 2023-02-25 10:00:20.000000 neworder-1.3.0/neworder/__init__.py
+-rw-rw-r--   0 az        (1000) az        (1000)    15911 2023-01-22 10:16:05.000000 neworder-1.3.0/neworder/__init__.pyi
+-rw-rw-r--   0 az        (1000) az        (1000)     1290 2022-08-17 09:35:42.000000 neworder-1.3.0/neworder/df.pyi
+-rw-rw-r--   0 az        (1000) az        (1000)     7660 2022-08-17 09:35:47.000000 neworder-1.3.0/neworder/domain.py
+-rw-rw-r--   0 az        (1000) az        (1000)     2783 2023-01-22 10:16:05.000000 neworder-1.3.0/neworder/graph.py
+-rw-rw-r--   0 az        (1000) az        (1000)      383 2022-08-17 19:43:06.000000 neworder-1.3.0/neworder/mc.py
+-rw-rw-r--   0 az        (1000) az        (1000)      298 2022-08-17 09:36:56.000000 neworder-1.3.0/neworder/mpi.pyi
+-rw-rw-r--   0 az        (1000) az        (1000)        0 2022-03-13 13:41:33.000000 neworder-1.3.0/neworder/py.typed
+-rw-rw-r--   0 az        (1000) az        (1000)     1328 2022-08-17 09:36:56.000000 neworder-1.3.0/neworder/stats.pyi
+-rw-rw-r--   0 az        (1000) az        (1000)     1164 2022-08-17 09:36:56.000000 neworder-1.3.0/neworder/time.pyi
+drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-02 07:35:49.850714 neworder-1.3.0/neworder.egg-info/
+-rw-rw-r--   0 az        (1000) az        (1000)     4957 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/PKG-INFO
+-rw-rw-r--   0 az        (1000) az        (1000)      741 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/SOURCES.txt
+-rw-rw-r--   0 az        (1000) az        (1000)        1 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/dependency_links.txt
+-rw-rw-r--   0 az        (1000) az        (1000)        1 2022-03-13 10:10:41.000000 neworder-1.3.0/neworder.egg-info/not-zip-safe
+-rw-rw-r--   0 az        (1000) az        (1000)       45 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/requires.txt
+-rw-rw-r--   0 az        (1000) az        (1000)       24 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/top_level.txt
+-rw-rw-r--   0 az        (1000) az        (1000)      228 2023-03-13 18:45:48.000000 neworder-1.3.0/pyproject.toml
+-rw-rw-r--   0 az        (1000) az        (1000)      290 2023-04-02 07:35:49.854714 neworder-1.3.0/setup.cfg
+-rwxrwxr-x   0 az        (1000) az        (1000)     1625 2023-01-22 10:16:05.000000 neworder-1.3.0/setup.py
+drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-02 07:35:49.854714 neworder-1.3.0/src/
+-rw-rw-r--   0 az        (1000) az        (1000)     4097 2022-01-15 09:49:56.000000 neworder-1.3.0/src/ArrayHelpers.h
+-rw-rw-r--   0 az        (1000) az        (1000)     5789 2021-06-27 21:14:58.000000 neworder-1.3.0/src/DataFrame.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)      633 2020-09-18 10:07:40.000000 neworder-1.3.0/src/DataFrame.h
+-rw-rw-r--   0 az        (1000) az        (1000)      410 2020-10-21 18:49:46.000000 neworder-1.3.0/src/Error.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)      547 2020-09-07 20:08:04.000000 neworder-1.3.0/src/Error.h
+-rw-rw-r--   0 az        (1000) az        (1000)      577 2021-11-13 15:52:34.000000 neworder-1.3.0/src/Log.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)     2313 2021-11-13 15:46:23.000000 neworder-1.3.0/src/Log.h
+-rw-rw-r--   0 az        (1000) az        (1000)     3232 2021-11-13 15:53:53.000000 neworder-1.3.0/src/Model.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)      893 2021-06-29 19:32:00.000000 neworder-1.3.0/src/Model.h
+-rw-rw-r--   0 az        (1000) az        (1000)    12404 2022-08-17 19:54:21.000000 neworder-1.3.0/src/Module.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)      662 2021-03-21 12:01:03.000000 neworder-1.3.0/src/Module.h
+-rw-rw-r--   0 az        (1000) az        (1000)    14430 2022-03-13 13:41:33.000000 neworder-1.3.0/src/Module_docstr.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)     9890 2023-01-07 19:45:30.000000 neworder-1.3.0/src/MonteCarlo.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)     2949 2022-08-17 19:43:06.000000 neworder-1.3.0/src/MonteCarlo.h
+-rw-rw-r--   0 az        (1000) az        (1000)      643 2021-07-05 18:31:34.000000 neworder-1.3.0/src/NPArray.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)      526 2021-07-05 18:32:01.000000 neworder-1.3.0/src/NPArray.h
+-rw-rw-r--   0 az        (1000) az        (1000)      393 2020-10-22 08:16:54.000000 neworder-1.3.0/src/NewOrder.h
+-rw-rw-r--   0 az        (1000) az        (1000)    11492 2021-06-29 19:31:41.000000 neworder-1.3.0/src/Timeline.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)     5911 2021-06-29 19:31:41.000000 neworder-1.3.0/src/Timeline.h
+-rw-rw-r--   0 az        (1000) az        (1000)      550 2022-01-14 19:17:46.000000 neworder-1.3.0/src/Timer.h
```

### Comparing `neworder-1.2.1/LICENCE.md` & `neworder-1.3.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/PKG-INFO` & `neworder-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neworder
-Version: 1.2.1
+Version: 1.3.0
 Summary: A dynamic microsimulation framework
 Home-page: https://neworder.readthedocs.io
 Author: Andrew P Smith
 Author-email: andrew@friarswood.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -43,20 +43,20 @@
 - **reproducibility**: built-in, customisable random generator seeding strategies
 - **speed**: the module is predominantly written in optimised C++ and provides fast Monte-Carlo, statistical and data manipulation functions.
 - **compatibility**: operate directly on *numpy* arrays and *pandas* DataFrames
 - **scalability**: can be run on a desktop or a HPC cluster, supporting parallel execution using MPI.
 
 ## System Requirements
 
-*neworder* requires python 3.10 or above and runs on 64-bit linux, OSX and Windows platforms. To take advantage of the  parallel execution functionality, you may also need to install:
+*neworder* requires python 3.6 or above and runs on 64-bit linux, OSX and Windows platforms. In order to take advantage of the parallel execution functionality, the following are also required:
 
 - an MPI implementation, such as [mpich](https://www.mpich.org/), [open-mpi](https://www.open-mpi.org/) or [ms-mpi](https://docs.microsoft.com/en-us/message-passing-interface/microsoft-mpi)
 - the [mpi4py](https://mpi4py.readthedocs.io/en/stable/) package that provides python MPI bindings
 
-but the package works perfectly well in serial mode.
+but the module will work perfectly well in serial mode without these.
 
 ## Installation
 
 ### PyPI
 
 ```bash
 pip install neworder
@@ -70,16 +70,16 @@
 
 ### Docker
 
 The docker image contains all the examples, and should be run interactively. Some of the examples require permission to connect to the host's graphical display.
 
 ```bash
 docker pull virgesmith/neworder
-xhost +local:
-docker run --net=host -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
+xhost +
+docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
 ```
 
 NB The above works on ubuntu but may require modification on other OSs.
 
 Then in the container, e.g.
 
 ```bash
```

### Comparing `neworder-1.2.1/README.md` & `neworder-1.3.0/neworder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: neworder
+Version: 1.3.0
+Summary: A dynamic microsimulation framework
+Home-page: https://neworder.readthedocs.io
+Author: Andrew P Smith
+Author-email: andrew@friarswood.net
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENCE.md
+
 # neworder
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neworder)](https://pypi.org/project/neworder/)
 [![PyPI](https://img.shields.io/pypi/v/neworder)](https://pypi.org/project/neworder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/neworder)](https://pypi.org/project/neworder/)
 [![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/neworder/badges/version.svg)](https://anaconda.org/conda-forge/neworder)
 [![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/neworder/badges/downloads.svg)](https://anaconda.org/conda-forge/neworder)
@@ -28,20 +43,20 @@
 - **reproducibility**: built-in, customisable random generator seeding strategies
 - **speed**: the module is predominantly written in optimised C++ and provides fast Monte-Carlo, statistical and data manipulation functions.
 - **compatibility**: operate directly on *numpy* arrays and *pandas* DataFrames
 - **scalability**: can be run on a desktop or a HPC cluster, supporting parallel execution using MPI.
 
 ## System Requirements
 
-*neworder* requires python 3.10 or above and runs on 64-bit linux, OSX and Windows platforms. To take advantage of the  parallel execution functionality, you may also need to install:
+*neworder* requires python 3.6 or above and runs on 64-bit linux, OSX and Windows platforms. In order to take advantage of the parallel execution functionality, the following are also required:
 
 - an MPI implementation, such as [mpich](https://www.mpich.org/), [open-mpi](https://www.open-mpi.org/) or [ms-mpi](https://docs.microsoft.com/en-us/message-passing-interface/microsoft-mpi)
 - the [mpi4py](https://mpi4py.readthedocs.io/en/stable/) package that provides python MPI bindings
 
-but the package works perfectly well in serial mode.
+but the module will work perfectly well in serial mode without these.
 
 ## Installation
 
 ### PyPI
 
 ```bash
 pip install neworder
@@ -55,16 +70,16 @@
 
 ### Docker
 
 The docker image contains all the examples, and should be run interactively. Some of the examples require permission to connect to the host's graphical display.
 
 ```bash
 docker pull virgesmith/neworder
-xhost +local:
-docker run --net=host -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
+xhost +
+docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
 ```
 
 NB The above works on ubuntu but may require modification on other OSs.
 
 Then in the container, e.g.
 
 ```bash
@@ -73,7 +88,9 @@
 
 [//]: # (!readme!)
 
 ## Documentation
 
 To get started first see the detailed documentation [here](https://neworder.readthedocs.io). Then, check out "Hello World"
 and the other examples.
+
+
```

### Comparing `neworder-1.2.1/neworder/__init__.pyi` & `neworder-1.3.0/neworder/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 
 import df  # type: ignore
 import mpi # type: ignore
 from .time import *
 import stats # type: ignore
 from .domain import *
+from .graph import *
 
 T = TypeVar("T")
 nparray = np.ndarray[T, np.dtype[T]]
 
 __all__ = [
     "CalendarTimeline",
     "LinearTimeline",
```

### Comparing `neworder-1.2.1/neworder/df.pyi` & `neworder-1.3.0/neworder/df.pyi`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/neworder/domain.py` & `neworder-1.3.0/neworder/domain.py`

 * *Files 17% similar despite different names*

```diff
@@ -161,18 +161,14 @@
     # fill diagonal so as not to include self - TODO how does this work if to_points!=positions
     np.fill_diagonal(ind, 0)
     return ind if not count else np.sum(ind, axis=1)
 
   def __repr__(self) -> str:
     return "%s dim=%d min=%s max=%s edge=%s" % (self.__class__.__name__, self.dim, self.min, self.max, self.edge)
 
-def _bounce(i: int, N: int) -> int:
-  s = (i // N) % 2
-  k = i % N
-  return N * s + (-1) ** s * k
 
 class StateGrid(Domain):
   """
   Discrete rectangular n-dimensional finite grid domain with each cell having an integer state.
   Allows for counting of neighbours according to the supported edge behaviours:
     CONSTRAIN (no neighburs over edge), WRAP (toroidal), BOUNCE (reflect)
   """
@@ -183,51 +179,28 @@
     Edge.BOUNCE: "reflect"
   }
 
   def __init__(self, initial_values: np.ndarray, edge: Edge=Edge.CONSTRAIN):
     super().__init__(initial_values.ndim, edge, False)
 
     # StateGrid supports two edge behaviours
-    if edge not in [Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE]:
-      raise ValueError("edge policy must be one of Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE")
+    if edge not in [Edge.WRAP, Edge.CONSTRAIN]:
+      raise ValueError("edge policy must be one of Edge.WRAP, Edge.CONSTRAIN")
 
     if initial_values.ndim < 1:
       raise ValueError("state array must have dimension of 1 or above")
     if initial_values.size < 1:
       raise ValueError("state array must have size of 1 or above in every dimension")
 
     self.state = initial_values
 
     # int neighbour kernel (not including self)
     self.kernel = np.ones([3] * self.dim)
     self.kernel[(1,) * self.dim] = 0
 
-  def __get_point(self, p: tuple[int, ...]) -> tuple[int, ...]:
-    assert len(p) == self.state.ndim, f"dimensionality mismatch: {len(p)} but grid has {self.state.ndim}"
-    match self.edge:
-      case Edge.WRAP:
-        p = tuple(p[i] % self.state.shape[i] for i in range(len(p)))
-      case Edge.CONSTRAIN:
-        p = tuple(np.clip(p[i], 0, self.state.shape[i] - 1) for i in range(len(p)))
-      case Edge.BOUNCE:
-        p = tuple(_bounce(p[i], self.state.shape[i] - 1) for i in range(len(p)))
-    return p
-
-  def __getitem__(self, p: tuple[int, ...]) -> Any:
-    return self.state[self.__get_point(p)]
-
-  def __setitem__(self, p: tuple[int, ...], value: Any) -> None:
-    self.state[self.__get_point(p)] = value
-
-  def shift(self, position: tuple[int, ...], delta: tuple[int, ...]) -> tuple[int, ...]:
-    """This translates a point according to the grid's edge behaviour. It does *not* change any state"""
-    point = self.__get_point(position)
-    p = tuple(point[i] + delta[i] for i in range(self.dim))
-    return self.__get_point(p)
-
   @property
   def extent(self) -> Any:
     """ The extent of the space in terms of two opposing points """
     return self.state.shape
 
   def count_neighbours(self, indicator: Callable[[float], bool]=lambda x: x == 1) -> np.ndarray:
     """ Counts neighbouring cells with a state indicated by supplied indicator function """
```

### Comparing `neworder-1.2.1/neworder/stats.pyi` & `neworder-1.3.0/neworder/stats.pyi`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/neworder/time.pyi` & `neworder-1.3.0/neworder/time.pyi`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/neworder.egg-info/PKG-INFO` & `neworder-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: neworder
-Version: 1.2.1
-Summary: A dynamic microsimulation framework
-Home-page: https://neworder.readthedocs.io
-Author: Andrew P Smith
-Author-email: andrew@friarswood.net
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENCE.md
-
 # neworder
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neworder)](https://pypi.org/project/neworder/)
 [![PyPI](https://img.shields.io/pypi/v/neworder)](https://pypi.org/project/neworder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/neworder)](https://pypi.org/project/neworder/)
 [![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/neworder/badges/version.svg)](https://anaconda.org/conda-forge/neworder)
 [![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/neworder/badges/downloads.svg)](https://anaconda.org/conda-forge/neworder)
@@ -43,20 +28,20 @@
 - **reproducibility**: built-in, customisable random generator seeding strategies
 - **speed**: the module is predominantly written in optimised C++ and provides fast Monte-Carlo, statistical and data manipulation functions.
 - **compatibility**: operate directly on *numpy* arrays and *pandas* DataFrames
 - **scalability**: can be run on a desktop or a HPC cluster, supporting parallel execution using MPI.
 
 ## System Requirements
 
-*neworder* requires python 3.10 or above and runs on 64-bit linux, OSX and Windows platforms. To take advantage of the  parallel execution functionality, you may also need to install:
+*neworder* requires python 3.6 or above and runs on 64-bit linux, OSX and Windows platforms. In order to take advantage of the parallel execution functionality, the following are also required:
 
 - an MPI implementation, such as [mpich](https://www.mpich.org/), [open-mpi](https://www.open-mpi.org/) or [ms-mpi](https://docs.microsoft.com/en-us/message-passing-interface/microsoft-mpi)
 - the [mpi4py](https://mpi4py.readthedocs.io/en/stable/) package that provides python MPI bindings
 
-but the package works perfectly well in serial mode.
+but the module will work perfectly well in serial mode without these.
 
 ## Installation
 
 ### PyPI
 
 ```bash
 pip install neworder
@@ -70,16 +55,16 @@
 
 ### Docker
 
 The docker image contains all the examples, and should be run interactively. Some of the examples require permission to connect to the host's graphical display.
 
 ```bash
 docker pull virgesmith/neworder
-xhost +local:
-docker run --net=host -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
+xhost +
+docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
 ```
 
 NB The above works on ubuntu but may require modification on other OSs.
 
 Then in the container, e.g.
 
 ```bash
@@ -88,9 +73,7 @@
 
 [//]: # (!readme!)
 
 ## Documentation
 
 To get started first see the detailed documentation [here](https://neworder.readthedocs.io). Then, check out "Hello World"
 and the other examples.
-
-
```

### Comparing `neworder-1.2.1/neworder.egg-info/SOURCES.txt` & `neworder-1.3.0/neworder.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 neworder/__init__.py
 neworder/__init__.pyi
 neworder/df.pyi
 neworder/domain.py
+neworder/graph.py
 neworder/mc.py
 neworder/mpi.pyi
 neworder/py.typed
 neworder/stats.pyi
 neworder/time.pyi
 neworder.egg-info/PKG-INFO
 neworder.egg-info/SOURCES.txt
```

### Comparing `neworder-1.2.1/setup.py` & `neworder-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   url='https://neworder.readthedocs.io',
   description='A dynamic microsimulation framework',
   long_description=readme(),
   long_description_content_type="text/markdown",
   packages=["neworder"],
   package_data={"neworder": ["py.typed", "*.pyi"]},
   ext_modules=ext_modules,
-  install_requires=['pandas>=1.0.5', 'scipy'],
+  install_requires=['pandas>=1.0.5', 'scipy', 'networkx', 'osmnx', 'geopandas'],
   setup_requires=['pybind11>=2.5.0', 'pytest-runner', 'numpy>=1.19.1'],
   tests_require=['pytest', 'mpi4py>=3.0.3'],
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
```

### Comparing `neworder-1.2.1/src/ArrayHelpers.h` & `neworder-1.3.0/src/ArrayHelpers.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/DataFrame.cpp` & `neworder-1.3.0/src/DataFrame.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/DataFrame.h` & `neworder-1.3.0/src/DataFrame.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Error.h` & `neworder-1.3.0/src/Error.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Log.cpp` & `neworder-1.3.0/src/Log.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Log.h` & `neworder-1.3.0/src/Log.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Model.cpp` & `neworder-1.3.0/src/Model.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Model.h` & `neworder-1.3.0/src/Model.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Module.cpp` & `neworder-1.3.0/src/Module.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Module.h` & `neworder-1.3.0/src/Module.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Module_docstr.cpp` & `neworder-1.3.0/src/Module_docstr.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/MonteCarlo.cpp` & `neworder-1.3.0/src/MonteCarlo.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/MonteCarlo.h` & `neworder-1.3.0/src/MonteCarlo.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/NPArray.cpp` & `neworder-1.3.0/src/NPArray.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/NPArray.h` & `neworder-1.3.0/src/NPArray.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Timeline.cpp` & `neworder-1.3.0/src/Timeline.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Timeline.h` & `neworder-1.3.0/src/Timeline.h`

 * *Files identical despite different names*

### Comparing `neworder-1.2.1/src/Timer.h` & `neworder-1.3.0/src/Timer.h`

 * *Files identical despite different names*

