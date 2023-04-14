# Comparing `tmp/slpkg-4.7.6.tar.gz` & `tmp/slpkg-4.7.8.tar.gz`

## Comparing `slpkg-4.7.6.tar` & `slpkg-4.7.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:54:05.000000 slpkg-4.7.6/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-06 16:45:48.000000 slpkg-4.7.6/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-06 16:45:48.000000 slpkg-4.7.6/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      793 2023-04-06 16:45:48.000000 slpkg-4.7.6/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-06 16:45:48.000000 slpkg-4.7.6/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-06 16:45:48.000000 slpkg-4.7.6/filelists/README
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-06 16:45:48.000000 slpkg-4.7.6/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-06 16:45:48.000000 slpkg-4.7.6/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-06 16:45:48.000000 slpkg-4.7.6/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4281 2023-04-06 16:45:48.000000 slpkg-4.7.6/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-06 16:45:48.000000 slpkg-4.7.6/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6655 2023-04-06 16:45:48.000000 slpkg-4.7.6/README.rst
--rw-r--r--   0 dslackw   (1000) users      (100)       58 2023-04-06 16:45:48.000000 slpkg-4.7.6/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8949 2023-04-06 16:45:48.000000 slpkg-4.7.6/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      273 2023-04-06 16:45:48.000000 slpkg-4.7.6/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     2456 2023-04-06 16:45:48.000000 slpkg-4.7.6/configs/slpkg.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2153 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2269 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1251 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      272 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      588 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1242 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2436 2023-04-06 16:45:48.000000 slpkg-4.7.6/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-06 16:45:48.000000 slpkg-4.7.6/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-06 16:45:48.000000 slpkg-4.7.6/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    44396 2023-04-06 16:45:48.000000 slpkg-4.7.6/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     7264 2023-04-06 16:45:48.000000 slpkg-4.7.6/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     8039 2023-04-06 16:45:48.000000 slpkg-4.7.6/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-06 16:45:48.000000 slpkg-4.7.6/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-06 16:45:48.000000 slpkg-4.7.6/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1850 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6792 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9818 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    62222 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    24339 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2515 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     4499 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    14578 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)      958 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3983 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/form_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)    32105 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1791 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2177 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/models/models.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     7147 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6318 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5546 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/views/ascii.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4004 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9824 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3357 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1316 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4931 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      874 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/clean_logs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7625 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4072 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)    10204 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5580 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1522 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2558 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3142 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    29668 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1461 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3502 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3392 2023-04-06 16:45:48.000000 slpkg-4.7.6/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1311 2023-04-06 16:45:48.000000 slpkg-4.7.6/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:54:00.000000 slpkg-4.7.6/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-06 16:54:00.000000 slpkg-4.7.6/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1106 2023-04-06 16:54:00.000000 slpkg-4.7.6/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-06 16:54:00.000000 slpkg-4.7.6/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       53 2023-04-06 16:54:00.000000 slpkg-4.7.6/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     7897 2023-04-06 16:54:00.000000 slpkg-4.7.6/slpkg.egg-info/PKG-INFO
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-06 16:45:48.000000 slpkg-4.7.6/tools/gen_sbo_txt.sh
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-06 16:45:48.000000 slpkg-4.7.6/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)    11470 2023-04-06 16:45:48.000000 slpkg-4.7.6/bin/slpkg_new-configs
--rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-06 16:45:48.000000 slpkg-4.7.6/bin/slpkg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:55:04.000000 slpkg-4.7.8/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/README
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:50:47.000000 slpkg-4.7.8/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-14 09:46:56.000000 slpkg-4.7.8/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-14 09:46:56.000000 slpkg-4.7.8/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-14 09:46:56.000000 slpkg-4.7.8/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4281 2023-04-14 09:46:56.000000 slpkg-4.7.8/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-14 09:46:56.000000 slpkg-4.7.8/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     8312 2023-04-14 09:53:51.000000 slpkg-4.7.8/README.rst
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-14 09:46:56.000000 slpkg-4.7.8/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8603 2023-04-14 09:46:56.000000 slpkg-4.7.8/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-14 09:46:56.000000 slpkg-4.7.8/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     3267 2023-04-14 09:46:56.000000 slpkg-4.7.8/configs/slpkg.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2394 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1894 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      588 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1590 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-14 09:46:56.000000 slpkg-4.7.8/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-14 09:46:56.000000 slpkg-4.7.8/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    44892 2023-04-14 09:46:56.000000 slpkg-4.7.8/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8987 2023-04-14 09:46:56.000000 slpkg-4.7.8/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9918 2023-04-14 09:46:56.000000 slpkg-4.7.8/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-14 09:46:56.000000 slpkg-4.7.8/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-14 09:46:56.000000 slpkg-4.7.8/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1954 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9717 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    62222 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    24043 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2488 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    14874 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1042 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3983 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/form_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    32658 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1791 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2246 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/models/models.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     7067 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6319 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5523 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/ascii.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4043 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9794 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3055 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1344 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5311 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/clean_logs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6613 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3970 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11019 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5690 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1521 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2617 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3136 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    30270 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1470 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3061 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2872 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1363 2023-04-14 09:46:56.000000 slpkg-4.7.8/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1106 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     9576 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/PKG-INFO
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-14 09:46:56.000000 slpkg-4.7.8/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/bin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)    11470 2023-04-14 09:46:56.000000 slpkg-4.7.8/bin/slpkg_new-configs
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-14 09:46:56.000000 slpkg-4.7.8/bin/slpkg
```

### Comparing `slpkg-4.7.6/filelists/multilib/README.ERIC` & `slpkg-4.7.8/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/filelists/multilib/README` & `slpkg-4.7.8/filelists/multilib/README`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 You will find the file README.ERIC for this purpose, or refer directly to:
 http://www.slackware.com/~alien/multilib/
 
 In this folder, there are two lists, as Eric says, you should install first the glibc packages
 and then the 32-bit compatibility packages. First, edit the '/etc/slpkg/repositories.toml' file
 and enable the 'multilib' repository and then:
 
+  $ slpkg update --bin-repo=multilib
+
   $ slpkg install glibc_packages.pkgs --reinstall --bin-repo=multilib
 
   and
 
   $ slpkg install compat32.pkgs --bin-repo=multilib
 
 Please read README.ERIC for more or visit the site as I say above.
```

### Comparing `slpkg-4.7.6/filelists/multilib/compat32.pkgs` & `slpkg-4.7.8/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slackbuild/slack-desc` & `slpkg-4.7.8/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slackbuild/slpkg.SlackBuild` & `slpkg-4.7.8/slackbuild/slpkg.SlackBuild`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/README.rst` & `slpkg-4.7.8/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 About
 -----
 
 Slpkg is a software package manager that installs, updates and removes packages on `Slackware <http://www.slackware.com/>`_-based systems.
 It automatically calculates dependencies and figures out what things need to happen to install packages. 
 Slpkg makes it easier to manage groups of machines without the need for manual updates.
 
-Slpkg works in accordance with the standards of the `SlackBuilds.org <https://www.slackbuilds.org>`_ organization to build packages. 
+Slpkg works in accordance with the standards of the `SlackBuilds.org <https://www.slackbuilds.org>`__ organization to build packages. 
 It also uses the Slackware Linux instructions for installing, upgrading or removing packages.
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_package.png
     :target: https://gitlab.com/dslackw/slpkg
 
 
 Requirements
@@ -23,20 +23,20 @@
     SQLAlchemy >= 1.4.46
     pythondialog >= 3.5.3
     progress >= 1.6
 
 Install
 -------
 
-Install from the official third-party `SBo repository <https://slackbuilds.org/repository/15.0/system/slpkg/>`_ or directly from source:
+Install it from the official third-party `SlackBuilds.org <https://slackbuilds.org/repository/15.0/system/slpkg/>`__ repository or directly from source:
 
 .. code-block:: bash
 
-    $ tar xvf slpkg-4.7.6.tar.gz
-    $ cd slpkg-4.7.6
+    $ tar xvf slpkg-4.7.8.tar.gz
+    $ cd slpkg-4.7.8
     $ ./install.sh
 
 Screenshots
 -----------
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png
     :target: https://gitlab.com/dslackw/slpkg
@@ -97,14 +97,79 @@
         -v, --version                 Print version and exit.
 
    If you need more information try to use slpkg manpage.
    Extra help for the commands, use: 'slpkg help [command]'.
    Edit the config file in the /etc/slpkg/slpkg.toml or 'slpkg configs'.
 
 
+How to start
+------------
+
+If you are going to use only the `SlackBuilds.org <https://slackbuilds.org/>`__ repository, you don't need to edit the
+:code:`/etc/slpkg/repositories.toml` file, otherwise edit the file and set :code:`true` the repositories you want.
+
+The second step is to update the package lists and install the data to the database, just run:
+
+.. code-block:: bash
+
+    $ slpkg update
+
+or for binary repositories:
+
+.. code-block:: bash
+
+    $ slpkg update --bin-repo='*'
+
+Now you are ready to start!
+
+To install a package from the `SlackBuilds.org <https://slackbuilds.org/>`__ or `Ponce <https://cgit.ponce.cc/slackbuilds/>`_ repository, run:
+
+.. code-block:: bash
+
+    $ slpkg install <package_name>
+
+or from a binary repository:
+
+.. code-block:: bash
+
+    $ slpkg install <package_name> --bin-repo=<repo_name>
+
+You can install a whole repository with the command:
+
+.. code-block:: bash
+
+    $ slpkg install '*' --bin-repo=<repository_name> --resolve-off
+
+Note: Apply the option '--resolve-off' to speed up the process, if the repository has no references to the dependencies.
+
+To remove a package with the dependencies:
+
+.. code-block:: bash
+
+    $ slpkg remove <package_name>
+
+If you wan to search a package from all binaries repositories, run:
+
+.. code-block:: bash
+
+    $ slpkg search <package_name> --bin-repo='*'
+
+Edit the configuration :code:`/etc/slpkg/slpkg.toml` file:
+
+.. code-block:: bash
+
+    $ slpkg configs
+
+
+For further information, please read the manpage:
+
+.. code-block:: bash
+
+    $ man slpkg
+
 
 Configuration files
 -------------------
 
 .. code-block:: bash
 
     /etc/slpkg/slpkg.toml
@@ -153,14 +218,19 @@
 ------
 
 If you feel satisfied with this project and want to thanks me make a donation.
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/donate/paypaldonate.png
    :target: https://www.paypal.me/dslackw
 
+Report bugs
+-----------
+
+Please report any issue here: `Issues <https://gitlab.com/dslackw/slpkg/-/issues>`_
+
 
 Copyright
 ---------
 
 - Copyright 2014-2023 © Dimitris Zlatanidis.
 - Slackware® is a Registered Trademark of Patrick Volkerding. 
 - Linux is a Registered Trademark of Linus Torvalds.
```

### Comparing `slpkg-4.7.6/configs/repositories.toml` & `slpkg-4.7.8/configs/repositories.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,197 +11,197 @@
 # Note: Before using a repository, make sure you have read about it.   #
 #       Some repositories are for -current only. Change the mirror if  #
 #       it is necessary. The mirror should end with a slash '/'.       #
 ########################################################################
 
 [REPOSITORIES]
 
