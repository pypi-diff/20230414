# Comparing `tmp/chibi_command-0.4.1.tar.gz` & `tmp/chibi_command-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chibi_command-0.4.1.tar", last modified: Mon Jan 24 03:52:31 2022, max compression
+gzip compressed data, was "chibi_command-0.4.2.tar", last modified: Fri Apr 14 17:44:27 2023, max compression
```

## Comparing `chibi_command-0.4.1.tar` & `chibi_command-0.4.2.tar`

### file list

```diff
@@ -1,105 +1,108 @@
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.125767 chibi_command-0.4.1/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-02-22 02:37:10.000000 chibi_command-0.4.1/AUTHORS.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3598 2020-02-22 02:37:10.000000 chibi_command-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       89 2020-02-22 02:37:10.000000 chibi_command-0.4.1/HISTORY.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2020-02-22 02:37:10.000000 chibi_command-0.4.1/LICENSE
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2020-02-22 02:37:10.000000 chibi_command-0.4.1/MANIFEST.in
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1884 2022-01-24 03:52:31.129101 chibi_command-0.4.1/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      889 2020-02-22 02:37:10.000000 chibi_command-0.4.1/README.rst
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.119101 chibi_command-0.4.1/chibi_command/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5502 2022-01-24 03:52:25.000000 chibi_command-0.4.1/chibi_command/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.119101 chibi_command-0.4.1/chibi_command/centos/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      145 2021-09-17 00:55:39.000000 chibi_command-0.4.1/chibi_command/centos/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1528 2022-01-24 03:51:53.000000 chibi_command-0.4.1/chibi_command/centos/dnf.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3788 2021-10-28 23:36:56.000000 chibi_command-0.4.1/chibi_command/centos/iptable.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2132 2021-09-17 00:55:32.000000 chibi_command-0.4.1/chibi_command/centos/yum.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      398 2019-09-09 16:26:47.000000 chibi_command-0.4.1/chibi_command/db.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      186 2019-10-02 15:07:59.000000 chibi_command-0.4.1/chibi_command/dd.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.122434 chibi_command-0.4.1/chibi_command/disk/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-24 07:17:23.000000 chibi_command-0.4.1/chibi_command/disk/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1057 2020-02-22 02:34:14.000000 chibi_command-0.4.1/chibi_command/disk/dd.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      176 2020-04-05 20:30:23.000000 chibi_command-0.4.1/chibi_command/disk/format.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      223 2020-04-05 21:53:54.000000 chibi_command-0.4.1/chibi_command/disk/mount.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      451 2020-03-02 15:15:53.000000 chibi_command-0.4.1/chibi_command/echo.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      124 2019-08-16 20:41:47.000000 chibi_command-0.4.1/chibi_command/ffmpeg.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      128 2020-03-10 21:10:35.000000 chibi_command-0.4.1/chibi_command/file.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3011 2021-12-09 01:34:46.000000 chibi_command-0.4.1/chibi_command/git.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.122434 chibi_command-0.4.1/chibi_command/image/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-09-03 15:04:53.000000 chibi_command-0.4.1/chibi_command/image/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      973 2019-09-03 15:15:41.000000 chibi_command-0.4.1/chibi_command/image/convert.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1427 2020-03-10 23:37:01.000000 chibi_command-0.4.1/chibi_command/image/qr.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.122434 chibi_command-0.4.1/chibi_command/lxc/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       63 2022-01-14 21:07:02.000000 chibi_command-0.4.1/chibi_command/lxc/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      569 2022-01-14 22:56:18.000000 chibi_command-0.4.1/chibi_command/lxc/delegate.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2753 2022-01-14 22:47:34.000000 chibi_command-0.4.1/chibi_command/lxc/lxc.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      509 2019-12-24 15:20:08.000000 chibi_command-0.4.1/chibi_command/mpd.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.122434 chibi_command-0.4.1/chibi_command/network/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       57 2020-03-02 15:17:31.000000 chibi_command-0.4.1/chibi_command/network/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      702 2021-06-22 05:36:13.000000 chibi_command-0.4.1/chibi_command/network/ifconfig.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2850 2021-06-22 20:27:11.000000 chibi_command-0.4.1/chibi_command/network/interfaces.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      742 2021-06-22 19:27:10.000000 chibi_command-0.4.1/chibi_command/network/iwconfig.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      460 2020-10-21 09:00:09.000000 chibi_command-0.4.1/chibi_command/network/nmap.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1918 2020-01-08 04:55:57.000000 chibi_command-0.4.1/chibi_command/network/nmcli.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.122434 chibi_command-0.4.1/chibi_command/nix/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      132 2021-03-29 04:54:05.000000 chibi_command-0.4.1/chibi_command/nix/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      393 2021-03-29 04:56:19.000000 chibi_command-0.4.1/chibi_command/nix/locale.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2309 2022-01-23 23:53:11.000000 chibi_command-0.4.1/chibi_command/nix/systemd.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1139 2022-01-24 00:00:33.000000 chibi_command-0.4.1/chibi_command/nix/systemd_run.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      943 2020-03-05 03:47:09.000000 chibi_command-0.4.1/chibi_command/nix/user.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      763 2021-03-29 04:59:39.000000 chibi_command-0.4.1/chibi_command/qr.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      796 2019-12-24 15:25:42.000000 chibi_command-0.4.1/chibi_command/rabbitmq.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      240 2019-12-24 15:28:53.000000 chibi_command-0.4.1/chibi_command/rpm.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2074 2021-09-16 23:22:52.000000 chibi_command-0.4.1/chibi_command/rsync.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      405 2021-09-16 23:19:35.000000 chibi_command-0.4.1/chibi_command/sysctl.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      758 2020-03-02 15:17:03.000000 chibi_command-0.4.1/chibi_command/xfce4.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.119101 chibi_command-0.4.1/chibi_command.egg-info/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1884 2022-01-24 03:52:30.000000 chibi_command-0.4.1/chibi_command.egg-info/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2056 2022-01-24 03:52:30.000000 chibi_command-0.4.1/chibi_command.egg-info/SOURCES.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2022-01-24 03:52:30.000000 chibi_command-0.4.1/chibi_command.egg-info/dependency_links.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2022-01-24 03:52:30.000000 chibi_command-0.4.1/chibi_command.egg-info/not-zip-safe
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       43 2022-01-24 03:52:30.000000 chibi_command-0.4.1/chibi_command.egg-info/requires.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       14 2022-01-24 03:52:30.000000 chibi_command-0.4.1/chibi_command.egg-info/top_level.txt
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.125767 chibi_command-0.4.1/docs/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      614 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/Makefile
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/authors.rst
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4872 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/conf.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/contributing.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/history.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      310 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/index.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1158 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/installation.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      775 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/make.bat
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/readme.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       81 2020-02-22 02:37:10.000000 chibi_command-0.4.1/docs/usage.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      451 2022-01-24 03:52:31.129101 chibi_command-0.4.1/setup.cfg
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1095 2022-01-24 03:52:25.000000 chibi_command-0.4.1/setup.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.125767 chibi_command-0.4.1/tests/
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2018-06-27 08:43:08.000000 chibi_command-0.4.1/tests/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2639 2021-10-28 23:37:46.000000 chibi_command-0.4.1/tests/centos.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3014 2022-01-23 23:33:44.000000 chibi_command-0.4.1/tests/command.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      888 2022-01-23 21:58:14.000000 chibi_command-0.4.1/tests/command_result.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.125767 chibi_command-0.4.1/tests/disk/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-02-09 22:05:59.000000 chibi_command-0.4.1/tests/disk/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      854 2020-03-05 03:19:52.000000 chibi_command-0.4.1/tests/disk/dd.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.125767 chibi_command-0.4.1/tests/echo/
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2018-06-27 08:43:08.000000 chibi_command-0.4.1/tests/echo/__init__.py
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1489 2019-09-09 15:53:10.000000 chibi_command-0.4.1/tests/echo/test_echo.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2080 2021-12-09 17:56:18.000000 chibi_command-0.4.1/tests/git.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.125767 chibi_command-0.4.1/tests/image/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-09-03 15:17:47.000000 chibi_command-0.4.1/tests/image/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       73 2019-09-03 16:47:29.000000 chibi_command-0.4.1/tests/image/convert.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5052 2022-01-23 22:26:47.000000 chibi_command-0.4.1/tests/lxc.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.125767 chibi_command-0.4.1/tests/network/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-24 15:36:50.000000 chibi_command-0.4.1/tests/network/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      441 2021-06-22 05:36:27.000000 chibi_command-0.4.1/tests/network/ifconfig.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2314 2021-06-22 20:26:55.000000 chibi_command-0.4.1/tests/network/interface.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      483 2021-06-22 19:27:41.000000 chibi_command-0.4.1/tests/network/iwconfig.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1305 2020-01-08 04:56:58.000000 chibi_command-0.4.1/tests/network/nmcli.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-01-24 03:52:31.125767 chibi_command-0.4.1/tests/nix/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-05 03:38:01.000000 chibi_command-0.4.1/tests/nix/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      296 2021-03-29 04:56:15.000000 chibi_command-0.4.1/tests/nix/locale.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1626 2022-01-23 23:31:52.000000 chibi_command-0.4.1/tests/nix/systemd.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      805 2022-01-14 23:15:07.000000 chibi_command-0.4.1/tests/nix/systemd_run.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      538 2020-03-05 03:42:36.000000 chibi_command-0.4.1/tests/nix/user.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      948 2020-04-07 22:27:40.000000 chibi_command-0.4.1/tests/rsync.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      560 2021-09-16 23:21:23.000000 chibi_command-0.4.1/tests/sysctl.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1976 2019-10-31 18:00:07.000000 chibi_command-0.4.1/tests/xfce4.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.462855 chibi_command-0.4.2/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-02-22 02:37:10.000000 chibi_command-0.4.2/AUTHORS.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3598 2020-02-22 02:37:10.000000 chibi_command-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       89 2020-02-22 02:37:10.000000 chibi_command-0.4.2/HISTORY.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2020-02-22 02:37:10.000000 chibi_command-0.4.2/LICENSE
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2020-02-22 02:37:10.000000 chibi_command-0.4.2/MANIFEST.in
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1525 2023-04-14 17:44:27.462855 chibi_command-0.4.2/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      889 2020-02-22 02:37:10.000000 chibi_command-0.4.2/README.rst
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.422855 chibi_command-0.4.2/chibi_command/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5502 2023-04-14 17:44:23.000000 chibi_command-0.4.2/chibi_command/__init__.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.422855 chibi_command-0.4.2/chibi_command/centos/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      145 2021-09-17 00:55:39.000000 chibi_command-0.4.2/chibi_command/centos/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1528 2022-01-24 03:51:53.000000 chibi_command-0.4.2/chibi_command/centos/dnf.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3788 2021-10-28 23:36:56.000000 chibi_command-0.4.2/chibi_command/centos/iptable.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2132 2021-09-17 00:55:32.000000 chibi_command-0.4.2/chibi_command/centos/yum.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      398 2019-09-09 16:26:47.000000 chibi_command-0.4.2/chibi_command/db.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      186 2019-10-02 15:07:59.000000 chibi_command-0.4.2/chibi_command/dd.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.422855 chibi_command-0.4.2/chibi_command/disk/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-24 07:17:23.000000 chibi_command-0.4.2/chibi_command/disk/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1057 2020-02-22 02:34:14.000000 chibi_command-0.4.2/chibi_command/disk/dd.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      176 2020-04-05 20:30:23.000000 chibi_command-0.4.2/chibi_command/disk/format.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      223 2020-04-05 21:53:54.000000 chibi_command-0.4.2/chibi_command/disk/mount.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      451 2020-03-02 15:15:53.000000 chibi_command-0.4.2/chibi_command/echo.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      124 2019-08-16 20:41:47.000000 chibi_command-0.4.2/chibi_command/ffmpeg.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1193 2023-04-14 17:43:11.000000 chibi_command-0.4.2/chibi_command/file.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3011 2021-12-09 01:34:46.000000 chibi_command-0.4.2/chibi_command/git.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.422855 chibi_command-0.4.2/chibi_command/image/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-09-03 15:04:53.000000 chibi_command-0.4.2/chibi_command/image/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      973 2019-09-03 15:15:41.000000 chibi_command-0.4.2/chibi_command/image/convert.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1427 2020-03-10 23:37:01.000000 chibi_command-0.4.2/chibi_command/image/qr.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.422855 chibi_command-0.4.2/chibi_command/lxc/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       63 2022-01-14 21:07:02.000000 chibi_command-0.4.2/chibi_command/lxc/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      569 2022-01-14 22:56:18.000000 chibi_command-0.4.2/chibi_command/lxc/delegate.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2753 2022-01-14 22:47:34.000000 chibi_command-0.4.2/chibi_command/lxc/lxc.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      509 2019-12-24 15:20:08.000000 chibi_command-0.4.2/chibi_command/mpd.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.426189 chibi_command-0.4.2/chibi_command/network/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       57 2020-03-02 15:17:31.000000 chibi_command-0.4.2/chibi_command/network/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      702 2021-06-22 05:36:13.000000 chibi_command-0.4.2/chibi_command/network/ifconfig.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2850 2021-06-22 20:27:11.000000 chibi_command-0.4.2/chibi_command/network/interfaces.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      742 2021-06-22 19:27:10.000000 chibi_command-0.4.2/chibi_command/network/iwconfig.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      460 2020-10-21 09:00:09.000000 chibi_command-0.4.2/chibi_command/network/nmap.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1918 2020-01-08 04:55:57.000000 chibi_command-0.4.2/chibi_command/network/nmcli.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.426189 chibi_command-0.4.2/chibi_command/nix/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      132 2021-03-29 04:54:05.000000 chibi_command-0.4.2/chibi_command/nix/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      393 2021-03-29 04:56:19.000000 chibi_command-0.4.2/chibi_command/nix/locale.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2309 2022-01-23 23:53:11.000000 chibi_command-0.4.2/chibi_command/nix/systemd.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1139 2022-01-24 00:00:33.000000 chibi_command-0.4.2/chibi_command/nix/systemd_run.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      943 2020-03-05 03:47:09.000000 chibi_command-0.4.2/chibi_command/nix/user.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      763 2021-03-29 04:59:39.000000 chibi_command-0.4.2/chibi_command/qr.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      796 2019-12-24 15:25:42.000000 chibi_command-0.4.2/chibi_command/rabbitmq.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      240 2019-12-24 15:28:53.000000 chibi_command-0.4.2/chibi_command/rpm.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2074 2021-09-16 23:22:52.000000 chibi_command-0.4.2/chibi_command/rsync.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      405 2021-09-16 23:19:35.000000 chibi_command-0.4.2/chibi_command/sysctl.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4938 2022-03-24 21:23:12.000000 chibi_command-0.4.2/chibi_command/wmctrl.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      758 2020-03-02 15:17:03.000000 chibi_command-0.4.2/chibi_command/xfce4.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.422855 chibi_command-0.4.2/chibi_command.egg-info/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1525 2023-04-14 17:44:26.000000 chibi_command-0.4.2/chibi_command.egg-info/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2110 2023-04-14 17:44:26.000000 chibi_command-0.4.2/chibi_command.egg-info/SOURCES.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-04-14 17:44:26.000000 chibi_command-0.4.2/chibi_command.egg-info/dependency_links.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-04-14 17:44:26.000000 chibi_command-0.4.2/chibi_command.egg-info/not-zip-safe
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       43 2023-04-14 17:44:26.000000 chibi_command-0.4.2/chibi_command.egg-info/requires.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       14 2023-04-14 17:44:26.000000 chibi_command-0.4.2/chibi_command.egg-info/top_level.txt
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.439522 chibi_command-0.4.2/docs/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      614 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/Makefile
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/authors.rst
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4872 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/conf.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/contributing.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/history.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      310 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/index.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1158 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/installation.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      775 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/make.bat
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/readme.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       81 2020-02-22 02:37:10.000000 chibi_command-0.4.2/docs/usage.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      451 2023-04-14 17:44:27.462855 chibi_command-0.4.2/setup.cfg
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1095 2023-04-14 17:44:23.000000 chibi_command-0.4.2/setup.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.459521 chibi_command-0.4.2/tests/
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2018-06-27 08:43:08.000000 chibi_command-0.4.2/tests/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2639 2021-10-28 23:37:46.000000 chibi_command-0.4.2/tests/centos.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3014 2022-01-23 23:33:44.000000 chibi_command-0.4.2/tests/command.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      888 2022-01-23 21:58:14.000000 chibi_command-0.4.2/tests/command_result.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.459521 chibi_command-0.4.2/tests/disk/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-02-09 22:05:59.000000 chibi_command-0.4.2/tests/disk/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      854 2020-03-05 03:19:52.000000 chibi_command-0.4.2/tests/disk/dd.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.459521 chibi_command-0.4.2/tests/echo/
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2018-06-27 08:43:08.000000 chibi_command-0.4.2/tests/echo/__init__.py
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1489 2019-09-09 15:53:10.000000 chibi_command-0.4.2/tests/echo/test_echo.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      376 2023-04-14 17:39:52.000000 chibi_command-0.4.2/tests/file.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2080 2021-12-09 17:56:18.000000 chibi_command-0.4.2/tests/git.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.459521 chibi_command-0.4.2/tests/image/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-09-03 15:17:47.000000 chibi_command-0.4.2/tests/image/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       73 2019-09-03 16:47:29.000000 chibi_command-0.4.2/tests/image/convert.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5052 2022-01-23 22:26:47.000000 chibi_command-0.4.2/tests/lxc.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.459521 chibi_command-0.4.2/tests/network/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-24 15:36:50.000000 chibi_command-0.4.2/tests/network/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      441 2021-06-22 05:36:27.000000 chibi_command-0.4.2/tests/network/ifconfig.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2314 2021-06-22 20:26:55.000000 chibi_command-0.4.2/tests/network/interface.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      483 2021-06-22 19:27:41.000000 chibi_command-0.4.2/tests/network/iwconfig.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1305 2020-01-08 04:56:58.000000 chibi_command-0.4.2/tests/network/nmcli.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 17:44:27.462855 chibi_command-0.4.2/tests/nix/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-05 03:38:01.000000 chibi_command-0.4.2/tests/nix/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      296 2021-03-29 04:56:15.000000 chibi_command-0.4.2/tests/nix/locale.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1626 2022-01-23 23:31:52.000000 chibi_command-0.4.2/tests/nix/systemd.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      805 2022-01-14 23:15:07.000000 chibi_command-0.4.2/tests/nix/systemd_run.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      538 2020-03-05 03:42:36.000000 chibi_command-0.4.2/tests/nix/user.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      948 2020-04-07 22:27:40.000000 chibi_command-0.4.2/tests/rsync.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      560 2021-09-16 23:21:23.000000 chibi_command-0.4.2/tests/sysctl.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2805 2022-03-24 21:23:46.000000 chibi_command-0.4.2/tests/wmctrl.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1976 2019-10-31 18:00:07.000000 chibi_command-0.4.2/tests/xfce4.py
```

### Comparing `chibi_command-0.4.1/CONTRIBUTING.rst` & `chibi_command-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/PKG-INFO` & `chibi_command-0.4.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,65 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: chibi_command
-Version: 0.4.1
+Version: 0.4.2
 Summary: run terminal commands
 Home-page: https://github.com/dem4ply/chibi_command
 Author: Dem4ply
 Author-email: dem4ply@gmail.com
 License: WTFPL
