# Comparing `tmp/z0lib-2.0.3.tar.gz` & `tmp/z0lib-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/z0lib-2.0.3.tar", last modified: Fri Jan 13 17:56:47 2023, max compression
+gzip compressed data, was "z0lib-2.0.4.tar", last modified: Fri Apr 14 15:32:52 2023, max compression
```

## Comparing `z0lib-2.0.3.tar` & `z0lib-2.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:56:47.000000 z0lib-2.0.3/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0lib-2.0.3/z0lib/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib/tests/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1269 2022-12-09 05:08:44.000000 z0lib-2.0.3/z0lib/tests/tmp.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4783 2023-01-09 05:29:34.000000 z0lib-2.0.3/z0lib/tests/z0lib_test_01.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      718 2022-12-09 05:08:44.000000 z0lib-2.0.3/z0lib/tests/tmp1.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3744 2023-01-09 05:29:34.000000 z0lib-2.0.3/z0lib/tests/test_z0lib.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 z0lib-2.0.3/z0lib/tests/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1940 2022-12-26 10:33:29.000000 z0lib-2.0.3/z0lib/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6393 2023-01-09 05:29:34.000000 z0lib-2.0.3/z0lib/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0lib-2.0.3/z0lib/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4118 2023-01-09 05:29:34.000000 z0lib-2.0.3/z0lib/xuname
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    58359 2023-01-09 05:29:34.000000 z0lib-2.0.3/z0lib/z0librc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      106 2022-12-09 05:08:44.000000 z0lib-2.0.3/z0lib/explore_env.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4999 2023-01-09 05:29:34.000000 z0lib-2.0.3/z0lib/optargs
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20207 2023-01-09 05:29:29.000000 z0lib-2.0.3/z0lib/z0librun.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      148 2022-12-09 05:08:44.000000 z0lib-2.0.3/z0lib/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-01-13 17:56:47.000000 z0lib-2.0.3/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1936 2023-01-09 05:29:34.000000 z0lib-2.0.3/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:08:41.000000 z0lib-2.0.3/z0lib.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       56 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      530 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1604 2023-01-13 17:56:47.000000 z0lib-2.0.3/z0lib.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1604 2023-01-13 17:56:47.000000 z0lib-2.0.3/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7242 2023-01-13 17:56:46.000000 z0lib-2.0.3/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1505 2023-04-14 15:32:52.842398 z0lib-2.0.4/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7402 2023-04-14 15:32:52.000000 z0lib-2.0.4/README.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-14 15:32:52.842398 z0lib-2.0.4/setup.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1936 2023-04-14 14:48:04.000000 z0lib-2.0.4/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/z0lib/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      148 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      106 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/explore_env.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4999 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/optargs
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/z0lib/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6393 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1936 2023-04-14 15:28:25.000000 z0lib-2.0.4/z0lib/scripts/setup.info
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/z0lib/tests/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/tests/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4783 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/tests/test_runtraced.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3744 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/tests/test_z0lib.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1269 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/tests/tmp.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      718 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/tests/tmp1.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4118 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/xuname
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    58413 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/z0librc
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20882 2023-04-14 14:47:59.000000 z0lib-2.0.4/z0lib/z0librun.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/z0lib.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1505 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      531 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       56 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:08:41.000000 z0lib-2.0.4/z0lib.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `z0lib-2.0.3/z0lib/tests/tmp.py` & `z0lib-2.0.4/z0lib/tests/tmp.py`

 * *Files identical despite different names*

### Comparing `z0lib-2.0.3/z0lib/tests/z0lib_test_01.py` & `z0lib-2.0.4/z0lib/tests/test_runtraced.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 from __future__ import print_function, unicode_literals
 import os
 import sys
 from zerobug import z0test
 from z0lib import z0lib
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 MODULE_ID = 'z0lib'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `z0lib-2.0.3/z0lib/tests/tmp1.py` & `z0lib-2.0.4/z0lib/tests/tmp1.py`

 * *Files identical despite different names*