-  # SBo Repository for Slackware 15.0 stable.
-  SBO_REPO_NAME = "sbo"
-  SBO_REPO_MIRROR = "https://slackbuilds.org/slackbuilds/15.0/"
-  SBO_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
-  SBO_REPO_CHANGELOG = "ChangeLog.txt"
-  SBO_REPO_TAR_SUFFIX = ".tar.gz"
-  SBO_REPO_TAG = "_SBo"  # Default repo TAG.
-  SBO_REPO_PATCH_TAG = ""  # Patch the TAG.
-
-  # Ponce Repository for Slackware -current.
-  PONCE_REPO = false
-  PONCE_REPO_NAME = "ponce"
-  PONCE_REPO_MIRROR = "https://cgit.ponce.cc/slackbuilds/plain/"
-  PONCE_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
-  PONCE_REPO_CHANGELOG = "ChangeLog.txt"
-  PONCE_REPO_TAG = "_SBo"  # Default repo TAG.
-  PONCE_REPO_PATCH_TAG = ""  # Patch the TAG.
-
-  # Official repository for Slackware x86_64 15.0 stable.
-  # For Slackware x86_64 -current:
-  # https://slackware.uk/slackware/slackware64-current/
-  SLACK_REPO = false
-  SLACK_REPO_NAME = "slack"
-  SLACK_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
-  SLACK_REPO_PACKAGES = "PACKAGES.TXT"
-  SLACK_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SLACK_REPO_CHANGELOG = "ChangeLog.txt"
-  SLACK_REPO_TAG = ""
-
-  # Official repository for Slackware patches x86_64 15.0 stable.
-  # For Slackware patches x86_64 -current:
-  # https://slackware.uk/slackware/slackware64-current/extra/
-  SLACK_EXTRA_REPO = false
-  SLACK_EXTRA_REPO_NAME = "slack_extra"
-  SLACK_EXTRA_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
-  SLACK_EXTRA_REPO_PACKAGES_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/extra/"
-  SLACK_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
-  SLACK_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SLACK_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
-  SLACK_EXTRA_REPO_TAG = ""
-
-  # Official repository for Slackware patches x86_64 15.0 stable.
-  # For Slackware patches x86_64 -current:
-  # https://slackware.uk/slackware/slackware64-current/patches/
-  SLACK_PATCHES_REPO = false
-  SLACK_PATCHES_REPO_NAME = "slack_patches"
-  SLACK_PATCHES_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
-  SLACK_PATCHES_REPO_PACKAGES_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/patches/"
-  SLACK_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
-  SLACK_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SLACK_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
-  SLACK_PATCHES_REPO_TAG = ""
-
-  # AlienBob Repository for Slackware x86_64 15.0 stable.
-  # For Slackware x86_64 -current:
-  # http://slackware.uk/people/alien/sbrepos/current/x86_64/
-  ALIEN_REPO = false
-  ALIEN_REPO_NAME = "alien"
-  ALIEN_REPO_MIRROR = "https://slackware.nl/people/alien/sbrepos/"
-  ALIEN_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/sbrepos/15.0/x86_64/"
-  ALIEN_REPO_PACKAGES = "PACKAGES.TXT"
-  ALIEN_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  ALIEN_REPO_CHANGELOG = "ChangeLog.txt"
-  ALIEN_REPO_TAG = "alien"
-
-  # Multilib Repository for Slackware x86_64 15.0 stable.
-  # For Slackware x86_64 -current:
-  # https://slackware.nl/people/alien/multilib/current/
-  MULTILIB_REPO = false
-  MULTILIB_REPO_NAME = "multilib"
-  MULTILIB_REPO_MIRROR = "https://slackware.nl/people/alien/multilib/"
-  MULTILIB_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/multilib/15.0/"
-  MULTILIB_REPO_PACKAGES = "PACKAGES.TXT"
-  MULTILIB_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  MULTILIB_REPO_CHANGELOG = "ChangeLog.txt"
-  MULTILIB_REPO_TAG = "alien"
-
-  # Restricted Repository for Slackware x86_64 15.0 stable.
-  # For Slackware x86_64 -current:
-  # https://slackware.nl/people/alien/restricted_sbrepos/current/x86_64/
-  RESTRICTED_REPO = false
-  RESTRICTED_REPO_NAME = "restricted"
-  RESTRICTED_REPO_MIRROR = "https://slackware.nl/people/alien/restricted_sbrepos/"
-  RESTRICTED_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/restricted_sbrepos/15.0/x86_64/"
-  RESTRICTED_REPO_PACKAGES = "PACKAGES.TXT"
-  RESTRICTED_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  RESTRICTED_REPO_CHANGELOG = "ChangeLog.txt"
-  RESTRICTED_REPO_TAG = "alien"
-
-  # Gnome Repository for Slackware x86_64 15.0 stable.
-  # For Slackware x86_64 -current:
-  # https://reddoglinux.ddns.net/linux/gnome/43.x/x86_64/
-  GNOME_REPO = false
-  GNOME_REPO_NAME = "gnome"
-  GNOME_REPO_MIRROR = "https://reddoglinux.ddns.net/linux/gnome/41.x/x86_64/"
-  GNOME_REPO_PACKAGES = "PACKAGES.TXT"
-  GNOME_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  GNOME_REPO_CHANGELOG = "ChangeLog.txt"
-  GNOME_REPO_TAG = "gfs"
-
-  # MATE Repository for Slackware x86_64 15.0 stable.
-  # For Slackware x86_64 -current:
-  # https://slackware.uk/msb/current/1.26/x86_64/
-  MSB_REPO = false
-  MSB_REPO_NAME = "msb"
-  MSB_REPO_MIRROR = "https://slackware.uk/msb/"
-  MSB_REPO_PACKAGES_MIRROR = 'https://slackware.uk/msb/15.0/1.26/x86_64/'
-  MSB_REPO_PACKAGES = "PACKAGES.TXT"
-  MSB_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  MSB_REPO_CHANGELOG = "ChangeLog.txt"
-  MSB_REPO_TAG = "msb"
-
-  # Cinnamon Repository for Slackware x86_64 15.0 stable.
-  # For Slackware x86_64 -current:
-  # https://slackware.uk/csb/current/x86_64/
-  CSB_REPO = false
-  CSB_REPO_NAME = "csb"
-  CSB_REPO_MIRROR = "https://slackware.uk/csb/"
-  CSB_REPO_PACKAGES_MIRROR = 'https://slackware.uk/csb/15.0/x86_64/'
-  CSB_REPO_PACKAGES = "PACKAGES.TXT"
-  CSB_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  CSB_REPO_CHANGELOG = "ChangeLog.txt"
-  CSB_REPO_TAG = "csb"
-
-  # Conraid Repository for Slackware x86_64 -current.
-  CONRAID_REPO = false
-  CONRAID_REPO_NAME = "conraid"
-  CONRAID_REPO_MIRROR = "https://slack.conraid.net/repository/slackware64-current/"
-  CONRAID_REPO_PACKAGES = "PACKAGES.TXT"
-  CONRAID_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  CONRAID_REPO_CHANGELOG = "ChangeLog.txt"
-  CONRAID_REPO_TAG = "cf"
-
-  # Slackonly Repository for Slackware x86_64 15.0 stable.
-  # For Slackware x86_64 -current:
-  # https://packages.slackonly.com/pub/packages/current-x86_64/
-  SLACKONLY_REPO = false
-  SLACKONLY_REPO_NAME = "slackonly"
-  SLACKONLY_REPO_MIRROR = "https://packages.slackonly.com/pub/packages/15.0-x86_64/"
-  SLACKONLY_REPO_PACKAGES = "PACKAGES.TXT"
-  SLACKONLY_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SLACKONLY_REPO_CHANGELOG = "ChangeLog.txt"
-  SLACKONLY_REPO_TAG = "slonly"
-
-  # Repository for Salix OS x86_64 15.0 stable.
-  SALIXOS_REPO = false
-  SALIXOS_REPO_NAME = "salixos"
-  SALIXOS_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
-  SALIXOS_REPO_PACKAGES = "PACKAGES.TXT"
-  SALIXOS_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SALIXOS_REPO_CHANGELOG = "ChangeLog.txt"
-  SALIXOS_REPO_TAG = ""
-
-  # Repository for Salix OS x86_64 15.0 stable.
-  SALIXOS_EXTRA_REPO = false
-  SALIXOS_EXTRA_REPO_NAME = "salixos_extra"
-  SALIXOS_EXTRA_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
-  SALIXOS_EXTRA_REPO_PACKAGES_MIRROR = 'https://download.salixos.org/x86_64/slackware-15.0/extra/'
-  SALIXOS_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
-  SALIXOS_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SALIXOS_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
-  SALIXOS_EXTRA_REPO_TAG = ""
-
-  # Repository for Salix OS x86_64 15.0 stable.
-  SALIXOS_PATCHES_REPO = false
-  SALIXOS_PATCHES_REPO_NAME = "salixos_patches"
-  SALIXOS_PATCHES_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
-  SALIXOS_PATCHES_REPO_PACKAGES_MIRROR = 'https://download.salixos.org/x86_64/slackware-15.0/patches/'
-  SALIXOS_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
-  SALIXOS_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SALIXOS_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
-  SALIXOS_PATCHES_REPO_TAG = "_slack15.0"
-
-  # Repository for Slackel OS x86_64 -current.
-  SLACKEL_REPO = false
-  SLACKEL_REPO_NAME = "slackel"
-  SLACKEL_REPO_MIRROR = "http://www.slackel.gr/repo/x86_64/current/"
-  SLACKEL_REPO_PACKAGES = "PACKAGES.TXT"
-  SLACKEL_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SLACKEL_REPO_CHANGELOG = "ChangeLog.txt"
-  SLACKEL_REPO_TAG = "dj"
-
-  # Slint Repository for Slackware x86_64 15.0 stable.
-  SLINT_REPO = false
-  SLINT_REPO_NAME = "slint"
-  SLINT_REPO_MIRROR = "https://slackware.uk/slint/x86_64/slint-15.0/"
-  SLINT_REPO_PACKAGES = "PACKAGES.TXT"
-  SLINT_REPO_CHECKSUMS = "CHECKSUMS.md5"
-  SLINT_REPO_CHANGELOG = "ChangeLog.txt"
-  SLINT_REPO_TAG = "slint"
+# SBo Repository for Slackware 15.0 stable.
+SBO_REPO_NAME = "sbo"
+SBO_REPO_MIRROR = "https://slackbuilds.org/slackbuilds/15.0/"
+SBO_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
+SBO_REPO_CHANGELOG = "ChangeLog.txt"
+SBO_REPO_TAR_SUFFIX = ".tar.gz"
+SBO_REPO_TAG = "_SBo"  # Default repo TAG.
+SBO_REPO_PATCH_TAG = ""  # Patch the TAG.
+
+# Ponce Repository for Slackware -current.
+PONCE_REPO = false
+PONCE_REPO_NAME = "ponce"
+PONCE_REPO_MIRROR = "https://cgit.ponce.cc/slackbuilds/plain/"
+PONCE_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
+PONCE_REPO_CHANGELOG = "ChangeLog.txt"
+PONCE_REPO_TAG = "_SBo"  # Default repo TAG.
+PONCE_REPO_PATCH_TAG = ""  # Patch the TAG.
+
+# Official repository for Slackware x86_64 15.0 stable.
+# For Slackware x86_64 -current:
+# https://slackware.uk/slackware/slackware64-current/
+SLACK_REPO = false
+SLACK_REPO_NAME = "slack"
+SLACK_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
+SLACK_REPO_PACKAGES = "PACKAGES.TXT"
+SLACK_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SLACK_REPO_CHANGELOG = "ChangeLog.txt"
+SLACK_REPO_TAG = ""
+
+# Official repository for Slackware patches x86_64 15.0 stable.
+# For Slackware patches x86_64 -current:
+# https://slackware.uk/slackware/slackware64-current/extra/
+SLACK_EXTRA_REPO = false
+SLACK_EXTRA_REPO_NAME = "slack_extra"
+SLACK_EXTRA_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
+SLACK_EXTRA_REPO_PACKAGES_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/extra/"
+SLACK_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
+SLACK_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SLACK_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
+SLACK_EXTRA_REPO_TAG = ""
+
+# Official repository for Slackware patches x86_64 15.0 stable.
+# For Slackware patches x86_64 -current:
+# https://slackware.uk/slackware/slackware64-current/patches/
+SLACK_PATCHES_REPO = false
+SLACK_PATCHES_REPO_NAME = "slack_patches"
+SLACK_PATCHES_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
+SLACK_PATCHES_REPO_PACKAGES_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/patches/"
+SLACK_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
+SLACK_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SLACK_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
+SLACK_PATCHES_REPO_TAG = ""
+
+# AlienBob Repository for Slackware x86_64 15.0 stable.
+# For Slackware x86_64 -current:
+# http://slackware.uk/people/alien/sbrepos/current/x86_64/
+ALIEN_REPO = false
+ALIEN_REPO_NAME = "alien"
+ALIEN_REPO_MIRROR = "https://slackware.nl/people/alien/sbrepos/"
+ALIEN_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/sbrepos/15.0/x86_64/"
+ALIEN_REPO_PACKAGES = "PACKAGES.TXT"
+ALIEN_REPO_CHECKSUMS = "CHECKSUMS.md5"
+ALIEN_REPO_CHANGELOG = "ChangeLog.txt"
+ALIEN_REPO_TAG = "alien"
+
+# Multilib Repository for Slackware x86_64 15.0 stable.
+# For Slackware x86_64 -current:
+# https://slackware.nl/people/alien/multilib/current/
+MULTILIB_REPO = false
+MULTILIB_REPO_NAME = "multilib"
+MULTILIB_REPO_MIRROR = "https://slackware.nl/people/alien/multilib/"
+MULTILIB_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/multilib/15.0/"
+MULTILIB_REPO_PACKAGES = "PACKAGES.TXT"
+MULTILIB_REPO_CHECKSUMS = "CHECKSUMS.md5"
+MULTILIB_REPO_CHANGELOG = "ChangeLog.txt"
+MULTILIB_REPO_TAG = "alien"
+
+# Restricted Repository for Slackware x86_64 15.0 stable.
+# For Slackware x86_64 -current:
+# https://slackware.nl/people/alien/restricted_sbrepos/current/x86_64/
+RESTRICTED_REPO = false
+RESTRICTED_REPO_NAME = "restricted"
+RESTRICTED_REPO_MIRROR = "https://slackware.nl/people/alien/restricted_sbrepos/"
+RESTRICTED_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/restricted_sbrepos/15.0/x86_64/"
+RESTRICTED_REPO_PACKAGES = "PACKAGES.TXT"
+RESTRICTED_REPO_CHECKSUMS = "CHECKSUMS.md5"
+RESTRICTED_REPO_CHANGELOG = "ChangeLog.txt"
+RESTRICTED_REPO_TAG = "alien"
+
+# Gnome Repository for Slackware x86_64 15.0 stable.
+# For Slackware x86_64 -current:
+# https://reddoglinux.ddns.net/linux/gnome/43.x/x86_64/
+GNOME_REPO = false
+GNOME_REPO_NAME = "gnome"
+GNOME_REPO_MIRROR = "https://reddoglinux.ddns.net/linux/gnome/41.x/x86_64/"
+GNOME_REPO_PACKAGES = "PACKAGES.TXT"
+GNOME_REPO_CHECKSUMS = "CHECKSUMS.md5"
+GNOME_REPO_CHANGELOG = "ChangeLog.txt"
+GNOME_REPO_TAG = "gfs"
+
+# MATE Repository for Slackware x86_64 15.0 stable.
+# For Slackware x86_64 -current:
+# https://slackware.uk/msb/current/1.26/x86_64/
+MSB_REPO = false
+MSB_REPO_NAME = "msb"
+MSB_REPO_MIRROR = "https://slackware.uk/msb/"
+MSB_REPO_PACKAGES_MIRROR = 'https://slackware.uk/msb/15.0/1.26/x86_64/'
+MSB_REPO_PACKAGES = "PACKAGES.TXT"
+MSB_REPO_CHECKSUMS = "CHECKSUMS.md5"
+MSB_REPO_CHANGELOG = "ChangeLog.txt"
+MSB_REPO_TAG = "msb"
+
+# Cinnamon Repository for Slackware x86_64 15.0 stable.
+# For Slackware x86_64 -current:
+# https://slackware.uk/csb/current/x86_64/
+CSB_REPO = false
+CSB_REPO_NAME = "csb"
+CSB_REPO_MIRROR = "https://slackware.uk/csb/"
+CSB_REPO_PACKAGES_MIRROR = 'https://slackware.uk/csb/15.0/x86_64/'
+CSB_REPO_PACKAGES = "PACKAGES.TXT"
+CSB_REPO_CHECKSUMS = "CHECKSUMS.md5"
+CSB_REPO_CHANGELOG = "ChangeLog.txt"
+CSB_REPO_TAG = "csb"
+
+# Conraid Repository for Slackware x86_64 -current.
+CONRAID_REPO = false
+CONRAID_REPO_NAME = "conraid"
+CONRAID_REPO_MIRROR = "https://slack.conraid.net/repository/slackware64-current/"
+CONRAID_REPO_PACKAGES = "PACKAGES.TXT"
+CONRAID_REPO_CHECKSUMS = "CHECKSUMS.md5"
+CONRAID_REPO_CHANGELOG = "ChangeLog.txt"
+CONRAID_REPO_TAG = "cf"
+
+# Slackonly Repository for Slackware x86_64 15.0 stable.
+# For Slackware x86_64 -current:
+# https://packages.slackonly.com/pub/packages/current-x86_64/
+SLACKONLY_REPO = false
+SLACKONLY_REPO_NAME = "slackonly"
+SLACKONLY_REPO_MIRROR = "https://packages.slackonly.com/pub/packages/15.0-x86_64/"
+SLACKONLY_REPO_PACKAGES = "PACKAGES.TXT"
+SLACKONLY_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SLACKONLY_REPO_CHANGELOG = "ChangeLog.txt"
+SLACKONLY_REPO_TAG = "slonly"
+
+# Repository for Salix OS x86_64 15.0 stable.
+SALIXOS_REPO = false
+SALIXOS_REPO_NAME = "salixos"
+SALIXOS_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
+SALIXOS_REPO_PACKAGES = "PACKAGES.TXT"
+SALIXOS_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SALIXOS_REPO_CHANGELOG = "ChangeLog.txt"
+SALIXOS_REPO_TAG = ""
+
+# Repository for Salix OS x86_64 15.0 stable.
+SALIXOS_EXTRA_REPO = false
+SALIXOS_EXTRA_REPO_NAME = "salixos_extra"
+SALIXOS_EXTRA_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
+SALIXOS_EXTRA_REPO_PACKAGES_MIRROR = 'https://download.salixos.org/x86_64/slackware-15.0/extra/'
+SALIXOS_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
+SALIXOS_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SALIXOS_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
+SALIXOS_EXTRA_REPO_TAG = ""
+
+# Repository for Salix OS x86_64 15.0 stable.
+SALIXOS_PATCHES_REPO = false
+SALIXOS_PATCHES_REPO_NAME = "salixos_patches"
+SALIXOS_PATCHES_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
+SALIXOS_PATCHES_REPO_PACKAGES_MIRROR = 'https://download.salixos.org/x86_64/slackware-15.0/patches/'
+SALIXOS_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
+SALIXOS_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SALIXOS_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
+SALIXOS_PATCHES_REPO_TAG = "_slack15.0"
+
+# Repository for Slackel OS x86_64 -current.
+SLACKEL_REPO = false
+SLACKEL_REPO_NAME = "slackel"
+SLACKEL_REPO_MIRROR = "http://www.slackel.gr/repo/x86_64/current/"
+SLACKEL_REPO_PACKAGES = "PACKAGES.TXT"
+SLACKEL_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SLACKEL_REPO_CHANGELOG = "ChangeLog.txt"
+SLACKEL_REPO_TAG = "dj"
+
+# Slint Repository for Slackware x86_64 15.0 stable.
+SLINT_REPO = false
+SLINT_REPO_NAME = "slint"
+SLINT_REPO_MIRROR = "https://slackware.uk/slint/x86_64/slint-15.0/"
+SLINT_REPO_PACKAGES = "PACKAGES.TXT"
+SLINT_REPO_CHECKSUMS = "CHECKSUMS.md5"
+SLINT_REPO_CHANGELOG = "ChangeLog.txt"
+SLINT_REPO_TAG = "slint"
```

### Comparing `slpkg-4.7.6/tests/test_configs.py` & `slpkg-4.7.8/tests/test_configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,11 +34,15 @@
         self.assertEqual(True, self.configs.silent_mode)
         self.assertEqual(True, self.configs.ascii_characters)
         self.assertEqual(True, self.configs.ask_question)
         self.assertEqual(False, self.configs.parallel_downloads)
         self.assertEqual('*', self.configs.file_pattern)
         self.assertEqual('pixel', self.configs.progress_spinner)
         self.assertEqual('green', self.configs.spinner_color)
+        self.assertEqual('', self.configs.http_proxy_address)
+        self.assertEqual('', self.configs.socks_proxy_address)
+        self.assertEqual('', self.configs.proxy_username)
+        self.assertEqual('', self.configs.proxy_password)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `slpkg-4.7.6/tests/test_checks.py` & `slpkg-4.7.8/tests/test_checks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 import unittest
 from slpkg.checks import Check
-from slpkg.configs import Configs
-from slpkg.repositories import Repositories
+from slpkg.binaries.queries import BinQueries
 
 
 class TestPkgInstalled(unittest.TestCase):
 
     def setUp(self):
-        self.check = Check([])
-        self.configs = Configs()
-        self.repos = Repositories()
-        self.packages = ['fish', 'ranger', 'pycharm']
+        self.bin_queries = BinQueries('alien')
+        self.data = self.bin_queries.repository_data()
+        self.check = Check(['-B', '--bin-repo='], self.data)
+        self.packages = ['audacity', 'vlc', 'dnspython']
 
     def test_check_exists(self):
         self.assertIsNone(self.check.exists_in_the_database(self.packages))
 
     def test_check_unsupported(self):
         self.assertIsNone(self.check.is_package_unsupported(self.packages))
 
     def test_check_is_installed(self):
         self.assertIsNone(self.check.is_package_unsupported(self.packages))
 
-    def test_check_blacklist(self):
-        self.assertIsNone(self.check.is_blacklist(self.packages))
-
-    def test_check_is_empty(self):
-        self.assertIsNone(self.check.is_blacklist(self.packages))
-
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `slpkg-4.7.6/tests/test_sbo_queries.py` & `slpkg-4.7.8/tests/test_sbo_queries.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import unittest
 from slpkg.sbos.queries import SBoQueries
 
 
 class TestSBoQueries(unittest.TestCase):
 
     def setUp(self):
-        self.query = SBoQueries('slpkg')
+        self.sbo_queries = SBoQueries()
+        self.data: dict = self.sbo_queries.repository_data()
+        self.name: str = 'slpkg'
 
     def test_slackbuild(self):
-        self.assertEqual('slpkg', self.query.slackbuild())
+        self.assertTrue(True, self.data[self.name])
 
     def test_location(self):
-        self.assertEqual('system', self.query.location())
+        self.assertEqual('system', self.data[self.name][0])
 
-    def test_sources(self):
+    def test_sources_x86(self):
         self.assertEqual(['https://gitlab.com/dslackw/slpkg/-/archive'
-                         '/4.6.1/slpkg-4.6.1.tar.gz'], self.query.sources())
+                         '/4.7.6/slpkg-4.7.6.tar.gz'], self.data[self.name][3].split())
+
+    def test_sources_x86_64(self):
+        self.assertEqual([], self.data[self.name][4].split())
 
     def test_requires(self):
-        self.assertEqual(['SQLAlchemy', 'python3-pythondialog', 'python3-progress'], self.query.requires())
+        self.assertEqual(['SQLAlchemy', 'python3-pythondialog', 'python3-progress'], self.data[self.name][7].split())
 
     def test_version(self):
-        self.assertEqual('4.6.1', self.query.version())
+        self.assertEqual('4.7.6', self.data[self.name][2])
+
+    def test_checksum_x86(self):
+        self.assertListEqual(['26577e39fa7f58d9fa24fa24d91d1012'], self.data[self.name][5].split())
 
-    def test_checksum(self):
-        self.assertListEqual(['8f98a8f666f8772be205ce65214dd538'],
-                             self.query.checksum())
+    def test_checksum_x86_64(self):
+        self.assertListEqual([], self.data[self.name][6].split())
 
     def test_files(self):
-        self.assertEqual(5, len(self.query.files().split()))
+        self.assertEqual(5, len(self.data[self.name][1].split()))
 
     def test_description(self):
-        self.assertEqual('slpkg (Slackware Packaging Tool)',
-                         self.query.description())
-
-    def test_names(self):
-        self.assertIn('slpkg', self.query.sbos())
+        self.assertEqual('slpkg (Slackware Packaging Tool)', self.data[self.name][8])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `slpkg-4.7.6/tests/test_colors.py` & `slpkg-4.7.8/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/LICENSE` & `slpkg-4.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/install.sh` & `slpkg-4.7.8/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/ChangeLog.txt` & `slpkg-4.7.8/ChangeLog.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+4.7.8 - 12/04/203
+Added:
+- Module to support for Unix shell-style wildcards for blacklist (Thanks yo marav)
+- Supports proxies (Thanks to tpiszcze) #160
+Updated:
+- Config file for --reinstall option (Thanks to rizitis)
+- Improve speed
+
+4.7.7 - 07/04/2023
+Updated:
+- Improve speed (Replace multi SQL queries)
+Fixed:
+- For binaries double dependencies
+- For remove package version
+- Alignment for package name and version
+Added:
+- Slots '__slots__' to improve speed
+- Remove local repository data
+
 4.7.6 - 04/04/2023
 Fixed:
 - Upgrade packages with build numbers greater to >= 10
 Updated:
 - Indicate colour for upgradable packages
 - Upgrade packages by repository
 Added:
```

### Comparing `slpkg-4.7.6/man/slpkg.1` & `slpkg-4.7.8/man/slpkg.1`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH slpkg 1 "Orestiada, Greece" "slpkg 4.7.3" dslackw
+.TH slpkg 1 "Orestiada, Greece" "slpkg 4.7.8" dslackw
 .SH NAME
 .P
 slpkg \- Package manager utility for Slackware.
 .SH SYNOPSIS
 .P
 slpkg \c
 [\fICOMMAND\fR] [\fIOPTIONS\fR] [\fIFILELIST|PACKAGES...\fR]
@@ -110,15 +110,15 @@
 Tracking the packages dependencies.
 .RE
 .SH OPTIONS
 .P
 .B -y, --yes
 .RS
 Answer Yes to all questions. (to be used with: -u, update, -U, upgrade, -L, clean-logs, -b, build,
--i, install, -R, remove, -d, download,) (Not used with -R, remove, option removed for security reasons)
+-i, install, -R, remove, -d, download,)
 .RE
 .P
 .B -j, --jobs
 .RS
 Acceleration of SlackBuild scripts. When the \fB--jobs\fR flag is set, slpkg automatically detects the number
 of processors and enters it into the MAKEFLAGS variable. Some SlackBuilds fail when MAKEFLAGS is declared or
 the number of processors (-j) is greater than one. (to be used with: -U, upgrade, -b, build, -i, install)
@@ -211,14 +211,41 @@
 .Ve
 .RE
 .SH FILELIST|PACKAGES
 .P
 Instead of packages, you can pass a text file with suffix '.pkgs' and with the names of the packages. Example: '\fIslpkg install list.pkgs\fR'.
 Edit the config '/etc/slpkg/slpkg.toml' file to change the suffix if you want. You can use lists from others, like '.sqf' files.
 .RE
+.SH MUST YOU KNOW
+.P
+There are five indicators when some commands are used, for example:
+
+Cyan: To install, Yellow: To build, Grey: It's installed, Violet: For the upgrade, Red: To remove.
+
+When you use the install, build, upgrade or remove commands you should know that, if the package is installed then its
+color will change to gray, if the package is upgradeable then it will change to violet, and if it is not installed then
+its color will be cyan. Also, if you try to remove a package you will see the package color turns red.
+
+Example: If the package is already installed and the indicator color is grey and the option '\fB-r, --reinstall\fR' is not applied,
+the package will skip from the installation and you will see a message '(already installed)'.
+If the package is upgradeable, the installation will continue and the package will go to upgrade.
+
+For the upgrade command, you should know, that you can upgrade packages from different repositories, if you edit
+the '\fI/etc/slpkg/repositories.toml\fR' file and remove the repository tag. Then the slpkg can't recognize the repository of the packages.
+
+With the remove command, it's going to remove the dependencies if the package had installed with the '\fIslpkg install\fR' command,
+otherwise, the slpkg does not know the dependencies that are installed with the packages that going to remove.
+
+You can apply the asterisk '*' instead of a package, to matching all the packages from a repository. You can't apply
+an asterisk to the '\fB-B, --bin-repos=\fR' option, except for the '\fB-s, search\fR', '\fB-u, update\fR' and '\fB-c, check-updates\fR' commands.
+
+Command clean-data, removes the local repository data and the database data.
+
+Note: There is currently no function to indicate the packages if the colors are disabled.
+.RE
 .SH CONFIGURATION FILES
 .P
 Configuration file in the /etc/slpkg/slpkg.toml file.
 .P
 Repositories file in the /etc/slpkg/repositories.toml file.
 .P
 Blacklist file in the /etc/slpkg/blacklist.toml file.
