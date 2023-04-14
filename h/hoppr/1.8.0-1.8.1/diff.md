# Comparing `tmp/hoppr-1.8.0.tar.gz` & `tmp/hoppr-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.0.tar", max compression
+gzip compressed data, was "hoppr-1.8.1.tar", max compression
```

## Comparing `hoppr-1.8.0.tar` & `hoppr-1.8.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1084 2023-04-04 21:04:31.000000 hoppr-1.8.0/LICENSE
--rw-r--r--   0        0        0     1214 2023-04-04 21:04:31.000000 hoppr-1.8.0/README.md
--rw-r--r--   0        0        0     1035 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    10990 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10732 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12882 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10337 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     3321 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4480 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     4082 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6369 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7927 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4472 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3127 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5403 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4630 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     4791 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/in_toto.py
--rw-r--r--   0        0        0     3074 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/models/base.py
--rw-r--r--   0        0        0     3778 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17044 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/models/py.typed
--rw-r--r--   0        0        0     3975 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/models/transfer.py
--rw-r--r--   0        0        0     1353 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/models/types.py
--rw-r--r--   0        0        0     2389 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    25427 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/result.py
--rw-r--r--   0        0        0     5305 2023-04-04 21:04:31.000000 hoppr-1.8.0/hoppr/utils.py
--rw-r--r--   0        0        0     3613 2023-04-04 21:04:31.000000 hoppr-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-12 18:43:58.000000 hoppr-1.8.1/LICENSE
+-rw-r--r--   0        0        0     1214 2023-04-12 18:43:58.000000 hoppr-1.8.1/README.md
+-rw-r--r--   0        0        0     1035 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    10990 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10732 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     6256 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/cli/hopctl.py
+-rw-r--r--   0        0        0      563 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12941 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0    10236 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     3321 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4664 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     4082 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6369 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7927 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     4472 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3127 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3739 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5403 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5301 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4577 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     4810 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6847 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3074 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1708 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1409 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/base.py
+-rw-r--r--   0        0        0     3778 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    17044 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/py.typed
+-rw-r--r--   0        0        0     3975 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     1353 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/net.py
+-rw-r--r--   0        0        0     4323 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    25427 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/resources/hoppr-hippo-large.ansi
+-rw-r--r--   0        0        0    10419 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0     4036 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/result.py
+-rw-r--r--   0        0        0     5305 2023-04-12 18:43:58.000000 hoppr-1.8.1/hoppr/utils.py
+-rw-r--r--   0        0        0     3613 2023-04-12 18:43:58.000000 hoppr-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.1/PKG-INFO
```

### Comparing `hoppr-1.8.0/LICENSE` & `hoppr-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/README.md` & `hoppr-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/__init__.py` & `hoppr-1.8.1/hoppr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
```

### Comparing `hoppr-1.8.0/hoppr/base_plugins/collector.py` & `hoppr-1.8.1/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/base_plugins/hoppr.py` & `hoppr-1.8.1/hoppr/base_plugins/hoppr.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/cli/hopctl.py` & `hoppr-1.8.1/hoppr/cli/hopctl.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/constants.py` & `hoppr-1.8.1/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.8.1/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         # Take the first URL and download filename if multiple are returned
         # Apt download output format:
         #   '<download URL>' <URL-encoded download filename> <download size> SHA512:<package hash>
         # Extract the output into a tuple of the form (<download URL>, <URL-encoded download filename>). For example:
         #   ("http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.34.1-1ubuntu1.5_amd64.deb",
         #    "git_1%3a2.34.1-1ubuntu1.5_amd64.deb")
         result = url_result.stdout.decode("utf-8").split("\n")[0]
-        found_url, download_filename = result.split(" ")[0:2]
+        found_url, download_filename = result.split(" ")[:2]
 
         self.get_logger().debug(msg=f"Found URL: {found_url}", indent_level=3)
         self.get_logger().debug(msg=f"Download filename: {download_filename}", indent_level=3)
 
         return found_url.strip("'"), download_filename
 
     def _get_download_url_path(self, purl: PackageURL) -> str:
@@ -163,19 +163,15 @@
 
         return pkg_info["Filename"]
 
     def _get_found_repo(self, found_url: str) -> str | None:
         """
         Identify the repository associated with the specified URL
         """
-        for repo in self.manifest_repos:
-            if found_url.startswith(repo):
-                return repo
-
-        return None
+        return next((repo for repo in self.manifest_repos if found_url.startswith(repo)), None)
 
     def _populate_apt_folder_structure(self, apt_path: Path, path_dict: Mapping[str, Mapping | None]) -> None:
         for key, value in path_dict.items():
             # None type indicates file to create
             if value is None:
                 apt_file = apt_path / key
                 apt_file.touch(exist_ok=True, mode=0o644)
@@ -189,22 +185,22 @@
             else:
                 raise TypeError("Value is not expected type.")
 
     def _populate_auth_conf(self, repo_list: list[Repository], file: Path) -> None:
         """
         Populate Apt authentication config file
         """
-        creds = []
+        creds: list[str] = []
         for repo in repo_list:
             repo_credentials = Credentials.find(repo.url)
             if repo_credentials is not None:
                 creds.append(
                     f"machine {urlparse(repo.url).netloc} "
                     f"login {repo_credentials.username} "
-                    f"password {repo_credentials.password}\n"
+                    f"password {repo_credentials.password.get_secret_value()}\n"
                 )
 
         # Set restrictive permissions on Apt authentication config file
         file.chmod(mode=0o600)
 
         with file.open(mode="w+", encoding="utf-8") as auth_conf:
             auth_conf.write("\n".join(creds))
@@ -217,30 +213,33 @@
         parser = ConfigParser()
 
         with (Path("/") / "etc" / "os-release").open(mode="r", encoding="utf-8") as os_release:
             parser.read_string(string=f"[os-release]\n{os_release.read()}")
 
         version_codename = parser["os-release"]["VERSION_CODENAME"]
 
-        sources = []
+        sources: list[str] = []
         for repo in repo_list:
             for component in ["main restricted", "universe", "multiverse"]:
-                sources.append(f"deb {repo} {version_codename} {component}")
-                sources.append(f"deb {repo} {version_codename}-updates {component}")
-                sources.append(f"deb {repo} {version_codename}-security {component}")
+                sources.extend(
+                    (
+                        f"deb {repo} {version_codename} {component}",
+                        f"deb {repo} {version_codename}-updates {component}",
+                        f"deb {repo} {version_codename}-security {component}",
+                    )
+                )
 
         with file.open(mode="w+", encoding="utf-8") as sources_list:
             sources_list.write("\n".join(sources))
 
     def _repo_proxy(self) -> set[str]:
         proxy_args: list[str] = []
 
         for proto in ["http", "https"]:
-            proxy = os.getenv(f"{proto}_proxy")
-            if proxy:
+            if proxy := os.getenv(f"{proto}_proxy"):
                 proxy_args = [*proxy_args, f"--option=Acquire::{proto}::Proxy={proxy}"]
 
         no_proxy_urls = [item for item in os.getenv("no_proxy", "").split(",") if item != ""]
 
         for url in self.manifest_repos:
             parsed_url = urlparse(url)
