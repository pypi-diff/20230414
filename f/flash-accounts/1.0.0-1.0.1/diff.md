# Comparing `tmp/flash-accounts-1.0.0.tar.gz` & `tmp/flash-accounts-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flash-accounts-1.0.0.tar", last modified: Thu Apr  6 13:05:07 2023, max compression
+gzip compressed data, was "flash-accounts-1.0.1.tar", last modified: Fri Apr 14 11:02:47 2023, max compression
```

## Comparing `flash-accounts-1.0.0.tar` & `flash-accounts-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 13:05:07.620400 flash-accounts-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-04-04 13:45:09.000000 flash-accounts-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       86 2023-04-06 12:54:49.000000 flash-accounts-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      779 2023-04-06 13:05:07.619405 flash-accounts-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-06 13:03:37.000000 flash-accounts-1.0.0/PyPIREADME.md
--rw-rw-rw-   0        0        0    10724 2023-04-06 12:52:12.000000 flash-accounts-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 13:05:07.581353 flash-accounts-1.0.0/flash_accounts/
--rw-rw-rw-   0        0        0      215 2023-04-06 12:54:49.000000 flash-accounts-1.0.0/flash_accounts/__init__.py
--rw-rw-rw-   0        0        0       66 2023-04-04 09:09:54.000000 flash-accounts-1.0.0/flash_accounts/admin.py
--rw-rw-rw-   0        0        0      165 2023-04-04 09:09:54.000000 flash-accounts-1.0.0/flash_accounts/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:05:07.612303 flash-accounts-1.0.0/flash_accounts/migrations/
--rw-rw-rw-   0        0        0     2489 2023-04-04 10:41:21.000000 flash-accounts-1.0.0/flash_accounts/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-04-04 09:09:54.000000 flash-accounts-1.0.0/flash_accounts/migrations/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-04-04 10:41:21.000000 flash-accounts-1.0.0/flash_accounts/models.py
--rw-rw-rw-   0        0        0     1965 2023-04-04 13:03:33.000000 flash-accounts-1.0.0/flash_accounts/serializers.py
--rw-rw-rw-   0        0        0     2512 2023-04-04 13:43:01.000000 flash-accounts-1.0.0/flash_accounts/services.py
--rw-rw-rw-   0        0        0     3451 2023-04-04 13:03:33.000000 flash-accounts-1.0.0/flash_accounts/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:05:07.564308 flash-accounts-1.0.0/flash_accounts/templates/
-drwxrwxrwx   0        0        0        0 2023-04-06 13:05:07.618402 flash-accounts-1.0.0/flash_accounts/templates/flash_accounts/
--rw-rw-rw-   0        0        0     2088 2023-04-04 13:03:33.000000 flash-accounts-1.0.0/flash_accounts/templates/flash_accounts/activate.html
--rw-rw-rw-   0        0        0      174 2023-04-04 13:03:33.000000 flash-accounts-1.0.0/flash_accounts/templates/flash_accounts/activate.txt
--rw-rw-rw-   0        0        0     2119 2023-04-04 13:03:33.000000 flash-accounts-1.0.0/flash_accounts/templates/flash_accounts/password_reset.html
--rw-rw-rw-   0        0        0      187 2023-04-04 13:03:33.000000 flash-accounts-1.0.0/flash_accounts/templates/flash_accounts/password_reset.txt
--rw-rw-rw-   0        0        0    20264 2023-04-04 13:38:16.000000 flash-accounts-1.0.0/flash_accounts/tests.py
--rw-rw-rw-   0        0        0      901 2023-04-04 15:44:42.000000 flash-accounts-1.0.0/flash_accounts/urls.py
--rw-rw-rw-   0        0        0     4163 2023-04-04 13:42:37.000000 flash-accounts-1.0.0/flash_accounts/views.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:05:07.608306 flash-accounts-1.0.0/flash_accounts.egg-info/
--rw-rw-rw-   0        0        0      779 2023-04-06 13:05:07.000000 flash-accounts-1.0.0/flash_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      807 2023-04-06 13:05:07.000000 flash-accounts-1.0.0/flash_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 13:05:07.000000 flash-accounts-1.0.0/flash_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-06 13:05:07.000000 flash-accounts-1.0.0/flash_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-06 13:05:07.000000 flash-accounts-1.0.0/flash_accounts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1020 2023-04-06 12:54:49.000000 flash-accounts-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 13:05:07.620400 flash-accounts-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 11:02:47.649372 flash-accounts-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-04 13:45:09.000000 flash-accounts-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       86 2023-04-06 12:54:49.000000 flash-accounts-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      779 2023-04-14 11:02:47.648340 flash-accounts-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-06 13:03:37.000000 flash-accounts-1.0.1/PyPIREADME.md
+-rw-rw-rw-   0        0        0    10767 2023-04-14 10:59:44.000000 flash-accounts-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 11:02:47.623337 flash-accounts-1.0.1/flash_accounts/
+-rw-rw-rw-   0        0        0      215 2023-04-14 10:59:44.000000 flash-accounts-1.0.1/flash_accounts/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-04 09:09:54.000000 flash-accounts-1.0.1/flash_accounts/admin.py
+-rw-rw-rw-   0        0        0      165 2023-04-04 09:09:54.000000 flash-accounts-1.0.1/flash_accounts/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:02:47.642348 flash-accounts-1.0.1/flash_accounts/migrations/
+-rw-rw-rw-   0        0        0     2489 2023-04-04 10:41:21.000000 flash-accounts-1.0.1/flash_accounts/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-04-04 09:09:54.000000 flash-accounts-1.0.1/flash_accounts/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-04-04 10:41:21.000000 flash-accounts-1.0.1/flash_accounts/models.py
+-rw-rw-rw-   0        0        0     1965 2023-04-04 13:03:33.000000 flash-accounts-1.0.1/flash_accounts/serializers.py
+-rw-rw-rw-   0        0        0     2512 2023-04-04 13:43:01.000000 flash-accounts-1.0.1/flash_accounts/services.py
+-rw-rw-rw-   0        0        0     3451 2023-04-04 13:03:33.000000 flash-accounts-1.0.1/flash_accounts/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:02:47.598336 flash-accounts-1.0.1/flash_accounts/templates/
+drwxrwxrwx   0        0        0        0 2023-04-14 11:02:47.647342 flash-accounts-1.0.1/flash_accounts/templates/flash_accounts/
+-rw-rw-rw-   0        0        0     2088 2023-04-04 13:03:33.000000 flash-accounts-1.0.1/flash_accounts/templates/flash_accounts/activate.html
+-rw-rw-rw-   0        0        0      174 2023-04-04 13:03:33.000000 flash-accounts-1.0.1/flash_accounts/templates/flash_accounts/activate.txt
+-rw-rw-rw-   0        0        0     2119 2023-04-04 13:03:33.000000 flash-accounts-1.0.1/flash_accounts/templates/flash_accounts/password_reset.html
+-rw-rw-rw-   0        0        0      187 2023-04-04 13:03:33.000000 flash-accounts-1.0.1/flash_accounts/templates/flash_accounts/password_reset.txt
+-rw-rw-rw-   0        0        0    20329 2023-04-14 10:59:44.000000 flash-accounts-1.0.1/flash_accounts/tests.py
+-rw-rw-rw-   0        0        0      901 2023-04-04 15:44:42.000000 flash-accounts-1.0.1/flash_accounts/urls.py
+-rw-rw-rw-   0        0        0     4289 2023-04-14 10:59:44.000000 flash-accounts-1.0.1/flash_accounts/views.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:02:47.640337 flash-accounts-1.0.1/flash_accounts.egg-info/
+-rw-rw-rw-   0        0        0      779 2023-04-14 11:02:47.000000 flash-accounts-1.0.1/flash_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2023-04-14 11:02:47.000000 flash-accounts-1.0.1/flash_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 11:02:47.000000 flash-accounts-1.0.1/flash_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-14 11:02:47.000000 flash-accounts-1.0.1/flash_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 11:02:47.000000 flash-accounts-1.0.1/flash_accounts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1020 2023-04-06 12:54:49.000000 flash-accounts-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 11:02:47.649372 flash-accounts-1.0.1/setup.cfg
```

### Comparing `flash-accounts-1.0.0/LICENSE` & `flash-accounts-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/PKG-INFO` & `flash-accounts-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash-accounts
-Version: 1.0.0
+Version: 1.0.1
 Summary: DRF lightweight reusable app for account management
 Author: Mateusz Meksuła
 License: MIT
 Project-URL: Homepage, https://github.com/MeksulaM/flash-accounts
 Keywords: django,restframework,djangorestframework,authentication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `flash-accounts-1.0.0/README.md` & `flash-accounts-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 -   user registration,
 -   user account activation,
 -   password reset.
 
 ## **Requirements**
 
--   python>=3.7
--   django>=3.0
--   djangorestframework>=3.11.0
+-   python >= 3.7
+-   django >= 3.0
+-   djangorestframework >= 3.11.0
 
 ## **Getting started**
 
 ### **Installation**
 
 Flash Accounts can be installed with pip by running the following command:
 
@@ -52,15 +52,15 @@
 
 Configure an email backend. During development, you can use the console backend. Add the following line to the projects's `settings.py` file:
 
 ```python
 EMAIL_BACKEND = "django.core.mail.backends.console.EmailBackend"
 ```
 
-**Note**: It is necessary to declare an email backend in project's `settings.py` file.  
+**Note**: It is necessary to declare an email backend for Flash Accounts to work correctly.  
 You can learn about Django email backends [here.](https://docs.djangoproject.com/en/4.2/topics/email/#email-backends)
 
 <br>
 Finally, run migrations by the following command:
 
 ```console
 python manage.py migrate
