# Comparing `tmp/pymediawikidocker-0.9.6.tar.gz` & `tmp/pymediawikidocker-0.9.7.tar.gz`

## Comparing `pymediawikidocker-0.9.6.tar` & `pymediawikidocker-0.9.7.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.pydevproject
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/.DS_Store
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/__init__.py
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/config.py
--rw-r--r--   0        0        0    23202 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/docker.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/html_table.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/logger.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/mariadb.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/mw.py
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/mwcluster.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/version.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/webscrape.py
--rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/extensions.json
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/addCronTabEntry.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/addSysopUser.sh
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/initdb.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/installExtensions.sh
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwCompose.yml
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwDockerfile
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings.php
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings127.php
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings131.php
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings135.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings136.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings137.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings138.php
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings139.php
--rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki127.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki131.sql
--rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki135.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki136.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki137.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki138.sql
--rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki139.sql
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/phpinfo.php
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/plantuml.sh
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/startRunJobs.sh
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/update.sh
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/upload.ini
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/scripts/install
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/basetest.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/test_config.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/test_extensions.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/test_html_tables.py
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/test_install.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/LICENSE
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/README.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.pydevproject
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/.DS_Store
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/__init__.py
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/config.py
+-rw-r--r--   0        0        0    23212 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/docker.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/html_table.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/logger.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/mariadb.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/mw.py
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/mwcluster.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/version.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/webscrape.py
+-rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/extensions.json
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/addCronTabEntry.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/addSysopUser.sh
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/initdb.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/installExtensions.sh
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/lang.sh
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwCompose.yml
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwDockerfile
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings.php
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings127.php
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings131.php
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings135.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings136.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings137.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings138.php
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings139.php
+-rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki127.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki131.sql
+-rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki135.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki136.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki137.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki138.sql
+-rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki139.sql
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/phpinfo.php
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/plantuml.sh
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/startRunJobs.sh
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/update.sh
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/mwdocker/resources/templates/upload.ini
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/scripts/install
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/basetest.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/test_config.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/test_extensions.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/test_html_tables.py
+-rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/tests/test_install.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/LICENSE
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/README.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.7/PKG-INFO
```

### Comparing `pymediawikidocker-0.9.6/.github/workflows/build.yml` & `pymediawikidocker-0.9.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/.github/workflows/upload-to-pypi.yml` & `pymediawikidocker-0.9.7/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/.DS_Store` & `pymediawikidocker-0.9.7/mwdocker/.DS_Store`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/config.py` & `pymediawikidocker-0.9.7/mwdocker/config.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/docker.py` & `pymediawikidocker-0.9.7/mwdocker/docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,15 @@
         self.generate("mwDockerfile",f"{self.dockerPath}/Dockerfile",composerVersion=self.composerVersion,overwrite=overwrite)
         self.generate("mwCompose.yml",f"{self.dockerPath}/docker-compose.yml",mySQLRootPassword=self.config.mySQLRootPassword,mySQLPassword=self.config.mySQLPassword,container_base_name=self.config.container_base_name,overwrite=overwrite)
         self.generate(f"mwLocalSettings{self.config.shortVersion}.php",f"{self.dockerPath}/LocalSettings.php",mySQLPassword=self.config.mySQLPassword,hostname=self.config.host,extensions=self.config.extensionMap.values(),mwShortVersion=self.config.shortVersion,logo=self.config.logo,overwrite=overwrite)
         self.generate(f"mwWiki{self.config.shortVersion}.sql",f"{self.dockerPath}/wiki.sql",overwrite=overwrite)
         self.generate(f"addSysopUser.sh",f"{self.dockerPath}/addSysopUser.sh",user=self.config.user,password=self.config.password,overwrite=overwrite)
         self.generate(f"installExtensions.sh",f"{self.dockerPath}/installExtensions.sh",extensions=self.config.extensionMap.values(),branch=self.branch,overwrite=overwrite)
         self.genComposerRequire(f"{self.dockerPath}/composer.local.json",overwrite=overwrite)
-        for fileName in ["addCronTabEntry.sh","startRunJobs.sh","initdb.sh","update.sh","phpinfo.php","upload.ini","plantuml.sh"]:
+        for fileName in ["addCronTabEntry.sh","startRunJobs.sh","initdb.sh","update.sh","phpinfo.php","upload.ini","lang.sh","plantuml.sh"]:
             self.generate(f"{fileName}",f"{self.dockerPath}/{fileName}",overwrite=overwrite)
         
     def down(self,forceRebuild:bool=False):
         """
         run docker compose down
         
         see https://docs.docker.com/engine/reference/commandline/compose_down/
```

### Comparing `pymediawikidocker-0.9.6/mwdocker/html_table.py` & `pymediawikidocker-0.9.7/mwdocker/html_table.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/logger.py` & `pymediawikidocker-0.9.7/mwdocker/logger.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/mariadb.py` & `pymediawikidocker-0.9.7/mwdocker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/mw.py` & `pymediawikidocker-0.9.7/mwdocker/mw.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/mwcluster.py` & `pymediawikidocker-0.9.7/mwdocker/mwcluster.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/version.py` & `pymediawikidocker-0.9.7/mwdocker/version.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/webscrape.py` & `pymediawikidocker-0.9.7/mwdocker/webscrape.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/extensions.json` & `pymediawikidocker-0.9.7/mwdocker/resources/extensions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972222222222222%*

 * *Differences: {"'extensions'": "{10: {'require_once_until': '139'}}"}*