@@ -226,8 +253,8 @@
 \fIslpkg_new-config\fR command it's managing the .new configuration files easily and fast. Move, copy or remove them.
 .RE
 .SH REPORT BUGS
 .P
 Please report any found to: https://gitlab.com/dslackw/slpkg/-/issues.
 .SH AUTHOR
 .P
-Dimitris Zlatanidis <d.zlatanidis@gmail.com>
+Dimitris Zlatanidis <dslackw@gmail.com>
```

### Comparing `slpkg-4.7.6/man/slpkg-fr.1` & `slpkg-4.7.8/man/slpkg-fr.1`

 * *Files 22% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 Suivre les dépendances des paquets.
 .RE
 .SH OPTIONS
 .P
 .B -y, --yes
 .RS
 Répondre \fBOui\fP à toutes les questions. (à utiliser avec: \fB-u, update, -U, upgrade, -L, clean-logs, -b, build,
--i, install, -R, remove, -d, download\fP) (Non utilisée avec \fB-R, remove\fP, option supprimée pour des raisons de sécurité)
+-i, install, -R, remove, -d, download\fP)
 .RE
 .P
 .B -j, --jobs
 .RS
 Accélération des scripts SlackBuild. Lorsque l'indicateur \fB--jobs\fP est activé, slpkg détecte automatiquement le nombre de
 de processeurs et le saisit dans la variable \fBMAKEFLAGS\fP. Certains SlackBuilds échouent lorsque \fBMAKEFLAGS\fP est déclaré ou que
 le nombre de processeurs (-j) est supérieur à 1. (à utiliser avec: \fB-U, upgrade, build, -i, install\fP)
@@ -206,14 +206,41 @@
 .Ve
 .RE
 .SH FILELIST|PACKAGES
 .P
 Au lieu de paquets, vous pouvez passer un fichier texte avec le suffixe '.pkgs' et les noms des paquets.  Exemple : 'slpkg install list.pkgs'.
 Éditer la configuration '/etc/slpkg/slpkg.toml' pour changer le suffixe si vous le souhaitez. Vous pouvez utiliser des listes provenant d'autres sources, avec des fichiers '.sqf'.
 .RE
+.SH A SAVOIR
+.P
+Il y a cinq indicateurs lorsque certaines commandes sont utilisées, par exemple :
+
+Cyan : Installer, Jaune : Pour construire, Gris : C'est installé, Violet : Pour la mise à jour, Rouge : Pour supprimer.
+
+Lorsque vous utilisez les commandes install, build, upgrade ou remove, vous devez savoir que si le paquet est installé, 
+sa couleur passera au gris, si le paquet peut être mis à niveau, il devient violet. Et s'il n'est pas installé alors 
+sa couleur sera cyan. De même, si vous essayez de supprimer un paquet, la couleur du paquet devient rouge.
+
+Exemple : Si le paquet est déjà installé, que la couleur de l'indicateur est grise et que l'option '\fB-r, --reinstall\fR' n'est pas appliquée,
+le paquetage ne sera pas installé et le message "(already installed)" s'affichera.
+Si le paquet peut être mis à niveau, l'installation se poursuivra et le paquet passera à la mise à niveau.
+
+Pour la commande de mise à niveau, vous devez savoir que vous pouvez mettre à niveau des paquets provenant de différents dépôts, si vous éditez
+le fichier '\fI/etc/slpkg/repositories.toml\fR' et supprimez la balise repository. Le slpkg ne peut alors pas reconnaître le dépôt des paquets.
+
+Avec la commande remove, il va supprimer les dépendances si le paquet a été installé avec la commande '\fIslpkg install\fR',
+sinon, le slpkg ne connaît pas les dépendances qui sont installées avec les paquets qu'il va supprimer.
+
+Vous pouvez appliquer l'astérisque '*' à la place d'un paquet, pour faire correspondre tous les paquets d'un dépôt. Vous ne pouvez pas appliquer
+un astérisque à l'option '\fB-B, --bin-repos=\fR', sauf pour les commandes '\fB-s, search\fR', '\fB-u, update\fR' et '\fB-c, check-updates\fR'.
+
+La commande clean-data supprime les données du référentiel local et de la base de données.
+
+Remarque : il n'existe actuellement aucune fonction permettant d'indiquer les paquets si les couleurs sont désactivées.
+.RE
 .SH FICHIERS DE CONFIGURATION
 .P
 Fichier de \fBconfiguration\fP : /etc/slpkg/slpkg.toml
 .P
 Fichier des \fBdépôts\fP : /etc/slpkg/repositories.toml
 .P
 Fichier \fBblacklist\fP : /etc/slpkg/blacklist.toml
@@ -221,8 +248,8 @@
 \fIslpkg_new-config\fR permet de gérer les fichiers de configuration \fB.new\fP facilement et rapidement. Déplacez, copiez ou supprimez-les.
 .RE
 .SH RAPPORT DE BOGUES
 .P
 Veuillez signaler tout bogue trouvé à \fBhttps://gitlab.com/dslackw/slpkg/-/issues\fP.
 .SH AUTEUR
 .P
-\fBDimitris Zlatanidis\fP <d.zlatanidis@gmail.com>
+\fBDimitris Zlatanidis\fP <dslackw@gmail.com>
```

### Comparing `slpkg-4.7.6/completion/slpkg` & `slpkg-4.7.8/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slpkg/binaries/required.py` & `slpkg-4.7.8/slpkg/binaries/required.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-from typing import Generator
-
+from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
-from slpkg.binaries.queries import BinQueries
 
 
 class Required:
     """ Creates a list of dependencies with
     the right order to install. """
 
-    def __init__(self, name: str, repo: str):
+    def __init__(self, data: dict, name: str, repo: str):
+        __slots__ = 'data', 'name,' 'repo'
+        self.data: dict = data
         self.name: str = name
         self.repo: str = repo
         self.repos = Repositories()
-        self.repo_package_names: Generator = BinQueries(
-            self.name, self.repo).all_package_names_by_repo()
+        self.utils = Utilities()
 
         self.special_repos: list = [
             self.repos.salixos_repo_name,
             self.repos.salixos_extra_repo_name,
             self.repos.slackel_repo_name,
             self.repos.slint_repo_name
         ]
 
     def resolve(self) -> list:
         """ Resolve the dependencies. """
-        required: list[str] = BinQueries(self.name, self.repo).required()
+        required: list[str] = self.data[self.name][6].split()
 
         # Resolve dependencies for some special repos.
         if self.repo in self.special_repos:
             requires: list = []
             for req in required:
-                if req in self.repo_package_names:
+                if req in list(self.data.keys()):
                     requires.append(req)
             return requires
 
         for req in required:
 
             # Remove requirements that are included as dependencies,
             # but are not included in the repository.
-            if req not in self.repo_package_names:
+            if req not in list(self.data.keys()) or self.utils.blacklist_pattern(req):
                 required.remove(req)
+                continue
 
             if req:
-                sub_required: list[str] = BinQueries(req, self.repo).required()
+                try:
+                    sub_required: list[str] = self.data[req][6].split()
+                except KeyError:
+                    sub_required: list[str] = []
 
                 for sub in sub_required:
                     required.append(sub)
 
         # Clean for dependencies not in the repository.
         for dep in required:
-            if dep not in self.repo_package_names:
+            if dep not in list(self.data.keys()):
                 required.remove(dep)
 
         required.reverse()
 
         return list(dict.fromkeys(required))
```

### Comparing `slpkg-4.7.6/slpkg/binaries/install.py` & `slpkg-4.7.8/slpkg/binaries/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
 import time
 import subprocess
+from collections import OrderedDict
 from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.checksum import Md5sum
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
 from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 from slpkg.binaries.required import Required
-from slpkg.binaries.queries import BinQueries
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class Packages(Configs):
 
-    def __init__(self, packages: list, flags: list, repo: str, mode: str):
+    def __init__(self, data: dict, packages: list, flags: list, repo: str, mode: str):
+        __slots__ = 'data', 'packages', 'flags', 'repo', 'mode'
         super(Configs, self).__init__()
+        self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
         self.repo: str = repo
         self.mode: str = mode
 
         self.progress = ProgressBar()
         self.color = self.colour()
         self.utils = Utilities()
         self.repos = Repositories()
         self.dialogbox = DialogBox()
-        self.upgrade = Upgrade(self.flags, self.repo)
-        self.view_message = ViewMessage(self.flags, self.repo)
+        self.upgrade = Upgrade(self.flags, self.data, self.repo)
+        self.view_message = ViewMessage(self.flags, self.data, self.repo)
         self.session = Session
 
         self.output: int = 0
         self.stderr = None
         self.stdout = None
         self.process_message: str = ''
         self.bold: str = self.color['bold']
@@ -50,20 +52,28 @@
         self.endc: str = self.color['endc']
         self.byellow: str = f'{self.bold}{self.yellow}'
         self.bred: str = f'{self.bold}{self.red}'
 
         self.packages_requires: list = []
         self.install_order: list = []
         self.binary_packages: list = []
-        self.flag_reinstall: list = ['-r', '--reinstall']
-        self.flag_skip_installed: list = ['-k', '--skip-installed']
-        self.flag_no_silent: list = ['-n', '--no-silent']
-        self.flag_resolve_off: list = ['-o', '--resolve-off']
 
-        self.packages: list = self.utils.apply_package_pattern(self.flags, self.packages, self.repo)
+        self.option_for_reinstall: bool = self.utils.is_option(
+            ['-r', '--reinstall'], self.flags)
+
+        self.option_for_skip_installed: bool = self.utils.is_option(
+            ['-k', '--skip-installed'], self.flags)
+
+        self.option_for_resolve_off: bool = self.utils.is_option(
+            ['-o', '--resolve-off'], self.flags)
+
+        self.option_for_no_silent: bool = self.utils.is_option(
+            ['-n', '--no-silent'], self.flags)
+
+        self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
 
     def execute(self) -> None:
         self.dependencies()
 
         self.view_message.install_packages(self.packages, self.packages_requires, self.mode)
         self.view_message.question()
 
@@ -73,116 +83,106 @@
         self.install_packages()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def dependencies(self):
         """ Creating the dependencies list and the order for install. """
-        requires: list = []
-
-        if not self.utils.is_option(self.flag_resolve_off, self.flags):
+        if not self.option_for_resolve_off:
 
             for pkg in self.packages:
 
                 # Skip installed package when the option --skip-installed is applied.
-                if (self.utils.is_option(self.flag_skip_installed, self.flags) and
-                        self.utils.is_package_installed(pkg)):
+                if self.option_for_skip_installed and self.utils.is_package_installed(pkg):
                     continue
 
-                self.packages_requires += Required(pkg, self.repo).resolve()
+                self.packages_requires += Required(self.data, pkg, self.repo).resolve()
 
             # Clean dependencies from the dependencies list if already added with main packages.
-            for req in self.packages_requires:
-                if req not in self.packages:
-                    requires.append(req)
-
-            requires = list(set(requires))
+            requires = list(OrderedDict.fromkeys(self.packages_requires))
 
             if requires:
                 self.packages_requires = self.choose_dependencies(requires)
 
         self.install_order = [*self.packages_requires, *self.packages]
 
     def download(self) -> None:
         """ Download packages from the repositories. """
         pkg_urls: list = []
 
         for pkg in self.install_order:
 
             if self.continue_install(pkg):
-                mirror: str = BinQueries(pkg, self.repo).mirror()
-                location: str = BinQueries(pkg, self.repo).location()
-                package: str = BinQueries(pkg, self.repo).package_bin()
+                package: str = self.data[pkg][1]
+                mirror: str = self.data[pkg][2]
+                location: str = self.data[pkg][3]
 
                 pkg_urls.append(f'{mirror}{location}/{package}')
                 self.binary_packages.append(package)
                 self.utils.remove_file_if_exists(self.tmp_slpkg, package)
             else:
-                version: str = BinQueries(pkg, self.repo).version()
+                version: str = self.data[pkg][0]
                 self.view_message.view_skipping_packages(pkg, version)
 
         if pkg_urls:
             down = Downloader(self.tmp_slpkg, pkg_urls, self.flags)
             down.download()
             print()
 
     def continue_install(self, name) -> bool:
         """ Skip installed package when the option --skip-installed is applied
             and continue to install if the package is upgradable or the --reinstall option
             applied.
          """
-        if (self.utils.is_option(self.flag_skip_installed, self.flags)
-                and not self.utils.is_option(self.flag_reinstall, self.flags)):
-            return False
-
-        if self.utils.is_option(self.flag_reinstall, self.flags):
+        if not self.utils.is_package_installed(name):
             return True
 
-        if not self.utils.is_package_installed(name):
+        if self.upgrade.is_package_upgradeable(name):
             return True
 
-        if not self.upgrade.is_package_upgradeable(name):
-            return False
+        if self.utils.is_package_installed(name) and self.option_for_reinstall:
+            return True
 
-        return True
+        return False
 
     def checksum(self) -> None:
         """ Packages checksums. """
         md5 = Md5sum(self.flags)
         for package in self.binary_packages:
-            pkg_checksum: str = BinQueries(package, self.repo).package_checksum()
+            name: str = self.utils.split_binary_pkg(package[:-4])[0]
+            pkg_checksum: str = self.data[name][10]
             md5.check(self.tmp_slpkg, package, pkg_checksum)
 
     def install_packages(self) -> None:
         """ Install the packages. """
         for package in self.binary_packages:
 
             message: str = f'{self.cyan}Installing{self.endc}'
             slack_command: str = self.installpkg
 
-            if (self.utils.is_option(self.flag_reinstall, self.flags) or
-                    self.utils.is_package_installed(package) or self.mode == 'upgrade'):
+            if (self.option_for_reinstall or self.utils.is_package_installed(package)
+                    or self.mode == 'upgrade'):
 
                 message: str = f'{self.cyan}Upgrade{self.endc}'
                 slack_command: str = self.reinstall
 
             command: str = f'{slack_command} {self.tmp_slpkg}/{package}'
             self.process_message: str = f"package '{package}' to install"
             self.multi_process(command, package, message)
 
-            if not self.utils.is_option(self.flag_resolve_off, self.flags):
+            if not self.option_for_resolve_off:
                 name: str = self.utils.split_binary_pkg(package[:-4])[0]
                 self.logging_installed_dependencies(name)
 
     def logging_installed_dependencies(self, name: str) -> None:
         """ Logging installed dependencies and used for remove. """
         exist = self.session.query(LogsDependencies.name).filter(
             LogsDependencies.name == name).first()
 
-        requires: list = Required(name, self.repo).resolve()
+        requires: list = Required(self.data, name, self.repo).resolve()
 
         # Update the dependencies if exist else create it.
         if exist:
             self.session.query(
                 LogsDependencies).filter(
                     LogsDependencies.name == name).update(
                         {LogsDependencies.requires: ' '.join(requires)})
@@ -190,15 +190,15 @@
         elif requires:
             deps: list = LogsDependencies(name=name, requires=' '.join(requires))
             self.session.add(deps)
         self.session.commit()
 
     def multi_process(self, command: str, filename: str, message: str) -> None:
         """ Starting multiprocessing install/upgrade process. """
-        if self.silent_mode and not self.utils.is_option(self.flag_no_silent, self.flags):
+        if self.silent_mode and not self.option_for_no_silent:
 
             done: str = f' {self.byellow} Done{self.endc}'
             self.stderr = subprocess.DEVNULL
             self.stdout = subprocess.DEVNULL
 
             # Starting multiprocessing
             p1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
@@ -235,28 +235,31 @@
         list_height: int = 0
         choices: list = []
         title: str = ' Choose dependencies you want to install '
 
         for package in dependencies:
             status: bool = False
 
-            repo_ver: str = BinQueries(package, self.repo).version()
+            repo_ver: str = self.data[package][0]
             help_text: str = f'Package: {package} {repo_ver}'
             upgradable: bool = self.upgrade.is_package_upgradeable(package)
             installed: str = self.utils.is_package_installed(package)
 
             if self.mode == 'upgrade' and upgradable:
                 status: bool = True
 
             if self.mode == 'install' and upgradable:
                 status: bool = True
 
             if self.mode == 'install' and not installed:
                 status: bool = True
 
+            if self.option_for_reinstall:
+                status: bool = True
+
             choices += [(package, repo_ver, status, help_text)]
 
         text: str = f'There are {len(choices)} dependencies:'
 
         code, tags = self.dialogbox.checklist(text, dependencies, title, height,
                                               width, list_height, choices)
```

### Comparing `slpkg-4.7.6/slpkg/install_data.py` & `slpkg-4.7.8/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slpkg/repositories.py` & `slpkg-4.7.8/slpkg/repositories.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,195 +7,196 @@
 from dataclasses import dataclass
 
 from slpkg.configs import Configs
 
 
 @dataclass
 class Repositories:
-    config = Configs
-    color = config.colour()
+    configs = Configs
+    color = configs.colour()
     bold: str = color['bold']
     red: str = color['red']
     cyan: str = color['cyan']
     endc: str = color['endc']
     bred: str = f'{bold}{red}'
 
-    repositories_file_toml = Path(config.etc_path, 'repositories.toml')
+    repositories_file_toml: Path = Path(configs.etc_path, 'repositories.toml')
+    repositories_path: Path = Path(configs.lib_path, 'repositories')
 
     repos_config = {}
     repositories = {}
     bin_repos_name = []
     bin_enabled_repos = []
     sbo_enabled_repo: bool = True
 
     sbo_repo_name: str = 'sbo'
-    sbo_repo_path: Path = Path(config.lib_path, 'repositories', sbo_repo_name)
+    sbo_repo_path: Path = Path(repositories_path, sbo_repo_name)
     sbo_repo_mirror: str = 'https://slackbuilds.org/slackbuilds/15.0/'
     sbo_repo_slackbuilds: str = 'SLACKBUILDS.TXT'
     sbo_repo_changelog: str = 'ChangeLog.txt'
     sbo_repo_tar_suffix: str = '.tar.gz'
     sbo_repo_tag: str = '_SBo'
     sbo_repo_patch_tag: str = ''
 
     ponce_repo: bool = False
     ponce_repo_name: str = 'ponce'
-    ponce_repo_path: Path = Path(config.lib_path, 'repositories', ponce_repo_name)
+    ponce_repo_path: Path = Path(repositories_path, ponce_repo_name)
     ponce_repo_mirror: str = 'https://cgit.ponce.cc/slackbuilds/plain/'
     ponce_repo_slackbuilds: str = 'SLACKBUILDS.TXT'
     ponce_repo_changelog: str = 'ChangeLog.txt'
     ponce_repo_tag: str = '_SBo'
     ponce_repo_patch_tag: str = ''
 
     slack_repo: bool = False
     slack_repo_name: str = 'slack'
-    slack_repo_path: Path = Path(config.lib_path, 'repositories', slack_repo_name)
+    slack_repo_path: Path = Path(repositories_path, slack_repo_name)
     slack_repo_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/'
     slack_repo_packages: str = 'PACKAGES.TXT'
     slack_repo_checksums: str = 'CHECKSUMS.md5'
     slack_repo_changelog: str = 'ChangeLog.txt'
     slack_repo_tag: str = ''
 
     slack_extra_repo: bool = False
     slack_extra_repo_name: str = 'slack_extra'
-    slack_extra_repo_path: Path = Path(config.lib_path, 'repositories', slack_extra_repo_name)
+    slack_extra_repo_path: Path = Path(repositories_path, slack_extra_repo_name)
     slack_extra_repo_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/'
     slack_extra_packages_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/extra/'
     slack_extra_repo_packages: str = 'PACKAGES.TXT'
     slack_extra_repo_checksums: str = 'CHECKSUMS.md5'
     slack_extra_repo_changelog: str = 'ChangeLog.txt'
     slack_extra_repo_tag: str = ''
 
     slack_patches_repo: bool = False
     slack_patches_repo_name: str = 'slack_patches'
-    slack_patches_repo_path: Path = Path(config.lib_path, 'repositories', slack_patches_repo_name)
+    slack_patches_repo_path: Path = Path(repositories_path, slack_patches_repo_name)
     slack_patches_repo_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/'
     slack_patches_packages_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/patches/'
     slack_patches_repo_packages: str = 'PACKAGES.TXT'
     slack_patches_repo_checksums: str = 'CHECKSUMS.md5'
     slack_patches_repo_changelog: str = 'ChangeLog.txt'
     slack_patches_repo_tag: str = '_slack15.0'
 
     alien_repo: bool = False
     alien_repo_name: str = 'alien'