-Description: =============
-        chibi_command
-        =============
-        
-        
-        .. image:: https://img.shields.io/pypi/v/chibi_command.svg
-                :target: https://pypi.python.org/pypi/chibi_command
-        
-        .. image:: https://img.shields.io/travis/dem4ply/chibi_command.svg
-                :target: https://travis-ci.org/dem4ply/chibi_command
-        
-        .. image:: https://readthedocs.org/projects/chibi-command/badge/?version=latest
-                :target: https://chibi-command.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        run terminal commands
-        
-        
-        * Free software: WTFPL
-        * Documentation: https://chibi-command.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.0.1 (2020-02-19)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: chibi_command
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=============
+chibi_command
+=============
+
+
+.. image:: https://img.shields.io/pypi/v/chibi_command.svg
+        :target: https://pypi.python.org/pypi/chibi_command
+
+.. image:: https://img.shields.io/travis/dem4ply/chibi_command.svg
+        :target: https://travis-ci.org/dem4ply/chibi_command
+
+.. image:: https://readthedocs.org/projects/chibi-command/badge/?version=latest
+        :target: https://chibi-command.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+
+
+run terminal commands
+
+
+* Free software: WTFPL
+* Documentation: https://chibi-command.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.0.1 (2020-02-19)
+------------------
+
+* First release on PyPI.
```

### Comparing `chibi_command-0.4.1/README.rst` & `chibi_command-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/__init__.py` & `chibi_command-0.4.2/chibi_command/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from subprocess import Popen, PIPE
 import json
 import itertools
 import logging
 
 __author__ = """dem4ply"""
 __email__ = 'dem4ply@gmail.com'
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 
 logger = logging.getLogger( 'chibi.command' )
 
 
 class Command_result:
     def __init__( self, result, error, return_code ):
         self.result = result
