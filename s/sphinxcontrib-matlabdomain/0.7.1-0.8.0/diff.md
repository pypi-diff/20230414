# Comparing `tmp/sphinxcontrib-matlabdomain-0.7.1.tar.gz` & `tmp/sphinxcontrib-matlabdomain-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxcontrib-matlabdomain-0.7.1.tar", last modified: Wed Apr  3 19:53:55 2019, max compression
+gzip compressed data, was "dist/sphinxcontrib-matlabdomain-0.8.0.tar", last modified: Sat May 11 20:58:32 2019, max compression
```

## Comparing `sphinxcontrib-matlabdomain-0.7.1.tar` & `sphinxcontrib-matlabdomain-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6979 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     9061 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/namespace_packages.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1333 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1418 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib/
--rw-rw-r--   0 travis    (2000) travis    (2000)    56248 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib/mat_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      365 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42359 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib/mat_documenters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27667 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib/matlab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     9061 2019-04-03 19:53:55.000000 sphinxcontrib-matlabdomain-0.7.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     9066 2019-04-03 19:52:47.000000 sphinxcontrib-matlabdomain-0.7.1/CHANGES.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       53 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9434 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/CHANGES.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9241 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9241 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/namespace_packages.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      545 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-11 20:58:32.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53860 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/mat_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6264 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/mat_lexer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27644 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/matlab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42335 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/mat_documenters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      365 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1418 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6979 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1333 2019-05-11 20:57:40.000000 sphinxcontrib-matlabdomain-0.8.0/setup.py
```

### Comparing `sphinxcontrib-matlabdomain-0.7.1/README.rst` & `sphinxcontrib-matlabdomain-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/PKG-INFO` & `sphinxcontrib-matlabdomain-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,198 +1,198 @@
 Metadata-Version: 1.2
 Name: sphinxcontrib-matlabdomain
-Version: 0.7.1
+Version: 0.8.0
 Summary: Sphinx "matlabdomain" extension
 Home-page: https://github.com/sphinx-contrib/matlabdomain
 Author: Mark Mikofski
 Author-email: bwana.marko@yahoo.com
 Maintainer: Jørgen Cederberg
 Maintainer-email: jorgen@cederberg.be
 License: BSD
 Download-URL: http://pypi.python.org/pypi/sphinxcontrib-matlabdomain