```

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import BatchCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_process, hoppr_rerunner
 from hoppr.exceptions import HopprPluginError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import Credentials
-from hoppr.models.types import PurlType
 from hoppr.models.manifest import Component
+from hoppr.models.types import PurlType
 from hoppr.result import Result
 
 
 def _artifact_string(purl: PackageURL) -> str:
     artifact_string = purl.name
 
     if purl.version is not None:
@@ -39,15 +39,15 @@
     if purl.qualifiers.get("arch") is not None:
         artifact_string = ".".join([artifact_string, purl.qualifiers.get("arch")])
 
     return artifact_string
 
 
 def _is_rpm_repo(repo_url: str) -> bool:
-    url = urljoin(repo_url + "/", "repodata/repomd.xml")
+    url = urljoin(f"{repo_url}/", "repodata/repomd.xml")
 
     basic_auth = None
     creds = Credentials.find(repo_url)
     if creds is not None:
         basic_auth = HTTPBasicAuth(username=creds.username, password=creds.password.get_secret_value())
 
     for attempt in range(3):
@@ -91,19 +91,15 @@
         context: HopprContext,
         config: dict | None = None,
         config_file: str | PathLike = Path.cwd() / ".hoppr-dnf" / "dnf.conf",
     ) -> None:
         super().__init__(context=context, config=config)
 
         self.password_list: list[str] = []
-        self.manifest_repos: list[str] = []
-
-        for repo in self.context.repositories[PurlType.RPM]:
-            self.manifest_repos.append(repo.url)
-
+        self.manifest_repos: list[str] = [repo.url for repo in self.context.repositories[PurlType.RPM]]
         self.config_file = Path(config_file)
 
         if self.config and "dnf_command" in self.config:
             self.required_commands = [self.config["dnf_command"]]
 
         self.base_command = [
             self.required_commands[0],
@@ -124,27 +120,21 @@
         if run_result.returncode != 0 or len(run_result.stdout.decode("utf-8")) == 0:
             msg = f"{self.required_commands[0]} failed to locate package for {purl}"
             self.get_logger().debug(msg=msg, indent_level=2)
 
             raise HopprPluginError(msg)
 
         # Taking the first URL if multiple are returned
-        found_url = run_result.stdout.decode("utf-8").strip().split("\n")[0]
-
-        return found_url
+        return run_result.stdout.decode("utf-8").strip().split("\n")[0]
 
     def _get_found_repo(self, found_url: str) -> str | None:
         """
         Identify the repository associated with the specified URL
         """
-        for repo in self.manifest_repos:
-            if found_url.startswith(repo):
-                return repo
-
-        return None
+        return next((repo for repo in self.manifest_repos if found_url.startswith(repo)), None)
 
     def get_version(self) -> str:
         return __version__
 
     @hoppr_process
     def pre_stage_process(self) -> Result:
         repo_config = ConfigParser()
@@ -170,15 +160,15 @@
                 "priority": "1",
                 "proxy": _repo_proxy(repo.url),
                 "module_hotfixes": "true",
             }
 
             if creds is not None:
                 repo_config[temp_repo]["username"] = f"{creds.username}"
-                repo_config[temp_repo]["password"] = f"{creds.password}"
+                repo_config[temp_repo]["password"] = f"{creds.password.get_secret_value()}"
 
         if not self.context.strict_repos:
             system_repos = ConfigParser()
 
             # Get all system-managed .repo files
             repo_files = Path("/", "etc", "yum.repos.d").glob("*.repo")
             system_repos.read([str(repo_file) for repo_file in repo_files])
```

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_git_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Collector plugin for git repositories
 """
 from __future__ import annotations
 
 import os
-import pathlib
 import re
 
-from typing import Any
+from pathlib import Path
 
 from packageurl import PackageURL  # type: ignore[import]
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
+from hoppr.models.manifest import Component
 from hoppr.result import Result
 
 
 class CollectGitPlugin(SerialCollectorPlugin):
     """
     Class to copy git repositories
 
@@ -34,20 +34,19 @@
     products: list[str] = ["git/*", "gitlab/*", "github/*"]
 
     def get_version(self) -> str:  # pylint: disable=duplicate-code
         return __version__
 
     def __init__(self, context: HopprContext, config: dict | None = None) -> None:
         super().__init__(context=context, config=config)
-        if self.config is not None:
-            if "git_command" in self.config:
-                self.required_commands = [self.config["git_command"]]
+        if self.config is not None and "git_command" in self.config:
+            self.required_commands = [self.config["git_command"]]
 
     @hoppr_rerunner
-    def collect(self, comp: Any, repo_url: str, creds: CredentialRequiredService | None = None):
+    def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None) -> Result:
         """
         Collect git repository
         """
         purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
 
         source_url = os.path.join(repo_url, purl.namespace, purl.name)
 
@@ -64,46 +63,51 @@
         if not git_result.is_success():
             return git_result
 
         self.set_collection_params(comp, repo_url, target_dir)
 
         return Result.success(return_obj=comp)
 
