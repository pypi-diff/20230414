# Comparing `tmp/feedgenerator-2.0.0.tar.gz` & `tmp/feedgenerator-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedgenerator-2.0.0.tar", last modified: Tue Sep 28 11:39:38 2021, max compression
+gzip compressed data, was "feedgenerator-2.1.0.tar", last modified: Fri Apr 14 10:40:55 2023, max compression
```

## Comparing `feedgenerator-2.0.0.tar` & `feedgenerator-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxr-xr-x   0 jm         (501) staff       (20)        0 2021-09-28 11:39:38.640110 feedgenerator-2.0.0/
--rw-r--r--   0 jm         (501) staff       (20)     1553 2021-08-18 10:33:01.000000 feedgenerator-2.0.0/LICENSE
--rw-r--r--   0 jm         (501) staff       (20)       75 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/MANIFEST.in
--rw-r--r--   0 jm         (501) staff       (20)     1724 2021-09-28 11:39:38.640296 feedgenerator-2.0.0/PKG-INFO
--rw-r--r--   0 jm         (501) staff       (20)      606 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/README.rst
-drwxr-xr-x   0 jm         (501) staff       (20)        0 2021-09-28 11:39:38.630188 feedgenerator-2.0.0/feedgenerator/
--rw-r--r--   0 jm         (501) staff       (20)      780 2020-02-09 08:40:59.000000 feedgenerator-2.0.0/feedgenerator/__init__.py
-drwxr-xr-x   0 jm         (501) staff       (20)        0 2021-09-28 11:39:38.632458 feedgenerator-2.0.0/feedgenerator/django/
--rw-r--r--   0 jm         (501) staff       (20)        0 2020-02-09 08:40:59.000000 feedgenerator-2.0.0/feedgenerator/django/__init__.py
-drwxr-xr-x   0 jm         (501) staff       (20)        0 2021-09-28 11:39:38.634588 feedgenerator-2.0.0/feedgenerator/django/utils/
--rw-r--r--   0 jm         (501) staff       (20)        0 2020-02-09 08:40:59.000000 feedgenerator-2.0.0/feedgenerator/django/utils/__init__.py
--rw-r--r--   0 jm         (501) staff       (20)     2685 2021-08-18 09:26:13.000000 feedgenerator-2.0.0/feedgenerator/django/utils/datetime_safe.py
--rw-r--r--   0 jm         (501) staff       (20)     7836 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/feedgenerator/django/utils/encoding.py
--rw-r--r--   0 jm         (501) staff       (20)    16360 2021-09-28 11:09:39.000000 feedgenerator-2.0.0/feedgenerator/django/utils/feedgenerator.py
--rw-r--r--   0 jm         (501) staff       (20)    11335 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/feedgenerator/django/utils/functional.py
--rw-r--r--   0 jm         (501) staff       (20)     8478 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/feedgenerator/django/utils/timezone.py
--rw-r--r--   0 jm         (501) staff       (20)      705 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/feedgenerator/django/utils/xmlutils.py
-drwxr-xr-x   0 jm         (501) staff       (20)        0 2021-09-28 11:39:38.632170 feedgenerator-2.0.0/feedgenerator.egg-info/
--rw-r--r--   0 jm         (501) staff       (20)     1724 2021-09-28 11:39:38.000000 feedgenerator-2.0.0/feedgenerator.egg-info/PKG-INFO
--rw-r--r--   0 jm         (501) staff       (20)      978 2021-09-28 11:39:38.000000 feedgenerator-2.0.0/feedgenerator.egg-info/SOURCES.txt
--rw-r--r--   0 jm         (501) staff       (20)        1 2021-09-28 11:39:38.000000 feedgenerator-2.0.0/feedgenerator.egg-info/dependency_links.txt
--rw-r--r--   0 jm         (501) staff       (20)        1 2020-02-09 10:52:08.000000 feedgenerator-2.0.0/feedgenerator.egg-info/not-zip-safe
--rw-r--r--   0 jm         (501) staff       (20)        9 2021-09-28 11:39:38.000000 feedgenerator-2.0.0/feedgenerator.egg-info/requires.txt
--rw-r--r--   0 jm         (501) staff       (20)       14 2021-09-28 11:39:38.000000 feedgenerator-2.0.0/feedgenerator.egg-info/top_level.txt
--rw-r--r--   0 jm         (501) staff       (20)      199 2021-09-28 11:39:38.641083 feedgenerator-2.0.0/setup.cfg
--rw-r--r--   0 jm         (501) staff       (20)     1958 2021-09-28 11:34:59.000000 feedgenerator-2.0.0/setup.py
-drwxr-xr-x   0 jm         (501) staff       (20)        0 2021-09-28 11:39:38.636441 feedgenerator-2.0.0/tests_feedgenerator/
--rw-r--r--   0 jm         (501) staff       (20)        0 2020-02-09 08:40:59.000000 feedgenerator-2.0.0/tests_feedgenerator/__init__.py
-drwxr-xr-x   0 jm         (501) staff       (20)        0 2021-09-28 11:39:38.639177 feedgenerator-2.0.0/tests_feedgenerator/__pycache__/
--rw-r--r--   0 jm         (501) staff       (20)      155 2021-09-27 15:07:34.000000 feedgenerator-2.0.0/tests_feedgenerator/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jm         (501) staff       (20)     6098 2021-09-28 11:37:39.000000 feedgenerator-2.0.0/tests_feedgenerator/__pycache__/test_feedgenerator.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jm         (501) staff       (20)     1511 2021-09-28 11:37:39.000000 feedgenerator-2.0.0/tests_feedgenerator/__pycache__/test_stringio.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jm         (501) staff       (20)     6267 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/tests_feedgenerator/test_feedgenerator.py
--rw-r--r--   0 jm         (501) staff       (20)     2568 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/tests_feedgenerator/test_stringio.py
--rw-r--r--   0 jm         (501) staff       (20)      923 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/tests_feedgenerator/usage_example.py
--rw-r--r--   0 jm         (501) staff       (20)      225 2021-09-28 11:03:34.000000 feedgenerator-2.0.0/tox.ini
+drwxr-xr-x   0 jm         (501) staff       (20)        0 2023-04-14 10:40:55.852393 feedgenerator-2.1.0/
+-rw-r--r--   0 jm         (501) staff       (20)     1552 2023-03-27 07:32:32.000000 feedgenerator-2.1.0/LICENSE
+-rw-r--r--   0 jm         (501) staff       (20)       89 2023-03-27 07:26:35.000000 feedgenerator-2.1.0/MANIFEST.in
+-rw-r--r--   0 jm         (501) staff       (20)     1762 2023-04-14 10:40:55.852462 feedgenerator-2.1.0/PKG-INFO
+-rw-r--r--   0 jm         (501) staff       (20)      629 2023-03-27 07:54:32.000000 feedgenerator-2.1.0/README.rst
+drwxr-xr-x   0 jm         (501) staff       (20)        0 2023-04-14 10:40:55.847263 feedgenerator-2.1.0/feedgenerator/
+-rw-r--r--   0 jm         (501) staff       (20)      780 2020-02-09 08:40:59.000000 feedgenerator-2.1.0/feedgenerator/__init__.py
+drwxr-xr-x   0 jm         (501) staff       (20)        0 2023-04-14 10:40:55.848772 feedgenerator-2.1.0/feedgenerator/django/
+-rw-r--r--   0 jm         (501) staff       (20)        0 2020-02-09 08:40:59.000000 feedgenerator-2.1.0/feedgenerator/django/__init__.py
+drwxr-xr-x   0 jm         (501) staff       (20)        0 2023-04-14 10:40:55.850985 feedgenerator-2.1.0/feedgenerator/django/utils/
+-rw-r--r--   0 jm         (501) staff       (20)        0 2020-02-09 08:40:59.000000 feedgenerator-2.1.0/feedgenerator/django/utils/__init__.py
+-rw-r--r--   0 jm         (501) staff       (20)     2685 2021-08-18 09:26:13.000000 feedgenerator-2.1.0/feedgenerator/django/utils/datetime_safe.py
+-rw-r--r--   0 jm         (501) staff       (20)     7829 2023-03-27 07:40:50.000000 feedgenerator-2.1.0/feedgenerator/django/utils/encoding.py
+-rw-r--r--   0 jm         (501) staff       (20)    16360 2021-09-28 11:09:39.000000 feedgenerator-2.1.0/feedgenerator/django/utils/feedgenerator.py
+-rw-r--r--   0 jm         (501) staff       (20)    11335 2021-09-28 11:03:34.000000 feedgenerator-2.1.0/feedgenerator/django/utils/functional.py
+-rw-r--r--   0 jm         (501) staff       (20)     8478 2021-09-28 11:03:34.000000 feedgenerator-2.1.0/feedgenerator/django/utils/timezone.py
+-rw-r--r--   0 jm         (501) staff       (20)      705 2021-09-28 11:03:34.000000 feedgenerator-2.1.0/feedgenerator/django/utils/xmlutils.py
+drwxr-xr-x   0 jm         (501) staff       (20)        0 2023-04-14 10:40:55.848621 feedgenerator-2.1.0/feedgenerator.egg-info/
+-rw-r--r--   0 jm         (501) staff       (20)     1762 2023-04-14 10:40:55.000000 feedgenerator-2.1.0/feedgenerator.egg-info/PKG-INFO
+-rw-r--r--   0 jm         (501) staff       (20)      728 2023-04-14 10:40:55.000000 feedgenerator-2.1.0/feedgenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 jm         (501) staff       (20)        1 2023-04-14 10:40:55.000000 feedgenerator-2.1.0/feedgenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 jm         (501) staff       (20)        1 2020-02-09 10:52:08.000000 feedgenerator-2.1.0/feedgenerator.egg-info/not-zip-safe
+-rw-r--r--   0 jm         (501) staff       (20)        9 2023-04-14 10:40:55.000000 feedgenerator-2.1.0/feedgenerator.egg-info/requires.txt
+-rw-r--r--   0 jm         (501) staff       (20)       14 2023-04-14 10:40:55.000000 feedgenerator-2.1.0/feedgenerator.egg-info/top_level.txt
+-rw-r--r--   0 jm         (501) staff       (20)      504 2023-04-14 10:34:42.000000 feedgenerator-2.1.0/pyproject.toml
+-rw-r--r--   0 jm         (501) staff       (20)      185 2023-04-14 10:40:55.852704 feedgenerator-2.1.0/setup.cfg
+-rw-r--r--   0 jm         (501) staff       (20)     2002 2023-04-14 10:36:03.000000 feedgenerator-2.1.0/setup.py
+drwxr-xr-x   0 jm         (501) staff       (20)        0 2023-04-14 10:40:55.851997 feedgenerator-2.1.0/tests/
+-rw-r--r--   0 jm         (501) staff       (20)        0 2021-11-03 16:07:18.000000 feedgenerator-2.1.0/tests/__init__.py
+-rw-r--r--   0 jm         (501) staff       (20)     5986 2023-03-27 07:36:36.000000 feedgenerator-2.1.0/tests/test_feedgenerator.py
+-rw-r--r--   0 jm         (501) staff       (20)     2200 2021-11-03 16:07:18.000000 feedgenerator-2.1.0/tests/test_stringio.py
+-rw-r--r--   0 jm         (501) staff       (20)      923 2021-11-03 16:07:18.000000 feedgenerator-2.1.0/tests/usage_example.py
+-rw-r--r--   0 jm         (501) staff       (20)      284 2023-03-27 07:32:32.000000 feedgenerator-2.1.0/tox.ini
```

### Comparing `feedgenerator-2.0.0/LICENSE` & `feedgenerator-2.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,7 @@
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
 ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `feedgenerator-2.0.0/PKG-INFO` & `feedgenerator-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 Metadata-Version: 2.1
 Name: feedgenerator
-Version: 2.0.0
+Version: 2.1.0
 Summary: Standalone version of django.utils.feedgenerator
 Home-page: https://github.com/getpelican/feedgenerator
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
 Maintainer: Pelican Dev Team
 Maintainer-email: authors@getpelican.com
-License: UNKNOWN
 Keywords: feed,atom,rss
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Pelican
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 FeedGenerator
 =============
 
 |githubci| |pypi|
 
-.. |githubci| image:: https://img.shields.io/github/workflow/status/getpelican/feedgenerator/build
+.. |githubci| image:: https://img.shields.io/github/actions/workflow/status/getpelican/feedgenerator/main.yml?branch=main
     :target: https://github.com/getpelican/feedgenerator/actions
     :alt: Build Status
 
 .. |pypi| image:: https://img.shields.io/pypi/v/feedgenerator
     :target: https://pypi.org/project/feedgenerator/
     :alt: PyPI Version
 
 FeedGenerator is a standalone version of Django’s feedgenerator_ module.
 It has evolved over time and includes numerous enhancements.
 
 .. _feedgenerator: https://github.com/django/django/blob/master/django/utils/feedgenerator.py
-
-
```

