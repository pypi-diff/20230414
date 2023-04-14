# Comparing `tmp/ubuntu-package-status-0.0.7.tar.gz` & `tmp/ubuntu-package-status-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubuntu-package-status-0.0.7.tar", last modified: Wed Feb 23 17:57:59 2022, max compression
+gzip compressed data, was "ubuntu-package-status-0.1.0.tar", last modified: Fri Apr 14 14:33:28 2023, max compression
```

## Comparing `ubuntu-package-status-0.0.7.tar` & `ubuntu-package-status-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-23 17:57:59.816311 ubuntu-package-status-0.0.7/
--rw-rw-r--   0 philroche  (1000) philroche  (1000)    35149 2021-01-18 12:34:39.000000 ubuntu-package-status-0.0.7/LICENSE
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      181 2021-01-18 12:34:17.000000 ubuntu-package-status-0.0.7/MANIFEST.in
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      309 2022-02-23 17:57:59.816311 ubuntu-package-status-0.0.7/PKG-INFO
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     1019 2021-01-22 09:51:56.000000 ubuntu-package-status-0.0.7/README.md
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      380 2022-02-23 17:57:59.816311 ubuntu-package-status-0.0.7/setup.cfg
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      973 2022-02-23 17:57:44.000000 ubuntu-package-status-0.0.7/setup.py
-drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-23 17:57:59.816311 ubuntu-package-status-0.0.7/src/
--rw-rw-r--   0 philroche  (1000) philroche  (1000)       62 2022-01-08 09:07:11.000000 ubuntu-package-status-0.0.7/src/requirements.txt
-drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-23 17:57:59.816311 ubuntu-package-status-0.0.7/src/ubuntu_package_status/
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      558 2022-02-02 16:41:00.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status/20220202-cnewcomer.yaml
--rw-rw-r--   0 philroche  (1000) philroche  (1000)        0 2021-01-18 12:34:17.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status/__init__.py
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      108 2022-02-22 18:15:21.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status/dist-config.yaml
--rw-rw-r--   0 philroche  (1000) philroche  (1000)       58 2022-01-20 15:45:13.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status/linux-fips-focal-config.yaml
--rw-rw-r--   0 philroche  (1000) philroche  (1000)    12444 2022-02-23 10:58:18.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status/ubuntu_package_status.py
-drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-23 17:57:59.816311 ubuntu-package-status-0.0.7/src/ubuntu_package_status.egg-info/
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      309 2022-02-23 17:57:59.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status.egg-info/PKG-INFO
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      602 2022-02-23 17:57:59.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status.egg-info/SOURCES.txt
--rw-rw-r--   0 philroche  (1000) philroche  (1000)        1 2022-02-23 17:57:59.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status.egg-info/dependency_links.txt
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      109 2022-02-23 17:57:59.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status.egg-info/entry_points.txt
--rw-rw-r--   0 philroche  (1000) philroche  (1000)       62 2022-02-23 17:57:59.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status.egg-info/requires.txt
--rw-rw-r--   0 philroche  (1000) philroche  (1000)       22 2022-02-23 17:57:59.000000 ubuntu-package-status-0.0.7/src/ubuntu_package_status.egg-info/top_level.txt
+drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2023-04-14 14:33:28.731005 ubuntu-package-status-0.1.0/
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)    35149 2021-01-18 12:34:39.000000 ubuntu-package-status-0.1.0/LICENSE
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      181 2021-01-18 12:34:17.000000 ubuntu-package-status-0.1.0/MANIFEST.in
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      309 2023-04-14 14:33:28.731005 ubuntu-package-status-0.1.0/PKG-INFO
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     1019 2021-01-22 09:51:56.000000 ubuntu-package-status-0.1.0/README.md
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      380 2023-04-14 14:33:28.731005 ubuntu-package-status-0.1.0/setup.cfg
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      973 2023-04-14 14:32:46.000000 ubuntu-package-status-0.1.0/setup.py
+drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2023-04-14 14:33:28.731005 ubuntu-package-status-0.1.0/src/
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)       62 2022-01-08 09:07:11.000000 ubuntu-package-status-0.1.0/src/requirements.txt
+drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2023-04-14 14:33:28.731005 ubuntu-package-status-0.1.0/src/ubuntu_package_status/
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)        0 2021-01-18 12:34:17.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status/__init__.py
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      108 2022-02-22 18:15:21.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status/dist-config.yaml
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      148 2023-04-14 10:06:15.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status/gke-kernel-config.yaml
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)    14196 2023-04-14 14:32:20.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status/ubuntu_package_status.py
+drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2023-04-14 14:33:28.731005 ubuntu-package-status-0.1.0/src/ubuntu_package_status.egg-info/
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      309 2023-04-14 14:33:28.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status.egg-info/PKG-INFO
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      546 2023-04-14 14:33:28.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status.egg-info/SOURCES.txt
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)        1 2023-04-14 14:33:28.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status.egg-info/dependency_links.txt
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      109 2023-04-14 14:33:28.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status.egg-info/entry_points.txt
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)       62 2023-04-14 14:33:28.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status.egg-info/requires.txt
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)       22 2023-04-14 14:33:28.000000 ubuntu-package-status-0.1.0/src/ubuntu_package_status.egg-info/top_level.txt
```

### Comparing `ubuntu-package-status-0.0.7/LICENSE` & `ubuntu-package-status-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubuntu-package-status-0.0.7/README.md` & `ubuntu-package-status-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ubuntu-package-status-0.0.7/setup.py` & `ubuntu-package-status-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 reqs_path = os.path.join(os.path.dirname(__file__), 'src/requirements.txt')
 
 with open(reqs_path, 'r') as req_file:
     dependencies = req_file.readlines()
 
 setup(
     name='ubuntu-package-status',
-    version='0.0.7',
+    version='0.1.0',
     install_requires=dependencies,
     url='',
     license='',
     author='philroche',
     author_email='phil.roche@canonical.com',
     description='Helpful utility to fetch package version data for specified '
                 'packages in the ubuntu archive.',
```

### Comparing `ubuntu-package-status-0.0.7/src/ubuntu_package_status/ubuntu_package_status.py` & `ubuntu-package-status-0.1.0/src/ubuntu_package_status/ubuntu_package_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,36 +37,38 @@
 
 
 def print_package_status_summary_txt(package_status):
     for ubuntu_version, package_stats in package_status.items():
         print(ubuntu_version)
         for package, arches in package_stats.items():
             print("\t{}".format(package))
-            for arch, pockets in arches.items():
-                for pocket, stats in pockets.items():
+            for pocket, pockets in arches.items():
+                for arch, stats in pockets.items():
                     if stats["full_version"]:
                         print(
-                            "\t\t{} {} {} @ {} ({})".format(
-                                arch,
+                            "\t\t{}/{} {} {} @ {} ({})".format(
                                 pocket,
+                                stats["component"],
+                                arch,
                                 stats["full_version"],
                                 stats["date_published_formatted"],
                                 stats["published_age"],
                             )
                         )
 
 
 def print_package_status_summary_csv(package_status):
     csv_stdout_writer = csv.writer(sys.stdout)
     csv_stdout_writer.writerow(
         [
             "ubuntu_version",
             "package",
             "pocket",
-            "architecture"
+            "component",
+            "architecture",
             "full_version",
             "date_published",
             "date_published_formatted",
             "published_age",
             "link",
             "build_link"
         ]
@@ -77,14 +79,15 @@
                 for arch, stats in arches.items():
                     if stats["full_version"]:
                         csv_stdout_writer.writerow(
                             [
                                 ubuntu_version,
                                 package,
                                 pocket,
+                                stats["component"],
                                 arch,
                                 stats["full_version"],
                                 stats["date_published"],
                                 stats["date_published_formatted"],
                                 stats["published_age"],
                                 stats["link"],
                                 stats["build_link"],
@@ -109,21 +112,31 @@
         # the package publish time
         launchpad = Launchpad.login_anonymously(
             "ubuntu-package-status", "production", version="devel"
         )
         ubuntu = launchpad.distributions["ubuntu"]
         ubuntu_archive = ubuntu.main_archive
 
+        is_pocket_ppa = False
+        if pocket.startswith("ppa:"):
+            is_pocket_ppa = True
+            ppa_owner_and_name = pocket.replace("ppa:", "")
+            ppa_owner, ppa_name = ppa_owner_and_name.split("/")
+            ubuntu_archive = launchpad.people[ppa_owner].getPPAByName(name=ppa_name)
+            archive_pocket = "Release"  # PPAs only have a release pocket
+        else:
+            archive_pocket = pocket
+
         lp_series = ubuntu.getSeries(name_or_version=ubuntu_version)
         lp_arch_series = lp_series.getDistroArchSeries(archtag=package_architecture)
 
         package_published_binaries = ubuntu_archive.getPublishedBinaries(
             exact_match=True,
             binary_name=package,
-            pocket=pocket,
+            pocket=archive_pocket,
             distro_arch_series=lp_arch_series,
             status="Published",
             order_by_date=True,
         )
 
         if len(package_published_binaries) > 0:
             package_published_binary = package_published_binaries[0]
@@ -160,28 +173,30 @@
                 # A negative timedelta means the time is in the future; this will be
                 # due to inconsistent clocks across systems, so assume that there is no
                 # delta
                 published_age = timedelta()
             published_age = humanize.naturaltime(published_age)
 
             package_stats["published_age"] = published_age
+            package_stats["component"] = package_published_binary.component_name
+
 
     except Exception as e:
         logging.error(
             "Error querying launchpad API: %s. \n " "We will retry. \n", str(e)
         )
 
     return {"package": package,
             "pocket": pocket,
             "ubuntu_version": ubuntu_version,
             "architecture": package_architecture,
             "status": package_stats}
 
 
-def initialize_package_stats_dict(package_config, package_architectures=["amd64"]):
+def initialize_package_stats_dict(package_config, package_architectures=["amd64"], ppas=[]):
     package_status = dict()
 
     ubuntu_versions = package_config.get("ubuntu-versions", {})
 
     # initialise package status
     for ubuntu_version, packages in ubuntu_versions.items():
         package_list = packages.get("packages", [])
@@ -193,27 +208,36 @@
                 package_status[ubuntu_version][package].setdefault(
                     pocket, defaultdict(dict)
                 )
                 for package_architecture in package_architectures:
                     package_status[ubuntu_version][package][pocket].setdefault(
                         package_architecture, defaultdict(dict)
                     )
+            for ppa in ppas:
+                package_status[ubuntu_version][package].setdefault(
+                    ppa, defaultdict(dict)
+                )
+                for package_architecture in package_architectures:
+                    package_status[ubuntu_version][package][ppa].setdefault(
+                        package_architecture, defaultdict(dict)
+                    )
 
     return package_status
 
 
-def get_status_for_all_packages(package_config, package_architectures=["amd64"]):
-    package_statuses = initialize_package_stats_dict(package_config, package_architectures)
+def get_status_for_all_packages(package_config, package_architectures=["amd64"], ppas=[]):
+    package_statuses = initialize_package_stats_dict(package_config, package_architectures, ppas)
     ubuntu_version_package_pocket_architecture_combinations = []
     for ubuntu_version, packages in package_statuses.items():
         # find all possible combinations of pocket, architecture and package name and create parallel jobs to query
         # launchpad for details on that package arch and pocket
         package_names = packages.keys()
         pockets = ARCHIVE_POCKETS
-
+        if ppas:
+            pockets.extend(ppas)
         # create a list of tuples of all combinations
         possible_combinations = list(product([ubuntu_version], package_names, pockets, package_architectures))
         ubuntu_version_package_pocket_architecture_combinations.extend(possible_combinations)
 
     n_jobs = -1
     single_package_statuses = Parallel(n_jobs=n_jobs)(
         get_status_for_single_package_by_pocket_and_architecture(ubuntu_version_name,
@@ -244,33 +268,51 @@
         " When using the ubuntu-package-status snap this"
         " config must reside under $HOME."
         if os.environ.get("SNAP", None)
         else ""
     ),
 )
 @click.option(
-    "--series", help='the Ubuntu series eg. "20.04" or "focal"', required=False, default=None
+    "--series",
+    "series",
+    multiple=True,
+    help="The Ubuntu series eg. '20.04' or 'focal'."
+    "This option can be specified multiple times.",
+    required=False,
+    default=[],
+
 )
 @click.option(
-    "--package-name", "package_names", multiple=True, help='Binary package name', required=False, default=[]
+    "--package-name",
+    "package_names",
+    multiple=True,
+    help="Binary package name"
+    "This option can be specified multiple times.",
+    required=False,
+    default=[]
 )
 @click.option(
     "--logging-level",
     type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR"]),
     required=False,
     default="ERROR",
     help="How detailed would you like the output.",
     show_default=True
 )
 @click.option(
-    "--config-skeleton", is_flag=True, default=False, help="Print example config.",
+    "--config-skeleton",
+    is_flag=True,
+    default=False,
+    help="Print example config.",
     show_default=True
 )
 @click.option(
-    "--output-format", type=click.Choice(["TXT", "CSV", "JSON"]), default="TXT",
+    "--output-format",
+    type=click.Choice(["TXT", "CSV", "JSON"]),
+    default="TXT",
     show_default=True
 )
 @click.option(
     "--package-architecture", "package_architectures",
     help="The architecture to use when querying package "
     "version in the archive. We use this in our Launchpad "
     'query to query either "source" package or "amd64" package '
@@ -280,22 +322,34 @@
     "the source package. The default is amd64. "
     "This option can be specified multiple times.",
     required=True,
     multiple=True,
     default=["amd64"],
     show_default=True
 )
+@click.option(
+    "--ppa",
+    "ppas",
+    required=False,
+    multiple=True,
+    type=click.STRING,
+    help="Additional PPAs that you wish to query for package version status."
+    "Expected format is "
+    "ppa:'%LAUNCHPAD_USERNAME%/%PPA_NAME%' eg. ppa:philroche/cloud-init"
+    "Multiple --ppa options can be specified",
+    default=[]
+)
 @click.pass_context
 def ubuntu_package_status(
-    ctx, config, series, package_names, logging_level, config_skeleton, output_format, package_architectures
+    ctx, config, series, package_names, logging_level, config_skeleton, output_format, package_architectures, ppas
 ):
-    # type: (Dict, Text, Text, bool, Text, Text) -> None
+    # type: (Dict, List[Text], List[Text], bool, Text, List[Text], List[Text]) -> None
     """
     Watch specified packages in the ubuntu archive for transition between
-    archive pockets. Useful when waiting for a package update to be published.
+    archive pockets/PPAs. Useful when waiting for a package update to be published.
 
     Usage:
     python ubuntu_package_status.py \
     --config="your-ubuntu-package-status-config.yaml"
     """
 
     # We log to stderr so that a shell calling this will not have logging
@@ -311,24 +365,23 @@
         with open(config, "r") as config_file:
             package_config = yaml.safe_load(config_file)
             if config_skeleton:
                 output = yaml.dump(package_config, Dumper=yaml.Dumper)
                 print(output)
                 exit(0)
     else:
+        # create a dict for each series specified
         package_config = {
-            'ubuntu-versions':
-                {
-                    series:
-                        {
-                            'packages': package_names
-                        }
-                }
+            'ubuntu-versions': {}
         }
+        for individual_series in series:
+            package_config['ubuntu-versions'][individual_series] = {
+                'packages': package_names
+            }
 
     # Initialise all package version
-    package_status = get_status_for_all_packages(package_config, package_architectures)
+    package_status = get_status_for_all_packages(package_config, package_architectures, list(ppas))
     print_package_status(package_status, output_format)
 
 
 if __name__ == "__main__":
     ubuntu_package_status(obj={})
```

### Comparing `ubuntu-package-status-0.0.7/src/ubuntu_package_status.egg-info/SOURCES.txt` & `ubuntu-package-status-0.1.0/src/ubuntu_package_status.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 src/requirements.txt
-src/ubuntu_package_status/20220202-cnewcomer.yaml
 src/ubuntu_package_status/__init__.py
 src/ubuntu_package_status/dist-config.yaml
-src/ubuntu_package_status/linux-fips-focal-config.yaml
+src/ubuntu_package_status/gke-kernel-config.yaml
 src/ubuntu_package_status/ubuntu_package_status.py
 src/ubuntu_package_status.egg-info/PKG-INFO
 src/ubuntu_package_status.egg-info/SOURCES.txt
 src/ubuntu_package_status.egg-info/dependency_links.txt
 src/ubuntu_package_status.egg-info/entry_points.txt
 src/ubuntu_package_status.egg-info/requires.txt
 src/ubuntu_package_status.egg-info/top_level.txt
```

