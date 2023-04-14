# Comparing `tmp/django_mfa3-0.8.0-py3-none-any.whl.zip` & `tmp/django_mfa3-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20077 bytes, number of entries: 38
+Zip file size: 20116 bytes, number of entries: 38
 -rw-r--r--  2.0 unx        0 b- defN 21-Jun-20 23:08 mfa/__init__.py
 -rw-r--r--  2.0 unx      745 b- defN 22-Apr-15 10:49 mfa/admin.py
 -rw-r--r--  2.0 unx      219 b- defN 22-Apr-15 10:49 mfa/apps.py
 -rw-r--r--  2.0 unx       55 b- defN 21-Jun-29 15:42 mfa/decorators.py
--rw-r--r--  2.0 unx      740 b- defN 22-Apr-15 10:49 mfa/forms.py
+-rw-r--r--  2.0 unx      912 b- defN 23-Feb-27 18:53 mfa/forms.py
 -rw-r--r--  2.0 unx     1184 b- defN 22-Dec-08 10:24 mfa/mail.py
 -rw-r--r--  2.0 unx      515 b- defN 21-Jun-29 15:42 mfa/middleware.py
 -rw-r--r--  2.0 unx     2010 b- defN 22-Apr-15 10:49 mfa/mixins.py
 -rw-r--r--  2.0 unx      495 b- defN 21-Aug-25 19:20 mfa/models.py
 -rw-r--r--  2.0 unx      580 b- defN 22-Jun-24 12:45 mfa/settings.py
 -rw-r--r--  2.0 unx      503 b- defN 21-Jun-29 15:42 mfa/urls.py
 -rw-r--r--  2.0 unx     4143 b- defN 22-Dec-08 10:24 mfa/views.py
@@ -27,14 +27,14 @@
 -rw-r--r--  2.0 unx      559 b- defN 21-Aug-25 19:20 mfa/templates/mfa/auth_recovery.html
 -rw-r--r--  2.0 unx      515 b- defN 22-Dec-08 09:59 mfa/templates/mfa/create_FIDO2.html
 -rw-r--r--  2.0 unx      485 b- defN 21-Jul-02 10:40 mfa/templates/mfa/create_TOTP.html
 -rw-r--r--  2.0 unx      789 b- defN 21-Aug-25 19:20 mfa/templates/mfa/create_recovery.html
 -rw-r--r--  2.0 unx      145 b- defN 21-Jun-20 23:08 mfa/templates/mfa/mfakey_confirm_delete.html
 -rw-r--r--  2.0 unx      922 b- defN 21-Aug-25 19:20 mfa/templates/mfa/mfakey_list.html
 -rw-r--r--  2.0 unx        0 b- defN 21-Jul-05 07:02 mfa/templatetags/__init__.py
--rw-r--r--  2.0 unx      418 b- defN 21-Jul-02 10:40 mfa/templatetags/mfa.py
--rw-r--r--  2.0 unx     1072 b- defN 22-Dec-08 11:53 django_mfa3-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5496 b- defN 22-Dec-08 11:53 django_mfa3-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-08 11:53 django_mfa3-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-Dec-08 11:53 django_mfa3-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3060 b- defN 22-Dec-08 11:53 django_mfa3-0.8.0.dist-info/RECORD
-38 files, 34151 bytes uncompressed, 15187 bytes compressed:  55.5%
+-rw-r--r--  2.0 unx      357 b- defN 23-Feb-27 18:53 mfa/templatetags/mfa.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Mar-02 06:30 django_mfa3-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5509 b- defN 23-Mar-02 06:30 django_mfa3-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-02 06:30 django_mfa3-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Mar-02 06:30 django_mfa3-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3060 b- defN 23-Mar-02 06:30 django_mfa3-0.9.0.dist-info/RECORD
+38 files, 34275 bytes uncompressed, 15226 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -93,23 +93,23 @@
 
 Filename: mfa/templatetags/__init__.py
 Comment: 
 
 Filename: mfa/templatetags/mfa.py
 Comment: 
 
