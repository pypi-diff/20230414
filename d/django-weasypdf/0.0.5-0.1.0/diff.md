# Comparing `tmp/django_weasypdf-0.0.5-py2.py3-none-any.whl.zip` & `tmp/django_weasypdf-0.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 35235 bytes, number of entries: 22
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-14 07:44 pdf/__init__.py
+Zip file size: 35263 bytes, number of entries: 22
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-14 07:59 pdf/__init__.py
 -rw-r--r--  2.0 unx      122 b- defN 19-Dec-13 18:03 pdf/apps.py
 -rw-r--r--  2.0 unx    12626 b- defN 23-Apr-14 07:44 pdf/plot.py
 -rw-r--r--  2.0 unx      319 b- defN 19-Dec-13 18:03 pdf/urls.py
 -rw-r--r--  2.0 unx     5551 b- defN 20-Apr-29 22:22 pdf/utils.py
 -rw-r--r--  2.0 unx     6008 b- defN 23-Apr-14 07:44 pdf/views.py
 -rw-r--r--  2.0 unx        0 b- defN 19-Dec-13 18:03 pdf/management/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 19-Dec-13 18:03 pdf/management/commands/__init__.py
@@ -13,12 +13,12 @@
 -rw-r--r--  2.0 unx      707 b- defN 19-Dec-14 09:39 pdf/templates/pdf/base.html
 -rw-r--r--  2.0 unx      707 b- defN 19-Dec-14 09:39 pdf/templates/pdf/base_nomargins.html
 -rw-r--r--  2.0 unx      536 b- defN 19-Dec-13 18:03 pdf/templates/pdf/footer.html
 -rw-r--r--  2.0 unx      805 b- defN 19-Dec-14 00:41 pdf/templates/pdf/header.html
 -rw-r--r--  2.0 unx      890 b- defN 23-Apr-14 07:44 pdf/templates/pdf/styles.css
 -rw-r--r--  2.0 unx       26 b- defN 19-Dec-13 18:03 pdf/templates/pdf/pages/test.css
 -rw-r--r--  2.0 unx      476 b- defN 23-Apr-14 07:44 pdf/templates/pdf/pages/test.html
--rw-r--r--  2.0 unx    15202 b- defN 23-Apr-14 07:56 django_weasypdf-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 07:56 django_weasypdf-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-14 07:56 django_weasypdf-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1787 b- defN 23-Apr-14 07:56 django_weasypdf-0.0.5.dist-info/RECORD
-22 files, 74492 bytes uncompressed, 32329 bytes compressed:  56.6%
+-rw-r--r--  2.0 unx    15296 b- defN 23-Apr-14 08:00 django_weasypdf-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 08:00 django_weasypdf-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-14 08:00 django_weasypdf-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1787 b- defN 23-Apr-14 08:00 django_weasypdf-0.1.0.dist-info/RECORD
+22 files, 74586 bytes uncompressed, 32357 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: pdf/templates/pdf/pages/test.css
 Comment: 
 
 Filename: pdf/templates/pdf/pages/test.html
 Comment: 
 
-Filename: django_weasypdf-0.0.5.dist-info/METADATA
+Filename: django_weasypdf-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: django_weasypdf-0.0.5.dist-info/WHEEL
+Filename: django_weasypdf-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: django_weasypdf-0.0.5.dist-info/top_level.txt
+Filename: django_weasypdf-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: django_weasypdf-0.0.5.dist-info/RECORD
+Filename: django_weasypdf-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pdf/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.5'
+__version__ = '0.1.0'
```

## Comparing `django_weasypdf-0.0.5.dist-info/METADATA` & `django_weasypdf-0.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-weasypdf
-Version: 0.0.5
+Version: 0.1.0
 Summary: A Django class-based view helper to generate PDF with WeasyPrint
 Home-page: http://github.com/morlandi/django-pdf
 Author: Mario Orlandi
 Author-email: morlandi@brainstorm.it
 License: MIT
 
 
@@ -26,16 +26,23 @@
 Installation
 ------------
 
 Install the package by running:
 
 .. code:: bash
 