-    alien_repo_path: Path = Path(config.lib_path, 'repositories', alien_repo_name)
+    alien_repo_path: Path = Path(repositories_path, alien_repo_name)
     alien_repo_mirror: str = 'https://slackware.nl/people/alien/sbrepos/'
     alien_repo_packages_mirror: str = 'https://slackware.nl/people/alien/sbrepos/15.0/x86_64/'
     alien_repo_packages: str = 'PACKAGES.TXT'
     alien_repo_checksums: str = 'CHECKSUMS.md5'
     alien_repo_changelog: str = 'ChangeLog.txt'
     alien_repo_tag: str = 'alien'
 
     multilib_repo: bool = False
     multilib_repo_name: str = 'multilib'
-    multilib_repo_path: Path = Path(config.lib_path, 'repositories', multilib_repo_name)
+    multilib_repo_path: Path = Path(repositories_path, multilib_repo_name)
     multilib_repo_mirror: str = 'https://slackware.nl/people/alien/multilib/'
     multilib_repo_packages_mirror: str = 'https://slackware.nl/people/alien/multilib/15.0/'
     multilib_repo_packages: str = 'PACKAGES.TXT'
     multilib_repo_checksums: str = 'CHECKSUMS.md5'
     multilib_repo_changelog: str = 'ChangeLog.txt'
     multilib_repo_tag: str = 'alien'
 
     restricted_repo: bool = False
     restricted_repo_name: str = 'restricted'
-    restricted_repo_path: Path = Path(config.lib_path, 'repositories', restricted_repo_name)
+    restricted_repo_path: Path = Path(repositories_path, restricted_repo_name)
     restricted_repo_mirror: str = 'https://slackware.nl/people/alien/restricted_sbrepos/'
     restricted_repo_packages_mirror: str = 'https://slackware.nl/people/alien/restricted_sbrepos/15.0/x86_64/'
     restricted_repo_packages: str = 'PACKAGES.TXT'
     restricted_repo_checksums: str = 'CHECKSUMS.md5'
     restricted_repo_changelog: str = 'ChangeLog.txt'
     restricted_repo_tag: str = 'alien'
 
     gnome_repo: bool = False
     gnome_repo_name: str = 'gnome'
-    gnome_repo_path: Path = Path(config.lib_path, 'repositories', gnome_repo_name)
+    gnome_repo_path: Path = Path(repositories_path, gnome_repo_name)
     gnome_repo_mirror: str = 'https://reddoglinux.ddns.net/linux/gnome/43.x/x86_64/'
     gnome_repo_packages: str = 'PACKAGES.TXT'
     gnome_repo_checksums: str = 'CHECKSUMS.md5'
     gnome_repo_changelog: str = 'ChangeLog.txt'
     gnome_repo_tag: str = 'gfs'
 
     msb_repo: bool = False
     msb_repo_name: str = 'msb'
-    msb_repo_path: Path = Path(config.lib_path, 'repositories', msb_repo_name)
+    msb_repo_path: Path = Path(repositories_path, msb_repo_name)
     msb_repo_mirror: str = 'https://slackware.uk/msb/'
     msb_repo_packages_mirror: str = 'https://slackware.uk/msb/15.0/1.26/x86_64/'
     msb_repo_packages: str = 'PACKAGES.TXT'
     msb_repo_checksums: str = 'CHECKSUMS.md5'
     msb_repo_changelog: str = 'ChangeLog.txt'
     msb_repo_tag: str = 'msb'
 
     csb_repo: bool = False
     csb_repo_name: str = 'csb'
-    csb_repo_path: Path = Path(config.lib_path, 'repositories', csb_repo_name)
+    csb_repo_path: Path = Path(repositories_path, csb_repo_name)
     csb_repo_mirror: str = 'https://slackware.uk/csb/'
     csb_repo_packages_mirror: str = 'https://slackware.uk/csb/15.0/x86_64/'
     csb_repo_packages: str = 'PACKAGES.TXT'
     csb_repo_checksums: str = 'CHECKSUMS.md5'
     csb_repo_changelog: str = 'ChangeLog.txt'
     csb_repo_tag: str = 'csb'
 
     conraid_repo: bool = False
     conraid_repo_name: str = 'conraid'
-    conraid_repo_path: Path = Path(config.lib_path, 'repositories', conraid_repo_name)
+    conraid_repo_path: Path = Path(repositories_path, conraid_repo_name)
     conraid_repo_mirror: str = 'https://slack.conraid.net/repository/slackware64-current/'
     conraid_repo_packages: str = 'PACKAGES.TXT'
     conraid_repo_checksums: str = 'CHECKSUMS.md5'
     conraid_repo_changelog: str = 'ChangeLog.txt'
     conraid_repo_tag: str = 'cf'
 
     slackonly_repo: bool = False
     slackonly_repo_name: str = 'slackonly'
-    slackonly_repo_path: Path = Path(config.lib_path, 'repositories', slackonly_repo_name)
+    slackonly_repo_path: Path = Path(repositories_path, slackonly_repo_name)
     slackonly_repo_mirror: str = 'https://packages.slackonly.com/pub/packages/15.0-x86_64/'
     slackonly_repo_packages: str = 'PACKAGES.TXT'
     slackonly_repo_checksums: str = 'CHECKSUMS.md5'
     slackonly_repo_changelog: str = 'ChangeLog.txt'
     slackonly_repo_tag: str = 'slonly'
 
     salixos_repo: bool = False
     salixos_repo_name: str = 'salixos'
-    salixos_repo_path: Path = Path(config.lib_path, 'repositories', salixos_repo_name)
+    salixos_repo_path: Path = Path(repositories_path, salixos_repo_name)
     salixos_repo_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/'
     salixos_repo_packages: str = 'PACKAGES.TXT'
     salixos_repo_checksums: str = 'CHECKSUMS.md5'
     salixos_repo_changelog: str = 'ChangeLog.txt'
     salixos_repo_tag: str = ''
 
     salixos_extra_repo: bool = False
     salixos_extra_repo_name: str = 'salixos_extra'
-    salixos_extra_repo_path: Path = Path(config.lib_path, 'repositories', salixos_extra_repo_name)
+    salixos_extra_repo_path: Path = Path(repositories_path, salixos_extra_repo_name)
     salixos_extra_repo_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/'
     salixos_extra_repo_packages_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/extra/'
     salixos_extra_repo_packages: str = 'PACKAGES.TXT'
     salixos_extra_repo_checksums: str = 'CHECKSUMS.md5'
     salixos_extra_repo_changelog: str = 'ChangeLog.txt'
     salixos_extra_repo_tag: str = ''
 
     salixos_patches_repo: bool = False
     salixos_patches_repo_name: str = 'salixos_patches'
-    salixos_patches_repo_path: Path = Path(config.lib_path, 'repositories', salixos_patches_repo_name)
+    salixos_patches_repo_path: Path = Path(repositories_path, salixos_patches_repo_name)
     salixos_patches_repo_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/'
     salixos_patches_repo_packages_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/patches/'
     salixos_patches_repo_packages: str = 'PACKAGES.TXT'
     salixos_patches_repo_checksums: str = 'CHECKSUMS.md5'
     salixos_patches_repo_changelog: str = 'ChangeLog.txt'
     salixos_patches_repo_tag: str = '_slack15.0'
 
     slackel_repo: bool = False
     slackel_repo_name: str = 'slackel'
-    slackel_repo_path: Path = Path(config.lib_path, 'repositories', slackel_repo_name)
+    slackel_repo_path: Path = Path(repositories_path, slackel_repo_name)
     slackel_repo_mirror: str = 'http://www.slackel.gr/repo/x86_64/current/'
     slackel_repo_packages: str = 'PACKAGES.TXT'
     slackel_repo_checksums: str = 'CHECKSUMS.md5'
     slackel_repo_changelog: str = 'ChangeLog.txt'
     slackel_repo_tag: str = 'dj'
 
     slint_repo: bool = False
     slint_repo_name: str = 'slint'
-    slint_repo_path: Path = Path(config.lib_path, 'repositories', slint_repo_name)
+    slint_repo_path: Path = Path(repositories_path, slint_repo_name)
     slint_repo_mirror: str = 'https://slackware.uk/slint/x86_64/slint-15.0/'
     slint_repo_packages: str = 'PACKAGES.TXT'
     slint_repo_checksums: str = 'CHECKSUMS.md5'
     slint_repo_changelog: str = 'ChangeLog.txt'
     slint_repo_tag: str = 'slint'
 
     try:
@@ -353,17 +354,17 @@
             slint_repo_mirror: str = repos_config['SLINT_REPO_MIRROR']
             slint_repo_packages: str = repos_config['SLINT_REPO_PACKAGES']
             slint_repo_checksums: str = repos_config['SLINT_REPO_CHECKSUMS']
             slint_repo_changelog: str = repos_config['SLINT_REPO_CHANGELOG']
             slint_repo_tag: str = repos_config['SLINT_REPO_TAG']
 
     except (tomli.TOMLDecodeError, KeyError) as error:
-        raise SystemExit(f'\n{config.prog_name} {bred}Error{endc}: {error}: in the configuration file '
+        raise SystemExit(f'\n{configs.prog_name} {bred}Error{endc}: {error}: in the configuration file '
                          f"'{repositories_file_toml}'.\n"
-                         f"\nIf you have upgraded the '{config.prog_name}' probably you need to run:\n"
+                         f"\nIf you have upgraded the '{configs.prog_name}' probably you need to run:\n"
                          f"'mv {repositories_file_toml}.new {repositories_file_toml}'.\n"
                          f"or '{cyan}slpkg_new-configs{endc}' command.\n")
 
     # Default sbo repository configs.
     repo_tag: str = sbo_repo_tag
     patch_repo_tag: str = sbo_repo_patch_tag
     sbo_enabled_repository: str = sbo_repo_name
@@ -466,11 +467,8 @@
                           slint_repo_tag]
     }
 
     # All the binary repositories names.
     bin_repos_names = list(repositories.keys())[2:]
 
     # All the enabled binary repositories names.
-    for repo, enabled in repositories.items():
-        if repo not in [sbo_repo_name, ponce_repo_name]:
-            if enabled[0]:
-                bin_enabled_repos.append(repo)
+    bin_enabled_repos = list(repositories.keys())[2:]
```

### Comparing `slpkg-4.7.6/slpkg/repo_info.py` & `slpkg-4.7.8/slpkg/repo_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import shutil
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
-from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
-from slpkg.binaries.queries import BinQueries
-from slpkg.models.models import LastRepoUpdated
 from slpkg.models.models import session as Session
+from slpkg.models.models import LastRepoUpdated, SBoTable, BinariesTable
 
 
 class RepoInfo(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
 
@@ -57,17 +55,17 @@
                 LastRepoUpdated.repo == repo).first()
 
             if last is None:
                 last: tuple = ('',)
 
             if value[0]:
                 if repo in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
-                    count = int(SBoQueries('').count_packages())
+                    count = self.session.query(SBoTable.id).count()
                 else:
-                    count = int(BinQueries('', repo).count_packages())
+                    count = self.session.query(BinariesTable).where(BinariesTable.repo == repo).count()
 
             total_packages += count
 
             print(f"{self.cyan}{repo:<18}{self.endc}{color}{status:<15}{self.endc}{last[0]:<35}"
                   f"{self.yellow}{count:>12}{self.endc}")
 
         print('=' * self.columns)
```

### Comparing `slpkg-4.7.6/slpkg/sbos/slackbuild.py` & `slpkg-4.7.8/slpkg/sbos/slackbuild.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,61 +13,71 @@
 from slpkg.checksum import Md5sum
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
-from slpkg.sbos.queries import SBoQueries
 from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 from slpkg.sbos.dependencies import Requires
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class Slackbuilds(Configs):
     """ Download build and install the SlackBuilds. """
 
-    def __init__(self, slackbuilds: list, flags: list, mode: str):
+    def __init__(self, data: dict, slackbuilds: list, flags: list, mode: str):
+        __slots__ = 'data', 'slackbuilds', 'flags', 'mode'
         super(Configs, self).__init__()
+        self.data = data
         self.slackbuilds: list = slackbuilds
         self.flags: list = flags
         self.mode: str = mode
 
         self.session = Session
         self.repos = Repositories()
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.dialogbox = DialogBox()
-        self.upgrade = Upgrade(self.flags)
-        self.view_message = ViewMessage(self.flags)
+        self.upgrade = Upgrade(self.flags, data)
+        self.view_message = ViewMessage(self.flags, data)
         self.color = self.colour()
 
-        self.install_order: list = []
-        self.dependencies: list = []
-        self.sbos: dict = {}
         self.stderr = None
         self.stdout = None
+        self.sbos: dict = {}
+        self.install_order: list = []
+        self.dependencies: list = []
         self.process_message: str = ''
         self.bold: str = self.color['bold']
         self.cyan: str = self.color['cyan']
         self.red: str = self.color['red']
         self.yellow: str = self.color['yellow']
         self.endc: str = self.color['endc']
         self.byellow: str = f'{self.bold}{self.yellow}'
         self.bred: str = f'{self.bold}{self.red}'
-        self.flag_reinstall: list = ['-r', '--reinstall']
-        self.flag_skip_installed: list = ['-k', '--skip-installed']
-        self.flag_resolve_off: list = ['-o', '--resolve-off']
-        self.flag_jobs: list = ['-j', '--jobs']
-        self.flag_no_silent: list = ['-n', '--no-silent']
-        self.flag_parallel: list = ['-P', '--parallel']
 
-        self.slackbuilds: list = self.utils.apply_package_pattern(self.flags, self.slackbuilds)
+        self.option_for_reinstall: bool = self.utils.is_option(
+            ['-r', '--reinstall'], self.flags)
+
+        self.option_for_skip_installed: bool = self.utils.is_option(
+            ['-k', '--skip-installed'], self.flags)
+
+        self.option_for_resolve_off: bool = self.utils.is_option(
+            ['-o', '--resolve-off'], self.flags)
+
+        self.option_for_jobs: bool = self.utils.is_option(
+            ['-j', '--jobs'], self.flags)
+
+        self.option_for_no_silent: bool = self.utils.is_option(
+            ['-n', '--no-silent'], self.flags)
+
+        self.slackbuilds: list = self.utils.apply_package_pattern(self.data, self.slackbuilds)
 
         # Patch the TAG from configs.
         if self.repos.patch_repo_tag:
             self.repos.repo_tag = self.repos.patch_repo_tag
 
     def execute(self) -> None:
         """ Starting build or install the slackbuilds. """
@@ -82,27 +92,26 @@
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dictionary(self) -> None:
         """ Dictionary with the main slackbuilds and dependencies. """
         for sbo in self.slackbuilds:
-            if self.utils.is_option(self.flag_resolve_off, self.flags):
+            if self.option_for_resolve_off:
                 self.sbos[sbo] = []
             else:
-                self.sbos[sbo] = Requires(sbo).resolve()
+                self.sbos[sbo] = Requires(self.data, sbo).resolve()
 
     def creating_dependencies_for_build(self) -> None:
         """ List with the dependencies. """
         for deps in self.sbos.values():
             for dep in deps:
 
                 # Skip installed package when the option --skip-installed is applied.
-                if (self.utils.is_option(self.flag_skip_installed, self.flags) and
-                        self.utils.is_package_installed(dep)):
+                if self.option_for_skip_installed and self.utils.is_package_installed(dep):
                     continue
 
                 self.dependencies.append(dep)
 
         # Remove duplicate packages and keeps the order.
         dependencies = list(OrderedDict.fromkeys(self.dependencies))
 
@@ -132,56 +141,59 @@
         self.view_message.question()
 
     def continue_build_or_install(self, name) -> bool:
         """ Skip installed package when the option --skip-installed is applied
             and continue to install if the package is upgradable or the --reinstall option
             applied.
         """
-        if (self.utils.is_option(self.flag_skip_installed, self.flags)
-                and not self.utils.is_option(self.flag_reinstall, self.flags)
-                and self.mode != 'build'):
-            return False
+        if self.mode == 'build':
+            return True
 
-        if self.utils.is_option(self.flag_reinstall, self.flags) and self.mode != 'build':
+        if not self.utils.is_package_installed(name):
             return True
 
-        if not self.utils.is_package_installed(name) and self.mode != 'build':
+        if self.upgrade.is_package_upgradeable(name):
             return True
 
-        if not self.upgrade.is_package_upgradeable(name) and self.mode not in ['build', 'upgrade']:
-            return False
+        if self.utils.is_package_installed(name) and self.option_for_reinstall:
+            return True
 
-        return True
+        return False
 
     def prepare_slackbuilds_for_build(self) -> None:
         """ Downloads files and sources. """
         sources_urls: list = []
         sources: dict = {}
 
         for sbo in self.install_order:
 
             if self.continue_build_or_install(sbo):
 
                 build_path: Path = Path(self.build_path, sbo)
 
                 self.utils.remove_folder_if_exists(build_path)
-                location: str = SBoQueries(sbo).location()
+                location: str = self.data[sbo][0]
                 slackbuild = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
 
                 # Copy slackbuilds to the build folder.
                 if self.repos.ponce_repo:
                     path_ponce_repo_package = Path(self.repos.ponce_repo_path, location, sbo)
                     shutil.copytree(path_ponce_repo_package, build_path)
                 else:
                     path_sbo_repo_package = Path(self.repos.sbo_repo_path, location, sbo)
                     shutil.copytree(path_sbo_repo_package, build_path)
 
                 os.chmod(slackbuild, 0o775)
-                sources[sbo] = SBoQueries(sbo).sources()
-                sources_urls += SBoQueries(sbo).sources()
+
+                if self.os_arch == 'x86_64' and self.data[sbo][4]:
+                    sources[sbo] = self.data[sbo][4].split()
+                    sources_urls += self.data[sbo][4].split()
+                else:
+                    sources[sbo] = self.data[sbo][3].split()
+                    sources_urls += self.data[sbo][3].split()
 
         # Download the sources.
         if sources:
             for sbo, sbo_sources in sources.items():
                 down_urls = Downloader(Path(self.build_path, sbo), sbo_sources, self.flags)
                 down_urls.download()
 
@@ -189,16 +201,21 @@
 
             self.checksum_downloads()
 
     def checksum_downloads(self) -> None:
         """ Checking the correct checksums. """
         for sbo in self.install_order:
             path = Path(self.build_path, sbo)
-            checksums = SBoQueries(sbo).checksum()
-            sources = SBoQueries(sbo).sources()
+
+            if self.os_arch == 'x86_64' and self.data[sbo][6]:
+                checksums: list = self.data[sbo][6].split()
+                sources: list = self.data[sbo][4].split()
+            else:
+                checksums: list = self.data[sbo][5].split()
+                sources: list = self.data[sbo][3].split()
 
             for source, checksum in zip(sources, checksums):
                 md5sum = Md5sum(self.flags)
                 md5sum.check(path, source, checksum)
 
     def build_and_install(self) -> None:
         """ Build the slackbuilds and install. """
@@ -211,15 +228,15 @@
                 self.build_the_script(self.build_path, sbo)
 
                 if self.mode in ['install', 'upgrade']:
 
                     pkg: str = self.package_for_install(sbo)
                     self.install_package(pkg)
 
-                    if not self.utils.is_option(self.flag_resolve_off, self.flags):
+                    if not self.option_for_resolve_off:
                         self.logging_installed_dependencies(sbo)
             else:
                 package: str = self.utils.is_package_installed(sbo)
                 version: str = self.utils.split_binary_pkg(package)[1]
                 self.view_message.view_skipping_packages(sbo, version)
 
     def patch_sbo_tag(self, sbo: str) -> None:
@@ -238,15 +255,15 @@
                     script.write(line)
 
     def logging_installed_dependencies(self, name: str) -> None:
         """ Logging installed dependencies and used for remove. """
         exist = self.session.query(LogsDependencies.name).filter(
             LogsDependencies.name == name).first()
 
-        requires: list = Requires(name).resolve()
+        requires: list = Requires(self.data, name).resolve()
 
         # Update the dependencies if exist else create it.
         if exist:
             self.session.query(
                 LogsDependencies).filter(
                     LogsDependencies.name == name).update(
                         {LogsDependencies.requires: ' '.join(requires)})
