# Comparing `tmp/saspy-5.0.2.tar.gz` & `tmp/saspy-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saspy-5.0.2.tar", last modified: Fri Mar 10 18:03:59 2023, max compression
+gzip compressed data, was "saspy-5.1.0.tar", last modified: Fri Apr 14 17:59:53 2023, max compression
```

## Comparing `saspy-5.0.2.tar` & `saspy-5.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-03-10 18:03:59.881213 saspy-5.0.2/
--rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-03-10 18:03:42.000000 saspy-5.0.2/LICENSE.md
--rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-03-10 18:03:42.000000 saspy-5.0.2/MANIFEST.in
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-03-10 18:03:59.880213 saspy-5.0.2/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-03-10 18:03:42.000000 saspy-5.0.2/README.md
--rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-03-10 18:03:42.000000 saspy-5.0.2/pyproject.toml
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-03-10 18:03:59.861211 saspy-5.0.2/saspy/
--rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/SASLogLexer.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/__init__.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/autocfg.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-03-10 18:03:59.862212 saspy-5.0.2/saspy/java/
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-03-10 18:03:59.871212 saspy-5.0.2/saspy/java/iomclient/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/log4j-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/log4j-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/log4j-core-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/log4j-core-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/sas.core.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/sas.security.sspi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/iomclient/sas.svc.connection.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-03-10 18:03:59.874212 saspy-5.0.2/saspy/java/pyiom/
--rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/pyiom/saspy2j.class
--rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/pyiom/saspy2j.java
--rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/saspyiom.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-03-10 18:03:59.880213 saspy-5.0.2/saspy/java/thirdparty/
--rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/thirdparty/NOTICE.md
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/thirdparty/glassfish-corba-orb.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/thirdparty/pfl-basic.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/java/thirdparty/pfl-tf.jar
--rw-r--r--   0 sastpw     (894) r&d        (100)     3542 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/libname_gen.sas
--rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasViyaML.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sas_magic.py
--rw-r--r--   0 sastpw     (894) r&d        (100)   136517 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasbase.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sascfg.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasdata.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasdecorator.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasets.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasexceptions.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasiocom.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    82968 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasiohttp.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    87068 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasioiom.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    99383 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasiostdio.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasml.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37478 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasproccommons.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasqc.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasresults.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasstat.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sastabulate.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/sasutil.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-03-10 18:03:59.880213 saspy-5.0.2/saspy/scripts/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/scripts/run_sas.py
--rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-03-10 18:03:42.000000 saspy-5.0.2/saspy/version.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-03-10 18:03:59.862212 saspy-5.0.2/saspy.egg-info/
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-03-10 18:03:59.000000 saspy-5.0.2/saspy.egg-info/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-03-10 18:03:59.000000 saspy-5.0.2/saspy.egg-info/SOURCES.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-03-10 18:03:59.000000 saspy-5.0.2/saspy.egg-info/dependency_links.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-03-10 18:03:59.000000 saspy-5.0.2/saspy.egg-info/requires.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-03-10 18:03:59.000000 saspy-5.0.2/saspy.egg-info/top_level.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-03-10 18:03:59.881213 saspy-5.0.2/setup.cfg
--rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-03-10 18:03:42.000000 saspy-5.0.2/setup.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.952901 saspy-5.1.0/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-04-14 17:59:34.000000 saspy-5.1.0/LICENSE.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-04-14 17:59:34.000000 saspy-5.1.0/MANIFEST.in
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-04-14 17:59:53.951901 saspy-5.1.0/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-04-14 17:59:34.000000 saspy-5.1.0/README.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-04-14 17:59:34.000000 saspy-5.1.0/pyproject.toml
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.923900 saspy-5.1.0/saspy/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/SASLogLexer.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/__init__.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/autocfg.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.925900 saspy-5.1.0/saspy/java/
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.938901 saspy-5.1.0/saspy/java/iomclient/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-core-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-core-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/sas.core.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/sas.security.sspi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/sas.svc.connection.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.942901 saspy-5.1.0/saspy/java/pyiom/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/pyiom/saspy2j.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/pyiom/saspy2j.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/saspyiom.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.950901 saspy-5.1.0/saspy/java/thirdparty/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/NOTICE.md
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-orb.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/pfl-basic.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/pfl-tf.jar
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/libname_gen.sas
+-rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasViyaML.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sas_magic.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)   130256 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasbase.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sascfg.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasdata.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasdecorator.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasets.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasexceptions.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasiocom.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    84218 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasiohttp.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    87068 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasioiom.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    99383 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasiostdio.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasml.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasproccommons.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasqc.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasresults.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasstat.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sastabulate.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasutil.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.951901 saspy-5.1.0/saspy/scripts/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/scripts/run_sas.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/version.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.925900 saspy-5.1.0/saspy.egg-info/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/SOURCES.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/dependency_links.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/requires.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/top_level.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-04-14 17:59:53.952901 saspy-5.1.0/setup.cfg
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-04-14 17:59:34.000000 saspy-5.1.0/setup.py
```

### Comparing `saspy-5.0.2/LICENSE.md` & `saspy-5.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/PKG-INFO` & `saspy-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.0.2
+Version: 5.1.0
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.0.2/README.md` & `saspy-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/SASLogLexer.py` & `saspy-5.1.0/saspy/SASLogLexer.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/__init__.py` & `saspy-5.1.0/saspy/__init__.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/autocfg.py` & `saspy-5.1.0/saspy/autocfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar` & `saspy-5.1.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar` & `saspy-5.1.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/log4j-api-2.12.4.jar` & `saspy-5.1.0/saspy/java/iomclient/log4j-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/log4j-api-2.17.1.jar` & `saspy-5.1.0/saspy/java/iomclient/log4j-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/log4j-core-2.12.4.jar` & `saspy-5.1.0/saspy/java/iomclient/log4j-core-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/log4j-core-2.17.1.jar` & `saspy-5.1.0/saspy/java/iomclient/log4j-core-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/sas.core.jar` & `saspy-5.1.0/saspy/java/iomclient/sas.core.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/sas.security.sspi.jar` & `saspy-5.1.0/saspy/java/iomclient/sas.security.sspi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/iomclient/sas.svc.connection.jar` & `saspy-5.1.0/saspy/java/iomclient/sas.svc.connection.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/pyiom/saspy2j.class` & `saspy-5.1.0/saspy/java/pyiom/saspy2j.class`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/pyiom/saspy2j.java` & `saspy-5.1.0/saspy/java/pyiom/saspy2j.java`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/saspyiom.jar` & `saspy-5.1.0/saspy/java/saspyiom.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/thirdparty/NOTICE.md` & `saspy-5.1.0/saspy/java/thirdparty/NOTICE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar` & `saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar` & `saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/thirdparty/glassfish-corba-orb.jar` & `saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-orb.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/thirdparty/pfl-basic.jar` & `saspy-5.1.0/saspy/java/thirdparty/pfl-basic.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/java/thirdparty/pfl-tf.jar` & `saspy-5.1.0/saspy/java/thirdparty/pfl-tf.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/libname_gen.sas` & `saspy-5.1.0/saspy/libname_gen.sas`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     proc document name=&objname..&objname.;
         ods output Properties=&objname.._&objname.properties;
         list \ /levels=all;
     quit;
     filename file1 temp;
     data _null_;
         length path $1000;
-        set &objname.._&objname.properties(where=(type = 'Dir' or type = {})) end=last;
+        set &objname.._&objname.properties(where=(type = 'Dir')) end=last;
         file file1;
         if _n_=1 then do;
             put "libname _&objname. sasedoc (";
         end;
         p=cat('"\&objname..&objname.', catt(path) , '"');
         put p;
         if last then do;
```