+    pip install django-weasypdf
+
+or:
+
+.. code:: bash
+
     pip install git+https://github.com/morlandi/django-pdf
 
+
 You will probably build you own app in the project to provide derived Views
 and custom templates; for example:
 
 .. code:: bash
 
     python manage.py startapp reports
 
@@ -539,16 +546,17 @@
 
 
 
 
 History
 =======
 
-v.....
+v0.1.0
 ------
+* Publish on Pypi as "django-weasypdf"
 * Support for 'line', 'bar', 'horizontalBar', 'pie', 'line', 'doughnut' plots
 
 v0.0.5
 ------
 * Support for plot added (only "line" chart type, at the moment; requires matplotlib)
 * Customization examples added to readme
```

## Comparing `django_weasypdf-0.0.5.dist-info/RECORD` & `django_weasypdf-0.1.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pdf/__init__.py,sha256=eB5tEg_BNHHsJgQexgmpZJr4c2VbfooQZMXAWuDHoIg,22
+pdf/__init__.py,sha256=IMjkMO3twhQzluVTo8Z6rE7Eg-9U79_LGKMcsWLKBkY,22
 pdf/apps.py,sha256=F5lKyM7EMjpDGNUkcXbvHtdKEVCZpqgu2U7ofaQOM3I,122
 pdf/plot.py,sha256=B1PsWQMBJt0QSucb3uFVDM3sviqBl6ui9O3mT7w9-kc,12626
 pdf/urls.py,sha256=lTpY-szxxoNia9x5fWH-QwcSzkV7lL-jWTFwmOTNAR8,319
 pdf/utils.py,sha256=_MxAL4oybgrxDERgzG6YAAWctqhE8ao5lyuRU6RkqOE,5551
 pdf/views.py,sha256=hG_6Sy-XpzxbSZ8QbZvzoajE-ZGB7a3bMAN2GiQpmJ4,6008
 pdf/management/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pdf/management/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -12,11 +12,11 @@
 pdf/templates/pdf/base.html,sha256=xJvIafKRl1h0ApHCwV7hOlDxSEoHY47LDL4M31r14cw,707
 pdf/templates/pdf/base_nomargins.html,sha256=_3fWaIlg6exEZReQ3fkkf_ifnxSUL_NjIldlXZoswDk,707
 pdf/templates/pdf/footer.html,sha256=mwLlOzuLY1Jo8f5iagzHHSZgKb8mtkGCrGBNutm-d5A,536
 pdf/templates/pdf/header.html,sha256=lfWnprehx3u87BUMWxT-Wicp_NivPcddlqCcHxN15do,805
 pdf/templates/pdf/styles.css,sha256=Q56icgKW0EDZfgrMTY0EqUoUtaQrHxNvrB1KhgDkMuk,890
 pdf/templates/pdf/pages/test.css,sha256=15R5nH8khpS05pw2uvYP73CH_aUSiU1tHueANH71kPI,26
 pdf/templates/pdf/pages/test.html,sha256=xf9DxkhjB9RariWoMb9cGil78wumOJDcE82i4YPbWvs,476
-django_weasypdf-0.0.5.dist-info/METADATA,sha256=yY-2ANBNDMOMvBCEe-BFUNYtVW4RjfgAmoKRYrnfAxI,15202
-django_weasypdf-0.0.5.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-django_weasypdf-0.0.5.dist-info/top_level.txt,sha256=wNR1kCNE3AcoLhlsahfUmQbycA3kKB-9os2LfjS2VWk,4
-django_weasypdf-0.0.5.dist-info/RECORD,,
+django_weasypdf-0.1.0.dist-info/METADATA,sha256=qQHvU9EkfhrDI3HJEms_HOrzANmu7XKXJWtJsWSf15s,15296
+django_weasypdf-0.1.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+django_weasypdf-0.1.0.dist-info/top_level.txt,sha256=wNR1kCNE3AcoLhlsahfUmQbycA3kKB-9os2LfjS2VWk,4
+django_weasypdf-0.1.0.dist-info/RECORD,,
```