@@ -207,26 +207,27 @@
     -d '{
         "password": "NEWpassword123",
         "password2": "NEWpassword123"
     }' \
     http://localhost:8000/api/auth/password-reset/confirm/8kRuuRApqEQAeFeyzMSyAiYKtyT5DKEhrSkuSBcm3bmb4Gmih6DEVhr/
 
 {
-    "password": "Password has been changed
+    "password": "Password has been changed."
 }
 ```
 
 ## **Settings**
 
 ### **Default settings**
 
 The default settings values are shown below:
 
 ```python
 from django.utils import timezone
+from django.conf import settings
 
 DEFAULT_SETTINGS = {
     "ACTIVATE_ACCOUNT": True,
     "ACTIVATION_TOKEN_LIFETIME": timezone.timedelta(hours=1),
     "ACTIVATION_EMAIL_TEMPLATE": "flash_accounts/activate",
     "ACTIVATION_EMAIL_SUBJECT": "Activate your account.",
     "PASSWORD_RESET_TOKEN_LIFETIME": timezone.timedelta(hours=1),
@@ -268,15 +269,15 @@
 Path to the password reset email templates, **without** the file extension. This path points to two files:
 
 -   password_reset.html
 -   password_reset.txt
 
 #### <li><b> `PASSWORD_RESET_EMAIL_SUBJECT` </b></li>
 
-Subject of password reset email that is sent when new user requests password reset.
+Subject of password reset email that is sent when user requests password reset.
 
 #### <li><b> `EMAIL_FROM` </b></li>
 
 An email address from which emails will appear to be sent.  
 Flash Accounts first checks if `DEFAULT_EMAIL_FROM` field is set in project's `settings.py` file.
 
 ### **Customizing settings**
```

### Comparing `flash-accounts-1.0.0/flash_accounts/migrations/0001_initial.py` & `flash-accounts-1.0.1/flash_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/flash_accounts/models.py` & `flash-accounts-1.0.1/flash_accounts/models.py`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/flash_accounts/serializers.py` & `flash-accounts-1.0.1/flash_accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/flash_accounts/services.py` & `flash-accounts-1.0.1/flash_accounts/services.py`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/flash_accounts/settings.py` & `flash-accounts-1.0.1/flash_accounts/settings.py`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/flash_accounts/templates/flash_accounts/activate.html` & `flash-accounts-1.0.1/flash_accounts/templates/flash_accounts/activate.html`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/flash_accounts/templates/flash_accounts/password_reset.html` & `flash-accounts-1.0.1/flash_accounts/templates/flash_accounts/password_reset.html`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/flash_accounts/tests.py` & `flash-accounts-1.0.1/flash_accounts/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,16 +168,18 @@
         self.url = reverse("sign_up")
 
     def test_register_user(self):
         response = self.client.post(self.url, data=self.valid_data)
 
         self.assertEquals(response.status_code, status.HTTP_201_CREATED)
         self.assertEqual(User.objects.count(), 1)
-        self.assertEqual(User.objects.first().username, "testUser")
-        self.assertEqual(User.objects.first().email, "testemail@test.com")
+        u = User.objects.first()
+        self.assertEqual(u.username, "testUser")
+        self.assertEqual(u.email, "testemail@test.com")
+        self.assertEqual(u.check_password("testpassword123"), True)
 
         if flash_settings.ACTIVATE_ACCOUNT:
             self.assertEqual(User.objects.first().is_active, False)
         else:
             self.assertEqual(User.objects.first().is_active, True)
 
     def test_register_user_invalid_data(self):
```

### Comparing `flash-accounts-1.0.0/flash_accounts/urls.py` & `flash-accounts-1.0.1/flash_accounts/urls.py`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/flash_accounts/views.py` & `flash-accounts-1.0.1/flash_accounts/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,28 @@
 User = get_user_model()
 
 
 class UserCreateAPIView(generics.CreateAPIView):
     permission_classes = [AllowAny]
     serializer_class = UserCreateSerializer
 
-    # Account activation
-    if flash_settings.ACTIVATE_ACCOUNT:
-
-        def perform_create(self, serializer):
-            """
-            Save user account as inactive, create token and
-            send mail with activation link.
-            """
 
+    def perform_create(self, serializer):
+        """
+        Save user account as inactive, create token and
+        send mail with activation link.
+        """
+        # Account activation
+        if flash_settings.ACTIVATE_ACCOUNT:
             user = serializer.save(is_active=False)
             services.create_and_send_activation_token(user, self.request)
+        else:
+            user = serializer.save()
+        user.set_password(serializer.validated_data["password"])
+        user.save()
 
 
 @api_view(["GET"])
 @permission_classes([AllowAny])
 def activate_account(request, token_value):
     """
     Activate user account if activation token is valid.
```

### Comparing `flash-accounts-1.0.0/flash_accounts.egg-info/PKG-INFO` & `flash-accounts-1.0.1/flash_accounts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash-accounts
-Version: 1.0.0
+Version: 1.0.1
 Summary: DRF lightweight reusable app for account management
 Author: Mateusz Meksuła
 License: MIT
 Project-URL: Homepage, https://github.com/MeksulaM/flash-accounts
 Keywords: django,restframework,djangorestframework,authentication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `flash-accounts-1.0.0/flash_accounts.egg-info/SOURCES.txt` & `flash-accounts-1.0.1/flash_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flash-accounts-1.0.0/pyproject.toml` & `flash-accounts-1.0.1/pyproject.toml`

 * *Files identical despite different names*