### Comparing `z0lib-2.0.3/z0lib/tests/test_z0lib.py` & `z0lib-2.0.4/z0lib/tests/test_z0lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # import pdb
 import os
 
 # import sys
 # from zerobug import Z0test
 from z0lib import z0lib
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 MODULE_ID = 'z0lib'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `z0lib-2.0.3/z0lib/scripts/setup.info` & `z0lib-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='z0lib',
-    version='2.0.2.1',
+    version='2.0.4',
     description='Bash zeroincombenze lib',
     long_description="""
 General purpose bash and python library for zeroincombenze(R) tools
 
 Features:
 
 * xuname: unix/linux platform recognizer (tested on various environments)
@@ -20,15 +20,15 @@
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        # 'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: System :: System Shells',
     ],
     keywords='bash, optargs',
     url='https://zeroincombenze-tools.readthedocs.io',
```

### Comparing `z0lib-2.0.3/z0lib/scripts/main.py` & `z0lib-2.0.4/z0lib/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `z0lib-2.0.3/z0lib/xuname` & `z0lib-2.0.4/z0lib/xuname`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.3
+__version__=2.0.4
 
 
 # Main program
 OPTOPTS=(h        a       c       d       f        i       k       m       p       r       s       v       V           x)
 OPTDEST=(opt_help opt_prm opt_prm opt_prm opt_prm  opt_prm opt_prm opt_prm opt_prm opt_prm opt_prm opt_prm opt_version opt_prm)
 OPTACTI=("+"      "*>"    "*>"    "*>"    "*>"     "*>"    "*>"    "*>"    "*>"    "*>"    "*>"    "*>"    "*>"        "*>")
 OPTDEFL=(1        ""      ""      ""      ""       ""      ""      ""      ""      ""      ""      ""      ""          "")
```

### Comparing `z0lib-2.0.3/z0lib/z0librc` & `z0lib-2.0.4/z0lib/z0librc`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) SHS-AV s.r.l. (<http://ww.zeroincombenze.it>)
 # This software is free software under GNU Affero GPL3
 # Bash general purpose library
-#__version__=2.0.3
+#__version__=2.0.4
 [ $BASH_VERSINFO -lt 4 ] && echo "This script $0 requires bash 4.0+!" && exit 4
 [ "${BASH_SOURCE-}" == "$0" ] && echo "You must source this script: \$ source $0" >&2 && exit 33
 STS_FAILED=1
 STS_SUCCESS=0
 
 ##############################################################################
 # Install this lib file in /etc if version is more recent
@@ -578,15 +578,15 @@
       fi
       if [[ ! $1 =~ ^# ]]; then
         eval "$xcmd"
         sts=$?
       fi
     elif [[ ! $1 =~ ^sleep[[:space:]] ]]; then
       [[ $verbose -gt 0 ]] && echo "$pfx$xcmd"
-      [[ $1 =~ ^(cd[[:space:]].*[\;\&\|]|cd)$ ]] && eval "$xcmd" 2>/dev/null
+      [[ $1 =~ ^(cd[[:space:]].*[\;\&\|]?|cd|pushd[[:space:]].*[\;\&\|]?|popd|export[[:space:]].*)$ ]] && eval "$xcmd" 2>/dev/null
     fi
     echo -en "\e[0m"
     ((Z0_STACK=Z0_STACK-2))
     $SETX
     return $sts
 }
 export -f run_traced
```

### Comparing `z0lib-2.0.3/z0lib/optargs` & `z0lib-2.0.4/z0lib/optargs`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.3
+__version__=2.0.4
 
 if [ "$OPTARGS_TEST_1_2" ]; then
   test_1_2=$OPTARGS_TEST_1_2
 else
   test_1_2=1
 fi
 if [ $test_1_2 -eq 1 ]; then
```

### Comparing `z0lib-2.0.3/z0lib/z0librun.py` & `z0lib-2.0.4/z0lib/z0librun.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "/etc/openerp-server.conf",
     "/etc/odoo/openerp-server.conf",
     "/etc/openerp/odoo-server.conf",
 ]
 # Read Odoo configuration file (False or /etc/openerp-server.conf)
 OE_CONF = False
 DEFDCT = {}
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 def nakedname(path):
     return os.path.splitext(os.path.basename(path))[0]
 
 
 def run_traced(cmd, verbose=None, dry_run=None, disable_alias=None, is_alias=None):