-Filename: django_mfa3-0.8.0.dist-info/LICENSE
+Filename: django_mfa3-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: django_mfa3-0.8.0.dist-info/METADATA
+Filename: django_mfa3-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: django_mfa3-0.8.0.dist-info/WHEEL
+Filename: django_mfa3-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: django_mfa3-0.8.0.dist-info/top_level.txt
+Filename: django_mfa3-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: django_mfa3-0.8.0.dist-info/RECORD
+Filename: django_mfa3-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mfa/forms.py

```diff
@@ -1,12 +1,12 @@
 from django import forms
 from django.utils.translation import gettext_lazy as _
 
 
-class MFAAuthForm(forms.Form):
+class MFABaseForm(forms.Form):
     code = forms.CharField(label=_('Authentication code'))
 
     def __init__(self, validate_code=None, **kwargs):
         self.validate_code = validate_code
         super().__init__(**kwargs)
 
     def clean(self):
@@ -16,9 +16,15 @@
             try:
                 cleaned_data['secret'] = self.validate_code(code)
             except ValueError as e:
                 raise forms.ValidationError(_('Validation failed')) from e
         return cleaned_data
 
 
-class MFACreateForm(MFAAuthForm):
+class MFAAuthForm(MFABaseForm):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.fields['code'].widget.attrs.update({'autofocus': True})
+
+
+class MFACreateForm(MFABaseForm):
     name = forms.CharField(label=_('Name'), max_length=32)
```

## mfa/templatetags/mfa.py

```diff
@@ -1,18 +1,14 @@
-from io import BytesIO
-
 import qrcode
 import qrcode.image.svg
 from django import template
 from django.utils.safestring import mark_safe
 
 register = template.Library()
 
 
 @register.filter(name='qrcode')
 def get_qrcode(url):
-    buf = BytesIO()
     img = qrcode.make(url, image_factory=qrcode.image.svg.SvgImage)
-    img.save(buf)
-    s = buf.getvalue().decode('utf-8')
+    s = img.to_string().decode('utf-8')
     i = s.find('<svg')
     return mark_safe(s[i:])
```

## Comparing `django_mfa3-0.8.0.dist-info/LICENSE` & `django_mfa3-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_mfa3-0.8.0.dist-info/METADATA` & `django_mfa3-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mfa3
-Version: 0.8.0
+Version: 0.9.0
 Summary: multi factor authentication for django
 Home-page: https://github.com/xi/django-mfa3
 Author: Tobias Bengfort
 Author-email: tobias.bengfort@posteo.de
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -12,18 +12,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyotp
-Requires-Dist: fido2 (>=1.0.0)
-Requires-Dist: qrcode
 Requires-Dist: django (>=2.2)
+Requires-Dist: fido2 (>=1.0.0)
+Requires-Dist: pyotp
+Requires-Dist: qrcode (<7.4,>=7.1)
 
 # django-mfa3
 
 An opinionated Django app that handles multi factor authentication (MFA) via
 FIDO2, TOTP, and recovery codes.
 
 ## Features
```

## Comparing `django_mfa3-0.8.0.dist-info/RECORD` & `django_mfa3-0.9.0.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mfa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mfa/admin.py,sha256=anbj_Imjm0nPhe_RGjgvAAZF1bC_nP98ReGCRKbW2qc,745
 mfa/apps.py,sha256=cPxdtq2aOdDVn1-Cm_DUmL_AfSUqK-zuiNirTuBbhBQ,219
 mfa/decorators.py,sha256=parNw11B767M2KVp17M9Z0RgftoQEsA6rxvrtB7il74,55