-    def git_clone(self, tmp_dir, source_url, source_creds, comp: Any):
-        """Git clone"""
-
+    def git_clone(
+        self,
+        tmp_dir: Path,
+        source_url: str,
+        source_creds: CredentialRequiredService | None,
+        comp: Component,
+    ) -> Result:
+        """
+        Git clone
+        """
         git_src = source_url
-        password_list = []
+        password_list: list[str] = []
         if re.match("^https?://", git_src) and source_creds is not None:
             git_src = git_src.replace("://", f"://{source_creds.username}@", 1)
             if source_creds.password:
-                git_src = git_src.replace("@", f":{source_creds.password}@")
-                password_list = [source_creds.password]
+                git_src = git_src.replace("@", f":{source_creds.password.get_secret_value()}@")
+                password_list = [source_creds.password.get_secret_value()]
 
         if git_src.startswith("ssh://") and source_creds is not None:
             git_src = git_src.replace("ssh://", f"ssh://{source_creds.username}@")
 
         if not git_src.endswith(".git"):
             git_src += ".git"
 
-        opts = []
+        opts: list[str] = []
         if str(comp.version).strip():
-            opts.append("--branch")
-            opts.append(str(comp.version))
+            opts.extend(("--branch", str(comp.version)))
 
         # Default depth
         depth = "1"
         if self.config is not None:
             # Allow for further depth default to 1
             depth = self.config.get("depth", depth)
 
         # Recognize the 'all' keyword as requesting all history
         if depth.lower() != "all":