@@ -140,40 +140,55 @@
         if (
             cmd_neutral_if(args, params=['dir'])
             or cmd_neutral_if(args, params=['ls'])
         ):
             dry_run = False
         if dry_run:
             0, prcout, prcerr
-        if sys.version_info[0] == 2:
-            try:
-                proc = Popen(args, stderr=PIPE, stdout=PIPE)
-                prcout, prcerr = proc.communicate()
-                sts = proc.returncode
-                prcout = prcout.decode("utf-8")
-                prcerr = prcerr.decode("utf-8")
-            except OSError as e:
-                if verbose:
-                    print(e)
-                sts = 127
-            except BaseException:
-                sts = 126
-        else:
-            try:
-                with Popen(args, stdin=PIPE, stdout=PIPE, stderr=PIPE) as proc:
+        with_shell = False
+        while 1:
+            if sys.version_info[0] == 2:
+                try:
+                    proc = Popen(
+                        args if not with_shell else " ".join(args),
+                        stderr=PIPE,
+                        stdout=PIPE,
+                        shell=with_shell)
                     prcout, prcerr = proc.communicate()
                     sts = proc.returncode
                     prcout = prcout.decode("utf-8")
                     prcerr = prcerr.decode("utf-8")
-            except FileNotFoundError as e:                                 # noqa: F821
-                if verbose:
-                    print(e)
-                sts = 127
-            except BaseException:
-                sts = 126
+                except OSError as e:
+                    if verbose:
+                        print(e)
+                    sts = 127
+                except BaseException:
+                    sts = 126
+            else:
+                try:
+                    with Popen(
+                            args if not with_shell else " ".join(args),
+                            stdin=PIPE,
+                            stdout=PIPE,
+                            stderr=PIPE,
+                            shell=with_shell
+                    ) as proc:
+                        prcout, prcerr = proc.communicate()
+                        sts = proc.returncode
+                        prcout = prcout.decode("utf-8")
+                        prcerr = prcerr.decode("utf-8")
+                except FileNotFoundError as e:                             # noqa: F821
+                    if verbose:
+                        print(e)
+                    sts = 127
+                except BaseException:
+                    sts = 126
+            if sts == 0 or with_shell:
+                break
+            with_shell = True
         return sts, prcout, prcerr
 
     def sh_cd(args, verbose=None, dry_run=None):
         argv, opt_unk, paths, params = simple_parse(args, {})
         sts = 0
         tgtpath = paths[0] if paths else os.environ["HOME"]
         if os.path.isdir(tgtpath):
@@ -347,16 +362,20 @@
         method = {
             "cd": sh_cd,
             # "cp": sh_cp,
             "git": sh_git,
             "mkdir": sh_mkdir,
             "rm": sh_rm,
         }.get(args[0])