@@ -257,16 +274,15 @@
         self.session.commit()
 
     def install_package(self, package: str) -> None:
         """ Install the packages that before created in the tmp directory. """
         pkg: str = self.utils.split_binary_pkg(package)[0]
 
         execute: str = self.installpkg
-        if (self.utils.is_option(self.flag_reinstall, self.flags) and
-                self.utils.is_package_installed(pkg)):
+        if self.option_for_reinstall and self.utils.is_package_installed(pkg):
             execute: str = self.reinstall
 
         message: str = f'{self.cyan}Installing{self.endc}'
         self.process_message: str = f"package '{pkg}' to install"
 
         if self.mode == 'upgrade':
             self.process_message: str = f"package '{pkg}' to upgrade"
@@ -274,39 +290,39 @@
 
         command: str = f'{execute} {self.tmp_path}{package}'
 
         self.multi_process(command, package, message)
 
     def package_for_install(self, name: str) -> str:
         """ Returns the package for install. """
-        package_to_install: str = ''
-        version: str = SBoQueries(name).version()
+        package: str = ''
+        version: str = self.data[name][2]
         pattern: str = f'{name}-{version}*{self.repos.repo_tag}*'
 
         tmp = Path(self.tmp_path)
         packages: list = [file.name for file in tmp.glob(pattern)]
 
         try:
-            package_to_install: str = max(packages)
+            package: str = max(packages)
         except ValueError:
             self.utils.raise_error_message(f"Package '{name}' not found for install")
 
-        return package_to_install
+        return package
 
     def build_the_script(self, path: Path, name: str) -> None:
         """ Run the .SlackBuild script. """
         folder: str = f'{Path(path, name)}/'
         execute: str = f'{folder}./{name}.SlackBuild'
 
         # Change to root privileges
         os.chown(folder, 0, 0)
         for file in os.listdir(folder):
             os.chown(f'{folder}{file}', 0, 0)
 
-        if self.utils.is_option(self.flag_jobs, self.flags):
+        if self.option_for_jobs:
             self.set_makeflags()
 
         name = f'{name}.SlackBuild'
         message: str = f'{self.red}Build{self.endc}'
         self.process_message: str = f"package '{name}' to build"
 
         self.multi_process(execute, name, message)
@@ -314,15 +330,15 @@
     @staticmethod
     def set_makeflags() -> None:
         """ Set number of processors. """
         os.environ['MAKEFLAGS'] = f'-j {cpu_count()}'
 
     def multi_process(self, command: str, filename: str, message: str) -> None:
         """ Starting multiprocessing install/upgrade process. """
-        if self.silent_mode and not self.utils.is_option(self.flag_no_silent, self.flags):
+        if self.silent_mode and not self.option_for_no_silent:
 
             done: str = f' {self.byellow} Done{self.endc}'
             self.stderr = subprocess.DEVNULL
             self.stdout = subprocess.DEVNULL
 
             # Starting multiprocessing
             p1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
@@ -358,16 +374,16 @@
         list_height: int = 0
         choices: list = []
         title: str = ' Choose dependencies you want to install '
 
         for package in dependencies:
             status: bool = False
 
-            repo_ver: str = SBoQueries(package).version()
-            description: str = SBoQueries(package).description()
+            repo_ver: str = self.data[package][2]
+            description: str = self.data[package][8]
             help_text: str = f'Description: {description}'
             upgradable: bool = self.upgrade.is_package_upgradeable(package)
             installed: str = self.utils.is_package_installed(package)
 
             if self.mode == 'build':
                 status: bool = True
 
@@ -376,14 +392,17 @@
 
             if self.mode == 'install' and upgradable:
                 status: bool = True
 
             if self.mode == 'install' and not installed:
                 status: bool = True
 
+            if self.option_for_reinstall:
+                status: bool = True
+
             choices += [(package, repo_ver, status, help_text)]
 
         text: str = f'There are {len(choices)} dependencies:'
 
         code, tags = self.dialogbox.checklist(text, dependencies, title, height,
                                               width, list_height, choices)
```

### Comparing `slpkg-4.7.6/slpkg/sbos/dependencies.py` & `slpkg-4.7.8/slpkg/sbos/dependencies.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-from slpkg.sbos.queries import SBoQueries
+from slpkg.utilities import Utilities
 
 
 class Requires:
     """ Creates a list of dependencies with
     the right order to install. """
 
-    def __init__(self, name: str):
+    def __init__(self, data: dict, name: str):
+        __slots__ = 'data', 'name'
+        self.data: dict = data
         self.name: str = name
-        self.repo_slackbuilds_names: list = list(SBoQueries(self.name).sbos())
+
+        self.utils = Utilities()
 
     def resolve(self) -> list:
         """ Resolve the dependencies. """
-        requires: list[str] = SBoQueries(self.name).requires()
+        requires: list[str] = self.data[self.name][7].split()
 
         for req in requires:
 
             # Remove requirements that are included as dependencies,
             # but are not included in the repository.
-            if req not in self.repo_slackbuilds_names:
+            if req not in list(self.data.keys()) or self.utils.blacklist_pattern(req):
                 requires.remove(req)
+                continue
 
             if req:
-                sub_requires: list[str] = SBoQueries(req).requires()
+                sub_requires: list[str] = self.data[req][7].split()
                 for sub in sub_requires:
                     requires.append(sub)
 
         requires.reverse()
 
         return list(dict.fromkeys(requires))
```

### Comparing `slpkg-4.7.6/slpkg/form_configs.py` & `slpkg-4.7.8/slpkg/form_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slpkg/update_repository.py` & `slpkg-4.7.8/slpkg/update_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
+import shutil
 from pathlib import Path
 from multiprocessing import Process, Queue
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
@@ -19,14 +20,15 @@
                                  LastRepoUpdated)
 
 
 class UpdateRepository(Configs):
     """ Deletes and install the data. """
 
     def __init__(self, flags: list, repo: str):
+        __slots__ = 'flags', 'repo'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repo: str = repo
         self.session = Session
         self.view = ViewMessage(self.flags)
 
         self.repos = Repositories()
@@ -46,15 +48,17 @@
         self.green: str = self.color['green']
         self.red: str = self.color['red']
         self.yellow: str = self.color['yellow']
         self.bgreen: str = f'{self.bold}{self.green}'
         self.bred: str = f'{self.bold}{self.red}'
         self.endc: str = self.color['endc']
         self.flag_generate: list = ['-G', '--generate-only']
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
+
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
 
     def update_the_repositories(self) -> None:
         if not self.repos_for_update.values() or self.repo not in self.repos_for_update.keys():
             self.view.question()
         else:
             print()
 
@@ -73,15 +77,15 @@
             self.repos.salixos_repo_name: self.salixos_repository,
             self.repos.salixos_extra_repo_name: self.salixos_extra_repository,
             self.repos.salixos_patches_repo_name: self.salixos_patches_repository,
             self.repos.slackel_repo_name: self.slackel_repository,
             self.repos.slint_repo_name: self.slint_repository
         }
 
-        if self.utils.is_option(self.flag_bin_repository, self.flags):
+        if self.option_for_binaries:
 
             for repo in bin_repositories.keys():
 
                 if repo == self.repo:
                     bin_repositories[repo]()
                     break
 
@@ -660,8 +664,24 @@
             PonceTable.__table__,
             SBoTable.__table__,
             BinariesTable.__table__,
             LastRepoUpdated.__table__
         ]
 
         Base.metadata.drop_all(bind=engine, tables=tables)
+
+        # Deletes local downloaded data.
+        self.delete_repositories_data()
+
         print("Successfully cleared!\n\nYou need to run 'slpkg update' now.")
+
+    def delete_repositories_data(self):
+        """ Deletes local folders with the repository downloaded data. """
+        for repo in self.repos.repositories.keys():
+
+            repo_path: Path = Path(self.repos.repositories_path, repo)
+
+            if repo_path.exists():
+                shutil.rmtree(repo_path)
+                print(f"Deleted: '{repo_path}'")
+
+        print()  # new line at the end
```

### Comparing `slpkg-4.7.6/slpkg/progress_bar.py` & `slpkg-4.7.8/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slpkg/downloader.py` & `slpkg-4.7.8/slpkg/downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 
 
 class Downloader(Configs):
 
     def __init__(self, path: Union[str, Path], urls: list, flags: list):
+        __slots__ = 'path', 'urls', 'flags'
         super(Configs, self).__init__()
         self.path = path
         self.urls: list = urls
         self.flags: list = flags
 
         self.utils = Utilities()
 
-        self.flag_parallel: list = ['-P', '--parallel']
+        self.option_for_parallel: bool = self.utils.is_option(
+            ['-P', '--parallel'], self.flags)
 
     def download(self) -> None:
         """ Starting the processing for downloading. """
         process: list = []
 
-        if self.parallel_downloads or self.utils.is_option(self.flag_parallel, self.flags):
+        if self.parallel_downloads or self.option_for_parallel:
             for url in self.urls:
                 p1 = Process(target=self.tools, args=(url,))
                 process.append(p1)
                 p1.start()
 
             for proc in process:
                 proc.join()
```

### Comparing `slpkg-4.7.6/slpkg/models/models.py` & `slpkg-4.7.8/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slpkg/views/view_package.py` & `slpkg-4.7.8/slpkg/views/view_package.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
-from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
-from slpkg.binaries.queries import BinQueries
 from slpkg.models.models import session as Session
 from slpkg.models.models import (SBoTable, PonceTable,
                                  BinariesTable, LastRepoUpdated)
 
 
 class ViewPackage(Configs):
     """ View the repository packages. """
 
     def __init__(self, flags: list):
+        __slots__ = 'flags'
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.utils = Utilities()
         self.repos = Repositories()
         self.session = Session
         
@@ -28,30 +27,32 @@
         self.green: str = self.color['green']
         self.blue: str = self.color['blue']
         self.yellow: str = self.color['yellow']
         self.cyan: str = self.color['cyan']
         self.red: str = self.color['red']
         self.violet: str = self.color['violet']
         self.endc: str = self.color['endc']
-        self.flag_pkg_version: list = ['-p', '--pkg-version']
 
         # Switch between sbo and ponce repository.
         self.sbo_table = SBoTable
         self.repo_url: str = self.repos.sbo_repo_mirror
         self.repo_path: Path = self.repos.sbo_repo_path
         self.repo_tar_suffix: str = self.repos.sbo_repo_tar_suffix
         if self.repos.ponce_repo:
             self.sbo_table = PonceTable
             self.repo_url: str = self.repos.ponce_repo_mirror
             self.repo_path: Path = self.repos.ponce_repo_path
             self.repo_tar_suffix: str = ''
 
-    def slackbuild(self, slackbuilds: list) -> None:
+        self.option_for_pkg_version: bool = self.utils.is_option(
+            ['-p', '--pkg-version'], self.flags)
+
+    def slackbuild(self, data: dict, slackbuilds: list) -> None:
         """ View the packages from the repository. """