-            opts.append("--depth")
-            opts.append(depth)
+            opts.extend(("--depth", depth))
 
         # Command
         command = [self.required_commands[0], "clone", *opts, git_src]
 
         # Only clone with a depth of one and reference the version specified.
         result = self.run_command(
             command,
@@ -113,23 +117,25 @@
         if result.returncode != 0:
             msg = f"Failed to clone {source_url}"
             self.get_logger().debug(msg=msg, indent_level=2)
             return Result.retry(message=msg)
 
         return Result.success()
 
-    def git_update(self, tmp_dir, name_git):
-        """Git update-server-info"""
-
-        repo_dir = os.path.join(pathlib.Path(tmp_dir), name_git)
+    def git_update(self, tmp_dir: Path, name_git: str) -> Result:
+        """
+        Git update-server-info
+        """
+        repo_dir = tmp_dir / name_git
 
         # Make the clone usable as a remote
         result = self.run_command(
             [self.required_commands[0], "update-server-info"],
             cwd=repo_dir,
         )
+
         if result.returncode != 0:
             msg = "Failed to make the clone usable as a remote"
             self.get_logger().debug(msg=msg, indent_level=2)
             return Result.retry(message=msg)
 
         return Result.success()
```

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_nexus_search.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.8.1/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/composite_collector.py` & `hoppr-1.8.1/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.8.1/hoppr/core_plugins/delta_sbom.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.8.1/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/oras_registry.py` & `hoppr-1.8.1/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,15 @@
         report_dir.mkdir(exist_ok=True)
 
         results_file_name = report_dir / "index.html"
 
         for dir_name in ("assets", "scripts", "styles"):
             source_dir = Path(__file__).parent / dir_name
             dest_dir = report_dir / dir_name
-            if not dest_dir.exists():
-                shutil.copytree(source_dir, dest_dir)
+            shutil.copytree(src=source_dir, dst=dest_dir, dirs_exist_ok=True)
 
         context = {
             "report_count": report_count,
             "error_count": error_count,
             "reports_by_stage": reports_by_stage,
             "reports_by_plugin": reports_by_plugin,
             "ResultStatus": ResultStatus,
@@ -110,21 +109,20 @@
         return len(successful_reports)
 
     def _get_overall_status_button_class(self, reports: list[Report]) -> str:
         """
         Determine the overall status of a list of reports and returns the appropriate css class.
         """
 
-        num_successful_reports = sum(1 for report in reports if report.result.numerator == ResultStatus.SUCCESS)
-        num_reports = len(reports)
+        num_successful_reports = sum(report.result.numerator == ResultStatus.SUCCESS for report in reports)
 
         if num_successful_reports == 0:
             return "btn-danger"
 
-        if num_successful_reports == num_reports:
+        if num_successful_reports == len(reports):
             return "btn-success"
 
         return "btn-warning"
 
     def _get_reports_by(self, sort_by: str, reports: list[Report]) -> dict:
         """
         Organize report data by plugin or stage.
```

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div
-    class="{{ 'collapse-card-container component-success' if report['result'] == 0 else 'collapse-card-container component-failure' }}"
+    class="{{ 'collapse-card-container component-success' if report['result'] == ResultStatus.SUCCESS else 'collapse-card-container component-failure' }}"
 >
     <div class="collapse-card-data">
         <div>
             <div><strong>Plugin: </strong>{{ report["plugin"] }}</div>
             <div>
                 <strong>Purl: </strong>
                 {{ report["component"].purl }}
```

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.8.1/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/in_toto.py` & `hoppr-1.8.1/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/main.py` & `hoppr-1.8.1/hoppr/main.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/mem_logger.py` & `hoppr-1.8.1/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/models/__init__.py` & `hoppr-1.8.1/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/models/__main__.py` & `hoppr-1.8.1/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/models/base.py` & `hoppr-1.8.1/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/models/credentials.py` & `hoppr-1.8.1/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/models/manifest.py` & `hoppr-1.8.1/hoppr/models/manifest.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/models/transfer.py` & `hoppr-1.8.1/hoppr/models/transfer.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/models/types.py` & `hoppr-1.8.1/hoppr/models/types.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/net.py` & `hoppr-1.8.1/hoppr/net.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,31 +16,29 @@
     """
     creds = Credentials.find(url)
 
     response = None
     if creds is not None:
         authorization_headers = {
             "PRIVATE-TOKEN": creds.password.get_secret_value(),
-            "Authorization": f"Bearer {creds.password}",
+            "Authorization": f"Bearer {creds.password.get_secret_value()}",
         }
 
         basic_auth = HTTPBasicAuth(username=creds.username, password=creds.password.get_secret_value())
         response = requests.get(url, auth=basic_auth, headers=authorization_headers, timeout=60)
     else:
         response = requests.get(url, timeout=60)
 
     response.raise_for_status()
     valid_data = True
     try:
         if isinstance(response.content, bytes):
-            data = load_string(response.content.decode("utf-8"))
-            return data
+            return load_string(response.content.decode("utf-8"))
         if isinstance(response.content, str):
-            data = load_string(response.content)
-            return data
+            return load_string(response.content)
         valid_data = False
     except HopprLoadDataError as parse_error:
         message = f"Unable to parse result from {url}."
         if response.url != url:
             message += f" Request was redirected to {response.url}. An auth issue might have occurred."
         raise HopprLoadDataError(message) from parse_error
 
@@ -59,14 +57,14 @@
 
     basic_auth = None
     if creds is not None:
         basic_auth = HTTPBasicAuth(username=creds.username, password=creds.password.get_secret_value())
 
     response = requests.get(url, auth=basic_auth, allow_redirects=True, stream=True, verify=True, timeout=60)
 
-    if 200 <= response.status_code and response.status_code < 300:
+    if 200 <= response.status_code < 300:
         with open(dest, "wb") as out_file:
             for chunk in response.iter_content(chunk_size=8192):
                 if chunk:
                     out_file.write(chunk)
 
     return response
```

### Comparing `hoppr-1.8.0/hoppr/oci_artifacts.py` & `hoppr-1.8.1/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/plugin_utils.py` & `hoppr-1.8.1/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/processor.py` & `hoppr-1.8.1/hoppr/processor.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.8.1/hoppr/resources/hoppr-hippo-large.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.8.1/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/result.py` & `hoppr-1.8.1/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/hoppr/utils.py` & `hoppr-1.8.1/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.0/pyproject.toml` & `hoppr-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.8.0"
+version = "1.8.1"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
```

### Comparing `hoppr-1.8.0/PKG-INFO` & `hoppr-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.0
+Version: 1.8.1
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

