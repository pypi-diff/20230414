# Comparing `tmp/django-forbid-0.0.4.tar.gz` & `tmp/django-forbid-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.0.4.tar", last modified: Sun Apr  9 17:40:45 2023, max compression
+gzip compressed data, was "django-forbid-0.0.5.tar", last modified: Fri Apr 14 15:00:56 2023, max compression
```

## Comparing `django-forbid-0.0.4.tar` & `django-forbid-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:40:45.924976 django-forbid-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 17:40:37.000000 django-forbid-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-09 17:40:45.924976 django-forbid-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-09 17:40:37.000000 django-forbid-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 17:40:37.000000 django-forbid-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-09 17:40:45.924976 django-forbid-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-09 17:40:37.000000 django-forbid-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:40:45.920976 django-forbid-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:40:45.920976 django-forbid-0.0.4/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/access.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:40:45.920976 django-forbid-0.0.4/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:56.387156 django-forbid-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 15:00:45.000000 django-forbid-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-14 15:00:56.387156 django-forbid-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-14 15:00:45.000000 django-forbid-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 15:00:45.000000 django-forbid-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 15:00:56.387156 django-forbid-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 15:00:45.000000 django-forbid-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:56.383156 django-forbid-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:56.387156 django-forbid-0.0.5/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:56.387156 django-forbid-0.0.5/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.0.4/LICENSE` & `django-forbid-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.4/PKG-INFO` & `django-forbid-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.0.4
+Version: 0.0.5
 Summary: Django app for forbidding access to some countries
 Home-page: https://github.com/pysnippet/django-forbid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Keywords: python,django,forbid,django-forbid
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: win32
-Classifier: Framework :: Django
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.1
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -25,16 +32,16 @@
 License-File: LICENSE
 
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 Django app for forbidding access to some countries.
 
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
-[![Django](https://img.shields.io/badge/django-%3E%3D2.1-blue.svg)](https://pypi.org/project/django-forbid/)
-[![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg)](https://pypi.org/project/django-forbid/)
+[![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
+[![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
 [![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
 
 ## Install
 
 ```shell
 python -m pip install django-forbid
@@ -64,59 +71,48 @@
 the GeoLite2 database file. You should [download](https://dev.maxmind.com/geoip/geoip2/geolite2/) the database and
 follow the Django [documentation](https://docs.djangoproject.com/en/2.1/ref/contrib/gis/geoip2/#settings) for proper
 configuration.
 
 ## Usage
 
 After connecting the Django Forbid to your project, you can define the set of desired zones to be forbidden or allowed.
-And there are four setting variables for describing any of your specific needs:
-
-- `WHITELIST_COUNTRIES` and `WHITELIST_TERRITORIES` - Correspondingly, the list of countries and territories that are
-  allowed to access the site.
-- `FORBIDDEN_COUNTRIES` and `FORBIDDEN_TERRITORIES` - Correspondingly, the list of countries and territories that are
-  forbidden to access the site.
-
-Forbidden countries and territories have a higher priority than allowed ones. If a country or territory is in both
-lists, then the user will be forbidden. And if the user is not allowed to access the resource, it will be redirected to
-the `FORBIDDEN_URL` page if the variable is set in your Django project's settings.
-
-```python
-# Only US, GB, and EU countries are allowed to access the site.
-WHITELIST_COUNTRIES = ['US', 'GB']
-WHITELIST_TERRITORIES = ['EU']
-```
+All you need is to set the `DJANGO_FORBID` variable in your project's settings. It should be a dictionary with the
+following keys:
 
-Needs can be different, so you can use any combination of these variables to describe your special needs.
+- `COUNTRIES` - list of countries to permit or forbid access to
+- `TERRITORIES` - list of territories to permit or forbid access to
+- `OPTIONS` - a dictionary for additional settings
+  - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
+  - `PERIOD` - time in seconds to check for access again, 0 means on each request
+  - `VPN` - use VPN detection and forbid access to VPN users
+  - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
+      - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
+      - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
 
 ```python
-# Forbid access for African countries and Russia, Belarus, and North Korea.
-FORBIDDEN_COUNTRIES = ['RU', 'BY', 'KP']
-FORBIDDEN_TERRITORIES = ['AF']
+DJANGO_FORBID = {
+    'COUNTRIES': ['US', 'GB'],
+    'TERRITORIES': ['EU'],
+    'OPTIONS': {
+        'ACTION': 'PERMIT',
+        'PERIOD': 300,
+        'VPN': True,
+        'URL': {
+            'FORBIDDEN_LOC': 'forbidden_country',
+            'FORBIDDEN_VPN': 'forbidden_network',
+        },
+    },
+}
 ```
 
 The available ISO 3166 alpha-2 country codes are listed in [here](https://www.iban.com/country-codes). And the available
 ISO continent codes are: `AF` - Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` -
 Oceania and `SA` - South America.
 
-### Check access on timeout
-
-Without additional configuration, the middleware will check the user's access on every request. This can slow down the
-site. To avoid this, you can use the `FORBID_TIMEOUT` variable to set the cache timeout in seconds. When the timeout
-expires, the middleware will check the user's access again.
-
-```python
-# Check the user's access every 10 minutes.
-FORBID_TIMEOUT = 60 * 10
-```
-
-### Detect usage of a VPN
-
-If you want to detect the usage of a VPN, you can use the `FORBID_VPN` variable. When this variable is set to `True`,
-the middleware will check if the user's timezone matches the timezone the IP address belongs to. If the timezones do not
-match, the user will be considered in the usage of a VPN and forbidden to access the site.
+_None of the settings are required. If you don't specify any settings, the middleware will not do anything._
 
 ## Contribute
 
 Any contribution is welcome. If you have any ideas or suggestions, feel free to open an issue or a pull request. And
 don't forget to add tests for your changes.
 
 ## License
```

### Comparing `django-forbid-0.0.4/README.md` & `django-forbid-0.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 Django app for forbidding access to some countries.
 
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
-[![Django](https://img.shields.io/badge/django-%3E%3D2.1-blue.svg)](https://pypi.org/project/django-forbid/)
-[![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg)](https://pypi.org/project/django-forbid/)
+[![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
+[![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
 [![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
 
 ## Install
 
 ```shell
 python -m pip install django-forbid
@@ -38,59 +38,48 @@
 the GeoLite2 database file. You should [download](https://dev.maxmind.com/geoip/geoip2/geolite2/) the database and
 follow the Django [documentation](https://docs.djangoproject.com/en/2.1/ref/contrib/gis/geoip2/#settings) for proper
 configuration.
 
 ## Usage
 
 After connecting the Django Forbid to your project, you can define the set of desired zones to be forbidden or allowed.
-And there are four setting variables for describing any of your specific needs:
+All you need is to set the `DJANGO_FORBID` variable in your project's settings. It should be a dictionary with the
+following keys:
 
-- `WHITELIST_COUNTRIES` and `WHITELIST_TERRITORIES` - Correspondingly, the list of countries and territories that are
-  allowed to access the site.
-- `FORBIDDEN_COUNTRIES` and `FORBIDDEN_TERRITORIES` - Correspondingly, the list of countries and territories that are
-  forbidden to access the site.
-
-Forbidden countries and territories have a higher priority than allowed ones. If a country or territory is in both
-lists, then the user will be forbidden. And if the user is not allowed to access the resource, it will be redirected to
-the `FORBIDDEN_URL` page if the variable is set in your Django project's settings.
+- `COUNTRIES` - list of countries to permit or forbid access to
+- `TERRITORIES` - list of territories to permit or forbid access to
+- `OPTIONS` - a dictionary for additional settings
+  - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
+  - `PERIOD` - time in seconds to check for access again, 0 means on each request
+  - `VPN` - use VPN detection and forbid access to VPN users
+  - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
+      - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
+      - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
 
 ```python
-# Only US, GB, and EU countries are allowed to access the site.
-WHITELIST_COUNTRIES = ['US', 'GB']
-WHITELIST_TERRITORIES = ['EU']
-```
-
-Needs can be different, so you can use any combination of these variables to describe your special needs.
-
-```python
-# Forbid access for African countries and Russia, Belarus, and North Korea.
-FORBIDDEN_COUNTRIES = ['RU', 'BY', 'KP']
-FORBIDDEN_TERRITORIES = ['AF']
+DJANGO_FORBID = {
+    'COUNTRIES': ['US', 'GB'],
+    'TERRITORIES': ['EU'],
+    'OPTIONS': {
+        'ACTION': 'PERMIT',
+        'PERIOD': 300,
+        'VPN': True,
+        'URL': {
+            'FORBIDDEN_LOC': 'forbidden_country',
+            'FORBIDDEN_VPN': 'forbidden_network',
+        },
+    },
+}
 ```
 
 The available ISO 3166 alpha-2 country codes are listed in [here](https://www.iban.com/country-codes). And the available
 ISO continent codes are: `AF` - Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` -
 Oceania and `SA` - South America.
 
-### Check access on timeout
-
-Without additional configuration, the middleware will check the user's access on every request. This can slow down the
-site. To avoid this, you can use the `FORBID_TIMEOUT` variable to set the cache timeout in seconds. When the timeout
-expires, the middleware will check the user's access again.
-
-```python
-# Check the user's access every 10 minutes.
-FORBID_TIMEOUT = 60 * 10
-```
-
-### Detect usage of a VPN
-
-If you want to detect the usage of a VPN, you can use the `FORBID_VPN` variable. When this variable is set to `True`,
-the middleware will check if the user's timezone matches the timezone the IP address belongs to. If the timezones do not
-match, the user will be considered in the usage of a VPN and forbidden to access the site.
+_None of the settings are required. If you don't specify any settings, the middleware will not do anything._
 
 ## Contribute
 
 Any contribution is welcome. If you have any ideas or suggestions, feel free to open an issue or a pull request. And
 don't forget to add tests for your changes.
 
 ## License
```

### Comparing `django-forbid-0.0.4/setup.cfg` & `django-forbid-0.0.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,23 @@
 	django
 	forbid
 	django-forbid
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
-	Framework :: Django
 	Operating System :: OS Independent
+	Framework :: Django
+	Framework :: Django :: 2.1
+	Framework :: Django :: 2.2
+	Framework :: Django :: 3.1
+	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
+	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: MIT License
```

### Comparing `django-forbid-0.0.4/src/django_forbid/access.py` & `django-forbid-0.0.5/src/django_forbid/access.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from django.conf import settings
 from django.contrib.gis.geoip2 import GeoIP2
 from geoip2.errors import AddressNotFoundError
 
+from .config import Settings
+
 
 class Rule:
     # Key in the geoip2 city object.
     # Subclasses should override this.
     key = None
 
     def __init__(self, code):
@@ -22,78 +24,80 @@
 
 
 class ContinentRule(Rule):
     key = "continent_code"
 
 
 class Access:
-    # Variables in the settings module.
-    # Subclasses should override this.
-    countries = None
-    territories = None
+    countries = "COUNTRIES"
+    territories = "TERRITORIES"
 
     # Hold the instance of GeoIP2.
     geoip = GeoIP2()
 
     def __init__(self):
         self.rules = []
 
-        for country in getattr(settings, self.countries, []):
-            self.rules.append(CountryRule(country.upper()))
-
-        for territory in getattr(settings, self.territories, []):
-            self.rules.append(ContinentRule(territory.upper()))
+        if Settings.has(self.countries):
+            for country in Settings.get(self.countries):
+                self.rules.append(CountryRule(country.upper()))
+
+        if Settings.has(self.territories):
+            for territory in Settings.get(self.territories):
+                self.rules.append(ContinentRule(territory.upper()))
 
     def accessible(self, city):
         """Checks if the IP address is in the white zone."""
         return any(map(lambda rule: rule(city), self.rules))
 
     def grants(self, city):
         """Checks if the IP address is permitted."""
         raise NotImplementedError
 
 
 class PermitAccess(Access):
-    countries = "WHITELIST_COUNTRIES"
-    territories = "WHITELIST_TERRITORIES"
-
     def grants(self, city):
         """Checks if the IP address is permitted."""
         return not self.rules or self.accessible(city)
 
 
 class ForbidAccess(Access):
-    countries = "FORBIDDEN_COUNTRIES"
-    territories = "FORBIDDEN_TERRITORIES"
-
     def grants(self, city):
         """Checks if the IP address is forbidden."""
         return not self.rules or not self.accessible(city)
 
 
+class Factory:
+    """Creates an instance of the Access class."""
+
+    FORBID = ForbidAccess
+    PERMIT = PermitAccess
+
+    @classmethod
+    def create_access(cls, action):
+        return getattr(cls, action)()
+
+
 def grants_access(request, ip_address):
     """Checks if the IP address is in the white zone."""
     try:
         city = Access.geoip.city(ip_address)
 
         # Saves the timezone in the session for
         # comparing it with the timezone in the
         # POST request sent from user's browser
         # to detect if the user is using VPN.
         timezone = city.get("time_zone")
         request.session["tz"] = timezone
 
-        # First, checks if the IP address is not
-        # forbidden. If it is, False is returned
-        # otherwise, checks if the IP address is
-        # permitted.
-        if ForbidAccess().grants(city):
-            return PermitAccess().grants(city)
-        return False
+        # Creates an instance of the Access class
+        # and checks if the IP address is granted.
+        action = Settings.get("OPTIONS.ACTION", "FORBID")
+        return Factory.create_access(action).grants(city)
     except (AddressNotFoundError, Exception):
         # This happens when the IP address is not
         # in  the  GeoIP2 database. Usually, this
         # happens when the IP address is a local.
         return not any([
-            ForbidAccess().rules,
-            PermitAccess().rules,
+            Settings.has(Access.countries),
+            Settings.has(Access.territories),
         ]) or getattr(settings, "DEBUG", False)
```

### Comparing `django-forbid-0.0.4/src/django_forbid/detect.py` & `django-forbid-0.0.5/src/django_forbid/detect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 import json
 import re
 
-from django.conf import settings
 from django.http import HttpResponse
 from django.http import HttpResponseForbidden
 from django.shortcuts import redirect
 from django.shortcuts import render
 
+from .config import Settings
+
 
 def detect_vpn(get_response, request):
     response_attributes = ("content", "charset", "status", "reason")
 
     def erase_response_attributes():
         for attr in response_attributes:
             request.session.pop(attr)
 
     if any([
         # The session key is checked to avoid
         # redirect loops in development mode.
         not request.session.has_key("tz"),
-        # Checks if FORBID_VPN is False or not set.
-        not getattr(settings, "FORBID_VPN", False),
+        # Checks if VPN is False or not set.
+        not Settings.get("OPTIONS.VPN", False),
         # Checks if the request is an AJAX request.
         not re.search(
             r"\w+\/(?:html|xhtml\+xml|xml)",
             request.META.get("HTTP_ACCEPT"),
         ),
     ]):
         return get_response(request)
 
     if all(map(request.session.has_key, ("tz", *response_attributes))):
         # Handles if the user's timezone differs from the
         # one determined by GeoIP API. If so, VPN is used.
         if request.POST.get("timezone", "N/A") != request.session.get("tz"):
             erase_response_attributes()
-            if hasattr(settings, "FORBIDDEN_URL"):
-                return redirect(settings.FORBIDDEN_URL)
+            # Redirects to the FORBIDDEN_VPN URL if set.
+            if Settings.has("OPTIONS.URL.FORBIDDEN_VPN"):
+                return redirect(Settings.get("OPTIONS.URL.FORBIDDEN_VPN"))
             return HttpResponseForbidden()
 
         # Restores the response from the session.
         response = HttpResponse(**{attr: request.session.get(attr) for attr in response_attributes})
         if hasattr(response, "headers"):
             response.headers = json.loads(request.session.get("headers"))
         erase_response_attributes()
         return response
 
     # Gets the response and saves attributes in the session to restore it later.
     response = get_response(request)
     if hasattr(response, "headers"):
-        # In older versions of Django, HttpResponse does not have headers attribute.
+        # In older versions of Django, HttpResponse does not have headers.
         request.session["headers"] = json.dumps(dict(response.headers))
     request.session["content"] = response.content.decode(response.charset)
     request.session["charset"] = response.charset
     request.session["status"] = response.status_code
     request.session["reason"] = response.reason_phrase
 
     return render(request, "timezone.html", status=302)
```

### Comparing `django-forbid-0.0.4/src/django_forbid/middleware.py` & `django-forbid-0.0.5/src/django_forbid/middleware.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from datetime import datetime
 
-from django.conf import settings
 from django.http import HttpResponseForbidden
 from django.shortcuts import redirect
 from django.utils.timezone import utc
 
 from .access import grants_access
+from .config import Settings
 from .detect import detect_vpn
 
 
 class ForbidMiddleware:
     """Middleware to forbid access to the site."""
 
     def __init__(self, get_response):
         self.get_response = get_response
 
     def __call__(self, request):
         address = request.META.get("REMOTE_ADDR")
         address = request.META.get("HTTP_X_FORWARDED_FOR", address)
 
-        # Checks if the timeout variable is set and the user has been granted access.
-        if hasattr(settings, "FORBID_TIMEOUT") and request.session.has_key("ACCESS"):
+        # Checks if the PERIOD attr is set and the user has been granted access.
+        if Settings.has("OPTIONS.PERIOD") and request.session.has_key("ACCESS"):
             acss = datetime.utcnow().replace(tzinfo=utc).timestamp()
 
             # Checks if access is not timed out yet.
-            if acss - request.session.get("ACCESS") < settings.FORBID_TIMEOUT:
+            if acss - request.session.get("ACCESS") < Settings.get("OPTIONS.PERIOD"):
                 return detect_vpn(self.get_response, request)
 
         # Checks if access is granted when timeout is reached.
         if grants_access(request, address.split(",")[0].strip()):
             acss = datetime.utcnow().replace(tzinfo=utc)
             request.session["ACCESS"] = acss.timestamp()
             return detect_vpn(self.get_response, request)
 
-        # Redirects to forbidden page if URL is set.
-        if hasattr(settings, "FORBIDDEN_URL"):
-            return redirect(settings.FORBIDDEN_URL)
+        # Redirects to the FORBIDDEN_LOC URL if set.
+        if Settings.has("OPTIONS.URL.FORBIDDEN_LOC"):
+            return redirect(Settings.get("OPTIONS.URL.FORBIDDEN_LOC"))
 
         return HttpResponseForbidden()
```

### Comparing `django-forbid-0.0.4/src/django_forbid.egg-info/PKG-INFO` & `django-forbid-0.0.5/src/django_forbid.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.0.4
+Version: 0.0.5
 Summary: Django app for forbidding access to some countries
 Home-page: https://github.com/pysnippet/django-forbid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Keywords: python,django,forbid,django-forbid
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: win32
-Classifier: Framework :: Django
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.1
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -25,16 +32,16 @@
 License-File: LICENSE
 
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 Django app for forbidding access to some countries.
 
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
-[![Django](https://img.shields.io/badge/django-%3E%3D2.1-blue.svg)](https://pypi.org/project/django-forbid/)
-[![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg)](https://pypi.org/project/django-forbid/)
+[![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
+[![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
 [![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
 
 ## Install
 
 ```shell
 python -m pip install django-forbid
@@ -64,59 +71,48 @@
 the GeoLite2 database file. You should [download](https://dev.maxmind.com/geoip/geoip2/geolite2/) the database and
 follow the Django [documentation](https://docs.djangoproject.com/en/2.1/ref/contrib/gis/geoip2/#settings) for proper
 configuration.
 
 ## Usage
 
 After connecting the Django Forbid to your project, you can define the set of desired zones to be forbidden or allowed.
-And there are four setting variables for describing any of your specific needs:
-
-- `WHITELIST_COUNTRIES` and `WHITELIST_TERRITORIES` - Correspondingly, the list of countries and territories that are
-  allowed to access the site.
-- `FORBIDDEN_COUNTRIES` and `FORBIDDEN_TERRITORIES` - Correspondingly, the list of countries and territories that are
-  forbidden to access the site.
-
-Forbidden countries and territories have a higher priority than allowed ones. If a country or territory is in both
-lists, then the user will be forbidden. And if the user is not allowed to access the resource, it will be redirected to
-the `FORBIDDEN_URL` page if the variable is set in your Django project's settings.
-
-```python
-# Only US, GB, and EU countries are allowed to access the site.
-WHITELIST_COUNTRIES = ['US', 'GB']
-WHITELIST_TERRITORIES = ['EU']
-```
+All you need is to set the `DJANGO_FORBID` variable in your project's settings. It should be a dictionary with the
+following keys:
 
-Needs can be different, so you can use any combination of these variables to describe your special needs.
+- `COUNTRIES` - list of countries to permit or forbid access to
+- `TERRITORIES` - list of territories to permit or forbid access to
+- `OPTIONS` - a dictionary for additional settings
+  - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
+  - `PERIOD` - time in seconds to check for access again, 0 means on each request
+  - `VPN` - use VPN detection and forbid access to VPN users
+  - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
+      - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
+      - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
 
 ```python
-# Forbid access for African countries and Russia, Belarus, and North Korea.
-FORBIDDEN_COUNTRIES = ['RU', 'BY', 'KP']
-FORBIDDEN_TERRITORIES = ['AF']
+DJANGO_FORBID = {
+    'COUNTRIES': ['US', 'GB'],
+    'TERRITORIES': ['EU'],
+    'OPTIONS': {
+        'ACTION': 'PERMIT',
+        'PERIOD': 300,
+        'VPN': True,
+        'URL': {
+            'FORBIDDEN_LOC': 'forbidden_country',
+            'FORBIDDEN_VPN': 'forbidden_network',
+        },
+    },
+}
 ```
 
 The available ISO 3166 alpha-2 country codes are listed in [here](https://www.iban.com/country-codes). And the available
 ISO continent codes are: `AF` - Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` -
 Oceania and `SA` - South America.
 
-### Check access on timeout
-
-Without additional configuration, the middleware will check the user's access on every request. This can slow down the
-site. To avoid this, you can use the `FORBID_TIMEOUT` variable to set the cache timeout in seconds. When the timeout
-expires, the middleware will check the user's access again.
-
-```python
-# Check the user's access every 10 minutes.
-FORBID_TIMEOUT = 60 * 10
-```
-
-### Detect usage of a VPN
-
-If you want to detect the usage of a VPN, you can use the `FORBID_VPN` variable. When this variable is set to `True`,
-the middleware will check if the user's timezone matches the timezone the IP address belongs to. If the timezones do not
-match, the user will be considered in the usage of a VPN and forbidden to access the site.
+_None of the settings are required. If you don't specify any settings, the middleware will not do anything._
 
 ## Contribute
 
 Any contribution is welcome. If you have any ideas or suggestions, feel free to open an issue or a pull request. And
 don't forget to add tests for your changes.
 
 ## License
```