-        slackbuilds: list = self.utils.apply_package_pattern(self.flags, slackbuilds)
+        slackbuilds: list = self.utils.apply_package_pattern(data, slackbuilds)
 
         for sbo in slackbuilds:
 
             info: list = self.session.query(
                 self.sbo_table.name,
                 self.sbo_table.version,
                 self.sbo_table.requires,
@@ -66,29 +67,28 @@
 
             path = Path(self.repo_path, info[9], info[0], 'README')
             readme = self.utils.read_file(path)
 
             path = Path(self.repo_path, info[9], info[0], f'{info[0]}.info')
             info_file = self.utils.read_file(path)
 
-            repo_build_tag = self.utils.read_sbo_build_tag(info[0])
+            repo_build_tag = self.utils.read_sbo_build_tag(info[0], info[9])
 
             maintainer, email, homepage = '', '', ''
             for line in info_file:
                 if line.startswith('HOMEPAGE'):
                     homepage: str = line[10:-2].strip()
                 if line.startswith('MAINTAINER'):
                     maintainer: str = line[12:-2].strip()
                 if line.startswith('EMAIL'):
                     email: str = line[7:-2].strip()
 
             deps: str = (', '.join([f'{self.cyan}{pkg}' for pkg in info[2].split()]))
-
-            if self.utils.is_option(self.flag_pkg_version, self.flags):
-                deps: str = (', '.join([f'{self.cyan}{pkg}{self.endc}-{self.yellow}{SBoQueries(pkg).version()}'
+            if self.option_for_pkg_version:
+                deps: str = (', '.join([f'{self.cyan}{pkg}{self.endc} {self.yellow}{data[pkg][2]}'
                              f'{self.green}' for pkg in info[2].split()]))
 
             print(f'Name: {self.green}{info[0]}{self.endc}\n'
                   f'Version: {self.green}{info[1]}{self.endc}\n'
                   f'Build: {self.green}{repo_build_tag}{self.endc}\n'
                   f'Requires: {self.green}{deps}{self.endc}\n'
                   f'Homepage: {self.blue}{homepage}{self.endc}\n'
@@ -103,16 +103,16 @@
                   f'Slackware: {self.cyan}{self.repo_url.split("/")[-1]}{self.endc}\n'
                   f'Category: {self.red}{info[9]}{self.endc}\n'
                   f'SBo url: {self.blue}{self.repo_url}{info[9]}/{info[0]}{self.endc}\n'
                   f'Maintainer: {self.yellow}{maintainer}{self.endc}\n'
                   f'Email: {self.yellow}{email}{self.endc}\n'
                   f'\nREADME: {self.cyan}{"".join(readme)}{self.endc}')
 
-    def package(self, packages: list, repo: str) -> None:
-        packages: list = self.utils.apply_package_pattern(self.flags, packages, repo)
+    def package(self, data: dict, packages: list, repo: str) -> None:
+        packages: list = self.utils.apply_package_pattern(data, packages)
 
         for package in packages:
 
             info: list = self.session.query(
                 BinariesTable.repo,
                 BinariesTable.name,
                 BinariesTable.version,
@@ -132,16 +132,16 @@
             build: str = self.utils.split_binary_pkg(info[3])[3]
 
             last: str = self.session.query(
                 LastRepoUpdated.date).where(
                 LastRepoUpdated.repo == repo).first()
 
             deps: str = (', '.join([f'{self.cyan}{pkg}' for pkg in info[9].split()]))
-            if self.utils.is_option(self.flag_pkg_version, self.flags):
-                deps: str = (', '.join([f'{self.cyan}{pkg}{self.endc}-{self.yellow}{BinQueries(pkg, repo).version()}'
+            if self.option_for_pkg_version:
+                deps: str = (', '.join([f'{self.cyan}{pkg}{self.endc} {self.yellow}{data[pkg][0]}'
                              f'{self.green}' for pkg in info[9].split()]))
 
             print(f'Repository: {self.yellow}{info[0]}{self.endc}\n'
                   f'Last Updated: {self.violet}{last[0]}{self.endc}\n'
                   f'Name: {self.green}{info[1]}{self.endc}\n'
                   f'Version: {self.green}{info[2]}{self.endc}\n'
                   f'Build: {self.green}{build}{self.endc}\n'
```

### Comparing `slpkg-4.7.6/slpkg/views/version.py` & `slpkg-4.7.8/slpkg/views/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 7, 6)
+        self.version_info: tuple = (4, 7, 8)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.7.6/slpkg/views/cli_menu.py` & `slpkg-4.7.8/slpkg/views/cli_menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.yellow: str = color['yellow']
         self.endc: str = color['endc']
 
     def help_minimal(self, message: str) -> NoReturn:
         """ Prints the minimal help menu. """
         print(message)
         args: str = (
-            f'\nUsage: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}]'
+            f'\nUsage: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}] '
             f'[FILELIST|PACKAGES...]\n'
             f"\nTry '{self.prog_name} --help' for more options.\n")
 
         print(args)
         raise SystemExit(1)
 
     def help_short(self, status: int) -> NoReturn:
```

### Comparing `slpkg-4.7.6/slpkg/views/ascii.py` & `slpkg-4.7.8/slpkg/views/ascii.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         self.draw_middle_line()
 
         print(f'{self.bgreen}{self.vertical_line}{self.endc} Package:' + ' ' * 22 + 'Version:' +
               ' ' * (self.columns - 66) + 'Size:' + ' ' * 14 + f'Repo:{self.bgreen} {self.vertical_line}{self.endc}')
 
     def draw_view_package(self, package: str, version: str, size: str, color: str, repo: str) -> None:
         """ Draw nad print the packages. """
-        if self.columns <= 80 and len(version) >= 11:
+        if len(version) >= 11 and self.columns <= 80:
             version: str = f'{version[:10]}...'
-        if self.columns <= 80 and len(package) >= 25:
+        if len(package) >= 25:
             package: str = f'{package[:24]}...'
         print(f'{self.bgreen}{self.vertical_line} {self.bold}{color}{package}{self.endc}' + ' ' * (30 - len(package)) +
               f'{self.bgreen}{version}' + ' ' * ((self.columns - 53) - len(version) - len(size)) +
               f'{self.endc}{size}' + ' ' * (19 - len(repo)) +
               f'{self.blue}{repo} {self.bgreen}{self.vertical_line}{self.endc}')
 
     def draw_log_package(self, package: str) -> None:
```

### Comparing `slpkg-4.7.6/slpkg/views/help_commands.py` & `slpkg-4.7.8/slpkg/views/help_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from slpkg.configs import Configs
 
 
 class Help(Configs):
 
     def __init__(self, command: str, flags: list):
+        __slots__ = 'command', 'flags'
         super(Configs, self).__init__()
         self.command: str = command
         self.flags: list = flags
 
         color = self.colour()
 
         self.bold: str = color['bold']
```

### Comparing `slpkg-4.7.6/slpkg/views/views.py` & `slpkg-4.7.8/slpkg/views/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,78 +6,86 @@
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
 from slpkg.views.ascii import Ascii
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
-from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
-from slpkg.binaries.queries import BinQueries
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class ViewMessage(Configs):
 
-    def __init__(self, flags: list, repo=None):
+    def __init__(self, flags: list, data=None, repo=None):
+        __slots__ = 'flags', 'data', 'repo'
         super(Configs, self).__init__()
         self.flags: list = flags
+        self.data: dict = data
         self.repo: str = repo
 
         self.session = Session
         self.utils = Utilities()
         self.dialogbox = DialogBox()
         self.ascii = Ascii()
-        self.upgrade = Upgrade(self.flags, self.repo)
+        self.upgrade = Upgrade(self.flags, self.data, self.repo)
         self.color = self.colour()
         self.repos = Repositories()
 
         self.yellow: str = self.color['yellow']
         self.cyan: str = self.color['cyan']
         self.red: str = self.color['red']
         self.grey: str = self.color['grey']
         self.violet: str = self.color['violet']
         self.endc: str = self.color['endc']
         self.download_only = self.tmp_slpkg
         self.installed_packages: list = []
-        self.flag_resolve_off: list = ['-o', '--resolve-off']
-        self.flag_reinstall: list = ['-r', '--reinstall']
-        self.flag_yes: list = ['-y', '--yes']
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
+
+        self.option_for_resolve_off: bool = self.utils.is_option(
+            ['-o', '--resolve-off'], self.flags)
+
+        self.option_for_reinstall: bool = self.utils.is_option(
+            ['-r', '--reinstall'], self.flags)
+
+        self.option_for_yes: bool = self.utils.is_option(
+            ['-y', '--yes'], self.flags)
+
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
 
     def view_packages(self, package: str, mode: str) -> None:
         """ Printing the main packages. """
         size: str = ''
         color: str = self.red
 
-        if self.utils.is_option(self.flag_bin_repository, self.flags):
-            version: str = BinQueries(package, self.repo).version()
-            size: str = BinQueries(package, self.repo).size_comp()
-            repo = BinQueries(package, self.repo).repository()
+        if self.option_for_binaries:
+            version: str = self.data[package][0]
+            size: str = self.data[package][4]
+            repo: str = self.repo
         else:
-            version: str = SBoQueries(package).version()
-            repo: str = SBoQueries('').repo_name()
+            version: str = self.data[package][2]
+            repo: str = self.repos.sbo_enabled_repository
 
         if mode in ['install', 'download']:
             color: str = self.cyan
         if mode == 'build':
             color: str = self.yellow
         if mode == 'upgrade':
             color: str = self.violet
 
         # If the package is installed and change the color to gray.
-        if package in self.utils.installed_package_names and mode == 'install':
+        if package in self.utils.installed_packages.keys() and mode == 'install':
             color: str = self.grey
 
         if self.upgrade.is_package_upgradeable(package) and mode == 'install':
             color: str = self.violet
 
-        if (package in self.utils.installed_package_names and mode == 'install'
-                and self.utils.is_option(self.flag_reinstall, self.flags)):
+        if (package in self.utils.installed_packages.keys() and mode == 'install'
+                and self.option_for_reinstall):
             color: str = self.violet
 
         self.ascii.draw_view_package(package, version, size, color, repo)
 
     def view_skipping_packages(self, package: str, version: str) -> None:
         """ Print the skipping packages. """
         print(f'[{self.yellow}Skipping{self.endc}] {package}-{version} {self.red}(already installed){self.endc}')
@@ -145,24 +153,24 @@
             requires = self.session.query(
                 LogsDependencies.requires).filter(
                     LogsDependencies.name == pkg).first()
 
             if requires:
                 dependencies += requires[0].split()
 
-        if dependencies and not self.utils.is_option(self.flag_resolve_off, self.flags):
+        if dependencies and not self.option_for_resolve_off:
             dependencies: list = self.choose_dependencies_for_remove(list(set(dependencies)))
 
         self.ascii.draw_package_title_box('The following packages will be removed:', 'Slpkg Remove Packages')
 
         for pkg in pkgs:
             if pkg not in dependencies:
                 self._view_removed(pkg)
 
-        if dependencies and not self.utils.is_option(self.flag_resolve_off, self.flags):
+        if dependencies and not self.option_for_resolve_off:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
             for pkg in dependencies:
                 self._view_removed(pkg)
         else:
             dependencies: list = []
@@ -186,17 +194,17 @@
         height: int = 10
         width: int = 70
         list_height: int = 0
         choices: list = []
         title: str = " Choose dependencies you want to remove "
 
         for package in dependencies:
-            repo_ver: str = SBoQueries(package).version()
             inst_pkg: str = self.utils.is_package_installed(package)
-            choices += [(package, repo_ver, True, f'Package: {inst_pkg}')]
+            inst_ver: str = self.utils.split_binary_pkg(inst_pkg)[1]
+            choices += [(package, inst_ver, True, f'Package: {inst_pkg}')]
 
         text: str = f'There are {len(choices)} dependencies:'
 
         code, tags = self.dialogbox.checklist(text, dependencies, title, height,
                                               width, list_height, choices)
 
         if not code:
@@ -205,29 +213,28 @@
         os.system('clear')
         return tags
 
     def summary(self, packages: list, dependencies: list, option: str) -> None:
         """ View the status of the packages action. """
         packages.extend(dependencies)
         install = upgrade = remove = 0
-        reinstall: bool = self.utils.is_option(self.flag_reinstall, self.flags)
 
         for pkg in packages:
 
             upgradeable: bool = False
             if option != 'remove':
                 upgradeable: bool = self.upgrade.is_package_upgradeable(pkg)
 
             installed: str = self.utils.is_package_installed(pkg)
 
             if not installed:
                 install += 1
-            elif installed and reinstall:
+            elif installed and self.option_for_reinstall:
                 upgrade += 1
-            elif installed and upgradeable and reinstall:
+            elif installed and upgradeable and self.option_for_reinstall:
                 upgrade += 1
             elif installed and upgradeable:
                 upgrade += 1
             elif installed and option == 'remove':
                 remove += 1
 
         self.ascii.draw_bottom_line()
@@ -256,12 +263,12 @@
             print(f'{self.yellow}{dep[0]}{self.endc}')
             self.ascii.draw_log_package(dep[1])
 
         print('Note: After cleaning you should remove them one by one.')
 
     def question(self) -> None:
         """ Manage to proceed. """
-        if not self.utils.is_option(self.flag_yes, self.flags) and self.ask_question:
+        if not self.option_for_yes and self.ask_question:
             answer: str = input('\nDo you want to continue? [y/N] ')
             if answer not in ['Y', 'y']:
                 raise SystemExit()
         print()
```

### Comparing `slpkg-4.7.6/slpkg/checks.py` & `slpkg-4.7.8/slpkg/checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 from slpkg.configs import Configs
-from slpkg.blacklist import Blacklist
 from slpkg.utilities import Utilities
-from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
-from slpkg.binaries.queries import BinQueries
 from slpkg.models.models import session as Session
 
 from slpkg.models.models import SBoTable, PonceTable, BinariesTable
 
 
 class Check(Configs):
     """ Some checks before proceed. """
 
-    def __init__(self, flags: list):
+    def __init__(self, flags: list, data: dict):
+        __slots__ = 'flags', 'sbo_repo_dict', 'bin_repo_dict'
         super(Configs, self).__init__()
         self.flags: list = flags
-        self.black = Blacklist()
+        self.data: dict = data
+
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.session = Session
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
 
-        if self.utils.is_option(self.flag_bin_repository, self.flags):
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
+
+        if self.option_for_binaries:
             self.repo_table = BinariesTable
         else:
             self.repo_table = SBoTable
             if self.repos.ponce_repo:
                 self.repo_table = PonceTable
 
-    def exists_in_the_database(self, packages: list, repo=None) -> None:
+    def exists_in_the_database(self, packages: list) -> None:
         """ Checking if the slackbuild exists in the database. """
         not_packages: list = []
 
         for pkg in packages:
 
-            if self.utils.is_option(self.flag_bin_repository, self.flags):
-                if not BinQueries(pkg, repo).package_name() and pkg != '*':
+            if self.option_for_binaries:
+                if not self.data.get(pkg) and pkg != '*':
+                    not_packages.append(pkg)
+            else:
+                if not self.data.get(pkg) and pkg != '*':
                     not_packages.append(pkg)
-
-            elif not SBoQueries(pkg).slackbuild() and pkg != '*':
-                not_packages.append(pkg)
 
         if not_packages:
             self.utils.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists")
 
     def is_package_unsupported(self, slackbuilds: list) -> None:
         """ Checking for unsupported slackbuilds. """
         for sbo in slackbuilds:
             if sbo != '*':
-                sources = SBoQueries(sbo).sources()
+                if self.os_arch == 'x86_64' and self.data[sbo][4]:
+                    sources: list = self.data[sbo][4].split()
+                else:
+                    sources: list = self.data[sbo][3].split()
 
                 if 'UNSUPPORTED' in sources:
                     self.utils.raise_error_message(f"Package '{sbo}' unsupported by arch")
 
     def is_installed(self, packages: list) -> None:
         """ Checking for installed packages. """
         not_found = []
@@ -67,25 +71,14 @@
             package: str = self.utils.is_package_installed(pkg)
             if not package:
                 not_found.append(pkg)
 
         if not_found:
             self.utils.raise_error_message(f'Not found \'{", ".join(not_found)}\' installed packages')
 
-    def is_blacklist(self, package: list) -> None:
-        """ Checking if the packages are blacklisted. """
-        blacklist: list = []
-
-        for pkg in package:
-            if pkg in self.black.packages():
-                blacklist.append(pkg)
-
-        if blacklist:
-            self.utils.raise_error_message(f"The packages '{', '.join(blacklist)}' is blacklisted")
-
     def is_empty_database(self) -> None:
         """ Checking for empty table and database file. """
         db = Path(self.db_path, self.database_name)
         if not self.session.query(self.repo_table).first() or not db.is_file():
             self.utils.raise_error_message("You need to update the package lists first, run:\n\n"
                                            "              $ 'slpkg update'\n"
                                            "              $ 'slpkg update --bin-repo='*' for binaries")
```

### Comparing `slpkg-4.7.6/slpkg/checksum.py` & `slpkg-4.7.8/slpkg/checksum.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 
 import hashlib
 from pathlib import Path
 from typing import Union
 from urllib.parse import unquote
 
 from slpkg.views.ascii import Ascii
-from slpkg.views.views import ViewMessage
 from slpkg.utilities import Utilities
+from slpkg.views.views import ViewMessage
 
 
 class Md5sum:
     """ Checksum the sources. """
 
     def __init__(self, flags: list):
+        __slots__ = 'flags'
         self.flags: list = flags
         self.ascii = Ascii()
         self.utils = Utilities()
 
     def check(self, path: Union[str, Path], source: str, checksum: str) -> None:
         """ Checksum the source. """
         source_file = unquote(source)
```

### Comparing `slpkg-4.7.6/slpkg/dialog_box.py` & `slpkg-4.7.8/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slpkg/configs.py` & `slpkg-4.7.8/slpkg/configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,14 +73,19 @@
     ascii_characters: bool = True
     ask_question: bool = True
     parallel_downloads: bool = False
     file_pattern: str = '*'
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
 
+    http_proxy_address: str = ''
+    socks_proxy_address: str = ''
+    proxy_username: str = ''
+    proxy_password: str = ''
+
     load = Load()
     configs = load.config_file(etc_path, prog_name)
 
     if configs:
         try:
             config = configs['CONFIGS']
 
@@ -100,14 +105,18 @@
             silent_mode: bool = config['SILENT_MODE']
             ascii_characters: bool = config['ASCII_CHARACTERS']
             file_list_suffix: str = config['FILE_LIST_SUFFIX']
             parallel_downloads: bool = config['PARALLEL_DOWNLOADS']
             file_pattern_conf: str = config['FILE_PATTERN']
             progress_spinner: str = config['PROGRESS_SPINNER']
             spinner_color: str = config['SPINNER_COLOR']
+            http_proxy_address: str = config['HTTP_PROXY_ADDRESS']
+            socks_proxy_address: str = config['SOCKS_PROXY_ADDRESS']
+            proxy_username: str = config['PROXY_USERNAME']
+            proxy_password: str = config['PROXY_PASSWORD']
 
         except KeyError as error:
             raise SystemExit(f"\n{prog_name}: {color['bold']}{color['red']}Error{color['endc']}: "
                              f"{error}: in the configuration file '/etc/slpkg/slpkg.toml'.\n"
                              f"\nIf you have upgraded the '{prog_name}' probably you need to run:\n"
                              f"'mv {etc_path}/{prog_name}.toml.new {etc_path}/{prog_name}.toml'.\n"
                              f"or '{color['cyan']}slpkg_new-configs{color['endc']}' command.\n")
```

### Comparing `slpkg-4.7.6/slpkg/clean_logs.py` & `slpkg-4.7.8/slpkg/clean_logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from slpkg.models.models import session as Session
 
 
 class CleanLogsDependencies:
     """ Cleans the logs from packages. """
 
     def __init__(self, flags: list):
+        __slots__ = 'flags'
         self.flags: list = flags
         self.session = Session
 
     def clean(self) -> None:
         """ Deletes the log table from the database. """
         dependencies: list = self.session.query(
             LogsDependencies.name, LogsDependencies.requires).all()  # type: ignore
```

### Comparing `slpkg-4.7.6/slpkg/utilities.py` & `slpkg-4.7.8/slpkg/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import re
 import time
 import shutil
 import logging
+import fnmatch
 import subprocess
 from pathlib import Path
 from typing import Generator, Union
 
 from slpkg.configs import Configs
 from slpkg.blacklist import Blacklist
-from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
-from slpkg.binaries.queries import BinQueries
 from slpkg.logging_config import LoggingConfig
 
 
 class Utilities:
 
     def __init__(self):
         self.configs = Configs
@@ -28,78 +27,58 @@
 
         self.bold: str = self.color['bold']
         self.yellow: str = self.color['yellow']
         self.cyan: str = self.color['cyan']
         self.red: str = self.color['red']
         self.endc: str = self.color['endc']
         self.bred: str = f'{self.bold}{self.red}'
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
 
-        self.installed_packages: list = list(self.all_installed())
-        self.installed_package_names: list = list(self.all_installed_names())
+        self.installed_packages: dict = dict(self.all_installed())
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode='w',
                             encoding='utf-8',
                             level=logging.INFO)
 
     def is_package_installed(self, name: str) -> str:
-        """ Returns the installed package name. """
-        for package in self.installed_packages:
-            pkg_name: str = self.split_binary_pkg(package)[0]
-
-            if pkg_name == name:
-                return package
-
-        return ''
+        """ Returns the installed package binary. """
+        try:
+            return self.installed_packages[name]
+        except KeyError:
+            return ''
 
-    def all_installed(self) -> Generator:
+    def all_installed(self) -> dict:
         """ Return all installed packages from /val/log/packages folder. """
         var_log_packages: Path = Path(self.configs.log_packages)
-        try:
-            for file in var_log_packages.glob(self.configs.file_pattern):
-                name = self.split_binary_pkg(file.name)[0]
-
-                if not name.startswith('.') and name not in self.black.packages():
-                    yield file.name
-        except ValueError as err:
-            logger = logging.getLogger(__name__)
-            logger.info('%s: %s: %s', self.__class__.__name__,
-                        Utilities.all_installed.__name__,
-                        err)
-
-    def all_installed_names(self) -> Generator:
-        """ Return all installed packages names from /val/log/packages folder. """
-        var_log_packages = Path(self.configs.log_packages)
 
         try:
             for file in var_log_packages.glob(self.configs.file_pattern):
                 name = self.split_binary_pkg(file.name)[0]
 
-                if not name.startswith('.') and name not in self.black.packages():
-                    yield name
+                if not name.startswith('.') and not self.blacklist_pattern(name):
+                    yield name, file.name
+
         except ValueError as err:
             logger = logging.getLogger(__name__)
             logger.info('%s: %s: %s', self.__class__.__name__,
-                        Utilities.all_installed_names.__name__,
+                        Utilities.all_installed.__name__,
                         err)
 
     @staticmethod
     def remove_file_if_exists(path: Path, file: str) -> None:
         """ Clean the old files. """
         archive = Path(path, file)
         if archive.is_file():
             archive.unlink()
 
     @staticmethod
     def remove_folder_if_exists(folder: Path) -> None:
         """ Clean the old folders. """
-        directory = Path(folder)
-        if directory.exists():
-            shutil.rmtree(directory)
+        if folder.exists():
+            shutil.rmtree(folder)
 
     @staticmethod
     def create_folder(path: Path, folder: str) -> None:
         """ Creates folder. """
         directory = Path(path, folder)
         if not directory.exists():
             directory.mkdir(parents=True, exist_ok=True)
@@ -117,18 +96,18 @@
 
     def finished_time(self, elapsed_time: float) -> None:
         """ Printing the elapsed time. """
         print(f'\n{self.yellow}Finished Successfully:{self.endc}',
               time.strftime(f'[{self.cyan}%H:%M:%S{self.endc}]',
                             time.gmtime(elapsed_time)))
 
-    def read_sbo_build_tag(self, sbo: str) -> str:
+    def read_sbo_build_tag(self, sbo: str, location: str) -> str:
         """ Returns build tag from .SlackBuild file. """
         build: str = ''
-        location: str = SBoQueries(sbo).location()
+
         sbo_script = Path(self.repos.sbo_repo_path, location, sbo, f'{sbo}.SlackBuild')
 
         if sbo_script.is_file():
             with open(sbo_script, 'r', encoding='utf-8') as f:
                 lines = f.readlines()
 
                 for line in lines:
@@ -197,19 +176,22 @@
 
         if gb >= 0.1:
             file_size = mb
             unit: str = 'GB'
 
         return f'{str(round(file_size, 2))} {unit}'
 
-    def apply_package_pattern(self, flags: list, packages: list, repo=None) -> list:
+    @staticmethod
+    def apply_package_pattern(data: dict, packages: list) -> list:
         """ Apply the pattern. """
         for pkg in packages:
+
             if pkg == '*':
                 packages.remove(pkg)
-
-                if self.is_option(self.flag_bin_repository, flags):
-                    packages += BinQueries('', repo).all_package_names_by_repo()
-                else:
-                    packages += SBoQueries('').sbos()
+                packages += list(data.keys())
 
         return packages
+
+    def blacklist_pattern(self, name):
+        """ This module provides support for Unix shell-style wildcards. """
+        if [black for black in self.black.packages() if fnmatch.fnmatch(name, black)]:
+            return True
```

### Comparing `slpkg-4.7.6/slpkg/dependees.py` & `slpkg-4.7.8/slpkg/dependees.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from typing import Generator
 from slpkg.configs import Configs
 from slpkg.views.ascii import Ascii
 from slpkg.utilities import Utilities
-from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
-from slpkg.binaries.queries import BinQueries
 
 
 class Dependees(Configs):
     """ Show which packages depend. """
 
-    def __init__(self, packages: list, flags: list):
+    def __init__(self, data: dict, packages: list, flags: list):
+        __slots__ = 'data', 'packages', 'flags'
         super(Configs, self).__init__()
+        self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
 
         self.ascii = Ascii()
         self.repos = Repositories()
         self.color = self.colour()
         self.utils = Utilities()
@@ -29,75 +29,83 @@
         self.bold: str = self.color['bold']
         self.violet: str = self.color['violet']
         self.cyan: str = self.color['cyan']
         self.grey: str = self.color['grey']
         self.yellow: str = self.color['yellow']
         self.byellow: str = f'{self.bold}{self.yellow}'
         self.endc: str = self.color['endc']
-        self.flag_full_reverse: list = ['-E', '--full-reverse']
-        self.flag_pkg_version: list = ['-p', '--pkg-version']
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
 
-    def find(self, repo: str) -> None:
+        self.option_for_full_reverse: bool = self.utils.is_option(
+            ['-E', '--full-reverse'], self.flags)
+
+        self.option_for_pkg_version: bool = self.utils.is_option(
+            ['-p', '--pkg-version'], self.flags)
+
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
+
+    def find(self) -> None:
         """ Collecting the dependees. """
         print(f"The list below shows the "
               f"packages that dependees on '{', '.join([p for p in self.packages])}':\n")
 
-        self.packages: list = self.utils.apply_package_pattern(self.flags, self.packages, repo)
+        self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
 
         for pkg in self.packages:
-            dependees: list = list(self.find_requires(pkg, repo))
+            dependees: dict = dict(self.find_requires(pkg))
 
             package: str = f'{self.byellow}{pkg}{self.endc}'
 
-            if self.utils.is_option(self.flag_pkg_version, self.flags):
-                if self.utils.is_option(self.flag_bin_repository, self.flags):
-                    version: str = BinQueries(pkg, repo).version()
+            if self.option_for_pkg_version:
+                if self.option_for_binaries:
+                    version: str = self.data[pkg][0]
                 else:
-                    version: str = SBoQueries(pkg).version()
+                    version: str = self.data[pkg][2]
 
                 package: str = f'{self.byellow}{pkg} {version}{self.endc}'
 
             print(package)
 
             print(f' {self.llc}{self.hl}', end='')
 
             if not dependees:
                 print(f'{self.cyan} No dependees{self.endc}')
 
             sp: str = ' ' * 4
-            for i, dep in enumerate(dependees, start=1):
-                dependency: str = f'{self.cyan}{dep[0]}{self.endc}'
+            for i, (name, requires) in enumerate(dependees.items(), start=1):
+                dependency: str = f'{self.cyan}{name}{self.endc}'
 
-                if self.utils.is_option(self.flag_pkg_version, self.flags):
+                if self.option_for_pkg_version:
 
-                    if self.utils.is_option(self.flag_bin_repository, self.flags):
-                        version: str = BinQueries(dep[0], repo).version()
+                    if self.option_for_binaries:
+                        version: str = self.data[name][0]
                     else:
-                        version: str = SBoQueries(dep[0]).version()
+                        version: str = self.data[name][2]
 
-                    dependency: str = (f'{self.cyan}{dep[0]}{self.endc} {self.yellow}'
+                    dependency: str = (f'{self.cyan}{name}{self.endc} {self.yellow}'
                                        f'{version}{self.endc}')
 
                 if i == 1:
                     print(f' {dependency}')
                 else:
                     print(f'{sp}{dependency}')
 
-                if self.utils.is_option(self.flag_full_reverse, self.flags):
+                if self.option_for_full_reverse:
                     if i == len(dependees):
-                        print(' ' * 4 + f' {self.llc}{self.hl} {self.violet}{dep[1]}{self.endc}')
+                        print(' ' * 4 + f' {self.llc}{self.hl} {self.violet}{requires}{self.endc}')
                     else:
-                        print(' ' * 4 + f' {self.var}{self.hl} {self.violet}{dep[1]}{self.endc}')
+                        print(' ' * 4 + f' {self.var}{self.hl} {self.violet}{requires}{self.endc}')
 
             print(f'\n{self.grey}{len(dependees)} dependees for {pkg}{self.endc}\n')
 
-    def find_requires(self, pkg: str, repo) -> Generator[str, None, None]:
-        """ Find requires that slackbuild dependees. """
-        if self.utils.is_option(self.flag_bin_repository, self.flags):
-            requires: list = BinQueries(pkg, repo).all_package_names_with_required()
-        else:
-            requires: list = SBoQueries('').all_sbo_and_requires()
+    def find_requires(self, pkg: str) -> Generator:
+        """ Find requires that package dependees. """
+        if self.option_for_binaries:
+
+            for name, data in self.data.items():
+                if pkg in data[6].split():
+                    yield name, data[6]
 
-        for req in requires:
-            if [r for r in req[1].split() if r == pkg]:
-                yield req
+        else:
+            for name, data in self.data.items():
+                if pkg in data[7].split():
+                    yield name, data[7]
```

### Comparing `slpkg-4.7.6/slpkg/check_updates.py` & `slpkg-4.7.8/slpkg/check_updates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
-import urllib3
 from pathlib import Path
 from multiprocessing import Process
+from urllib3 import PoolManager, ProxyManager, make_headers
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 
 
 class CheckUpdates(Configs):
     """ Check for changes in the ChangeLog file. """
 
     def __init__(self, flags: list, repo: str):
+        __slots__ = 'flags', 'repo'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repo = repo
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.color = self.colour()
         self.repos = Repositories()
 
+        self.compare: dict = {}
+        self.local_chg_txt = None
+        self.repo_chg_txt = None
         self.bold: str = self.color['bold']
         self.green: str = self.color['green']
         self.yellow: str = self.color['yellow']
         self.bgreen: str = f'{self.bold}{self.green}'
         self.endc: str = self.color['endc']
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
-        self.compare: dict = {}
 
-        self.local_chg_txt = None
-        self.repo_chg_txt = None
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
 
     def check(self) -> dict:
         bin_repositories: dict = {
             self.repos.slack_repo_name: self.slack_repository,
             self.repos.slack_extra_repo_name: self.slack_extra_repository,
             self.repos.slack_patches_repo_name: self.slack_patches_repository,
             self.repos.alien_repo_name: self.alien_repository,
@@ -51,15 +53,15 @@
             self.repos.salixos_repo_name: self.salixos_repository,
             self.repos.salixos_extra_repo_name: self.salixos_extra_repository,
             self.repos.salixos_patches_repo_name: self.salixos_patches_repository,
             self.repos.slackel_repo_name: self.slackel_repository,
             self.repos.slint_repo_name: self.slint_repository
         }
 
-        if self.utils.is_option(self.flag_bin_repository, self.flags):
+        if self.option_for_binaries:
 
             for repo in bin_repositories.keys():
                 if repo in self.repos.bin_enabled_repos and repo == self.repo:
                     bin_repositories[repo]()
                     break
 
                 if repo in self.repos.bin_enabled_repos and self.repo == '*':
@@ -162,15 +164,29 @@
         self.local_chg_txt: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
         self.repo_chg_txt: str = f'{self.repos.ponce_repo_mirror}{self.repos.ponce_repo_changelog}'
         self.compare[self.repos.ponce_repo_name] = self.compare_dates()
 
     def compare_dates(self) -> bool:
         local_date: int = 0
         try:
-            http = urllib3.PoolManager()
+            http = PoolManager()
+            proxy_default_headers = make_headers(proxy_basic_auth=f'{self.proxy_username}:{self.proxy_password}')
+
+            if self.http_proxy_address:
+                http = ProxyManager(f'{self.http_proxy_address}', headers=proxy_default_headers)
+
+            elif self.socks_proxy_address:
+                # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
+                try:  # Try to import PySocks if it's installed.
+                    from urllib3.contrib.socks import SOCKSProxyManager
+                except (ModuleNotFoundError, ImportError):
+                    raise SystemExit()
+
+                http = SOCKSProxyManager(f'{self.socks_proxy_address}', headers=proxy_default_headers)
+
             repo = http.request('GET', self.repo_chg_txt)
         except KeyboardInterrupt:
             raise SystemExit(1)
 
         if self.local_chg_txt.is_file():
             local_date = int(os.stat(self.local_chg_txt).st_size)
```

### Comparing `slpkg-4.7.6/slpkg/remove_packages.py` & `slpkg-4.7.8/slpkg/remove_packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from slpkg.models.models import session as Session
 
 
 class RemovePackages(Configs):
     """ Removes installed packages. """
 
     def __init__(self, packages: list, flags: list):
+        __slots__ = 'packages', 'flags'
         super(Configs, self).__init__()
         self.packages: list = packages
         self.flags: list = flags
 
         self.session = Session
         self.color = self.colour()
         self.utils = Utilities()
@@ -35,28 +36,34 @@
         self.bold: str = self.color['bold']
         self.cyan: str = self.color['cyan']
         self.yellow: str = self.color['yellow']
         self.red: str = self.color['red']
         self.endc: str = self.color['endc']
         self.byellow: str = f'{self.bold}{self.yellow}'
         self.bred: str = f'{self.bold}{self.red}'
-        self.flag_resolve_off: list = ['-o', '--resolve-off']
-        self.flag_no_silent: list = ['-n', '--no-silent']
-        self.flag_yes: list = ['-y', '--yes']
+
+        self.option_resolve_off: bool = self.utils.is_option(
+            ['-o', '--resolve-off'], self.flags)
+
+        self.option_for_no_silent: bool = self.utils.is_option(
+            ['-n', '--no-silent'], self.flags)
+
+        self.option_for_yes: bool = self.utils.is_option(
+            ['-y', '--yes'], self.flags)
 
     def remove(self) -> None:
         """ Removes package with dependencies. """
         self.installed_packages, self.dependencies = self.view.remove_packages(self.packages)
 
         self.view.question()
 
         start: float = time.time()
         self.remove_packages()
 
-        if self.dependencies and not self.utils.is_option(self.flag_resolve_off, self.flags):
+        if self.dependencies and not self.option_resolve_off:
             self.delete_deps_logs()
 
         self.delete_main_logs()
 
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
@@ -74,15 +81,15 @@
         dependencies: list = []
         logs: dict = self.query_dependencies()
 
         for package, requires in logs.items():
             if name in requires:
                 dependencies.append(package)
 
-        if dependencies and not self.utils.is_option(self.flag_yes, self.flags) and self.ask_question:
+        if dependencies and not self.option_for_yes and self.ask_question:
             print(f"\n[{self.bred}WARNING!{self.endc}] The package '{self.red}{name}{self.endc}' "
                   f"is a dependency for the packages:")
 
             for dep in dependencies:
                 print(f"{self.cyan:>16}-> {dep}{self.endc}")
 
             answer: str = input('\nDo you want to remove? [y/N] ')
@@ -118,15 +125,15 @@
         for pkg in self.dependencies:
             self.session.query(LogsDependencies).filter(
                 LogsDependencies.name == pkg).delete()
         self.session.commit()
 
     def multi_process(self, command: str, package: str) -> None:
         """ Starting multiprocessing remove process. """
-        if self.silent_mode and not self.utils.is_option(self.flag_no_silent, self.flags):
+        if self.silent_mode and not self.option_for_no_silent:
 
             done: str = f' {self.byellow} Done{self.endc}'
             message: str = f'{self.red}Remove{self.endc}'
             self.stderr = subprocess.DEVNULL
             self.stdout = subprocess.DEVNULL
 
             # Starting multiprocessing
```

### Comparing `slpkg-4.7.6/slpkg/blacklist.py` & `slpkg-4.7.8/slpkg/blacklist.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         self.cyan: str = self.color['cyan']
         self.endc: str = self.color['endc']
         self.bred: str = f'{self.bold}{self.red}'
         self.blacklist_file_toml = Path(self.etc_path, 'blacklist.toml')
 
     def packages(self) -> list:
         """ Reads the blacklist file. """
-
         if self.blacklist_file_toml.is_file():
             try:
                 with open(self.blacklist_file_toml, 'rb') as black:
                     return tomli.load(black)['BLACKLIST']['PACKAGES']
             except (tomli.TOMLDecodeError, KeyError) as error:
                 raise SystemExit(f"\n{self.prog_name} {self.bred}Error{self.endc}: {error}: in the configuration file "
                                  f"'{self.blacklist_file_toml}'.\n"
```

### Comparing `slpkg-4.7.6/slpkg/download_only.py` & `slpkg-4.7.8/slpkg/download_only.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,58 +5,65 @@
 import shutil
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
-from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
-from slpkg.binaries.queries import BinQueries
 from slpkg.models.models import session as Session
 
 
 class Download(Configs):
     """ Download the slackbuilds with the sources only. """
 
     def __init__(self, directory: Path, flags: list):
+        __slots__ = 'directory', 'flags'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.directory: Path = directory
 
         self.repos = Repositories()
         self.utils = Utilities()
         self.session = Session
 
-        self.flag_directory: list = ['-z', '--directory=']
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
+        self.option_for_directory: bool = self.utils.is_option(
+            ['-z', '--directory='], self.flags)
 
-    def packages(self, packages: list, repo=None) -> None:
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
+
+    def packages(self, data: dict, packages: list, repo=None) -> None:
         """ Download the package only. """
-        packages: list = self.utils.apply_package_pattern(self.flags, packages, repo)
-        view = ViewMessage(self.flags, repo)
+        packages: list = self.utils.apply_package_pattern(data, packages)
+
+        view = ViewMessage(self.flags, data, repo)
         view.download_packages(packages, self.directory)
         view.question()
 
         download_path: Path = self.download_only_path
-        if self.utils.is_option(self.flag_directory, self.flags):
+        if self.option_for_directory:
             download_path: Path = self.directory
 
         start: float = time.time()
         urls: list = []
         for pkg in packages:
 
-            if self.utils.is_option(self.flag_bin_repository, self.flags):
-                mirror: str = BinQueries(pkg, repo).mirror()
-                location: str = BinQueries(pkg, repo).location()
-                package: str = BinQueries(pkg, repo).package_bin()
+            if self.option_for_binaries:
+                package: str = data[pkg][1]
+                mirror: str = data[pkg][2]
+                location: str = data[pkg][3]
                 urls.append(f'{mirror}{location}/{package}')
             else:
-                location: str = SBoQueries(pkg).location()
-                sources = SBoQueries(pkg).sources()
+                location: str = data[pkg][0]
+                if self.os_arch == 'x86_64' and data[pkg][4]:
+                    sources = data[pkg][4].split()
+                else:
+                    sources = data[pkg][3].split()
+
                 urls += sources
 
                 if self.repos.ponce_repo:
                     ponce_repo_path_package = Path(self.repos.ponce_repo_path, location, pkg)
                     shutil.copytree(ponce_repo_path_package, Path(download_path, pkg))
                 else:
                     file: str = f'{pkg}{self.repos.sbo_repo_tar_suffix}'
```

### Comparing `slpkg-4.7.6/slpkg/tracking.py` & `slpkg-4.7.8/slpkg/tracking.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,91 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from slpkg.configs import Configs
 from slpkg.views.ascii import Ascii
 from slpkg.utilities import Utilities
-from slpkg.sbos.queries import SBoQueries
-from slpkg.sbos.dependencies import Requires
-from slpkg.binaries.required import Required
-from slpkg.binaries.queries import BinQueries
 
 
 class Tracking(Configs):
     """ Tracking of the package dependencies. """
 
     def __init__(self, flags: list):
+        __slots__ = 'flags'
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.ascii = Ascii()
         self.color = self.colour()
         self.utils = Utilities()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.vl: str = self.ascii.vertical_line
         self.cyan: str = self.color['cyan']
         self.grey: str = self.color['grey']
         self.yellow: str = self.color['yellow']
         self.endc: str = self.color['endc']
-        self.flag_pkg_version: list = ['-p', '--pkg-version']
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
 
-    def packages(self, packages: list, repo: str) -> None:
+        self.option_for_pkg_version: bool = self.utils.is_option(
+            ['-p', '--pkg-version'], self.flags)
+
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
+
+    def packages(self, data: dict, packages: list) -> None:
         """ Prints the packages dependencies. """
         print(f"The list below shows the packages '{', '.join([p for p in packages])}' with dependencies:\n")
 
-        packages: list = self.utils.apply_package_pattern(self.flags, packages, repo)
+        packages: list = self.utils.apply_package_pattern(data, packages)
 
         char: str = f' {self.llc}{self.hl}'
         sp: str = ' ' * 4
 
         for package in packages:
             pkg = f'{self.yellow}{package}{self.endc}'
 
-            if self.utils.is_option(self.flag_pkg_version, self.flags):
+            if self.option_for_pkg_version:
 
-                version: str = SBoQueries(package).version()
-                if self.utils.is_option(self.flag_bin_repository, self.flags):
-                    version: str = BinQueries(package, repo).version()
+                if self.option_for_binaries:
+                    version: str = data[package][0]
+                else:
+                    version: str = data[package][2]
 
                 pkg = f'{self.yellow}{package} {version}{self.endc}'
 
-            if self.utils.is_option(self.flag_bin_repository, self.flags):
-                requires: list = Required(package, repo).resolve()
+            if self.option_for_binaries:
+                requires: list = data[package][6].split()
             else:
-                requires: list = Requires(package).resolve()
+                requires: list = data[package][7].split()
 
             how_many: int = len(requires)
 
             print(pkg)
             print(char, end='')
 
             if not requires:
                 print(f' {self.cyan}No dependencies{self.endc}')
             else:
                 for i, req in enumerate(requires, start=1):
-                    require: str = f'{self.cyan}{req}{self.endc}'
 
-                    if self.utils.is_option(self.flag_pkg_version, self.flags):
+                    if not self.utils.blacklist_pattern(req):
+
+                        require: str = f'{self.cyan}{req}{self.endc}'
+
+                        if self.option_for_pkg_version:
 
-                        version: str = f" {self.yellow}{SBoQueries(req).version()}{self.endc}"
-                        if self.utils.is_option(self.flag_bin_repository, self.flags):
-                            version: str = f" {self.yellow}{BinQueries(req, repo).version()}{self.endc}"
+                            if self.option_for_binaries:
+                                version: str = ' (not included)'
+                                if data.get(req):
+                                    version: str = f' {self.yellow}{data[req][0]}{self.endc}'
+                            else:
+                                version: str = f' {self.yellow}{data[req][2]}{self.endc}'
 
-                        require: str = f'{self.cyan}{req}{self.endc}{version}'
+                            require: str = f'{self.cyan}{req}{self.endc}{version}'
 
-                    if i == 1:
-                        print(f' {require}')
-                    else:
-                        print(f'{sp}{require}')
+                        if i == 1:
+                            print(f' {require}')
+                        else:
+                            print(f'{sp}{require}')
 
             print(f'\n{self.grey}{how_many} dependencies for {package}{self.endc}\n')
```

### Comparing `slpkg-4.7.6/slpkg/main.py` & `slpkg-4.7.8/slpkg/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from slpkg.clean_logs import CleanLogsDependencies
 from slpkg.update_repository import UpdateRepository
 
 
 class Argparse(Configs):
 
     def __init__(self, args: list):
+        __slots__ = 'args'
         super(Configs).__init__()
         self.args: list = args
         self.flags: list = []
         self.directory = self.tmp_slpkg
         self.dialogbox = DialogBox()
         self.utils = Utilities()
         self.usage = Usage()
@@ -54,14 +55,15 @@
         self.endc: str = self.color['endc']
         self.bred: str = f'{self.bold}{self.red}'
         self.binary_repo: str = ''
 
         if len(self.args) == 0 or '' in self.args:
             self.usage.help_short(1)
 
+        self.data: dict = {}
         self.flag_yes: str = '--yes'
         self.flag_short_yes: str = '-y'
         self.flag_jobs: str = '--jobs'
         self.flag_short_jobs: str = '-j'
         self.flag_resolve_off: str = '--resolve-off'
         self.flag_short_resolve_off: str = '-o'
         self.flag_reinstall: str = '--reinstall'
@@ -278,16 +280,20 @@
 
         self.split_options()
         self.split_options_from_args()
         self.move_options()
         self.invalid_options()
         self.check_for_bin_repositories()
 
-        self.check = Check(self.flags)
-        self.check.is_blacklist(self.args[1:])
+        if self.utils.is_option(self.flag_binaries, self.flags):
+            self.data: dict = BinQueries(self.binary_repo).repository_data()
+        else:
+            self.data: dict = SBoQueries().repository_data()
+
+        self.check = Check(self.flags, self.data)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode='w',
                             encoding='utf-8',
                             level=logging.INFO)
 
     def check_for_bin_repositories(self) -> None:
@@ -296,15 +302,18 @@
 
             except_options: list = [
                 '-s', 'search',
                 '-u', 'update',
                 '-c', 'check-updates',
             ]
 
-            if self.binary_repo == '*' and not self.utils.is_option(except_options, self.args):
+            if self.binary_repo in self.repos.bin_repos_names and self.binary_repo not in self.repos.bin_enabled_repos:
+                self.usage.help_minimal(f"{self.prog_name}: repository '{self.binary_repo}' is disabled")
+
+            elif self.binary_repo == '*' and not self.utils.is_option(except_options, self.args):
                 self.usage.help_minimal(f"{self.prog_name}: invalid binary repository '{self.binary_repo}'")
 
             elif self.binary_repo not in self.repos.bin_repos_names and self.binary_repo != '*':
                 self.usage.help_minimal(f"{self.prog_name}: invalid binary repository '{self.binary_repo}'")
 
     def invalid_options(self) -> None:
         """ Checks for invalid options. """
@@ -422,58 +431,60 @@
         """ Choose packages with dialog utility and -S, --search flag. """
         height: int = 10
         width: int = 70
         list_height: int = 0
         choices: list = []
         title: str = f' Choose packages you want to {method} '
 
-        repo_packages: list = list(SBoQueries('').sbos())
-        if self.utils.is_option(self.flag_binaries, self.flags):
-            repo_packages: list = list(BinQueries('', self.binary_repo).all_package_names_by_repo())
-
-        installed: list = self.utils.installed_packages
+        repo_packages: list = list(self.data.keys())
 
         if method in ['remove', 'find']:
+            installed: list = list(self.utils.installed_packages.values())
 
             for package in installed:
                 split_package: list = self.utils.split_binary_pkg(package)
 
                 for pkg in packages:
-                    if pkg in split_package[0]:
+
+                    if pkg in package or pkg == '*':
                         choices += [(split_package[0], split_package[1], False, f'Package: {package}')]
 
         elif method == 'upgrade':
             for pkg in packages:
                 for package in repo_packages:
 
                     if pkg == package:
 
                         inst_pkg: str = self.utils.is_package_installed(package)
                         split_inst_pkg: list = self.utils.split_binary_pkg(inst_pkg)
 
                         if self.utils.is_option(self.flag_binaries, self.flags):
-                            repo_ver: str = BinQueries(package, self.binary_repo).version()
-                            bin_pkg: str = BinQueries(package, self.binary_repo).package_bin()
+                            repo_ver: str = self.data[package][0]
+                            bin_pkg: str = self.data[package][1]
                             repo_build_tag: str = self.utils.split_binary_pkg(bin_pkg[:-4])[3]
                         else:
-                            repo_ver: str = SBoQueries(package).version()
-                            repo_build_tag: str = self.utils.read_sbo_build_tag(package)
+                            repo_ver: str = self.data[package][2]
+                            repo_location: str = self.data[package][0]
+                            repo_build_tag: str = self.utils.read_sbo_build_tag(package, repo_location)
 
                         choices += [(package, f'{split_inst_pkg[1]} -> {repo_ver}', True,
                                      f'Installed: {package}-{split_inst_pkg[1]} Build: {split_inst_pkg[3]} -> '
                                      f'Available: {repo_ver} Build: {repo_build_tag}')]
         else:
             for pkg in packages:
                 for package in repo_packages:
-                    if pkg in package:
+                    if pkg in package or pkg == '*':
                         if self.utils.is_option(self.flag_binaries, self.flags):
-                            repo_ver: str = BinQueries(package, self.binary_repo).version()
-                            repo: str = BinQueries(package, self.binary_repo).repository()
+                            try:
+                                repo_ver: str = self.data[pkg][0]
+                            except KeyError:
+                                repo_ver: str = ''
+                            repo: str = self.binary_repo
                         else:
-                            repo_ver: str = SBoQueries(package).version()
+                            repo_ver: str = self.data[package][2]
                             repo: str = self.repos.sbo_enabled_repository
                         choices += [(package, repo_ver, False, f'Package: {package}-{repo_ver} '
                                                                f'> {repo}')]
 
         if not choices:
             return packages
 
@@ -511,28 +522,28 @@
 
     def upgrade(self) -> None:
         command = Argparse.upgrade.__name__
 
         if len(self.args) == 1:
             self.check.is_empty_database()
 
-            upgrade = Upgrade(self.flags, self.binary_repo)
+            upgrade = Upgrade(self.flags, self.data, self.binary_repo)
             packages: list = list(upgrade.packages())
 
             packages: list = self.choose_packages(packages, command)
 
             if not packages:
                 print('\nEverything is up-to-date!\n')
                 raise SystemExit()
 
             if self.utils.is_option(self.flag_binaries, self.flags):
-                install = Packages(packages, self.flags, self.binary_repo, mode=command)
+                install = Packages(self.data, packages, self.flags, self.binary_repo, mode=command)
                 install.execute()
             else:
-                install = Slackbuilds(packages, self.flags, mode=command)
+                install = Slackbuilds(self.data, packages, self.flags, mode=command)
                 install.execute()
             raise SystemExit()
         self.usage.help_short(1)
 
     def check_updates(self) -> None:
         if len(self.args) == 1:
             check = CheckUpdates(self.flags, self.binary_repo)
@@ -596,15 +607,15 @@
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.exists_in_the_database(packages)
             self.check.is_package_unsupported(packages)
 
-            build = Slackbuilds(packages, self.flags, mode=command)
+            build = Slackbuilds(self.data, packages, self.flags, mode=command)
             build.execute()
             raise SystemExit()
         self.usage.help_short(1)
 
     def install(self) -> None:
         command = Argparse.install.__name__
 
@@ -613,23 +624,23 @@
             self.check.is_empty_database()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             if self.utils.is_option(self.flag_binaries, self.flags):
-                self.check.exists_in_the_database(packages, self.binary_repo)
+                self.check.exists_in_the_database(packages)
 
-                install = Packages(packages, self.flags, self.binary_repo, mode=command)
+                install = Packages(self.data, packages, self.flags, self.binary_repo, mode=command)
                 install.execute()
             else:
                 self.check.exists_in_the_database(packages)
                 self.check.is_package_unsupported(packages)
 
-                install = Slackbuilds(packages, self.flags, mode=command)
+                install = Slackbuilds(self.data, packages, self.flags, mode=command)
                 install.execute()
             raise SystemExit()
         self.usage.help_short(1)
 
     def download(self) -> None:
         command = Argparse.download.__name__
 
@@ -637,17 +648,17 @@
 
             self.check.is_empty_database()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages, self.binary_repo)
+            self.check.exists_in_the_database(packages)
             download = Download(self.directory, self.flags)
-            download.packages(packages, self.binary_repo)
+            download.packages(self.data, packages, self.binary_repo)
             raise SystemExit()
         self.usage.help_short(1)
 
     def remove(self) -> None:
         command = Argparse.remove.__name__
 
         if len(self.args) >= 2:
@@ -687,22 +698,22 @@
 
             self.check.is_empty_database()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages, self.binary_repo)
+            self.check.exists_in_the_database(packages)
 
             view = ViewPackage(self.flags)
 
             if self.utils.is_option(self.flag_binaries, self.flags):
-                view.package(packages, self.binary_repo)
+                view.package(self.data, packages, self.binary_repo)
             else:
-                view.slackbuild(packages)
+                view.slackbuild(self.data, packages)
             raise SystemExit()
         self.usage.help_short(1)
 
     def search(self) -> None:
         command = Argparse.search.__name__
 
         if len(self.args) >= 2:
@@ -710,51 +721,51 @@
             self.check.is_empty_database()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             search = SearchPackage(self.flags)
-            search.package(packages, self.binary_repo)
+            search.package(self.data, packages, self.binary_repo)
             raise SystemExit()
         self.usage.help_short(1)
 
     def dependees(self) -> None:
         command = Argparse.dependees.__name__
 
         if len(self.args) >= 2:
 
             self.check.is_empty_database()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages, self.binary_repo)
+            self.check.exists_in_the_database(packages)
 
-            dependees = Dependees(packages, self.flags)
-            dependees.find(self.binary_repo)
+            dependees = Dependees(self.data, packages, self.flags)
+            dependees.find()
             raise SystemExit()
         self.usage.help_short(1)
 
     def tracking(self) -> None:
         command = Argparse.tracking.__name__
 
         if len(self.args) >= 2:
 
             self.check.is_empty_database()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages, self.binary_repo)
+            self.check.exists_in_the_database(packages)
 
             tracking = Tracking(self.flags)
-            tracking.packages(packages, self.binary_repo)
+            tracking.packages(self.data, packages)
             raise SystemExit()
         self.usage.help_short(1)
 
     def help_for_commands(self) -> None:
         """ Extra help information for commands. """
         if len(self.args) == 2:
             try:
@@ -811,17 +822,23 @@
         '-s': argparse.search,
         'dependees': argparse.dependees,
         '-e': argparse.dependees,
         'tracking': argparse.tracking,
         '-t': argparse.tracking
     }
 
-    try:
-        arguments[args[0]]()
-    except (KeyError, IndexError) as err:
-        logger = logging.getLogger(__name__)
-        logger.info('%s: %s', main.__name__, err)
-        usage.help_short(1)
+    # try:
+    #     arguments[args[0]]()
+    # except (KeyError, IndexError) as err:
+    #     logger = logging.getLogger(__name__)
+    #     logger.info('%s: %s', main.__name__, err)
+    #     usage.help_short(1)
+
+    # For development mode.
+    arguments[args[0]]()
+    logger = logging.getLogger(__name__)
+    logger.info('%s: %s', main.__name__, err)
+    usage.help_short(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `slpkg-4.7.6/slpkg/find_installed.py` & `slpkg-4.7.8/slpkg/find_installed.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,25 +17,25 @@
         self.yellow: str = self.color['yellow']
         self.cyan: str = self.color['cyan']
         self.green: str = self.color['green']
         self.blue: str = self.color['blue']
         self.endc: str = self.color['endc']
         self.grey: str = self.color['grey']
 
-        self.installed: list = self.utils.installed_packages
+        self.installed: dict = self.utils.installed_packages
 
     def find(self, packages: list) -> None:
         """ Find the packages. """
         matching: list = []
 
         print(f'The list below shows the installed packages '
               f'that contains \'{", ".join([p for p in packages])}\' files:\n')
 
         for pkg in packages:
-            for package in self.installed:
+            for package in self.installed.values():
                 if pkg in package or pkg == '*':
                     matching.append(package)
 
         self.matched(matching)
 
     def matched(self, matching: list) -> None:
         """ Print the matched packages. """
```

### Comparing `slpkg-4.7.6/slpkg/upgrade.py` & `slpkg-4.7.8/slpkg/upgrade.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,77 +3,71 @@
 
 import logging
 from typing import Generator
 from packaging.version import parse, InvalidVersion
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
-from slpkg.sbos.queries import SBoQueries
-from slpkg.binaries.queries import BinQueries
-from slpkg.logging_config import LoggingConfig
 from slpkg.repositories import Repositories
+from slpkg.logging_config import LoggingConfig
 
 
 class Upgrade(Configs):
     """ Upgrade the installed packages. """
 
-    def __init__(self, flags: list, repo=None):
+    def __init__(self, flags: list, data: dict, repo=None):
+        __slots__ = 'flags', 'data', 'repo'
         super(Configs, self).__init__()
         self.flags: list = flags
+        self.data: dict = data
         self.repo: str = repo
         self.utils = Utilities()
         self.repos = Repositories()
 
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
-        self.repo_for_binaries: bool = self.utils.is_option(self.flag_bin_repository, self.flags)
-
-        self.all_installed: list = self.utils.installed_package_names
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
 
         logging.basicConfig(filename=str(LoggingConfig.log_file),
                             filemode='w',
                             encoding='utf-8',
                             level=logging.INFO)
 
-    def packages(self) -> Generator[str, None, None]:
+    def packages(self) -> Generator:
         """ Returns the upgradable packages. """
-        if self.utils.is_option(self.flag_bin_repository, self.flags):
-            repo_packages: list = list(BinQueries('', self.repo).all_package_names_by_repo())
-        else:
-            repo_packages: list = list(SBoQueries('').sbos())
 
-        # Compares two lists and get only the installed packages from the repository.
-        packages: list = list(set(self.all_installed) & set(repo_packages))
+        # Returns the matched packages between two lists.
+        packages: list = list(set(self.utils.installed_packages.keys()) & set(list(self.data.keys())))
 
         for pkg in packages:
-
             if self.is_package_upgradeable(pkg):
                 yield pkg
 
     def is_package_upgradeable(self, name: str) -> bool:
         """ Compares version of packages and returns the maximum. """
         repo_version = repo_build = '0'
         inst_version = inst_build = '0'
         inst_package: str = self.utils.is_package_installed(name)
 
         repo_tag: str = self.repos.repo_tag
-        if self.repo_for_binaries:
+        if self.option_for_binaries:
             repo_tag: str = self.repos.repositories[self.repo][3]
 
         if inst_package and inst_package.endswith(repo_tag):
             inst_version: str = self.utils.split_binary_pkg(inst_package)[1]
             inst_build: str = self.utils.split_binary_pkg(inst_package)[3]
 
-            if self.repo_for_binaries and BinQueries(name, self.repo).package_bin():
-                repo_package: str = BinQueries(name, self.repo).package_bin()
-                repo_version: str = BinQueries(name, self.repo).version()
+            if self.option_for_binaries and self.data.get(name):
+                repo_version: str = self.data[name][0]
+                repo_package: str = self.data[name][1]
                 repo_build: str = self.utils.split_binary_pkg(repo_package)[3]
 
-            elif not self.repo_for_binaries and SBoQueries(name).slackbuild():
-                repo_version: str = SBoQueries(name).version()
-                repo_build: str = self.utils.read_sbo_build_tag(name)
+            else:
+                repo_version: str = self.data[name][2]
+                repo_location: str = self.data[name][0]
+                repo_build: str = self.utils.read_sbo_build_tag(name, repo_location)
 
         try:
             if parse(repo_version) > parse(inst_version):
                 return True
 
             if parse(repo_version) == parse(inst_version) and parse(repo_build) > parse(inst_build):
                 return True
```

### Comparing `slpkg-4.7.6/slpkg/search.py` & `slpkg-4.7.8/slpkg/search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,80 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-from typing import Generator
-
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
-from slpkg.sbos.queries import SBoQueries
 from slpkg.repositories import Repositories
 from slpkg.binaries.queries import BinQueries
 
 
 class SearchPackage(Configs):
     """ Search packages from the repositories. """
 
     def __init__(self, flags=None):
+        __slots__ = 'flags'
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.color = self.colour()
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.yellow: str = self.color['yellow']
         self.cyan: str = self.color['cyan']
         self.green: str = self.color['green']
         self.grey: str = self.color['grey']
         self.endc: str = self.color['endc']
 
-        self.flag_bin_repository: list = ['-B', '--bin-repo=']
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], self.flags)
 
-    def package(self, packages: list, repo=None) -> None:
+    def package(self, data: dict, packages: list, repo: str) -> None:
         """ Searching and print the matched packages. """
-        matching: int = 0
-        repository: str = ''
-
         print(f'The list below shows the repo '
               f'packages that contains \'{", ".join([p for p in packages])}\':\n')
 
+        matching: int = 0
+
         # Searching for binaries.
-        if self.utils.is_option(self.flag_bin_repository, self.flags):
-            if repo == '*':
-                pkg_repo: tuple = BinQueries('', repo).all_package_names_from_repositories()
+        if self.option_for_binaries:
 
-                for pkg in packages:
-                    for pr in pkg_repo:
+            if repo == '*':
+                data: dict = BinQueries('').repositories_data()
+                for package in packages:
+                    for data_pkg in data.values():
 
-                        if pkg in pr[0] or pkg == '*':
+                        if package in data_pkg[0] or package == '*':
                             matching += 1
 
-                            desc: str = BinQueries(pr[0], pr[1]).description()
-                            version: str = BinQueries(pr[0], pr[1]).version()
-
-                            if repo == '*':
-                                repository: str = f'{pr[1]}: '
+                            print(f'{data_pkg[12]}: {self.cyan}{data_pkg[0]}{self.endc} '
+                                  f'{self.yellow}{data_pkg[1]}{self.endc} {self.green}{data_pkg[10]}{self.endc}')
 
-                            print(f'{repository}{self.cyan}{pr[0]}{self.endc} {self.yellow}{version}{self.endc}'
-                                  f'{self.green}{desc}{self.endc}')
             else:
-                pkg_repo: Generator = BinQueries('', repo).all_package_names_by_repo()
-
-                for pkg in packages:
-                    for pr in pkg_repo:
+                for package in packages:
+                    for name, data_pkg in data.items():
 
-                        if pkg in pr or pkg == '*':
+                        if package in name or package == '*':
                             matching += 1
 
-                            desc: str = BinQueries(pr, repo).description()
-                            version: str = BinQueries(pr, repo).version()
-
-                            print(f'{repository}{self.cyan}{pr}{self.endc} {self.yellow}{version}{self.endc}'
-                                  f'{self.green}{desc}{self.endc}')
+                            print(f'{data_pkg[11]}: {self.cyan}{name}{self.endc} {self.yellow}{data_pkg[0]}{self.endc}'
+                                  f'{self.green}{data_pkg[9]}{self.endc}')
 
         else:
             # Searching for slackbuilds.
-            names: Generator = SBoQueries('').sbos()
-            for name in names:
-                for package in packages:
+            names: list = list(data.keys())
+            for package in packages:
+                for name in names:
 
                     if package in name or package == '*':
                         matching += 1
 
-                        desc: str = SBoQueries(name).description().replace(name, '')
-                        version: str = SBoQueries(name).version()
+                        version: str = data[name][2]
+                        desc: str = data[name][8].replace(name, '')
 
-                        print(f'{self.cyan}{name}{self.endc}-{self.yellow}'
-                              f'{version}{self.endc}{self.green}{desc}{self.endc}')
+                        print(f'{self.cyan}{name}{self.endc} {self.yellow}{version}{self.endc}'
+                              f'{self.green}{desc}{self.endc}')
 
         if not matching:
             print('\nDoes not match any package.\n')
         else:
             print(f'\n{self.grey}Total found {matching} packages.{self.endc}')
```

### Comparing `slpkg-4.7.6/setup.cfg` & `slpkg-4.7.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.7.6
+version = 4.7.8
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = d.zlatanidis@gmail.com
 description = Packaging tool that interacts with the SBo repository
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls = 
@@ -39,9 +39,13 @@
 python_requires = >= 3.9
 install_requires = 
 	SQLAlchemy >= 1.4.46
 	pythondialog >= 3.5.3
 	progress >= 1.6
 include_package_data = True
 
+[options.extras_require]
+socks =
+	PySocks >= 1.7.1
+
 [options.packages.find]
 where = .
```

### Comparing `slpkg-4.7.6/slpkg.egg-info/SOURCES.txt` & `slpkg-4.7.8/slpkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/slpkg.egg-info/PKG-INFO` & `slpkg-4.7.8/slpkg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.7.6
+Version: 4.7.8
 Summary: Packaging tool that interacts with the SBo repository
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: d.zlatanidis@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
@@ -23,27 +23,28 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Software Distribution
 Requires-Python: >=3.9
+Provides-Extra: socks
 License-File: LICENSE
 
 .. contents:: Table of Contents:
 
 
 About
 -----
 
 Slpkg is a software package manager that installs, updates and removes packages on `Slackware <http://www.slackware.com/>`_-based systems.
 It automatically calculates dependencies and figures out what things need to happen to install packages. 
 Slpkg makes it easier to manage groups of machines without the need for manual updates.
 
-Slpkg works in accordance with the standards of the `SlackBuilds.org <https://www.slackbuilds.org>`_ organization to build packages. 
+Slpkg works in accordance with the standards of the `SlackBuilds.org <https://www.slackbuilds.org>`__ organization to build packages. 
 It also uses the Slackware Linux instructions for installing, upgrading or removing packages.
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_package.png
     :target: https://gitlab.com/dslackw/slpkg
 
 
 Requirements
@@ -54,20 +55,20 @@
     SQLAlchemy >= 1.4.46
     pythondialog >= 3.5.3
     progress >= 1.6
 
 Install
 -------
 
-Install from the official third-party `SBo repository <https://slackbuilds.org/repository/15.0/system/slpkg/>`_ or directly from source:
+Install it from the official third-party `SlackBuilds.org <https://slackbuilds.org/repository/15.0/system/slpkg/>`__ repository or directly from source:
 
 .. code-block:: bash
 
-    $ tar xvf slpkg-4.7.6.tar.gz
-    $ cd slpkg-4.7.6
+    $ tar xvf slpkg-4.7.8.tar.gz
+    $ cd slpkg-4.7.8
     $ ./install.sh
 
 Screenshots
 -----------
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png
     :target: https://gitlab.com/dslackw/slpkg
@@ -128,14 +129,79 @@
         -v, --version                 Print version and exit.
 
    If you need more information try to use slpkg manpage.
    Extra help for the commands, use: 'slpkg help [command]'.
    Edit the config file in the /etc/slpkg/slpkg.toml or 'slpkg configs'.
 
 
+How to start
+------------
+
+If you are going to use only the `SlackBuilds.org <https://slackbuilds.org/>`__ repository, you don't need to edit the
+:code:`/etc/slpkg/repositories.toml` file, otherwise edit the file and set :code:`true` the repositories you want.
+
+The second step is to update the package lists and install the data to the database, just run:
+
+.. code-block:: bash
+
+    $ slpkg update
+
+or for binary repositories:
+
+.. code-block:: bash
+
+    $ slpkg update --bin-repo='*'
+
+Now you are ready to start!
+
+To install a package from the `SlackBuilds.org <https://slackbuilds.org/>`__ or `Ponce <https://cgit.ponce.cc/slackbuilds/>`_ repository, run:
+
+.. code-block:: bash
+
+    $ slpkg install <package_name>
+
+or from a binary repository:
+
+.. code-block:: bash
+
+    $ slpkg install <package_name> --bin-repo=<repo_name>
+
+You can install a whole repository with the command:
+
+.. code-block:: bash
+
+    $ slpkg install '*' --bin-repo=<repository_name> --resolve-off
+
+Note: Apply the option '--resolve-off' to speed up the process, if the repository has no references to the dependencies.
+
+To remove a package with the dependencies:
+
+.. code-block:: bash
+
+    $ slpkg remove <package_name>
+
+If you wan to search a package from all binaries repositories, run:
+
+.. code-block:: bash
+
+    $ slpkg search <package_name> --bin-repo='*'
+
+Edit the configuration :code:`/etc/slpkg/slpkg.toml` file:
+
+.. code-block:: bash
+
+    $ slpkg configs
+
+
+For further information, please read the manpage:
+
+.. code-block:: bash
+
+    $ man slpkg
+
 
 Configuration files
 -------------------
 
 .. code-block:: bash
 
     /etc/slpkg/slpkg.toml
@@ -184,14 +250,19 @@
 ------
 
 If you feel satisfied with this project and want to thanks me make a donation.
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/donate/paypaldonate.png
    :target: https://www.paypal.me/dslackw
 
+Report bugs
+-----------
+
+Please report any issue here: `Issues <https://gitlab.com/dslackw/slpkg/-/issues>`_
+
 
 Copyright
 ---------
 
 - Copyright 2014-2023 © Dimitris Zlatanidis.
 - Slackware® is a Registered Trademark of Patrick Volkerding. 
 - Linux is a Registered Trademark of Linus Torvalds.
```

### Comparing `slpkg-4.7.6/tools/gen_sbo_txt.sh` & `slpkg-4.7.8/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.6/bin/slpkg_new-configs` & `slpkg-4.7.8/bin/slpkg_new-configs`

 * *Files identical despite different names*