### Comparing `feedgenerator-2.0.0/README.rst` & `feedgenerator-2.1.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 FeedGenerator
 =============
 
 |githubci| |pypi|
 
-.. |githubci| image:: https://img.shields.io/github/workflow/status/getpelican/feedgenerator/build
+.. |githubci| image:: https://img.shields.io/github/actions/workflow/status/getpelican/feedgenerator/main.yml?branch=main
     :target: https://github.com/getpelican/feedgenerator/actions
     :alt: Build Status
 
 .. |pypi| image:: https://img.shields.io/pypi/v/feedgenerator
     :target: https://pypi.org/project/feedgenerator/
     :alt: PyPI Version
```

### Comparing `feedgenerator-2.0.0/feedgenerator/__init__.py` & `feedgenerator-2.1.0/feedgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `feedgenerator-2.0.0/feedgenerator/django/utils/datetime_safe.py` & `feedgenerator-2.1.0/feedgenerator/django/utils/datetime_safe.py`

 * *Files identical despite different names*

### Comparing `feedgenerator-2.0.0/feedgenerator/django/utils/encoding.py` & `feedgenerator-2.1.0/feedgenerator/django/utils/encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,11 +191,11 @@
     # some flexibility for hardcoding separators.
     return quote(smart_bytes(path.replace("\\", "/")), safe=b"/~!*()'")
 
 # The encoding of the default system locale but falls back to the
 # given fallback encoding if the encoding is unsupported by python or could
 # not be determined.  See tickets #10335 and #5846
 try:
-    DEFAULT_LOCALE_ENCODING = locale.getdefaultlocale()[1] or 'ascii'
+    DEFAULT_LOCALE_ENCODING = locale.getlocale()[1] or 'ascii'
     codecs.lookup(DEFAULT_LOCALE_ENCODING)
 except:
     DEFAULT_LOCALE_ENCODING = 'ascii'
```

### Comparing `feedgenerator-2.0.0/feedgenerator/django/utils/feedgenerator.py` & `feedgenerator-2.1.0/feedgenerator/django/utils/feedgenerator.py`

 * *Files identical despite different names*

### Comparing `feedgenerator-2.0.0/feedgenerator/django/utils/functional.py` & `feedgenerator-2.1.0/feedgenerator/django/utils/functional.py`

 * *Files identical despite different names*

### Comparing `feedgenerator-2.0.0/feedgenerator/django/utils/timezone.py` & `feedgenerator-2.1.0/feedgenerator/django/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `feedgenerator-2.0.0/feedgenerator/django/utils/xmlutils.py` & `feedgenerator-2.1.0/feedgenerator/django/utils/xmlutils.py`

 * *Files identical despite different names*

### Comparing `feedgenerator-2.0.0/feedgenerator.egg-info/PKG-INFO` & `feedgenerator-2.1.0/feedgenerator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 Metadata-Version: 2.1
 Name: feedgenerator