-Description: .. image:: https://travis-ci.org/sphinx-contrib/matlabdomain.svg?branch=master
-            :target: https://travis-ci.org/sphinx-contrib/matlabdomain
-        
-        This package contains the MATLAB Sphinx domain and autodoc extensions.
-        
-        `Changes <https://github.com/sphinx-contrib/matlabdomain/blob/master/CHANGES.rst>`_
-        
-        Installation
-        ============
-        Use `Pip <http://www.pip-installer.org/en/latest/index.html>`_,
-        `Setuptools Easy Install <http://pythonhosted.org/setuptools/>`_ or
-        `Python Distributions Utilities (Distutils) <http://docs.python.org/2/install/>`_.
-        
-        Pip::
-        
-           ~$ pip install -U sphinxcontrib-matlabdomain
-        
-        Easy Install::
-        
-            ~$ easy_install -U sphinxcontrib-matlabdomain
-        
-        Distutils::
-        
-            ~/downloads$ curl https://pypi.python.org/packages/source/s/sphinxcontrib-matlabdomain/sphinxcontrib-matlabdomain-0.X.tar.gz
-            ~/downloads$ tar -xf sphinxcontrib-matlabdomain-0.X.tar.gz
-            ~/downloads$ cd sphinxcontrib_matlabdomain-0.X
-            ~/downloads/sphinxcontrib_matlabdomain-0.X$ python setup.py install
-        
-        Requirements
-        ============
-        This package is an extension to `Sphinx <http://sphinx-doc.org>`_.
-        
-        Usage
-        =====
-        In general usage is the same as for documenting Python code.
-        
-        Configuration
-        -------------
-        In your Sphinx ``conf.py`` file add ``sphinxcontrib.matlab`` to the list of
-        extensions. To use auto-documentation features, also add ``sphinx.ext.autodoc``
-        to the list of extensions.
-        
-        In order for the Sphinx MATLAB domain to auto-document MATLAB source code, set
-        the config value of ``matlab_src_dir`` to the absolute path instead of adding
-        them to ``sys.path``. Currently only one MATLAB path can be specified, but all
-        subfolders in that tree will be searched.
-        
-        For convenience the `primary domain <http://sphinx-doc.org/config.html#confval-primary_domain>`_
-        can be set to ``mat``.
-        
-        Roles and Directives
-        --------------------
-        Please see `Sphinx Domains <http://sphinx-doc.org/domains.html>`_ and
-        `sphinx.ext.autodoc <http://sphinx-doc.org/ext/autodoc.html>`_ for
-        documentation on the use of roles and directives. MATLAB code can be documented
-        using the following roles and directives:
-        
-        ====================================  ===========================================
-        Directive                             MATLAB object
-        ====================================  ===========================================
-        ``.. module:: foldername``            **folders, packages and namespaces**
-        ``.. curremtmodule:: foldername``     * set folder but do not link
-        ``.. automodule:: foldername``        * auto-document
-        ``:mod:`foldername```                 * reference
-        ``.. function:: funcname``            **function definition and signature**
-        ``.. autofunction:: funcname()``      * auto-document
-        ``:func:`funcname```                  * reference
-        ``.. script:: scriptname``            **script definition**
-        ``.. autoscript:: scriptname``        * auto-document
-        ``:scpt:`scriptname```                * reference
-        ``.. class:: classname()``            **class definition and optional signature**
-        ``.. autoclass:: classname``          * auto-document
-        ``:class:`classname```                * reference
-        ``.. method:: methname()``            **method definition and signature**
-        ``.. automethod:: methname``          * auto-document
-        ``:meth:`methname```                  * reference
-        ``.. staticmethod:: statmethname()``  **static method definition and signature**
-        ``.. automethod:: statmethname``      * auto-document
-        ``:meth:`methname```                  * reference
-        ``.. attribute:: attrname``           **property definition**
-        ``.. autoattribute:: attrname``       * auto-document
-        ``:attr:`attrname```                  * reference
-        ====================================  ===========================================
-        
-        Several options are available for auto-directives.
-        
-        * ``:members:`` auto-document public members
-        * ``:show-inheritance:`` list bases
-        * ``:undoc-members:`` document members without docstrings
-        * ``:annotation:`` specifies attribute annotation instead of default
-        
-        There are also several config values that can be set in ``conf.py`` that will
-        affect auto-docementation.
-        
-        * ``autoclass_content`` can be set to ``class``, ``both`` or ``init``, which
-          determines which docstring is used for classes. The constructor docstring
-          is used when this is set to ``init``.
-        * ``autodoc_member_order`` can be set to ``alphabetical``, ``groupwise`` or
-          ``bysource``.
-        * ``autodoc_default_flags`` can be set to a list of options to apply. Use
-          the ``no-flag`` directive option to disable this config value once.
-        
-        .. note::
-        
-            The module roles and directives create a psuedo namespace for MATLAB
-            objects, similar to a package. They represent the path to the folder
-            containing the MATLAB object. If no module is specified then Sphinx will
-            assume that the object is a built-in.
-        
-        Example: given the following MATLAB source in folder ``test_data``::
-        
-            classdef MyHandleClass < handle & my.super.Class
-                % a handle class
-                %
-                % :param x: a variable
-        
-                %% some comments
-                properties
-                    x % a property
-                end
-                methods
-                    function h = MyHandleClass(x)
-                        h.x = x
-                    end
-                    function x = get.x(obj)
-                    % how is this displayed?
-                        x = obj.x
-                    end
-                end
-                methods (Static)
-                    function w = my_static_function(z)
-                    % A static function in :class:`MyHandleClass`.
-                    %
-                    % :param z: input z
-                    % :returns: w
-        
-                        w = z
-                    end
-                end    
-            end
-        
-        Use the following to document::
-        
-            Test Data
-            =========
-            This is the test data module.
-        
-            .. automodule:: test_data
-        
-            :mod:`test_data` is a really cool module.
-        
-            My Handle Class
-            ---------------
-            This is the handle class definition.
-        
-            .. autoclass:: MyHandleClass
-                :show-inheritance:
-                :members:
-        
-        Online Demo
-        -----------
-        The test docs in the repository are online here:
-        http://bwanamarko.alwaysdata.net/matlabdomain/
-        
-        .. note::
-        
-            Sphinx style markup are used to document parameters, types, returns and
-            exceptions. There must be a blank comment line before and after the
-            parameter descriptions. Currently property docstrings are only collected if
-            they are on the same line following the property definition. Getter and
-            setter methods are documented like methods currently, but the dot is
-            replaced by an underscore. Default values for properties are represented as
-            unicode strings, therefore strings will be double quoted.
-        
-        Users
-        -----
-        
-        * `Cantera <http://cantera.github.io/docs/sphinx/html/compiling/dependencies.html?highlight=matlabdomain>`_
-        * `CoSMo MVPA <http://cosmomvpa.org/download.html?highlight=matlabdomain#developers>`_
-        * `The Cobra Toolbox <https://opencobra.github.io/cobratoolbox/stable/index.html#>`_
+Description: .. image:: https://travis-ci.org/sphinx-contrib/matlabdomain.svg?branch=master
+            :target: https://travis-ci.org/sphinx-contrib/matlabdomain
+        
+        This package contains the MATLAB Sphinx domain and autodoc extensions.
+        
+        `Changes <https://github.com/sphinx-contrib/matlabdomain/blob/master/CHANGES.rst>`_
+        
+        Installation
+        ============
+        Use `Pip <http://www.pip-installer.org/en/latest/index.html>`_,
+        `Setuptools Easy Install <http://pythonhosted.org/setuptools/>`_ or
+        `Python Distributions Utilities (Distutils) <http://docs.python.org/2/install/>`_.
+        
+        Pip::
+        
+           ~$ pip install -U sphinxcontrib-matlabdomain
+        
+        Easy Install::
+        
+            ~$ easy_install -U sphinxcontrib-matlabdomain
+        
+        Distutils::
+        
+            ~/downloads$ curl https://pypi.python.org/packages/source/s/sphinxcontrib-matlabdomain/sphinxcontrib-matlabdomain-0.X.tar.gz
+            ~/downloads$ tar -xf sphinxcontrib-matlabdomain-0.X.tar.gz
+            ~/downloads$ cd sphinxcontrib_matlabdomain-0.X
+            ~/downloads/sphinxcontrib_matlabdomain-0.X$ python setup.py install
+        
+        Requirements
+        ============
+        This package is an extension to `Sphinx <http://sphinx-doc.org>`_.
+        
+        Usage
+        =====
+        In general usage is the same as for documenting Python code.
+        
+        Configuration
+        -------------
+        In your Sphinx ``conf.py`` file add ``sphinxcontrib.matlab`` to the list of
+        extensions. To use auto-documentation features, also add ``sphinx.ext.autodoc``
+        to the list of extensions.
+        
+        In order for the Sphinx MATLAB domain to auto-document MATLAB source code, set
+        the config value of ``matlab_src_dir`` to the absolute path instead of adding
+        them to ``sys.path``. Currently only one MATLAB path can be specified, but all
+        subfolders in that tree will be searched.
+        
+        For convenience the `primary domain <http://sphinx-doc.org/config.html#confval-primary_domain>`_
+        can be set to ``mat``.
+        
+        Roles and Directives
+        --------------------
+        Please see `Sphinx Domains <http://sphinx-doc.org/domains.html>`_ and
+        `sphinx.ext.autodoc <http://sphinx-doc.org/ext/autodoc.html>`_ for
+        documentation on the use of roles and directives. MATLAB code can be documented
+        using the following roles and directives:
+        
+        ====================================  ===========================================
+        Directive                             MATLAB object
+        ====================================  ===========================================
+        ``.. module:: foldername``            **folders, packages and namespaces**
+        ``.. curremtmodule:: foldername``     * set folder but do not link
+        ``.. automodule:: foldername``        * auto-document
+        ``:mod:`foldername```                 * reference
+        ``.. function:: funcname``            **function definition and signature**
+        ``.. autofunction:: funcname()``      * auto-document
+        ``:func:`funcname```                  * reference
+        ``.. script:: scriptname``            **script definition**
+        ``.. autoscript:: scriptname``        * auto-document
+        ``:scpt:`scriptname```                * reference
+        ``.. class:: classname()``            **class definition and optional signature**
+        ``.. autoclass:: classname``          * auto-document
+        ``:class:`classname```                * reference
+        ``.. method:: methname()``            **method definition and signature**
+        ``.. automethod:: methname``          * auto-document
+        ``:meth:`methname```                  * reference
+        ``.. staticmethod:: statmethname()``  **static method definition and signature**
+        ``.. automethod:: statmethname``      * auto-document
+        ``:meth:`methname```                  * reference
+        ``.. attribute:: attrname``           **property definition**
+        ``.. autoattribute:: attrname``       * auto-document
+        ``:attr:`attrname```                  * reference
+        ====================================  ===========================================
+        
+        Several options are available for auto-directives.
+        
+        * ``:members:`` auto-document public members
+        * ``:show-inheritance:`` list bases
+        * ``:undoc-members:`` document members without docstrings
+        * ``:annotation:`` specifies attribute annotation instead of default
+        
+        There are also several config values that can be set in ``conf.py`` that will
+        affect auto-docementation.
+        
+        * ``autoclass_content`` can be set to ``class``, ``both`` or ``init``, which
+          determines which docstring is used for classes. The constructor docstring
+          is used when this is set to ``init``.
+        * ``autodoc_member_order`` can be set to ``alphabetical``, ``groupwise`` or
+          ``bysource``.
+        * ``autodoc_default_flags`` can be set to a list of options to apply. Use
+          the ``no-flag`` directive option to disable this config value once.
+        
+        .. note::
+        
+            The module roles and directives create a psuedo namespace for MATLAB
+            objects, similar to a package. They represent the path to the folder
+            containing the MATLAB object. If no module is specified then Sphinx will
+            assume that the object is a built-in.
+        
+        Example: given the following MATLAB source in folder ``test_data``::
+        
+            classdef MyHandleClass < handle & my.super.Class
+                % a handle class
+                %
+                % :param x: a variable
+        
+                %% some comments
+                properties
+                    x % a property
+                end
+                methods
+                    function h = MyHandleClass(x)
+                        h.x = x
+                    end
+                    function x = get.x(obj)
+                    % how is this displayed?
+                        x = obj.x
+                    end
+                end
+                methods (Static)
+                    function w = my_static_function(z)
+                    % A static function in :class:`MyHandleClass`.
+                    %
+                    % :param z: input z
+                    % :returns: w
+        
+                        w = z
+                    end
+                end    
+            end
+        
+        Use the following to document::
+        
+            Test Data
+            =========
+            This is the test data module.
+        
+            .. automodule:: test_data
+        
+            :mod:`test_data` is a really cool module.
+        
+            My Handle Class
+            ---------------
+            This is the handle class definition.
+        
+            .. autoclass:: MyHandleClass
+                :show-inheritance:
+                :members:
+        
+        Online Demo
+        -----------
+        The test docs in the repository are online here:
+        http://bwanamarko.alwaysdata.net/matlabdomain/
+        
+        .. note::
+        
+            Sphinx style markup are used to document parameters, types, returns and
+            exceptions. There must be a blank comment line before and after the
+            parameter descriptions. Currently property docstrings are only collected if
+            they are on the same line following the property definition. Getter and
+            setter methods are documented like methods currently, but the dot is
+            replaced by an underscore. Default values for properties are represented as
+            unicode strings, therefore strings will be double quoted.
+        
+        Users
+        -----
+        
+        * `Cantera <http://cantera.github.io/docs/sphinx/html/compiling/dependencies.html?highlight=matlabdomain>`_
+        * `CoSMo MVPA <http://cosmomvpa.org/download.html?highlight=matlabdomain#developers>`_
+        * `The Cobra Toolbox <https://opencobra.github.io/cobratoolbox/stable/index.html#>`_
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib_matlabdomain.egg-info/SOURCES.txt` & `sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGES.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 sphinxcontrib/__init__.py
 sphinxcontrib/mat_documenters.py
