# Comparing `tmp/bassmap-0.0.1.tar.gz` & `tmp/bassmap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bassmap-0.0.1.tar", last modified: Tue Feb 28 05:52:41 2023, max compression
+gzip compressed data, was "bassmap-0.0.2.tar", last modified: Fri Apr 14 20:01:32 2023, max compression
```

## Comparing `bassmap-0.0.1.tar` & `bassmap-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 05:52:41.547165 bassmap-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-02-28 05:02:23.000000 bassmap-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-02-28 05:02:23.000000 bassmap-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1454 2023-02-28 05:52:41.547165 bassmap-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-02-28 05:02:23.000000 bassmap-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 05:52:41.530162 bassmap-0.0.1/bassmap/
--rw-rw-rw-   0        0        0      132 2023-02-28 05:02:23.000000 bassmap-0.0.1/bassmap/__init__.py
--rw-rw-rw-   0        0        0       20 2023-02-28 05:02:23.000000 bassmap-0.0.1/bassmap/bassmap.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:52:41.546166 bassmap-0.0.1/bassmap.egg-info/
--rw-rw-rw-   0        0        0     1454 2023-02-28 05:52:41.000000 bassmap-0.0.1/bassmap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-02-28 05:52:41.000000 bassmap-0.0.1/bassmap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 05:52:41.000000 bassmap-0.0.1/bassmap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-28 05:52:41.000000 bassmap-0.0.1/bassmap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-02-28 05:52:41.000000 bassmap-0.0.1/bassmap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-28 05:02:23.000000 bassmap-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      415 2023-02-28 05:52:41.548166 bassmap-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1841 2023-02-28 05:02:23.000000 bassmap-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:01:32.695640 bassmap-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 20:01:19.000000 bassmap-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 20:01:19.000000 bassmap-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 20:01:32.695640 bassmap-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 20:01:19.000000 bassmap-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:01:32.695640 bassmap-0.0.2/bassmap/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 20:01:19.000000 bassmap-0.0.2/bassmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-14 20:01:19.000000 bassmap-0.0.2/bassmap/bassmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:01:32.695640 bassmap-0.0.2/bassmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 20:01:19.000000 bassmap-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 20:01:32.695640 bassmap-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-14 20:01:19.000000 bassmap-0.0.2/setup.py
```

### Comparing `bassmap-0.0.1/PKG-INFO` & `bassmap-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
-Name: bassmap
-Version: 0.0.1
-Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
-Home-page: https://github.com/bassneel/bassmap
-Author: Bass Neel
-Author-email: maps.bassneel@gmail.com
-License: MIT license
-Keywords: bassmap
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# bassmap
-
-
-[![image](https://img.shields.io/pypi/v/bassmap.svg)](https://pypi.python.org/pypi/bassmap)
-[![image](https://img.shields.io/conda/vn/conda-forge/bassmap.svg)](https://anaconda.org/conda-forge/bassmap)
-
-
-**Python Boilerplate contains all the boilerplate you need to create a Python package.**
-
-
--   Free software: MIT license
--   Documentation: https://bassneel.github.io/bassmap
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: bassmap
+Version: 0.0.2
+Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
+Home-page: https://github.com/bassneel/bassmap
+Author: Bass Neel
+Author-email: maps.bassneel@gmail.com
+License: MIT license
+Keywords: bassmap
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# bassmap
+
+
+[![image](https://img.shields.io/pypi/v/bassmap.svg)](https://pypi.python.org/pypi/bassmap)
+[![image](https://img.shields.io/conda/vn/conda-forge/bassmap.svg)](https://anaconda.org/conda-forge/bassmap)
+
+
+**Python Boilerplate contains all the boilerplate you need to create a Python package.**
+
+
+-   Free software: MIT license
+-   Documentation: https://bassneel.github.io/bassmap
+    
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `bassmap-0.0.1/bassmap.egg-info/PKG-INFO` & `bassmap-0.0.2/bassmap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
-Name: bassmap
-Version: 0.0.1
-Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
-Home-page: https://github.com/bassneel/bassmap
-Author: Bass Neel
-Author-email: maps.bassneel@gmail.com
-License: MIT license
-Keywords: bassmap
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# bassmap
-
-
-[![image](https://img.shields.io/pypi/v/bassmap.svg)](https://pypi.python.org/pypi/bassmap)
-[![image](https://img.shields.io/conda/vn/conda-forge/bassmap.svg)](https://anaconda.org/conda-forge/bassmap)
-
-
-**Python Boilerplate contains all the boilerplate you need to create a Python package.**
-
-
--   Free software: MIT license
--   Documentation: https://bassneel.github.io/bassmap
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: bassmap
+Version: 0.0.2
+Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
+Home-page: https://github.com/bassneel/bassmap
+Author: Bass Neel
+Author-email: maps.bassneel@gmail.com
+License: MIT license
+Keywords: bassmap
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# bassmap
+
+
+[![image](https://img.shields.io/pypi/v/bassmap.svg)](https://pypi.python.org/pypi/bassmap)
+[![image](https://img.shields.io/conda/vn/conda-forge/bassmap.svg)](https://anaconda.org/conda-forge/bassmap)
+
+
+**Python Boilerplate contains all the boilerplate you need to create a Python package.**
+
+
+-   Free software: MIT license
+-   Documentation: https://bassneel.github.io/bassmap
+    
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `bassmap-0.0.1/setup.py` & `bassmap-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="Bass Neel",
-    author_email='maps.bassneel@gmail.com',
-    python_requires='>=3.7',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
-    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='bassmap',
-    name='bassmap',
-    packages=find_packages(include=['bassmap', 'bassmap.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/bassneel/bassmap',
-    version='0.0.1',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="Bass Neel",
+    author_email='maps.bassneel@gmail.com',
+    python_requires='>=3.7',
+    classifiers=[
+        'Development Status :: 2 - Pre-Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ],
+    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='bassmap',
+    name='bassmap',
+    packages=find_packages(include=['bassmap', 'bassmap.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/bassneel/bassmap',
+    version='0.0.2',
+    zip_safe=False,
+)
```