### Comparing `saspy-5.0.2/saspy/sasViyaML.py` & `saspy-5.1.0/saspy/sasViyaML.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sas_magic.py` & `saspy-5.1.0/saspy/sas_magic.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasbase.py` & `saspy-5.1.0/saspy/sasbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -509,14 +509,16 @@
     Other attrritubes of the SASsession object that you may use for various purposes.
 
     - hostsep - simply a forward slash for linux systems and a backslash on windows clients; just for convenience
     - check_error_log - Boolean that identifies an ERROR has been found in the SASLOG. You should set this to False prior \
                  to running a saspy method that where you check it after. saspy does not reset it to False for you.
     - reconuri - the uri (token) for connecting back to the workspace server after you've disconnected. \
                  not needed unless connecting back from a different Python process; not the usual case.
+    - HTML_Style - This is the Style for ODS output, set from SAS_output_options {'style' : ''} value in your config file. \
+                   You can change this value on the fly by setting the value for this attribute.
 
     """
     # SAS Epoch: 1960-01-01
     SAS_EPOCH = datetime.datetime(1960, 1, 1)
 
     # def __init__(self, cfgname: str ='', kernel: 'SAS_kernel' =None, saspath :str ='', options: list =[]) -> 'SASsession':
     def __init__(self, **kwargs):
@@ -605,28 +607,28 @@
               pass
 
            if failed:
               raise SASIOConnectionError(res)
 
            if self.pyenc is not None:
               if self._io.sascfg.encoding != '':
-                 if self._io.sascfg.encoding.lower() not in self.pyenc[1]:
+                 if self._io.sascfg.encoding.lower() not in self.pyenc:
                     msg  = "The encoding value provided doesn't match the SAS session encoding.\n"
                     msg += "SAS encoding is "+self.sascei+". Specified encoding is "+self._io.sascfg.encoding+".\n"
-                    msg += "Using encoding "+self.pyenc[1][0]+" instead to avoid transcoding problems.\n"
+                    msg += "Using encoding "+self.pyenc[1]+" instead to avoid transcoding problems.\n"
                     logging.info(msg)
                     msg  = "You can override this change, if you think you must, by changing the encoding attribute of the SASsession object, as follows.\n"
                     msg += """If you had 'sas = saspy.SASsession(), then submit: "sas._io.sascfg.encoding='override_encoding'" to change it.\n"""
                     logging.debug(msg)