+sphinxcontrib/mat_lexer.py
 sphinxcontrib/mat_types.py
 sphinxcontrib/matlab.py
 sphinxcontrib_matlabdomain.egg-info/PKG-INFO
 sphinxcontrib_matlabdomain.egg-info/SOURCES.txt
 sphinxcontrib_matlabdomain.egg-info/dependency_links.txt
 sphinxcontrib_matlabdomain.egg-info/namespace_packages.txt
 sphinxcontrib_matlabdomain.egg-info/not-zip-safe
```

### Comparing `sphinxcontrib-matlabdomain-0.7.1/setup.py` & `sphinxcontrib-matlabdomain-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as f_readme:
     long_desc = f_readme.read()
 
-version = '0.7.1'
+version = '0.8.0'
 
 requires = ['Sphinx>=1.7.2', 'Pygments>=2.0.1', 'future>=0.16.0']
 
 setup(
     name='sphinxcontrib-matlabdomain',
     version=version,
     url='https://github.com/sphinx-contrib/matlabdomain',
```

### Comparing `sphinxcontrib-matlabdomain-0.7.1/LICENSE` & `sphinxcontrib-matlabdomain-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib/mat_types.py` & `sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/mat_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,22 @@
     ~~~~~~~~~~~~~~~~~~~~~~~
 
     Types for MATLAB.
 
     :copyright: Copyright 2014 Mark Mikofski
     :license: BSD, see LICENSE for details.
 """
-from __future__ import unicode_literals, print_function
-from builtins import *
+from __future__ import unicode_literals
 from io import open  # for opening files with encoding in Python 2
 import os
 import re
 import sys
 from copy import copy
 from sphinx.util import logging
-
-# Pygments MatlabLexer is in pygments.lexers.math, but recommended way to load
-# is from lexers, which has LEXERS dictionary, which PyDev doesn't see.
-from pygments.lexers import MatlabLexer  # @UnresolvedImport
-# PyDev doesn't see Token methods and subtypes that are generated at runtime
+from sphinxcontrib.mat_lexer import MatlabLexer
 from pygments.token import Token
 
 logger = logging.getLogger('matlab-domain')
 
 MAT_DOM = 'sphinxcontrib-matlabdomain'
 __all__ = ['MatObject', 'MatModule', 'MatFunction', 'MatClass',  \
            'MatProperty', 'MatMethod', 'MatScript', 'MatException', \
@@ -50,26 +45,17 @@
 
     MATLAB objects can be :class:`MatModule`, :class:`MatFunction` or
     :class:`MatClass`. :class:`MatModule` are just folders that define a psuedo
     namespace for :class:`MatFunction` and :class:`MatClass` in that folder.
     :class:`MatFunction` and :class:`MatClass` must begin with either
     ``function`` or ``classdef`` keywords.
     """
-
-    @staticmethod
-    def dbg(msg, *args):
-        """
-        Alternate for sphinx_dbg for test-mode.
-        """
-        print('\t<test-mode>\n' + msg % args)
-
     basedir = None
     sphinx_env = None
     sphinx_app = None
-    sphinx_dbg = dbg
 
     def __init__(self, name):
         #: name of MATLAB object
         self.name = name
 
     @property
     def __name__(self):
@@ -154,39 +140,39 @@
 
         Assumes that the first token in the file is either one of the keywords:
         "classdef" or "function" otherwise it is assumed to be a script.
         """
         # use Pygments to parse mfile to determine type: function/classdef
         # read mfile code
         with open(mfile, 'r', encoding='utf-8') as code_f:
-            code = code_f.read().replace('\r\n', '\n')  # repl crlf with lf
+            code = code_f.read().replace('\r\n', '\n')
 
-        # remove the top comment header (if there is one) from the code string
         full_code = code
+        # remove the top comment header (if there is one) from the code string
         code = MatObject._remove_comment_header(code)
-
-        # functions must be contained in one line, no ellipsis, classdef is OK
         code = MatObject._remove_line_continuations(code)
         code = MatObject._fix_function_signatures(code)
-        code = MatObject._fix_string_double_quotes(code)
 
-        # Produce tokes, but fix incorrect (Token.Keyword, 'function')
         tks = list(MatlabLexer().get_tokens(code))
-        tks = MatObject._fix_function_variables(tks)
 
         modname = path.replace(os.sep, '.')  # module name
+
         # assume that functions and classes always start with a keyword
-        if tks[0] == (Token.Keyword, 'function'):
-            logger.debug('[%s] parsing function %s from %s.', MAT_DOM,
-                                 name, modname)
-            return MatFunction(name, modname, tks)
-        elif tks[0] == (Token.Keyword, 'classdef'):
-            logger.debug('[%s] parsing classdef %s from %s.', MAT_DOM,
-                                 name, modname)
+        def isFunction(token):
+            return token == (Token.Keyword, 'function')
+
+        def isClass(token):
+            return token == (Token.Keyword, 'classdef')
+
+        if isClass(tks[0]):
+            logger.debug('[%s] parsing classdef %s from %s.', MAT_DOM, name, modname)
             return MatClass(name, modname, tks)
+        elif isFunction(tks[0]):
+            logger.debug('[%s] parsing function %s from %s.', MAT_DOM, name, modname)
+            return MatFunction(name, modname, tks)
         else:
             # it's a script file retoken with header comment
             tks = list(MatlabLexer().get_tokens(full_code))
             return MatScript(name, modname, tks)
         return None
 
     @staticmethod
@@ -260,67 +246,14 @@
             return retv
 
         code = pat.sub(repl, code)  # search for functions and apply replacement
         msg = '[%s] replaced ellipsis & appended parentheses in function signatures'
         logger.debug(msg, MAT_DOM)
         return code
 
-    @staticmethod
-    def _fix_function_variables(tokens):
-        """ Fixes invalid `function` tokens
-
-        Pygments will mark any text matching `token` as Token.Keyword. This
-        function fixes this issue, by converting invalid marked functions as
-        Token.Text.
-
-        :param tokens:
-        :type code: list of Tokens
-        :return: Modified list of tokens
-        """
-        for idx, token in enumerate(tokens):
-            temp_token = (token[0], token[1].lstrip())
-            if temp_token == (Token.Keyword, 'function'):
-                previous_token = tokens[idx-1] if idx > 0 else None
-                if previous_token and not previous_token == (Token.Text, '\n'):
-                    # This is not a real function as it is not after a new line
-                    tokens[idx] = (Token.Text, token[1])
-                    continue
-                next_token = tokens[idx+1] if idx < len(tokens)-1 else None
-                if next_token and not re.match(r'[\s[]', next_token[1]):
-                    # This is not a real function as it is not followed by '\s' or '['
-                    tokens[idx] = (Token.Text, token[1])
-                    continue
-        return tokens
-
-    @staticmethod
-    def _fix_string_double_quotes(code):
-        """
-        Convert double quotes to single qoute strings, pygments doesn't know
-        these.
-
-        :param code:
-        :type code: str
-        :return: Code string where %s is removed from strings
-        """
-        pat = r"(?!\s*%)(.*)([\"].*[\"]{1})(.*)"
-        pat = re.compile(pat, re.X | re.MULTILINE)  # search start of every line
-
-        # replacement function
-        def repl(m):
-            retv = m.group(0)
-            if m.group(2):
-                retv = m.group(1) + "''" + m.group(3)
-            return retv
-
-        code = pat.sub(repl, code)  # search for string spec and apply replacement
-        return code
-
-
-
-
 
 # TODO: get docstring and __all__ from contents.m if exists
 class MatModule(MatObject):
     """
     All MATLAB modules are packages. A package is a folder that serves as the
     namespace for any :class:`MatObjects` in the package folder. Sphinx will
     treats objects without a namespace as builtins, so all MATLAB projects
@@ -951,18 +884,18 @@
                              meth_tk[1].strip() == 'function'
                              and self.tokens[idx+1][0] is Token.Name.Function) or
                             self._tk_eq(idx, (Token.Punctuation, '[')) or
                             self._tk_eq(idx, (Token.Punctuation, ']')) or
                             self._tk_eq(idx, (Token.Punctuation, '=')) or
                             self._tk_eq(idx, (Token.Punctuation, '(')) or
                             self._tk_eq(idx, (Token.Punctuation, ')')) or