-mfa/forms.py,sha256=3XDOPVn9mnTQx7k8m-rSZsRAvsQiPvgCOCaRZ_U1oxw,740
+mfa/forms.py,sha256=yynFTfbGWTWBHWPaQhyHiHsbKQcsStUrOQ_H3ETtlUM,912
 mfa/mail.py,sha256=K-oSyuIRU8spEWB2G-3u9Pdj1Vo6lahj_11XgYTZDc4,1184
 mfa/middleware.py,sha256=H0ZXWENzE59f3scFHzXhn8T8oemB7uIVuCxbPmJuLEY,515
 mfa/mixins.py,sha256=GjIJcVdDaWajeBRTN-UqB0Qg-P3dSMSnJZSYUZd9oJ8,2010
 mfa/models.py,sha256=reI334RSgOGTHraLRYfJUyW91GMNnTZEXZQWJVH2iSI,495
 mfa/settings.py,sha256=9ornEq2HkawKaltY317UGnPaVuNmkaFFHRNMrcsuyAM,580
 mfa/urls.py,sha256=P10xCERbsifb89MYMtn-tBVxyenNYFMAR0_VTZc1WYk,503
 mfa/views.py,sha256=pzyTfGeZ-NE92xE1opaoDFuJ_K_u84UTlFqJlQkSWpI,4143
@@ -26,13 +26,13 @@
 mfa/templates/mfa/auth_recovery.html,sha256=MzSxJCRMur3z-FFKgfdsIqOmtoxUA2AfPLpLS3yMA64,559
 mfa/templates/mfa/create_FIDO2.html,sha256=77aDc--0zlHW-Oho8CsD-WhtVg26LmGJgN6tYD6c9_w,515
 mfa/templates/mfa/create_TOTP.html,sha256=YGPB7OpiNYPRJAY3aEKvWx3Hw1-JRAsnOsU7oX3-BSY,485
 mfa/templates/mfa/create_recovery.html,sha256=ajSSI6z92l7phcM06QkMGuOvz0UlK2a3AmBrgIxs3UA,789
 mfa/templates/mfa/mfakey_confirm_delete.html,sha256=-UbBPhGMm6_LzNmgAzKBMTYpdlDELP9JHWW3qW20FfA,145
 mfa/templates/mfa/mfakey_list.html,sha256=HxrEBqb6wD9KTS62W3M7wzIThV4SEgVwfc8PVoqQ1rw,922
 mfa/templatetags/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mfa/templatetags/mfa.py,sha256=xT3fQp9kYtgyGB4KGflDTkxYLaQlfbWMohWNJEHIljU,418
-django_mfa3-0.8.0.dist-info/LICENSE,sha256=EkquIKss4DZm4qkc_GjBTxvoWZBLC4T2mBkTaZgpSFI,1072
-django_mfa3-0.8.0.dist-info/METADATA,sha256=Wn_N0BtjiFLKvsCM0OUoB3NzpmYY81FlRrOobfG9lSg,5496
-django_mfa3-0.8.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-django_mfa3-0.8.0.dist-info/top_level.txt,sha256=ItdOgQwaWEFSLJh4ixZHTU0g2uIDY5v9VXtqHlSQckE,4
-django_mfa3-0.8.0.dist-info/RECORD,,
+mfa/templatetags/mfa.py,sha256=I6jDhPDk-lYj9y6oBQX7HaKgjv7pzoIJxxA2TQYXjVU,357
+django_mfa3-0.9.0.dist-info/LICENSE,sha256=EkquIKss4DZm4qkc_GjBTxvoWZBLC4T2mBkTaZgpSFI,1072
+django_mfa3-0.9.0.dist-info/METADATA,sha256=lkxJ3GrBLEJ6EqJS51f5S9Ifa0qMZXBcDit7BFmdXAo,5509
+django_mfa3-0.9.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+django_mfa3-0.9.0.dist-info/top_level.txt,sha256=ItdOgQwaWEFSLJh4ixZHTU0g2uIDY5v9VXtqHlSQckE,4
+django_mfa3-0.9.0.dist-info/RECORD,,
```