-                    self._io.sascfg.encoding = self.pyenc[1][0]
+                    self._io.sascfg.encoding = self.pyenc[1]
               else:
-                 self._io.sascfg.encoding = self.pyenc[1][0]
+                 self._io.sascfg.encoding = self.pyenc[1]
                  if self._io.sascfg.verbose:
                     msg  = "No encoding value provided. Will try to determine the correct encoding.\n"
-                    msg += "Setting encoding to "+self.pyenc[1][0]+" based upon the SAS session encoding value of "+self.sascei+".\n"
+                    msg += "Setting encoding to "+self.pyenc[1]+" based upon the SAS session encoding value of "+self.sascei+".\n"
                     logging.info(msg)
            else:
               msg  = "The SAS session encoding for this session ("+self.sascei+") doesn't have a known Python equivalent encoding.\n"
               if self._io.sascfg.encoding == '':
                  self._io.sascfg.encoding  = 'utf_8'
                  msg += "Proceeding using the default encoding of 'utf_8', though you may encounter transcoding problems.\n"
               else:
@@ -1007,19 +1009,19 @@
         """
         Load the SAS macros at the start of the session
 
         :return:
         """
         macro_path = os.path.dirname(os.path.realpath(__file__))
         fd = os.open(macro_path + '/' + 'libname_gen.sas', os.O_RDONLY)
-        code  = b'options nosource;\n'
+        code = b'options nosource;\n'
         code += os.read(fd, 32767)
         code += b'\noptions source;'
-        code  = code.decode().format(self.pyenc[2])
-        self._io._asubmit(code, results='text')
+
+        self._io._asubmit(code.decode(), results='text')
         os.close(fd)
 
     def _render_html_or_log(self, ll):
         """
         This method renders the html lst if it's there else the log
         """
         if len(ll['LST']) > 0:
@@ -2675,75 +2677,75 @@
     'NLDATMMN', 'NLDATMS', 'NLDATMTM', 'NLDATMTZ', 'NLDATMW', 'NLDATMW', 'NLDATMWN', 'NLDATMWZ', 'NLDATMYM', 'NLDATMYML',
     'NLDATMYMM', 'NLDATMYMS', 'NLDATMYQ', 'NLDATMYQL', 'NLDATMYQM', 'NLDATMYQS', 'NLDATMYR', 'NLDATMYW', 'NLDATMZ',
     'NLDDFDT', 'NLDDFDT', 'NORDFDT', 'NORDFDT', 'POLDFDT', 'POLDFDT', 'PTGDFDT', 'PTGDFDT', 'RUSDFDT', 'RUSDFDT',
     'SLODFDT', 'SLODFDT', 'SVEDFDT', 'SVEDFDT', 'TWMDY', 'YMDDTTM',
 )
 
 sas_encoding_mapping = {
-'arabic':      [1, ['iso8859_6', 'iso-8859-6', 'arabic'],                                                                                "'Dir'"      ], # No
-'big5':        [2, ['big5', 'big5-tw', 'csbig5'],                                                                                        "'Dir'"      ], # No
-'cyrillic':    [1, ['iso8859_5', 'iso-8859-5', 'cyrillic'],                                                                              "'Dir'"      ], # No
-'ebcdic037':   [1, ['cp037', 'ibm037', 'ibm039'],                                                                                        "'Dir'"      ], # No
-'ebcdic273':   [1, ['cp273', '273', 'ibm273', 'csibm273'],                                                                               "'Dir'"      ], # No
-'ebcdic500':   [1, ['cp500', 'ebcdic-cp-be', 'ebcdic-cp-ch', 'ibm500'],                                                                  "'Dir'"      ], # No                                                                          ],
-'euc-cn':      [2, ['gb2312', 'chinese', 'csiso58gb231280', 'euc-cn', 'euccn', 'eucgb2312-cn', 'gb2312-1980', 'gb2312-80', 'iso-ir-58'], "'C4BFC2BC'x"],
-'euc-jp':      [4, ['euc_jis_2004', 'jisx0213', 'eucjis2004'],                                                                           "'Dir'"      ], # No
-'euc-kr':      [4, ['euc_kr', 'euckr', 'korean', 'ksc5601', 'ks_c-5601', 'ks_c-5601-1987', 'ksx1001', 'ks_x-1001'],                      "'B5F0B7BAC5CDB8AE'x"],
-'greek':       [1, ['iso8859_7', 'iso-8859-7', 'greek', 'greek8'],                                                                       "'Dir'"      ], # No
-'hebrew':      [1, ['iso8859_8', 'iso-8859-8', 'hebrew'],                                                                                "'Dir'"      ], # No
-'ibm-949':     [1, ['cp949', '949', 'ms949', 'uhc'],                                                                                     "'Dir'"      ], # No
-'kz1048':      [1, ['kz1048', 'kz_1048', 'strk1048_2002', 'rk1048'],                                                                     "'Dir'"      ], # No
-'latin10':     [1, ['iso8859_16', 'iso-8859-16', 'latin10', 'l10'],                                                                      "'Dir'"      ], # No
-'latin1':      [1, ['latin_1', 'iso-8859-1', 'iso8859-1', '8859', 'cp819', 'latin', 'latin1', 'l1'],                                     "'Dir'"      ], # No
-'latin2':      [1, ['iso8859_2', 'iso-8859-2', 'latin2', 'l2'],                                                                          "'Dir'"      ], # No
-'latin3':      [1, ['iso8859_3', 'iso-8859-3', 'latin3', 'l3'],                                                                          "'Dir'"      ], # No
-'latin4':      [1, ['iso8859_4', 'iso-8859-4', 'latin4', 'l4'],                                                                          "'Dir'"      ], # No
-'latin5':      [1, ['iso8859_9', 'iso-8859-9', 'latin5', 'l5'],                                                                          "'Dir'"      ], # No
-'latin6':      [1, ['iso8859_10', 'iso-8859-10', 'latin6', 'l6'],                                                                        "'Dir'"      ], # No
-'latin7':      [1, ['iso8859_13', 'iso-8859-13', 'latin7', 'l7'],                                                                        "'Dir'"      ], # No
-'latin8':      [1, ['iso8859_14', 'iso-8859-14', 'latin8', 'l8'],                                                                        "'Dir'"      ], # No
-'latin9':      [1, ['iso8859_15', 'iso-8859-15', 'latin9', 'l9'],                                                                        "'Dir'"      ], # No
-'ms-932':      [2, ['cp932', '932', 'ms932', 'mskanji', 'ms-kanji'],                                                                     "'Dir'"      ], # No
-'msdos737':    [1, ['cp737'],                                                                                                            "'Dir'"      ], # No
-'msdos775':    [1, ['cp775', 'ibm775'],                                                                                                  "'Dir'"      ], # No
-'open_ed-1026':[1, ['cp1026', 'ibm1026'],                                                                                                "'Dir'"      ], # No
-'open_ed-1047':[1, ['cp1047'],                                                                                                           "'Dir'"      ], # No # Though this isn't available in base python, it's 3rd party
-'open_ed-1140':[1, ['cp1140', 'ibm1140'],                                                                                                "'Dir'"      ], # No
-'open_ed-424': [1, ['cp424', 'ebcdic-cp-he', 'ibm424'],                                                                                  "'Dir'"      ], # No
-'open_ed-875': [1, ['cp875'],                                                                                                            "'Dir'"      ], # No
-'pcoem437':    [1, ['cp437', '437', 'ibm437'],                                                                                           "'Dir'"      ], # No
-'pcoem850':    [1, ['cp850', '850', 'ibm850'],                                                                                           "'Dir'"      ], # No
-'pcoem852':    [1, ['cp852', '852', 'ibm852'],                                                                                           "'Dir'"      ], # No
-'pcoem857':    [1, ['cp857', '857', 'ibm857'],                                                                                           "'Dir'"      ], # No
-'pcoem858':    [1, ['cp858', '858', 'ibm858'],                                                                                           "'Dir'"      ], # No
-'pcoem860':    [1, ['cp860', '860', 'ibm860'],                                                                                           "'Dir'"      ], # No
-'pcoem862':    [1, ['cp862', '862', 'ibm862'],                                                                                           "'Dir'"      ], # No
-'pcoem863':    [1, ['cp863'],                                                                                                            "'Dir'"      ], # No
-'pcoem864':    [1, ['cp864', 'ibm864'],                                                                                                  "'Dir'"      ], # No
-'pcoem865':    [1, ['cp865', '865', 'ibm865'],                                                                                           "'Dir'"      ], # No
-'pcoem866':    [1, ['cp866', '866', 'ibm866'],                                                                                           "'Dir'"      ], # No
-'pcoem869':    [1, ['cp869', '869', 'cp-gr', 'ibm869'],                                                                                  "'Dir'"      ], # No
-'pcoem874':    [1, ['cp874'],                                                                                                            "'Dir'"      ], # No
-'shift-jis':   [2, ['shift_jis', 'csshiftjis', 'shiftjis', 'sjis', 's_jis'],                                                             "'Dir'"      ], # No
-'thai':        [1, ['iso8859_11', 'so-8859-11', 'thai'],                                                                                 "'Dir'"      ], # No
-'us-ascii':    [1, ['ascii', '646', 'us-ascii'],                                                                                         "'Dir'"      ], # No
-'utf-8':       [4, ['utf_8', 'u8', 'utf', 'utf8', 'utf-8'],                                                                              "'Dir'"      ], # No
-'warabic':     [1, ['cp1256', 'windows-1256'],                                                                                           "'Dir'"      ], # No
-'wbaltic':     [1, ['cp1257', 'windows-1257'],                                                                                           "'Dir'"      ], # No
-'wcyrillic':   [1, ['cp1251', 'windows-1251'],                                                                                           "'Dir'"      ], # No
-'wgreek':      [1, ['cp1253', 'windows-1253'],                                                                                           "'Dir'"      ], # No
-'whebrew':     [1, ['cp1255', 'windows-1255'],                                                                                           "'Dir'"      ], # No
-'wlatin1':     [1, ['cp1252', 'windows-1252'],                                                                                           "'Dir'"      ], # No
-'wlatin2':     [1, ['cp1250', 'windows-1250'],                                                                                           "'Dir'"      ], # No
-'wturkish':    [1, ['cp1254', 'windows-1254'],                                                                                           "'Dir'"      ], # No
-'wvietnamese': [1, ['cp1258', 'windows-1258'],                                                                                           "'Dir'"      ], # No
-'any':None,                                                                                                                            
-'dec-cn':None,                                                                                                                         
-'dec-jp':None,                                                                                                                         
-'dec-tw':None,                                                                                                                         
+'arabic':      [1, 'iso8859_6', 'iso-8859-6', 'arabic'],
+'big5':        [2, 'big5', 'big5-tw', 'csbig5'],
+'cyrillic':    [1, 'iso8859_5', 'iso-8859-5', 'cyrillic'],
+'ebcdic037':   [1, 'cp037', 'ibm037', 'ibm039'],
+'ebcdic273':   [1, 'cp273', '273', 'ibm273', 'csibm273'],
+'ebcdic500':   [1, 'cp500', 'ebcdic-cp-be', 'ebcdic-cp-ch', 'ibm500'],
+'euc-cn':      [2, 'gb2312', 'chinese', 'csiso58gb231280', 'euc-cn', 'euccn', 'eucgb2312-cn', 'gb2312-1980', 'gb2312-80', 'iso-ir-58'],
+'euc-jp':      [4, 'euc_jis_2004', 'jisx0213', 'eucjis2004'],
+'euc-kr':      [4, 'euc_kr', 'euckr', 'korean', 'ksc5601', 'ks_c-5601', 'ks_c-5601-1987', 'ksx1001', 'ks_x-1001'],
+'greek':       [1, 'iso8859_7', 'iso-8859-7', 'greek', 'greek8'],
+'hebrew':      [1, 'iso8859_8', 'iso-8859-8', 'hebrew'],
+'ibm-949':     [1, 'cp949', '949', 'ms949', 'uhc'],
+'kz1048':      [1, 'kz1048', 'kz_1048', 'strk1048_2002', 'rk1048'],
+'latin10':     [1, 'iso8859_16', 'iso-8859-16', 'latin10', 'l10'],
+'latin1':      [1, 'latin_1', 'iso-8859-1', 'iso8859-1', '8859', 'cp819', 'latin', 'latin1', 'l1'],
+'latin2':      [1, 'iso8859_2', 'iso-8859-2', 'latin2', 'l2'],
+'latin3':      [1, 'iso8859_3', 'iso-8859-3', 'latin3', 'l3'],
+'latin4':      [1, 'iso8859_4', 'iso-8859-4', 'latin4', 'l4'],
+'latin5':      [1, 'iso8859_9', 'iso-8859-9', 'latin5', 'l5'],
+'latin6':      [1, 'iso8859_10', 'iso-8859-10', 'latin6', 'l6'],
+'latin7':      [1, 'iso8859_13', 'iso-8859-13', 'latin7', 'l7'],
+'latin8':      [1, 'iso8859_14', 'iso-8859-14', 'latin8', 'l8'],
+'latin9':      [1, 'iso8859_15', 'iso-8859-15', 'latin9', 'l9'],
+'ms-932':      [2, 'cp932', '932', 'ms932', 'mskanji', 'ms-kanji'],
+'msdos737':    [1, 'cp737'],
+'msdos775':    [1, 'cp775', 'ibm775'],
+'open_ed-1026':[1, 'cp1026', 'ibm1026'],
+'open_ed-1047':[1, 'cp1047'],              # Though this isn't available in base python, it's 3rd party
+'open_ed-1140':[1, 'cp1140', 'ibm1140'],
+'open_ed-424': [1, 'cp424', 'ebcdic-cp-he', 'ibm424'],
+'open_ed-875': [1, 'cp875'],
+'pcoem437':    [1, 'cp437', '437', 'ibm437'],
+'pcoem850':    [1, 'cp850', '850', 'ibm850'],
+'pcoem852':    [1, 'cp852', '852', 'ibm852'],
+'pcoem857':    [1, 'cp857', '857', 'ibm857'],
+'pcoem858':    [1, 'cp858', '858', 'ibm858'],
+'pcoem860':    [1, 'cp860', '860', 'ibm860'],
+'pcoem862':    [1, 'cp862', '862', 'ibm862'],
+'pcoem863':    [1, 'cp863'],
+'pcoem864':    [1, 'cp864', 'ibm864'],
+'pcoem865':    [1, 'cp865', '865', 'ibm865'],
+'pcoem866':    [1, 'cp866', '866', 'ibm866'],
+'pcoem869':    [1, 'cp869', '869', 'cp-gr', 'ibm869'],
+'pcoem874':    [1, 'cp874'],
+'shift-jis':   [2, 'shift_jis', 'csshiftjis', 'shiftjis', 'sjis', 's_jis'],
+'thai':        [1, 'iso8859_11', 'so-8859-11', 'thai'],
+'us-ascii':    [1, 'ascii', '646', 'us-ascii'],
+'utf-8':       [4, 'utf_8', 'u8', 'utf', 'utf8', 'utf-8'],
+'warabic':     [1, 'cp1256', 'windows-1256'],
+'wbaltic':     [1, 'cp1257', 'windows-1257'],
+'wcyrillic':   [1, 'cp1251', 'windows-1251'],
+'wgreek':      [1, 'cp1253', 'windows-1253'],
+'whebrew':     [1, 'cp1255', 'windows-1255'],
+'wlatin1':     [1, 'cp1252', 'windows-1252'],
+'wlatin2':     [1, 'cp1250', 'windows-1250'],
+'wturkish':    [1, 'cp1254', 'windows-1254'],
+'wvietnamese': [1, 'cp1258', 'windows-1258'],
+'any':None,
+'dec-cn':None,
+'dec-jp':None,
+'dec-tw':None,
 'ebcdic1025':None,
 'ebcdic1026':None,
 'ebcdic1047':None,
 'ebcdic1112':None,
 'ebcdic1122':None,
 'ebcdic1130':None,
 'ebcdic1137':None,
```

### Comparing `saspy-5.0.2/saspy/sascfg.py` & `saspy-5.1.0/saspy/sascfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasdata.py` & `saspy-5.1.0/saspy/sasdata.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasdecorator.py` & `saspy-5.1.0/saspy/sasdecorator.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasets.py` & `saspy-5.1.0/saspy/sasets.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasexceptions.py` & `saspy-5.1.0/saspy/sasexceptions.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasiocom.py` & `saspy-5.1.0/saspy/sasiocom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasiohttp.py` & `saspy-5.1.0/saspy/sasiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import json
 import os
 import ssl
 import sys
 import urllib
 import warnings
 import io
+import ssl
 
 import tempfile as tf
 from time import sleep
 from threading import Thread
 
 from saspy.sasexceptions import (SASHTTPauthenticateError, SASHTTPconnectionError, SASHTTPsubmissionError)
 
@@ -55,15 +56,16 @@
       self.serverid  = cfg.get('serverid', None)
       self.ip        = cfg.get('ip', '')
       self.port      = cfg.get('port', None)
       self.ctxname   = cfg.get('context', '')
       self.ctx       = {}
       self.options   = cfg.get('options', [])
       self.ssl       = cfg.get('ssl', True)
-      self.verify    = cfg.get('verify', True)
+      self.cafile    = cfg.get('cafile', None)
+      self.verify    = cfg.get('verify', None)
       self.timeout   = cfg.get('timeout', None)
       user           = cfg.get('user', '')
       pw             = cfg.get('pw', '')
       client_id      = cfg.get('client_id', None)
       client_secret  = cfg.get('client_secret', '')
       authcode       = cfg.get('authcode', None)
       jwt            = cfg.get('jwt', None)
@@ -221,14 +223,21 @@
       inssl = kwargs.get('ssl', None)
       if inssl is not None:
          if lock and self.ssl:
             logger.warning("Parameter 'ssl' passed to SAS_session was ignored due to configuration restriction.")
          else:
             self.ssl = bool(inssl)
 
+      incaf = kwargs.get('cafile', None)
+      if incaf is not None:
+         if lock and self.cafile:
+            logger.warning("Parameter 'cafile' passed to SAS_session was ignored due to configuration restriction.")
+         else:
+            self.cafile = incaf
+
       inver = kwargs.get('verify', None)
       if inver is not None:
          if lock and self.verify:
             logger.warning("Parameter 'verify' passed to SAS_session was ignored due to configuration restriction.")
          else:
             self.verify = bool(inver)
 
@@ -352,24 +361,36 @@
          #else:
          #   logger.warning("Parameter 'proxy' not in recognized format. Expeting '[http[s]://]host:port'. Ignoring parameter.")
       else:
          self.pip = None
 
       # get Connections
       if self.ssl:
-         if self.verify:
+         sslctx = ssl.create_default_context(cafile=self.cafile)
+         if   self.verify is None:
             # handle having self signed certificate default on Viya w/out copies on client; still ssl, just not verifiable
             try:
-               self.REFConn  = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout); self.REFConn.connect();  self.REFConn.close()
-               self.HTTPConn = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout); self.HTTPConn.connect(); self.HTTPConn.close()
+               self.REFConn  = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=sslctx)
+               self.REFConn.connect();  self.REFConn.close()
+               self.HTTPConn = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=sslctx)
+               self.HTTPConn.connect(); self.HTTPConn.close()
             except ssl.SSLError as e:
                logger.warning("SSL certificate verification failed, creating an unverified SSL connection. Error was:"+str(e))
                self.REFConn  = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=ssl._create_unverified_context())
                self.HTTPConn = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=ssl._create_unverified_context())
                logger.warning("You can set 'verify=False' to get rid of this message ")