-Version: 2.0.0
+Version: 2.1.0
 Summary: Standalone version of django.utils.feedgenerator
 Home-page: https://github.com/getpelican/feedgenerator
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
 Maintainer: Pelican Dev Team
 Maintainer-email: authors@getpelican.com
-License: UNKNOWN
 Keywords: feed,atom,rss
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Pelican
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 FeedGenerator
 =============
 
 |githubci| |pypi|
 
-.. |githubci| image:: https://img.shields.io/github/workflow/status/getpelican/feedgenerator/build
+.. |githubci| image:: https://img.shields.io/github/actions/workflow/status/getpelican/feedgenerator/main.yml?branch=main
     :target: https://github.com/getpelican/feedgenerator/actions
     :alt: Build Status
 
 .. |pypi| image:: https://img.shields.io/pypi/v/feedgenerator
     :target: https://pypi.org/project/feedgenerator/
     :alt: PyPI Version
 
 FeedGenerator is a standalone version of Django’s feedgenerator_ module.
 It has evolved over time and includes numerous enhancements.
 
 .. _feedgenerator: https://github.com/django/django/blob/master/django/utils/feedgenerator.py
-
-
```

### Comparing `feedgenerator-2.0.0/feedgenerator.egg-info/SOURCES.txt` & `feedgenerator-2.1.0/feedgenerator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 feedgenerator/__init__.py
 feedgenerator.egg-info/PKG-INFO
 feedgenerator.egg-info/SOURCES.txt
 feedgenerator.egg-info/dependency_links.txt
