# Comparing `tmp/crc_jupyter_auth-1.0.3.tar.gz` & `tmp/crc_jupyter_auth-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc_jupyter_auth-1.0.3.tar", max compression
+gzip compressed data, was "crc_jupyter_auth-1.0.4.tar", max compression
```

## Comparing `crc_jupyter_auth-1.0.3.tar` & `crc_jupyter_auth-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     4663 2023-02-28 17:21:24.773869 crc_jupyter_auth-1.0.3/README.md
--rw-r--r--   0        0        0      170 2023-02-28 17:21:24.773869 crc_jupyter_auth-1.0.3/crc_jupyter_auth/__init__.py
--rw-r--r--   0        0        0     6358 2023-02-28 17:21:24.773869 crc_jupyter_auth-1.0.3/crc_jupyter_auth/remote_user_auth.py
--rw-r--r--   0        0        0     1184 2023-02-28 17:21:53.094920 crc_jupyter_auth-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 crc_jupyter_auth-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34893 2023-04-14 16:50:49.714533 crc_jupyter_auth-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0     4465 2023-04-14 16:50:49.714533 crc_jupyter_auth-1.0.4/README.md
+-rw-r--r--   0        0        0      170 2023-04-14 16:50:49.714533 crc_jupyter_auth-1.0.4/crc_jupyter_auth/__init__.py
+-rw-r--r--   0        0        0     6358 2023-04-14 16:50:49.714533 crc_jupyter_auth-1.0.4/crc_jupyter_auth/remote_user_auth.py
+-rw-r--r--   0        0        0     1184 2023-04-14 16:51:07.638801 crc_jupyter_auth-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 crc_jupyter_auth-1.0.4/PKG-INFO
```

### Comparing `crc_jupyter_auth-1.0.3/README.md` & `crc_jupyter_auth-1.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CRC JupyterHub Authenticator
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5e1a00bf8dbe4daf8275fc88ce748ea6)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pitt-crc/Jupyter-Authenticator&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/5e1a00bf8dbe4daf8275fc88ce748ea6)](https://www.codacy.com/gh/pitt-crc/Jupyter-Authenticator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=pitt-crc/Jupyter-Authenticator&utm_campaign=Badge_Coverage)
-[![Tests](https://github.com/pitt-crc/Jupyter-Authenticator/actions/workflows/PackageTest.yml/badge.svg)](https://github.com/pitt-crc/Jupyter-Authenticator/actions/workflows/PackageTest.yml)
+[![](https://app.codacy.com/project/badge/Grade/5e1a00bf8dbe4daf8275fc88ce748ea6)](https://app.codacy.com/gh/pitt-crc/Jupyter-Authenticator/dashboard)
+[![](https://app.codacy.com/project/badge/Coverage/5e1a00bf8dbe4daf8275fc88ce748ea6)](https://app.codacy.com/gh/pitt-crc/Jupyter-Authenticator/dashboard)
+[![](https://github.com/pitt-crc/Jupyter-Authenticator/actions/workflows/PackageTest.yml/badge.svg)](https://github.com/pitt-crc/Jupyter-Authenticator/actions/workflows/PackageTest.yml)
 
 The `crc_jupyter_auth` package is a Jupyter authentication plugin for redirecting users based on their account status and VPN role.
 The utility is based on the [jhub_remote_user_authenticator](https://github.com/cwaldbieser/jhub_remote_user_authenticator)
 package originally created for more general applications.
 The CRC version builds on the original utility by providing significantly improved test coverage and a refined set of configuration options.
 
 ## How It Works
@@ -31,43 +31,43 @@
 To enable the same functionality plus local account management, use `RemoteUserLocalAuthenticator`:
 
 ```bash
 c.JupyterHub.authenticator_class = "crc_jupyter_auth.RemoteUserLocalAuthenticator"
 ```
 
 The `RemoteUserLocalAuthenticator` class provides the same authentication functionality
-as `RemoteUserAuthenticator` but is derived from Jupyter's builtin `LocalAuthenticator` class. 
+as `RemoteUserAuthenticator` but is derived from Jupyter's built-in `LocalAuthenticator` class. 
 This provides extra features such as the ability to add local accounts through the admin interface.
 
 ## Package Configuration
 
 The authenticator works by fetching the authenticated username from the HTTP header `Cn`.
 If found, and not blank, the client will be logged in as that user.
 Otherwise, the user is redirected.
 
 The HTTP header names and failure redirects are configurable via the Jupyter settings file.
 Setting names and default values are provided in the table below:
 
-| Setting Name            | Default        | Description                                                                                |
-|-------------------------|----------------|--------------------------------------------------------------------------------------------|
-| `username_header`       | `"Cn"`         | HTTP header name to inspect for the authenticated username                                 |
-| `vpn_header`            | `"isMemberOf"` | HTTP header name to inspect for the user VPN role(s).                                      |
-| `required_vpn_role`     | `""`           | Required VPN role for accessing the service. Ignored if an empty string.                   |
-| `missing_user_redirect` | `""`           | Redirect URL if the user has no home directory. Defaults to 404 if empty string.           |
-| `missing_role_redirect` | `""`           | Redirect URL if the user is missing necessary VPN role. Defaults to 404 if empty string.   |
+| Setting Name            | Default        | Description                                                                                   |
+|-------------------------|----------------|-----------------------------------------------------------------------------------------------|
+| `username_header`       | `"Cn"`         | HTTP header name to inspect for the authenticated username         -                          |
+| `vpn_header`            | `"isMemberOf"` | HTTP header name to inspect for the user VPN role(s).                                         |
+| `required_vpn_role`     | `""`           | Required VPN role for accessing the service. Ignored if an empty string.                      |
+| `missing_user_redirect` | `""`           | Redirect URL if the user has no home directory. Defaults to 404 if empty string.              |
+| `missing_role_redirect` | `""`           | Redirect URL if the user is missing the required VPN header. Defaults to 404 if empty string. |
 
 To modify a settings value, use the `c.Authenticator` object in the configuration file.
 For example:
 
 ```python
 c.Authenticator.missing_role_redirect = "https://my.redirect.domain"
 ```
 
 If your system assigns multiple VPN roles to users and more than a single role is reported by the header
-`vpn_header`, the VPN roles should be provided in the header as a semicolon delimited list
+`vpn_header`, the VPN roles should be provided in the header as a semicolon-delimited list
 (e.g., `role1;role2`).
 
 ## Architecture and Security Recommendations
 
 This authenticator relies on HTTP headers that can be spoofed by a malicious client.
 To protect against this, an authenticating proxy should be placed in front
 of Jupyterhub. The JupyterHub daemon should **only** be accessible from the proxy
```

### Comparing `crc_jupyter_auth-1.0.3/crc_jupyter_auth/remote_user_auth.py` & `crc_jupyter_auth-1.0.4/crc_jupyter_auth/remote_user_auth.py`

 * *Files identical despite different names*

### Comparing `crc_jupyter_auth-1.0.3/pyproject.toml` & `crc_jupyter_auth-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crc_jupyter_auth"
-version = "1.0.3"  # Version is set dynamically by the CI tool on publication
+version = "1.0.4"  # Version is set dynamically by the CI tool on publication
 authors = ["Pitt Center for Research Computing", ]
 license = "GPL-3.0-only"
 readme = "README.md"
 description = "Jupyter authentication plugin that checks for account existence and VPN roles."
 homepage = "https://github.com/pitt-crc/Jupyter-Authenticator"
 repository = "https://github.com/pitt-crc/Jupyter-Authenticator"
 documentation = "https://github.com/pitt-crc/Jupyter-Authenticator"
```

### Comparing `crc_jupyter_auth-1.0.3/PKG-INFO` & `crc_jupyter_auth-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-jupyter-auth
-Version: 1.0.3
+Version: 1.0.4
 Summary: Jupyter authentication plugin that checks for account existence and VPN roles.
 Home-page: https://github.com/pitt-crc/Jupyter-Authenticator
 License: GPL-3.0-only
 Keywords: Pitt,CRC,Jupyter,JupyterHub,JupyterLab,Authentication
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.7
 Classifier: Framework :: Jupyter
@@ -26,17 +26,17 @@
 Requires-Dist: tornado
 Requires-Dist: traitlets
 Project-URL: Documentation, https://github.com/pitt-crc/Jupyter-Authenticator
 Project-URL: Repository, https://github.com/pitt-crc/Jupyter-Authenticator
 Description-Content-Type: text/markdown
 
 # CRC JupyterHub Authenticator
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5e1a00bf8dbe4daf8275fc88ce748ea6)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pitt-crc/Jupyter-Authenticator&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/5e1a00bf8dbe4daf8275fc88ce748ea6)](https://www.codacy.com/gh/pitt-crc/Jupyter-Authenticator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=pitt-crc/Jupyter-Authenticator&utm_campaign=Badge_Coverage)
-[![Tests](https://github.com/pitt-crc/Jupyter-Authenticator/actions/workflows/PackageTest.yml/badge.svg)](https://github.com/pitt-crc/Jupyter-Authenticator/actions/workflows/PackageTest.yml)
+[![](https://app.codacy.com/project/badge/Grade/5e1a00bf8dbe4daf8275fc88ce748ea6)](https://app.codacy.com/gh/pitt-crc/Jupyter-Authenticator/dashboard)
+[![](https://app.codacy.com/project/badge/Coverage/5e1a00bf8dbe4daf8275fc88ce748ea6)](https://app.codacy.com/gh/pitt-crc/Jupyter-Authenticator/dashboard)
+[![](https://github.com/pitt-crc/Jupyter-Authenticator/actions/workflows/PackageTest.yml/badge.svg)](https://github.com/pitt-crc/Jupyter-Authenticator/actions/workflows/PackageTest.yml)
 
 The `crc_jupyter_auth` package is a Jupyter authentication plugin for redirecting users based on their account status and VPN role.
 The utility is based on the [jhub_remote_user_authenticator](https://github.com/cwaldbieser/jhub_remote_user_authenticator)
 package originally created for more general applications.
 The CRC version builds on the original utility by providing significantly improved test coverage and a refined set of configuration options.
 
 ## How It Works
@@ -62,43 +62,43 @@
 To enable the same functionality plus local account management, use `RemoteUserLocalAuthenticator`:
 
 ```bash
 c.JupyterHub.authenticator_class = "crc_jupyter_auth.RemoteUserLocalAuthenticator"
 ```
 
 The `RemoteUserLocalAuthenticator` class provides the same authentication functionality
-as `RemoteUserAuthenticator` but is derived from Jupyter's builtin `LocalAuthenticator` class. 
+as `RemoteUserAuthenticator` but is derived from Jupyter's built-in `LocalAuthenticator` class. 
 This provides extra features such as the ability to add local accounts through the admin interface.
 
 ## Package Configuration
 
 The authenticator works by fetching the authenticated username from the HTTP header `Cn`.
 If found, and not blank, the client will be logged in as that user.
 Otherwise, the user is redirected.
 
 The HTTP header names and failure redirects are configurable via the Jupyter settings file.
 Setting names and default values are provided in the table below:
 
-| Setting Name            | Default        | Description                                                                                |
-|-------------------------|----------------|--------------------------------------------------------------------------------------------|
-| `username_header`       | `"Cn"`         | HTTP header name to inspect for the authenticated username                                 |
-| `vpn_header`            | `"isMemberOf"` | HTTP header name to inspect for the user VPN role(s).                                      |
-| `required_vpn_role`     | `""`           | Required VPN role for accessing the service. Ignored if an empty string.                   |
-| `missing_user_redirect` | `""`           | Redirect URL if the user has no home directory. Defaults to 404 if empty string.           |
-| `missing_role_redirect` | `""`           | Redirect URL if the user is missing necessary VPN role. Defaults to 404 if empty string.   |
+| Setting Name            | Default        | Description                                                                                   |
+|-------------------------|----------------|-----------------------------------------------------------------------------------------------|
+| `username_header`       | `"Cn"`         | HTTP header name to inspect for the authenticated username         -                          |
+| `vpn_header`            | `"isMemberOf"` | HTTP header name to inspect for the user VPN role(s).                                         |
+| `required_vpn_role`     | `""`           | Required VPN role for accessing the service. Ignored if an empty string.                      |
+| `missing_user_redirect` | `""`           | Redirect URL if the user has no home directory. Defaults to 404 if empty string.              |
+| `missing_role_redirect` | `""`           | Redirect URL if the user is missing the required VPN header. Defaults to 404 if empty string. |
 
 To modify a settings value, use the `c.Authenticator` object in the configuration file.
 For example:
 
 ```python
 c.Authenticator.missing_role_redirect = "https://my.redirect.domain"
 ```
 
 If your system assigns multiple VPN roles to users and more than a single role is reported by the header
-`vpn_header`, the VPN roles should be provided in the header as a semicolon delimited list
+`vpn_header`, the VPN roles should be provided in the header as a semicolon-delimited list
 (e.g., `role1;role2`).
 
 ## Architecture and Security Recommendations
 
 This authenticator relies on HTTP headers that can be spoofed by a malicious client.
 To protect against this, an authenticating proxy should be placed in front
 of Jupyterhub. The JupyterHub daemon should **only** be accessible from the proxy
```