```diff
@@ -79,14 +79,15 @@
             "since": "2008-03-20T00:00:00",
             "url": "https://www.mediawiki.org/wiki/Extension:Header_Tabs"
         },
         {
             "extension": "ImageLink",
             "giturl": "https://github.com/BITPlan/ImageLink",
             "name": "ImageLink",
+            "require_once_until": "139",
             "url": "https://wiki.bitplan.com/index.php/ImageLink"
         },
         {
             "extension": "ImageMap",
             "giturl": "https://github.com/wikimedia/mediawiki-extensions-ImageMap",
             "localSettings": "$wgEnableUploads = true;\r\n$wgUseImageMagick = true;\r\n$wgImageMagickConvertCommand = \"/usr/bin/convert\";",
             "name": "ImageMap",
```

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwCompose.yml` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwCompose.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwDockerfile` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwDockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -74,16 +74,20 @@
 
 #copy the startRunJobs.sh script
 COPY startRunJobs.sh /root
 
 # copy the script to add a crontab entry
 COPY addCronTabEntry.sh /root
 
+# copy the script to add languages
+COPY lang.sh /root
+
 # copy the plantuml script
 COPY plantuml.sh /root
 
+
 # make the scripts executable
 RUN chmod +x /tmp/initdb.sh /tmp/update.sh /tmp/addSysopUser.sh /tmp/installExtensions.sh /root/addCronTabEntry.sh /root/startRunJobs.sh /root/plantuml.sh
 
 # restore the mediawiki initial database backup
 # can not do this before SQL server is up see https://docs.docker.com/compose/startup-order/
 # RUN /tmp/initdb.sh
```

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings.php` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings127.php` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings127.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings131.php` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings131.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings135.php` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings135.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings136.php` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings136.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings137.php` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings137.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings138.php` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings138.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings139.php` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwLocalSettings139.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki127.sql` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki127.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki131.sql` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki131.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki135.sql` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki135.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki136.sql` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki136.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki137.sql` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki137.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki138.sql` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki138.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki139.sql` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/mwWiki139.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/mwdocker/resources/templates/plantuml.sh` & `pymediawikidocker-0.9.7/mwdocker/resources/templates/plantuml.sh`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/tests/basetest.py` & `pymediawikidocker-0.9.7/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/tests/test_config.py` & `pymediawikidocker-0.9.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/tests/test_extensions.py` & `pymediawikidocker-0.9.7/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/tests/test_html_tables.py` & `pymediawikidocker-0.9.7/tests/test_html_tables.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/tests/test_install.py` & `pymediawikidocker-0.9.7/tests/test_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,22 +114,28 @@
                     'phpinfo.php',
                     'wiki.sql',
                     'composer.local.json',
                     'plantuml.sh'
                 ]:
                 fpath=f"{epath}/{fname}"
                 self.assertTrue(os.path.isfile(fpath))
+                
+    def newClusterApps(self):
+        self.removeFolderContent(self.docker_path)
+        mwCluster=self.getMwCluster(withGenerate=True)
+        mwCluster.down(forceRebuild=True)
+        mwCluster.start(forceRebuild=True)
+        apps=mwCluster.apps.values()
+        return mwCluster,apps
     
     def testInstallation(self):
         '''
         test the MediaWiki docker image installation
         '''
-        mwCluster=self.getMwCluster(withGenerate=True)
-        mwCluster.start(forceRebuild=True)
-        apps=mwCluster.apps.values()
+        mwCluster,apps=self.newClusterApps()
         self.assertEqual(len(mwCluster.config.versions),len(apps))
         for mwApp in apps:
             self.assertTrue(mwApp.dbContainer is not None)
             self.assertTrue(mwApp.mwContainer is not None)
             dbStatus=mwApp.checkDBConnection()
             self.assertTrue(dbStatus.ok,f"{mwApp.config.version}")
             userCountRecords=mwApp.sqlQuery("select count(*) from user;")
@@ -140,16 +146,15 @@
         
     def testPortBindingAccess(self):
         """
         https://github.com/WolfgangFahl/pymediawikidocker/issues/48
         
         refactor port binding access 
         """    
-        mwCluster=self.getMwCluster(withGenerate=False)
-        apps=mwCluster.apps.values()
+        mwCluster,apps=self.newClusterApps()
         debug=self.debug
         debug=True
         for mwApp in apps:
             config_json=mwApp.config.as_json()
             if debug:
                 print(config_json)
             self.assertTrue(mwApp.dbContainer is not None)
```

### Comparing `pymediawikidocker-0.9.6/.gitignore` & `pymediawikidocker-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/LICENSE` & `pymediawikidocker-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/README.md` & `pymediawikidocker-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/pyproject.toml` & `pymediawikidocker-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.6/PKG-INFO` & `pymediawikidocker-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediawikidocker
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python controlled (semantic) mediawiki docker application cluster installation
 Project-URL: Home, https://github.com/WolfgangFahl/pymediawikidocker
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/pymediawikidocker
 Project-URL: Source, https://github.com/WolfgangFahl/pymediawikidocker
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License: Apache-2.0
```