@@ -15,14 +16,11 @@
 feedgenerator/django/utils/__init__.py
 feedgenerator/django/utils/datetime_safe.py
 feedgenerator/django/utils/encoding.py
 feedgenerator/django/utils/feedgenerator.py
 feedgenerator/django/utils/functional.py
 feedgenerator/django/utils/timezone.py
 feedgenerator/django/utils/xmlutils.py
-tests_feedgenerator/__init__.py
-tests_feedgenerator/test_feedgenerator.py
-tests_feedgenerator/test_stringio.py
-tests_feedgenerator/usage_example.py
-tests_feedgenerator/__pycache__/__init__.cpython-39.pyc
-tests_feedgenerator/__pycache__/test_feedgenerator.cpython-39-pytest-6.2.5.pyc
-tests_feedgenerator/__pycache__/test_stringio.cpython-39-pytest-6.2.5.pyc
+tests/__init__.py
+tests/test_feedgenerator.py
+tests/test_stringio.py
+tests/usage_example.py
```

### Comparing `feedgenerator-2.0.0/setup.py` & `feedgenerator-2.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,41 +16,42 @@
 CLASSIFIERS = ['Development Status :: 5 - Production/Stable',
                'Environment :: Web Environment',
                'Framework :: Pelican',
                'Intended Audience :: Developers',
                'License :: OSI Approved :: BSD License',
                'Operating System :: OS Independent',
                'Programming Language :: Python',
-               'Programming Language :: Python :: 3.6',
                'Programming Language :: Python :: 3.7',
                'Programming Language :: Python :: 3.8',
                'Programming Language :: Python :: 3.9',
+               'Programming Language :: Python :: 3.10',
+               'Programming Language :: Python :: 3.11',
                'Topic :: Internet :: WWW/HTTP',
                'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
                'Topic :: Software Development :: Libraries :: Python Modules',
                ]
 
 AUTHOR = 'Django Software Foundation'
 AUTHOR_EMAIL = 'foundation@djangoproject.com'
 MAINTAINER = 'Pelican Dev Team'
 MAINTAINER_EMAIL = 'authors@getpelican.com'
 KEYWORDS = "feed atom rss".split(' ')
-VERSION = '2.0.0'
+VERSION = '2.1.0'
 