+                            self._tk_eq(idx, (Token.Punctuation, ';')) or
                             self._tk_eq(idx, (Token.Punctuation, ','))):
-                            msg = ['[%s] Skipping tokens for methods defined in separate files.',
-                                   'token #%d: %r']
-                            MatClass.sphinx_dbg('\n'.join(msg), MAT_DOM, idx, self.tokens[idx])
+                            msg = '[%s] Skipping tokens for methods defined in separate files.\ntoken #%d: %r'
+                            logger.debug(msg, MAT_DOM, idx, self.tokens[idx])
                             idx += 1 + self._whitespace(idx + 1)
                         elif self._tk_eq(idx, (Token.Keyword, 'end')):
                             idx += 1
                             break
                         else:
                             # find methods
                             meth = MatMethod(self.module, self.tokens[idx:],
@@ -1017,14 +950,20 @@
                 elif k is Token.Name:
                     msg = '[sphinxcontrib-matlabdomain] Unexpected class attribute: "%s".' % str(self.tokens[idx][1])
                     msg += ' In "{0}.{1}".'.format(self.module, self.name)
                     logger.warning(msg)
                     idx += 1
 
                 idx += self._blanks(idx)  # skip blanks
+
+                # Continue if attribute is assigned a boolean value
+                if self.tokens[idx][0] == Token.Name.Builtin:
+                    idx += 1
+                    continue
+
                 # continue to next attribute separated by commas
                 if self._tk_eq(idx, (Token.Punctuation, ',')):
                     idx += 1
                     continue
                 # attribute values
                 elif self._tk_eq(idx, (Token.Punctuation, '=')):
                     idx += 1
```

### Comparing `sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib/mat_documenters.py` & `sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/mat_documenters.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
     Extend autodoc directives to matlabdomain.
 
     :copyright: Copyright 2014 Mark Mikofski
     :license: BSD, see LICENSE for details.
 """
 from __future__ import unicode_literals
-from builtins import *
 import re
 import sys
 import inspect
 import traceback
 from six import itervalues
 
 from docutils.statemachine import ViewList
```

### Comparing `sphinxcontrib-matlabdomain-0.7.1/sphinxcontrib/matlab.py` & `sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib/matlab.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
     The MATLAB domain.
 
     :copyright: Copyright 2007-2011 by the Sphinx team, see AUTHORS.
     :license: BSD, see LICENSE for details.
 """
 from __future__ import absolute_import, unicode_literals
-from builtins import *
 from . import mat_documenters as doc
 
 import re
 
 from docutils import nodes
 from docutils.parsers.rst import directives, Directive
```

### Comparing `sphinxcontrib-matlabdomain-0.7.1/PKG-INFO` & `sphinxcontrib-matlabdomain-0.8.0/sphinxcontrib_matlabdomain.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,198 +1,198 @@
 Metadata-Version: 1.2
 Name: sphinxcontrib-matlabdomain
-Version: 0.7.1
+Version: 0.8.0
 Summary: Sphinx "matlabdomain" extension
 Home-page: https://github.com/sphinx-contrib/matlabdomain
 Author: Mark Mikofski
 Author-email: bwana.marko@yahoo.com
 Maintainer: Jørgen Cederberg
 Maintainer-email: jorgen@cederberg.be
 License: BSD
 Download-URL: http://pypi.python.org/pypi/sphinxcontrib-matlabdomain
-Description: .. image:: https://travis-ci.org/sphinx-contrib/matlabdomain.svg?branch=master
-            :target: https://travis-ci.org/sphinx-contrib/matlabdomain
-        
-        This package contains the MATLAB Sphinx domain and autodoc extensions.
-        
-        `Changes <https://github.com/sphinx-contrib/matlabdomain/blob/master/CHANGES.rst>`_
-        
-        Installation
-        ============
-        Use `Pip <http://www.pip-installer.org/en/latest/index.html>`_,
-        `Setuptools Easy Install <http://pythonhosted.org/setuptools/>`_ or
-        `Python Distributions Utilities (Distutils) <http://docs.python.org/2/install/>`_.
-        
-        Pip::
-        
-           ~$ pip install -U sphinxcontrib-matlabdomain
-        
-        Easy Install::
-        
-            ~$ easy_install -U sphinxcontrib-matlabdomain
-        
-        Distutils::
-        
-            ~/downloads$ curl https://pypi.python.org/packages/source/s/sphinxcontrib-matlabdomain/sphinxcontrib-matlabdomain-0.X.tar.gz
-            ~/downloads$ tar -xf sphinxcontrib-matlabdomain-0.X.tar.gz
-            ~/downloads$ cd sphinxcontrib_matlabdomain-0.X
-            ~/downloads/sphinxcontrib_matlabdomain-0.X$ python setup.py install
-        
-        Requirements
-        ============
-        This package is an extension to `Sphinx <http://sphinx-doc.org>`_.
-        
-        Usage
-        =====
-        In general usage is the same as for documenting Python code.
-        
-        Configuration
-        -------------
-        In your Sphinx ``conf.py`` file add ``sphinxcontrib.matlab`` to the list of
-        extensions. To use auto-documentation features, also add ``sphinx.ext.autodoc``
-        to the list of extensions.
-        
-        In order for the Sphinx MATLAB domain to auto-document MATLAB source code, set
-        the config value of ``matlab_src_dir`` to the absolute path instead of adding
-        them to ``sys.path``. Currently only one MATLAB path can be specified, but all
-        subfolders in that tree will be searched.
-        
-        For convenience the `primary domain <http://sphinx-doc.org/config.html#confval-primary_domain>`_
-        can be set to ``mat``.
-        
-        Roles and Directives
-        --------------------
-        Please see `Sphinx Domains <http://sphinx-doc.org/domains.html>`_ and
-        `sphinx.ext.autodoc <http://sphinx-doc.org/ext/autodoc.html>`_ for
-        documentation on the use of roles and directives. MATLAB code can be documented
-        using the following roles and directives:
-        
-        ====================================  ===========================================
-        Directive                             MATLAB object
-        ====================================  ===========================================
-        ``.. module:: foldername``            **folders, packages and namespaces**
-        ``.. curremtmodule:: foldername``     * set folder but do not link
-        ``.. automodule:: foldername``        * auto-document
-        ``:mod:`foldername```                 * reference
-        ``.. function:: funcname``            **function definition and signature**
-        ``.. autofunction:: funcname()``      * auto-document
-        ``:func:`funcname```                  * reference
-        ``.. script:: scriptname``            **script definition**
-        ``.. autoscript:: scriptname``        * auto-document
-        ``:scpt:`scriptname```                * reference
-        ``.. class:: classname()``            **class definition and optional signature**
-        ``.. autoclass:: classname``          * auto-document
-        ``:class:`classname```                * reference
-        ``.. method:: methname()``            **method definition and signature**
-        ``.. automethod:: methname``          * auto-document
-        ``:meth:`methname```                  * reference
-        ``.. staticmethod:: statmethname()``  **static method definition and signature**
-        ``.. automethod:: statmethname``      * auto-document
-        ``:meth:`methname```                  * reference
-        ``.. attribute:: attrname``           **property definition**
-        ``.. autoattribute:: attrname``       * auto-document
-        ``:attr:`attrname```                  * reference
-        ====================================  ===========================================
-        
-        Several options are available for auto-directives.
-        
-        * ``:members:`` auto-document public members
-        * ``:show-inheritance:`` list bases
-        * ``:undoc-members:`` document members without docstrings
-        * ``:annotation:`` specifies attribute annotation instead of default
-        
-        There are also several config values that can be set in ``conf.py`` that will
-        affect auto-docementation.
-        
-        * ``autoclass_content`` can be set to ``class``, ``both`` or ``init``, which
-          determines which docstring is used for classes. The constructor docstring
-          is used when this is set to ``init``.
-        * ``autodoc_member_order`` can be set to ``alphabetical``, ``groupwise`` or
-          ``bysource``.
-        * ``autodoc_default_flags`` can be set to a list of options to apply. Use
-          the ``no-flag`` directive option to disable this config value once.
-        
-        .. note::
-        
-            The module roles and directives create a psuedo namespace for MATLAB
-            objects, similar to a package. They represent the path to the folder
-            containing the MATLAB object. If no module is specified then Sphinx will
-            assume that the object is a built-in.
-        
-        Example: given the following MATLAB source in folder ``test_data``::
-        
-            classdef MyHandleClass < handle & my.super.Class
-                % a handle class
-                %
-                % :param x: a variable
-        
-                %% some comments
-                properties
-                    x % a property
-                end
-                methods
-                    function h = MyHandleClass(x)
-                        h.x = x
-                    end
-                    function x = get.x(obj)
-                    % how is this displayed?
-                        x = obj.x
-                    end
-                end
-                methods (Static)
-                    function w = my_static_function(z)
-                    % A static function in :class:`MyHandleClass`.
-                    %
-                    % :param z: input z
-                    % :returns: w
-        
-                        w = z
-                    end
-                end    
-            end
-        
-        Use the following to document::
-        
-            Test Data
-            =========
-            This is the test data module.
-        
-            .. automodule:: test_data
-        
-            :mod:`test_data` is a really cool module.
-        
-            My Handle Class
-            ---------------
-            This is the handle class definition.
-        
-            .. autoclass:: MyHandleClass
-                :show-inheritance:
-                :members:
-        
-        Online Demo
-        -----------
-        The test docs in the repository are online here:
-        http://bwanamarko.alwaysdata.net/matlabdomain/
-        
-        .. note::
-        
-            Sphinx style markup are used to document parameters, types, returns and
-            exceptions. There must be a blank comment line before and after the
-            parameter descriptions. Currently property docstrings are only collected if
-            they are on the same line following the property definition. Getter and
-            setter methods are documented like methods currently, but the dot is
-            replaced by an underscore. Default values for properties are represented as
-            unicode strings, therefore strings will be double quoted.
-        
-        Users
-        -----
-        
-        * `Cantera <http://cantera.github.io/docs/sphinx/html/compiling/dependencies.html?highlight=matlabdomain>`_
-        * `CoSMo MVPA <http://cosmomvpa.org/download.html?highlight=matlabdomain#developers>`_
-        * `The Cobra Toolbox <https://opencobra.github.io/cobratoolbox/stable/index.html#>`_
+Description: .. image:: https://travis-ci.org/sphinx-contrib/matlabdomain.svg?branch=master
+            :target: https://travis-ci.org/sphinx-contrib/matlabdomain
+        
+        This package contains the MATLAB Sphinx domain and autodoc extensions.
+        
+        `Changes <https://github.com/sphinx-contrib/matlabdomain/blob/master/CHANGES.rst>`_
+        
+        Installation
+        ============
+        Use `Pip <http://www.pip-installer.org/en/latest/index.html>`_,
+        `Setuptools Easy Install <http://pythonhosted.org/setuptools/>`_ or
+        `Python Distributions Utilities (Distutils) <http://docs.python.org/2/install/>`_.
+        
+        Pip::
+        
+           ~$ pip install -U sphinxcontrib-matlabdomain
+        
+        Easy Install::
+        
+            ~$ easy_install -U sphinxcontrib-matlabdomain
+        
+        Distutils::
+        
+            ~/downloads$ curl https://pypi.python.org/packages/source/s/sphinxcontrib-matlabdomain/sphinxcontrib-matlabdomain-0.X.tar.gz
+            ~/downloads$ tar -xf sphinxcontrib-matlabdomain-0.X.tar.gz
+            ~/downloads$ cd sphinxcontrib_matlabdomain-0.X
+            ~/downloads/sphinxcontrib_matlabdomain-0.X$ python setup.py install
+        
+        Requirements
+        ============
+        This package is an extension to `Sphinx <http://sphinx-doc.org>`_.
+        
+        Usage
+        =====
+        In general usage is the same as for documenting Python code.
+        
+        Configuration
+        -------------
+        In your Sphinx ``conf.py`` file add ``sphinxcontrib.matlab`` to the list of
+        extensions. To use auto-documentation features, also add ``sphinx.ext.autodoc``
+        to the list of extensions.
+        
+        In order for the Sphinx MATLAB domain to auto-document MATLAB source code, set
+        the config value of ``matlab_src_dir`` to the absolute path instead of adding
+        them to ``sys.path``. Currently only one MATLAB path can be specified, but all
+        subfolders in that tree will be searched.
+        
+        For convenience the `primary domain <http://sphinx-doc.org/config.html#confval-primary_domain>`_
+        can be set to ``mat``.
+        
+        Roles and Directives
+        --------------------
+        Please see `Sphinx Domains <http://sphinx-doc.org/domains.html>`_ and
+        `sphinx.ext.autodoc <http://sphinx-doc.org/ext/autodoc.html>`_ for
+        documentation on the use of roles and directives. MATLAB code can be documented
+        using the following roles and directives:
+        
+        ====================================  ===========================================
+        Directive                             MATLAB object
+        ====================================  ===========================================
+        ``.. module:: foldername``            **folders, packages and namespaces**
+        ``.. curremtmodule:: foldername``     * set folder but do not link
+        ``.. automodule:: foldername``        * auto-document
+        ``:mod:`foldername```                 * reference
+        ``.. function:: funcname``            **function definition and signature**
+        ``.. autofunction:: funcname()``      * auto-document
+        ``:func:`funcname```                  * reference
+        ``.. script:: scriptname``            **script definition**
+        ``.. autoscript:: scriptname``        * auto-document
+        ``:scpt:`scriptname```                * reference
+        ``.. class:: classname()``            **class definition and optional signature**
+        ``.. autoclass:: classname``          * auto-document
+        ``:class:`classname```                * reference
+        ``.. method:: methname()``            **method definition and signature**
+        ``.. automethod:: methname``          * auto-document
+        ``:meth:`methname```                  * reference
+        ``.. staticmethod:: statmethname()``  **static method definition and signature**
+        ``.. automethod:: statmethname``      * auto-document
+        ``:meth:`methname```                  * reference
+        ``.. attribute:: attrname``           **property definition**
+        ``.. autoattribute:: attrname``       * auto-document
+        ``:attr:`attrname```                  * reference
+        ====================================  ===========================================
+        
+        Several options are available for auto-directives.
+        
+        * ``:members:`` auto-document public members
+        * ``:show-inheritance:`` list bases
+        * ``:undoc-members:`` document members without docstrings
+        * ``:annotation:`` specifies attribute annotation instead of default
+        
+        There are also several config values that can be set in ``conf.py`` that will
+        affect auto-docementation.
+        
+        * ``autoclass_content`` can be set to ``class``, ``both`` or ``init``, which
+          determines which docstring is used for classes. The constructor docstring
+          is used when this is set to ``init``.
+        * ``autodoc_member_order`` can be set to ``alphabetical``, ``groupwise`` or
+          ``bysource``.
+        * ``autodoc_default_flags`` can be set to a list of options to apply. Use
+          the ``no-flag`` directive option to disable this config value once.
+        
+        .. note::
+        
+            The module roles and directives create a psuedo namespace for MATLAB
+            objects, similar to a package. They represent the path to the folder
+            containing the MATLAB object. If no module is specified then Sphinx will
+            assume that the object is a built-in.
+        
+        Example: given the following MATLAB source in folder ``test_data``::
+        
+            classdef MyHandleClass < handle & my.super.Class
+                % a handle class
+                %
+                % :param x: a variable
+        
+                %% some comments
+                properties
+                    x % a property
+                end
+                methods
+                    function h = MyHandleClass(x)
+                        h.x = x
+                    end
+                    function x = get.x(obj)
+                    % how is this displayed?
+                        x = obj.x
+                    end
+                end
+                methods (Static)
+                    function w = my_static_function(z)
+                    % A static function in :class:`MyHandleClass`.
+                    %
+                    % :param z: input z
+                    % :returns: w
+        
+                        w = z
+                    end
+                end    
+            end
+        
+        Use the following to document::
+        
+            Test Data
+            =========
+            This is the test data module.
+        
+            .. automodule:: test_data
+        
+            :mod:`test_data` is a really cool module.
+        
+            My Handle Class
+            ---------------
+            This is the handle class definition.
+        
+            .. autoclass:: MyHandleClass
+                :show-inheritance:
+                :members:
+        
+        Online Demo
+        -----------
+        The test docs in the repository are online here:
+        http://bwanamarko.alwaysdata.net/matlabdomain/
+        
+        .. note::
+        
+            Sphinx style markup are used to document parameters, types, returns and
+            exceptions. There must be a blank comment line before and after the
+            parameter descriptions. Currently property docstrings are only collected if
+            they are on the same line following the property definition. Getter and
+            setter methods are documented like methods currently, but the dot is
+            replaced by an underscore. Default values for properties are represented as
+            unicode strings, therefore strings will be double quoted.
+        
+        Users
+        -----
+        
+        * `Cantera <http://cantera.github.io/docs/sphinx/html/compiling/dependencies.html?highlight=matlabdomain>`_
+        * `CoSMo MVPA <http://cosmomvpa.org/download.html?highlight=matlabdomain#developers>`_
+        * `The Cobra Toolbox <https://opencobra.github.io/cobratoolbox/stable/index.html#>`_
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `sphinxcontrib-matlabdomain-0.7.1/CHANGES.rst` & `sphinxcontrib-matlabdomain-0.8.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+sphinxcontrib-matlabdomain-0.8.0 (2019-05-11)
+=============================================
+
+* Fixed ``Issue 91 <https://github.com/sphinx-contrib/matlabdomain/issues/91>`_.
+  Static methods in folder based classes.
+* Replaced Pygments MATLAB lexer with own. Removes issues with functions being
+  incorrectly parsed, handles double qouted string correctly.
+
+
 sphinxcontrib-matlabdomain-0.7.1 (2019-04-03)
 =============================================
 
 * Fixed ``Issue 90 <https://github.com/sphinx-contrib/matlabdomain/issues/90>`_.
   Wrong function name parsed when method escapes first argument with ~.
```