+         elif self.verify:
+            try:
+               self.REFConn  = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=sslctx)
+               self.REFConn.connect();  self.REFConn.close()
+               self.HTTPConn = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=sslctx)
+               self.HTTPConn.connect(); self.HTTPConn.close()
+            except ssl.SSLError as e:
+               logger.error("SSL certificate verification failed and verify was True; no connection established.\nError was:"+str(e))
+               raise SASHTTPconnectionError(msg="SSL certificate verification failed and verify was True; no connection established.")
          else:
             self.REFConn  = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=ssl._create_unverified_context())
             self.HTTPConn = hc.HTTPSConnection(self.ip, self.port, timeout=self.timeout, context=ssl._create_unverified_context())
       else:
          self.REFConn  = hc.HTTPConnection(self.ip, self.port, timeout=self.timeout)
          self.HTTPConn = hc.HTTPConnection(self.ip, self.port, timeout=self.timeout)
 
@@ -381,15 +402,15 @@
       if not self._token:
          js = self._authenticate(user, pw, authcode, client_id, client_secret, jwt)
          self._token   = js.get('access_token',  None)
          self._refresh = js.get('refresh_token', None)
 
       if not self._token:
          logger.error("Could not acquire an Authentication Token")
-         return
+         raise SASHTTPconnectionError(msg="Could not acquire an Authentication Token. No connection established.")
 
       # GET Contexts
       contexts = self._get_contexts()
       if contexts == None:
          self._token = None
          raise SASHTTPconnectionError(msg="No Contexts found on Compute Service at ip="+self.ip)