```

### Comparing `chibi_command-0.4.1/chibi_command/centos/dnf.py` & `chibi_command-0.4.2/chibi_command/centos/dnf.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/centos/iptable.py` & `chibi_command-0.4.2/chibi_command/centos/iptable.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/centos/yum.py` & `chibi_command-0.4.2/chibi_command/centos/yum.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/disk/dd.py` & `chibi_command-0.4.2/chibi_command/disk/dd.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/git.py` & `chibi_command-0.4.2/chibi_command/git.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/image/convert.py` & `chibi_command-0.4.2/chibi_command/image/convert.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/image/qr.py` & `chibi_command-0.4.2/chibi_command/image/qr.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/lxc/delegate.py` & `chibi_command-0.4.2/chibi_command/lxc/delegate.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/lxc/lxc.py` & `chibi_command-0.4.2/chibi_command/lxc/lxc.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/network/ifconfig.py` & `chibi_command-0.4.2/chibi_command/network/ifconfig.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/network/interfaces.py` & `chibi_command-0.4.2/chibi_command/network/interfaces.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/network/iwconfig.py` & `chibi_command-0.4.2/chibi_command/network/iwconfig.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/network/nmcli.py` & `chibi_command-0.4.2/chibi_command/network/nmcli.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/nix/systemd.py` & `chibi_command-0.4.2/chibi_command/nix/systemd.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/nix/systemd_run.py` & `chibi_command-0.4.2/chibi_command/nix/systemd_run.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/nix/user.py` & `chibi_command-0.4.2/chibi_command/nix/user.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/qr.py` & `chibi_command-0.4.2/chibi_command/qr.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/rabbitmq.py` & `chibi_command-0.4.2/chibi_command/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/rsync.py` & `chibi_command-0.4.2/chibi_command/rsync.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command/xfce4.py` & `chibi_command-0.4.2/chibi_command/xfce4.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/chibi_command.egg-info/SOURCES.txt` & `chibi_command-0.4.2/chibi_command.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 chibi_command/git.py
 chibi_command/mpd.py
 chibi_command/qr.py
 chibi_command/rabbitmq.py
 chibi_command/rpm.py
 chibi_command/rsync.py
 chibi_command/sysctl.py
