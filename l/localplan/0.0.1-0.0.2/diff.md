# Comparing `tmp/localplan-0.0.1.tar.gz` & `tmp/localplan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localplan-0.0.1.tar", last modified: Thu Apr 13 23:39:52 2023, max compression
+gzip compressed data, was "localplan-0.0.2.tar", last modified: Fri Apr 14 02:29:51 2023, max compression
```

## Comparing `localplan-0.0.1.tar` & `localplan-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 23:39:52.288237 localplan-0.0.1/
--rw-rw-rw-   0        0        0     1099 2023-04-13 23:07:47.000000 localplan-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-13 23:07:47.000000 localplan-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1398 2023-04-13 23:39:52.288237 localplan-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-13 23:07:47.000000 localplan-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 23:39:52.270626 localplan-0.0.1/localplan/
--rw-rw-rw-   0        0        0      144 2023-04-13 23:07:47.000000 localplan-0.0.1/localplan/__init__.py
--rw-rw-rw-   0        0        0       20 2023-04-13 23:07:47.000000 localplan-0.0.1/localplan/localplan.py
-drwxrwxrwx   0        0        0        0 2023-04-13 23:39:52.287239 localplan-0.0.1/localplan.egg-info/
--rw-rw-rw-   0        0        0     1398 2023-04-13 23:39:52.000000 localplan-0.0.1/localplan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-04-13 23:39:52.000000 localplan-0.0.1/localplan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 23:39:52.000000 localplan-0.0.1/localplan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 23:39:52.000000 localplan-0.0.1/localplan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-04-13 23:39:52.000000 localplan-0.0.1/localplan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-13 23:07:47.000000 localplan-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      417 2023-04-13 23:39:52.290232 localplan-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1819 2023-04-13 23:07:47.000000 localplan-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:29:51.191774 localplan-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 02:29:38.000000 localplan-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 02:29:38.000000 localplan-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-14 02:29:51.191774 localplan-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-14 02:29:38.000000 localplan-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:29:51.191774 localplan-0.0.2/localplan/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 02:29:38.000000 localplan-0.0.2/localplan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 02:29:38.000000 localplan-0.0.2/localplan/localplan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:29:51.191774 localplan-0.0.2/localplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-14 02:29:51.000000 localplan-0.0.2/localplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 02:29:51.000000 localplan-0.0.2/localplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 02:29:51.000000 localplan-0.0.2/localplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 02:29:51.000000 localplan-0.0.2/localplan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 02:29:51.000000 localplan-0.0.2/localplan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 02:29:38.000000 localplan-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 02:29:51.191774 localplan-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-14 02:29:38.000000 localplan-0.0.2/setup.py
```

### Comparing `localplan-0.0.1/LICENSE` & `localplan-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Elgenied Elqurashi
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Elgenied Elqurashi
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `localplan-0.0.1/PKG-INFO` & `localplan-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
-Name: localplan
-Version: 0.0.1
-Summary: python tool for local area energy planning
-Home-page: https://github.com/elgenied/localplan
-Author: Elgenied Elqurashi
-Author-email: e.elqurashi@surrey.ac.uk
-License: MIT license
-Keywords: localplan
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
-# localplan
-
-
-[![image](https://img.shields.io/pypi/v/localplan.svg)](https://pypi.python.org/pypi/localplan)
-[![image](https://img.shields.io/conda/vn/conda-forge/localplan.svg)](https://anaconda.org/conda-forge/localplan)
-
-
-**python tool for local area energy planning**
-
-
--   Free software: MIT license
--   Documentation: https://elgenied.github.io/localplan
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
+Name: localplan
+Version: 0.0.2
+Summary: python tool for local area energy planning
+Home-page: https://github.com/elgenied/localplan
+Author: Elgenied Elqurashi
+Author-email: e.elqurashi@surrey.ac.uk
+License: MIT license
+Keywords: localplan
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
+# localplan
+
+
+[![image](https://img.shields.io/pypi/v/localplan.svg)](https://pypi.python.org/pypi/localplan)
+[![image](https://img.shields.io/conda/vn/conda-forge/localplan.svg)](https://anaconda.org/conda-forge/localplan)
+
+
+**python tool for local area energy planning**
+
+
+-   Free software: MIT license
+-   Documentation: https://elgenied.github.io/localplan
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

### Comparing `localplan-0.0.1/README.md` & `localplan-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# localplan
-
-
-[![image](https://img.shields.io/pypi/v/localplan.svg)](https://pypi.python.org/pypi/localplan)
-[![image](https://img.shields.io/conda/vn/conda-forge/localplan.svg)](https://anaconda.org/conda-forge/localplan)
-
-
-**python tool for local area energy planning**
-
-
--   Free software: MIT license
--   Documentation: https://elgenied.github.io/localplan
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+# localplan
+
+
+[![image](https://img.shields.io/pypi/v/localplan.svg)](https://pypi.python.org/pypi/localplan)
+[![image](https://img.shields.io/conda/vn/conda-forge/localplan.svg)](https://anaconda.org/conda-forge/localplan)
+
+
+**python tool for local area energy planning**
+
+
+-   Free software: MIT license
+-   Documentation: https://elgenied.github.io/localplan
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

### Comparing `localplan-0.0.1/localplan.egg-info/PKG-INFO` & `localplan-0.0.2/localplan.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
-Name: localplan
-Version: 0.0.1
-Summary: python tool for local area energy planning
-Home-page: https://github.com/elgenied/localplan
-Author: Elgenied Elqurashi
-Author-email: e.elqurashi@surrey.ac.uk
-License: MIT license
-Keywords: localplan
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
-# localplan
-
-
-[![image](https://img.shields.io/pypi/v/localplan.svg)](https://pypi.python.org/pypi/localplan)
-[![image](https://img.shields.io/conda/vn/conda-forge/localplan.svg)](https://anaconda.org/conda-forge/localplan)
-
-
-**python tool for local area energy planning**
-
-
--   Free software: MIT license
--   Documentation: https://elgenied.github.io/localplan
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
+Name: localplan
+Version: 0.0.2
+Summary: python tool for local area energy planning
+Home-page: https://github.com/elgenied/localplan
+Author: Elgenied Elqurashi
+Author-email: e.elqurashi@surrey.ac.uk
+License: MIT license
+Keywords: localplan
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
+# localplan
+
+
+[![image](https://img.shields.io/pypi/v/localplan.svg)](https://pypi.python.org/pypi/localplan)
+[![image](https://img.shields.io/conda/vn/conda-forge/localplan.svg)](https://anaconda.org/conda-forge/localplan)
+
+
+**python tool for local area energy planning**
+
+
+-   Free software: MIT license
+-   Documentation: https://elgenied.github.io/localplan
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

### Comparing `localplan-0.0.1/setup.py` & `localplan-0.0.2/setup.py`

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
-    author="Elgenied Elqurashi",
-    author_email='e.elqurashi@surrey.ac.uk',
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
-    description="python tool for local area energy planning",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='localplan',
-    name='localplan',
-    packages=find_packages(include=['localplan', 'localplan.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/elgenied/localplan',
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
+    author="Elgenied Elqurashi",
+    author_email='e.elqurashi@surrey.ac.uk',
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
+    description="python tool for local area energy planning",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='localplan',
+    name='localplan',
+    packages=find_packages(include=['localplan', 'localplan.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/elgenied/localplan',
+    version='0.0.2',
+    zip_safe=False,
+)
```