```

### Comparing `saspy-5.0.2/saspy/sasioiom.py` & `saspy-5.1.0/saspy/sasioiom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasiostdio.py` & `saspy-5.1.0/saspy/sasiostdio.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasml.py` & `saspy-5.1.0/saspy/sasml.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasproccommons.py` & `saspy-5.1.0/saspy/sasproccommons.py`

 * *Files 1% similar despite different names*

```diff
@@ -648,22 +648,22 @@
             if len(error) > 1:
                 RuntimeWarning("ERRORS found in SAS log: \n%s" % error)
                 self.sas._lastlog = self.sas._io._log[lastlog:]
                 return SASresults(obj1, self.sas, objname, nosub, log)
 
             code = """
             data _null_;
-               set {}._{}properties(where=(type NE 'Dir' and type NE {})) end=last;
+               set {}._{}properties(where=(type NE 'Dir')) end=last;
                if _n_ = 1  then
                   put %upcase("libStart=");
                put path;
                if last then
                   put %upcase("libEND=");
             run;
-            """.format(objname, objname, self.sas.pyenc[2])
+            """.format(objname, objname)
             ll  = self.sas._io.submit(code, results='text')
             #import pdb; pdb.set_trace()
 
             if ll['LOG'].find("LIBSTART") and ll['LOG'].find("LIBEND"):
                paths = ll['LOG'].rpartition('LIBEND=')[0].rpartition('LIBSTART=')[2][1:].splitlines()
                all = {}
                for path in paths:
```

### Comparing `saspy-5.0.2/saspy/sasqc.py` & `saspy-5.1.0/saspy/sasqc.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasresults.py` & `saspy-5.1.0/saspy/sasresults.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasstat.py` & `saspy-5.1.0/saspy/sasstat.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sastabulate.py` & `saspy-5.1.0/saspy/sastabulate.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/sasutil.py` & `saspy-5.1.0/saspy/sasutil.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy/scripts/run_sas.py` & `saspy-5.1.0/saspy/scripts/run_sas.py`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/saspy.egg-info/PKG-INFO` & `saspy-5.1.0/saspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.0.2
+Version: 5.1.0
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.0.2/saspy.egg-info/SOURCES.txt` & `saspy-5.1.0/saspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saspy-5.0.2/setup.py` & `saspy-5.1.0/setup.py`

 * *Files identical despite different names*