+chibi_command/wmctrl.py
 chibi_command/xfce4.py
 chibi_command.egg-info/PKG-INFO
 chibi_command.egg-info/SOURCES.txt
 chibi_command.egg-info/dependency_links.txt
 chibi_command.egg-info/not-zip-safe
 chibi_command.egg-info/requires.txt
 chibi_command.egg-info/top_level.txt
@@ -61,18 +62,20 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
 tests/centos.py
 tests/command.py
 tests/command_result.py
+tests/file.py
 tests/git.py
 tests/lxc.py
 tests/rsync.py
 tests/sysctl.py
+tests/wmctrl.py
 tests/xfce4.py
 tests/disk/__init__.py
 tests/disk/dd.py
 tests/echo/__init__.py
 tests/echo/test_echo.py
 tests/image/__init__.py
 tests/image/convert.py
```

### Comparing `chibi_command-0.4.1/docs/Makefile` & `chibi_command-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/docs/conf.py` & `chibi_command-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/docs/installation.rst` & `chibi_command-0.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/docs/make.bat` & `chibi_command-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/setup.py` & `chibi_command-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,10 +29,10 @@
     license="WTFPL",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='chibi_command',
     name='chibi_command',
     packages=find_packages(include=['chibi_command', 'chibi_command.*']),
     url='https://github.com/dem4ply/chibi_command',