-TEST_SUITE = 'tests_feedgenerator'
+TEST_SUITE = 'tests'
 
 REQUIRES = ['pytz >= 0a']
 
 setup(
     name=NAME,
     version=VERSION,
     packages=PACKAGES,
     test_suite=TEST_SUITE,
     install_requires=REQUIRES,
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     # metadata for upload to PyPI
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     maintainer=MAINTAINER,
     maintainer_email=MAINTAINER_EMAIL,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

### Comparing `feedgenerator-2.0.0/tests_feedgenerator/test_feedgenerator.py` & `feedgenerator-2.1.0/tests/test_feedgenerator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,107 +1,104 @@
-import unittest
-
 import datetime
 
+import pytest
+
 import feedgenerator
 
-import pytest
 
 FIXT_FEED = dict(
     title="Poynter E-Media Tidbits",
     link="http://www.poynter.org/column.asp?id=31",
     description="""A group Weblog by the sharpest minds in online media/journalism/publishing.
     Umlauts: äöüßÄÖÜ
     Chinese: 老师是四十四，是不是？
     Finnish: Mustan kissan paksut posket. (ah, no special chars) Kärpänen sanoi kärpäselle: tuu kattoon kattoon ku kaveri tapettiin tapettiin.
     """,
     language="en"
 )
 FIXT_ITEM = dict(
     title="Hello",
-    link="http://www.holovaty.com/test/",
+    link="http://www.holovaty.com/täst/",
     description="Testing.",
     content="Full content of our testing entry.",
     pubdate=datetime.datetime(2016,8,11,0,0,0,0),
 )
 
 
 EXPECTED_RESULT_RSS = """<?xml version="1.0" encoding="utf-8"?>
 <rss version="2.0"><channel><title>Poynter E-Media Tidbits</title><link>http://www.poynter.org/column.asp?id=31</link><description>A group Weblog by the sharpest minds in online media/journalism/publishing.
     Umlauts: äöüßÄÖÜ
     Chinese: 老师是四十四，是不是？
     Finnish: Mustan kissan paksut posket. (ah, no special chars) Kärpänen sanoi kärpäselle: tuu kattoon kattoon ku kaveri tapettiin tapettiin.
-    </description><language>en</language><lastBuildDate>%DATE%</lastBuildDate><item><title>Hello</title><link>http://www.holovaty.com/test/</link><description>Testing.</description><pubDate>Thu, 11 Aug 2016 00:00:00 -0000</pubDate></item></channel></rss>"""
+    </description><language>en</language><lastBuildDate>%DATE%</lastBuildDate><item><title>Hello</title><link>http://www.holovaty.com/t%C3%A4st/</link><description>Testing.</description><pubDate>Thu, 11 Aug 2016 00:00:00 -0000</pubDate></item></channel></rss>"""
 
 EXPECTED_RESULT_ATOM = """<?xml version="1.0" encoding="utf-8"?>
 <feed xml:lang="en" xmlns="http://www.w3.org/2005/Atom"><title>Poynter E-Media Tidbits</title><link href="http://www.poynter.org/column.asp?id=31" rel="alternate"></link><id>http://www.poynter.org/column.asp?id=31</id><updated>%DATE%</updated><subtitle>A group Weblog by the sharpest minds in online media/journalism/publishing.
     Umlauts: äöüßÄÖÜ
     Chinese: 老师是四十四，是不是？
     Finnish: Mustan kissan paksut posket. (ah, no special chars) Kärpänen sanoi kärpäselle: tuu kattoon kattoon ku kaveri tapettiin tapettiin.
-    </subtitle><entry><title>Hello</title><link href="http://www.holovaty.com/test/" rel="alternate"></link><published>2016-08-11T00:00:00Z</published><updated>2016-08-11T00:00:00Z</updated><id>tag:www.holovaty.com,2016-08-11:/test/</id><summary type="html">Testing.</summary><content type="html">Full content of our testing entry.</content></entry></feed>"""
+    </subtitle><entry><title>Hello</title><link href="http://www.holovaty.com/t%C3%A4st/" rel="alternate"></link><published>2016-08-11T00:00:00Z</published><updated>2016-08-11T00:00:00Z</updated><id>tag:www.holovaty.com,2016-08-11:/t%C3%A4st/</id><summary type="html">Testing.</summary><content type="html">Full content of our testing entry.</content></entry></feed>"""
 
 ENCODING = 'utf-8'
 
 def build_expected_rss_result(feed, expected_result, encoding):
     # Result's date is of course different from the date in the fixture.
     # So make them equal!
     d = feedgenerator.rfc2822_date(feed.latest_post_date())
     s = expected_result.replace('%DATE%', d)
     if encoding:
         return s.encode(encoding)
     else:
         return s
 
+
 def build_expected_atom_result(feed, expected_result, encoding):
     # Result's date is of course different from the date in the fixture.
     # So make them equal!
     d = feedgenerator.rfc3339_date(feed.latest_post_date())
     s = expected_result.replace('%DATE%', d)
     if encoding:
         return s.encode(encoding)
     else:
         return s
 
-class TestFeedGenerator(unittest.TestCase):
-
-    def setUp(self):
-        self.maxDiff = None
 
-    def test_000_types(self):
-        ty = str
-        for k, v in FIXT_FEED.items():
-            self.assertEqual(type(v), ty)
-        for k, v in FIXT_ITEM.items():
-            if k == "pubdate" or k == "updateddate":
-                self.assertEqual(type(v), datetime.datetime)
-            else:
-                self.assertEqual(type(v), ty)
-        self.assertEqual(type(EXPECTED_RESULT_RSS), ty)
-
-    def test_001_string_results_rss(self):
-        #import ipdb; ipdb.set_trace()
-        feed = feedgenerator.Rss201rev2Feed(**FIXT_FEED)
-        feed.add_item(**FIXT_ITEM)
-        result = feed.writeString(ENCODING)
-        # On Python 3, result of feedgenerator is a unicode string!
-        # So do not encode our expected_result.
-        expected_result = build_expected_rss_result(feed, EXPECTED_RESULT_RSS, None)
-        self.assertEqual(type(result), type(expected_result))
-        self.assertEqual(result, expected_result)
-
-    def test_002_string_results_atom(self):
-        #import ipdb; ipdb.set_trace()
-        feed = feedgenerator.Atom1Feed(**FIXT_FEED)
-        feed.add_item(**FIXT_ITEM)
-        result = feed.writeString(ENCODING)
-        # On Python 3, result of feedgenerator is a unicode string!
-        # So do not encode our expected_result.
-        expected_result = build_expected_atom_result(feed, EXPECTED_RESULT_ATOM, None)
-        self.assertEqual(type(result), type(expected_result))
-        self.assertEqual(result, expected_result)
+def test_000_types():
+    for k, v in FIXT_FEED.items():
+        assert isinstance(v, str)
+    for k, v in FIXT_ITEM.items():
+        if k == "pubdate" or k == "updateddate":
+            assert isinstance(v, datetime.datetime)
+        else:
+            assert isinstance(v, str)
+    assert isinstance(EXPECTED_RESULT_RSS, str)
+
+
+def test_001_string_results_rss():
+    #import ipdb; ipdb.set_trace()
+    feed = feedgenerator.Rss201rev2Feed(**FIXT_FEED)
+    feed.add_item(**FIXT_ITEM)
+    result = feed.writeString(ENCODING)
+    # On Python 3, result of feedgenerator is a unicode string!
+    # So do not encode our expected_result.
+    expected_result = build_expected_rss_result(feed, EXPECTED_RESULT_RSS, None)
+    assert isinstance(result, type(expected_result))
+    assert result == expected_result
+
+
+def test_002_string_results_atom():
+    #import ipdb; ipdb.set_trace()
+    feed = feedgenerator.Atom1Feed(**FIXT_FEED)
+    feed.add_item(**FIXT_ITEM)
+    result = feed.writeString(ENCODING)
+    # On Python 3, result of feedgenerator is a unicode string!
+    # So do not encode our expected_result.
+    expected_result = build_expected_atom_result(feed, EXPECTED_RESULT_ATOM, None)
+    assert isinstance(result, type(expected_result))
+    assert result == expected_result
 
 
 @pytest.mark.parametrize("description, subtitle, fragment, nonfragment", [
     # Neither description nor subtitle are provided
     (None, None, None, "<subtitle></subtitle>"),
     ("", "", None, "<subtitle></subtitle>"),
     # Description is provided
```

### Comparing `feedgenerator-2.0.0/tests_feedgenerator/usage_example.py` & `feedgenerator-2.1.0/tests/usage_example.py`

 * *Files identical despite different names*