-        if method:
-            return method(args, verbose=verbose, dry_run=dry_run)
+    else:
+        method = {
+            "cd": sh_cd,
+        }.get(args[0])
+    if method:
+        return method(args, verbose=verbose, dry_run=dry_run)
     return sh_any(args, verbose=verbose, dry_run=dry_run)
 
 
 class CountAction(argparse.Action):
     def __init__(self, option_strings, dest, default=None, required=False, help=None):
         super(CountAction, self).__init__(
             option_strings=option_strings,
```

### Comparing `z0lib-2.0.3/setup.py` & `z0lib-2.0.4/z0lib/scripts/setup.info`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='z0lib',
-    version='2.0.3',
+    version='2.0.4',
     description='Bash zeroincombenze lib',
     long_description="""
 General purpose bash and python library for zeroincombenze(R) tools
 
 Features:
 
 * xuname: unix/linux platform recognizer (tested on various environments)
```

### Comparing `z0lib-2.0.3/z0lib.egg-info/SOURCES.txt` & `z0lib-2.0.4/z0lib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 z0lib.egg-info/not-zip-safe
 z0lib.egg-info/requires.txt
 z0lib.egg-info/top_level.txt
 z0lib/scripts/__init__.py
 z0lib/scripts/main.py
 z0lib/scripts/setup.info
 z0lib/tests/__init__.py
+z0lib/tests/test_runtraced.py
 z0lib/tests/test_z0lib.py
 z0lib/tests/tmp.py
-z0lib/tests/tmp1.py
-z0lib/tests/z0lib_test_01.py
+z0lib/tests/tmp1.py
```

### Comparing `z0lib-2.0.3/z0lib.egg-info/PKG-INFO` & `z0lib-2.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: z0lib
-Version: 2.0.3
+Version: 2.0.4
 Summary: Bash zeroincombenze lib
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        General purpose bash and python library for zeroincombenze(R) tools
-        
-        Features:
-        
-        * xuname: unix/linux platform recognizer (tested on various environments)
-        * parseoptargs: line command parser; expands python argparse and adds same functionalities to bash scripts
-        * tracelog: manage tracelog (only bash)
-        * findpkg: find package in file system (only bash)
-        * run_traced: execute (or dry_run) shell command (only bash)
-        * CFG: local dictionary values from config file like python ConfigParser (only bash)
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: bash,optargs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+General purpose bash and python library for zeroincombenze(R) tools
+
+Features:
+
+* xuname: unix/linux platform recognizer (tested on various environments)
+* parseoptargs: line command parser; expands python argparse and adds same functionalities to bash scripts
+* tracelog: manage tracelog (only bash)
+* findpkg: find package in file system (only bash)
+* run_traced: execute (or dry_run) shell command (only bash)
+* CFG: local dictionary values from config file like python ConfigParser (only bash)
+
+
```

### Comparing `z0lib-2.0.3/PKG-INFO` & `z0lib-2.0.4/z0lib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: z0lib
-Version: 2.0.3
+Version: 2.0.4
 Summary: Bash zeroincombenze lib
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        General purpose bash and python library for zeroincombenze(R) tools
-        
-        Features:
-        
-        * xuname: unix/linux platform recognizer (tested on various environments)
-        * parseoptargs: line command parser; expands python argparse and adds same functionalities to bash scripts
-        * tracelog: manage tracelog (only bash)
-        * findpkg: find package in file system (only bash)
-        * run_traced: execute (or dry_run) shell command (only bash)
-        * CFG: local dictionary values from config file like python ConfigParser (only bash)
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: bash,optargs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+General purpose bash and python library for zeroincombenze(R) tools
+
+Features:
+
+* xuname: unix/linux platform recognizer (tested on various environments)
+* parseoptargs: line command parser; expands python argparse and adds same functionalities to bash scripts
+* tracelog: manage tracelog (only bash)
+* findpkg: find package in file system (only bash)
+* run_traced: execute (or dry_run) shell command (only bash)
+* CFG: local dictionary values from config file like python ConfigParser (only bash)
+
+
```

### Comparing `z0lib-2.0.3/README.rst` & `z0lib-2.0.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-=============
-z0lib 2.0.2.1
-=============
+===========
+z0lib 2.0.4
+===========
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
 
@@ -99,16 +99,22 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
-2.0.2.2 (2022-12-22)
-~~~~~~~~~~~~~~~~~~~~
+2.0.4 (2023-04-10)
+~~~~~~~~~~~~~~~~~~
+
+* [FIX] run_traced: cd does not work w/o alias
+* [IMP] coveralls and codecov are not more dependencies
+
+2.0.3 (2022-12-22)
+~~~~~~~~~~~~~~~~~~
 
 * [FIX] run_traced: --switch sometime crashes
 
 2.0.2.1 (2022-12-15)
 ~~~~~~~~~~~~~~~~~~~~
 
 * [FIX] run_traced: alias function
@@ -170,21 +176,24 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio Maria Vigliotti <info@shs-av.com>
+Contributors
+------------
+
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2022-12-26
+Last Update / Ultimo aggiornamento: 2023-04-14
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