-    version='0.4.1',
+    version='0.4.2',
     zip_safe=False,
 )
```

### Comparing `chibi_command-0.4.1/tests/centos.py` & `chibi_command-0.4.2/tests/centos.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/command.py` & `chibi_command-0.4.2/tests/command.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/command_result.py` & `chibi_command-0.4.2/tests/command_result.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/disk/dd.py` & `chibi_command-0.4.2/tests/disk/dd.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/echo/test_echo.py` & `chibi_command-0.4.2/tests/echo/test_echo.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/git.py` & `chibi_command-0.4.2/tests/git.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/lxc.py` & `chibi_command-0.4.2/tests/lxc.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/network/interface.py` & `chibi_command-0.4.2/tests/network/interface.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/network/nmcli.py` & `chibi_command-0.4.2/tests/network/nmcli.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/nix/systemd.py` & `chibi_command-0.4.2/tests/nix/systemd.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/nix/systemd_run.py` & `chibi_command-0.4.2/tests/nix/systemd_run.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/nix/user.py` & `chibi_command-0.4.2/tests/nix/user.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/rsync.py` & `chibi_command-0.4.2/tests/rsync.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/sysctl.py` & `chibi_command-0.4.2/tests/sysctl.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.1/tests/xfce4.py` & `chibi_command-0.4.2/tests/xfce4.py`

 * *Files identical despite different names*

