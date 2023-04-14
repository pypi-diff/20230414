# Comparing `tmp/vicedtools-0.0.7.1.tar.gz` & `tmp/vicedtools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicedtools-0.0.7.1.tar", last modified: Mon Jun 13 14:55:37 2022, max compression
+gzip compressed data, was "vicedtools-0.0.8.tar", last modified: Fri Apr 14 07:48:37 2023, max compression
```

## Comparing `vicedtools-0.0.7.1.tar` & `vicedtools-0.0.8.tar`

### file list

```diff
@@ -1,92 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.715779 vicedtools-0.0.7.1/
--rw-rw-rw-   0        0        0    11558 2021-05-29 17:10:03.000000 vicedtools-0.0.7.1/LICENSE
--rw-rw-rw-   0        0        0     1374 2022-06-13 14:55:37.715779 vicedtools-0.0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      800 2022-04-20 01:27:08.000000 vicedtools-0.0.7.1/README.md
--rw-rw-rw-   0        0        0      108 2021-05-29 17:13:52.000000 vicedtools-0.0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0      854 2022-06-13 14:55:37.722763 vicedtools-0.0.7.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-05-29 17:22:45.000000 vicedtools-0.0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.554111 vicedtools-0.0.7.1/src/
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.568635 vicedtools-0.0.7.1/src/vicedtools/
--rw-rw-rw-   0        0        0       67 2022-06-13 14:12:00.000000 vicedtools-0.0.7.1/src/vicedtools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.614059 vicedtools-0.0.7.1/src/vicedtools/acer/
--rw-rw-rw-   0        0        0      733 2022-06-13 14:12:01.000000 vicedtools-0.0.7.1/src/vicedtools/acer/__init__.py
--rw-rw-rw-   0        0        0     4191 2022-06-13 14:12:00.000000 vicedtools-0.0.7.1/src/vicedtools/acer/ewritesittings.py
--rw-rw-rw-   0        0        0     7222 2022-06-13 14:12:00.000000 vicedtools-0.0.7.1/src/vicedtools/acer/oars.py
--rw-rw-rw-   0        0        0     4902 2022-06-13 14:12:00.000000 vicedtools-0.0.7.1/src/vicedtools/acer/oarscandidates.py
--rw-rw-rw-   0        0        0    17208 2022-06-13 14:12:00.000000 vicedtools-0.0.7.1/src/vicedtools/acer/oarssession.py
--rw-rw-rw-   0        0        0     5368 2022-06-13 14:12:00.000000 vicedtools-0.0.7.1/src/vicedtools/acer/oarstests.py
--rw-rw-rw-   0        0        0     1878 2022-06-13 14:12:00.000000 vicedtools-0.0.7.1/src/vicedtools/acer/patitems.py
--rw-rw-rw-   0        0        0    15527 2022-06-13 14:12:01.000000 vicedtools-0.0.7.1/src/vicedtools/acer/patresults.py
--rw-rw-rw-   0        0        0     6800 2022-06-13 14:12:01.000000 vicedtools-0.0.7.1/src/vicedtools/acer/patsittings.py
--rw-rw-rw-   0        0        0    11115 2022-06-13 14:12:01.000000 vicedtools-0.0.7.1/src/vicedtools/acer/plots.py
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.623018 vicedtools-0.0.7.1/src/vicedtools/compass/
--rw-rw-rw-   0        0        0      962 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/compass/__init__.py
--rw-rw-rw-   0        0        0    21133 2022-06-13 14:12:01.000000 vicedtools-0.0.7.1/src/vicedtools/compass/compasssession.py
--rw-rw-rw-   0        0        0    28307 2022-06-13 14:32:24.000000 vicedtools-0.0.7.1/src/vicedtools/compass/compasswebdriver.py
--rw-rw-rw-   0        0        0    15871 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/compass/exports.py
--rw-rw-rw-   0        0        0    18343 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/compass/reports.py
--rw-rw-rw-   0        0        0     3645 2022-06-13 14:12:00.000000 vicedtools-0.0.7.1/src/vicedtools/educationperfect.py
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.628006 vicedtools-0.0.7.1/src/vicedtools/gcp/
--rw-rw-rw-   0        0        0     1338 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/gcp/__init__.py
--rw-rw-rw-   0        0        0     2725 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/gcp/api.py
--rw-rw-rw-   0        0        0     2042 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/gcp/format.py
--rw-rw-rw-   0        0        0     6576 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/gcp/schema.py
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.633990 vicedtools-0.0.7.1/src/vicedtools/naplan/
--rw-rw-rw-   0        0        0      815 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/naplan/__init__.py
--rw-rw-rw-   0        0        0     5816 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/naplan/dataservicesession.py
--rw-rw-rw-   0        0        0     6190 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/naplan/sssrdata.py
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.639974 vicedtools-0.0.7.1/src/vicedtools/vce/
--rw-rw-rw-   0        0        0      702 2022-06-13 14:12:03.000000 vicedtools-0.0.7.1/src/vicedtools/vce/__init__.py
--rw-rw-rw-   0        0        0     3020 2022-06-13 14:12:02.000000 vicedtools-0.0.7.1/src/vicedtools/vce/schoolscores.py
--rw-rw-rw-   0        0        0    33784 2022-06-13 14:26:01.000000 vicedtools-0.0.7.1/src/vicedtools/vce/vasssession.py
--rw-rw-rw-   0        0        0    32221 2022-06-13 14:12:03.000000 vicedtools-0.0.7.1/src/vicedtools/vce/vasswebdriver.py
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.713776 vicedtools-0.0.7.1/src/vicedtools/workflows/
--rw-rw-rw-   0        0        0      553 2022-06-13 14:44:57.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/__init__.py
--rw-rw-rw-   0        0        0     1383 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/compassreportstobq.py
--rw-rw-rw-   0        0        0     3656 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/compassstudentdetailstobq.py
--rw-rw-rw-   0        0        0     2755 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/compassstudentenrolmenttobq.py
--rw-rw-rw-   0        0        0     8372 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/config sample.py
--rw-rw-rw-   0        0        0     8054 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/config.py
--rw-rw-rw-   0        0        0     2709 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/createcompassreportssummaries.py
--rw-rw-rw-   0        0        0     4372 2022-06-13 14:52:19.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/createpatparentlettertable.py
--rw-rw-rw-   0        0        0     1527 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/ewritescorestobq.py
--rw-rw-rw-   0        0        0     4708 2022-06-13 14:53:41.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/ewritesittingstoscores.py
--rw-rw-rw-   0        0        0     1278 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassacademicgroups.py
--rw-rw-rw-   0        0        0     2287 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassclasses.py
--rw-rw-rw-   0        0        0     2226 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompasslearningtask.py
--rw-rw-rw-   0        0        0     2316 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompasslearningtasks.py
--rw-rw-rw-   0        0        0     1718 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassprogressreport.py
--rw-rw-rw-   0        0        0     1313 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassprogressreportcycles.py
--rw-rw-rw-   0        0        0     2486 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassprogressreports.py
--rw-rw-rw-   0        0        0     1609 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassreport.py
--rw-rw-rw-   0        0        0     1878 2022-06-13 14:53:38.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassreportcycles.py
--rw-rw-rw-   0        0        0     2204 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassreports.py
--rw-rw-rw-   0        0        0     2068 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompasssds.py
--rw-rw-rw-   0        0        0     1190 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassstudenthouseholdinformation.py
--rw-rw-rw-   0        0        0     1132 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassstudents.py
--rw-rw-rw-   0        0        0     2163 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompasssubjectmetadata.py
--rw-rw-rw-   0        0        0     1428 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportnaplanoutcomes.py
--rw-rw-rw-   0        0        0     1410 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportnaplansssr.py
--rw-rw-rw-   0        0        0     1406 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportoarsmetadata.py
--rw-rw-rw-   0        0        0     2901 2022-06-13 14:53:58.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportoarssittings.py
--rw-rw-rw-   0        0        0     1061 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportoarsstaff.py
--rw-rw-rw-   0        0        0     1178 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportoarsstudents.py
--rw-rw-rw-   0        0        0     1680 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportvassexternalscores.py
--rw-rw-rw-   0        0        0     1605 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportvassgatscores.py
--rw-rw-rw-   0        0        0     2029 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportvassmoderatedscores.py
--rw-rw-rw-   0        0        0     1685 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportvasspredictedscores.py
--rw-rw-rw-   0        0        0     1685 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportvassschoolprogram.py
--rw-rw-rw-   0        0        0     1912 2022-06-13 14:44:56.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportvassschoolscores.py
--rw-rw-rw-   0        0        0     1684 2022-06-13 14:44:59.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/exportvassstudentdetails.py
--rw-rw-rw-   0        0        0     8985 2022-06-13 14:44:57.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/gwsc-config.py
--rw-rw-rw-   0        0        0     2915 2022-06-13 14:44:57.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/naplanoutcomestobq.py
--rw-rw-rw-   0        0        0     2293 2022-06-13 14:44:57.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/patmostrecentobq.py
--rw-rw-rw-   0        0        0     1928 2022-06-13 14:44:57.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/patscorestobq.py
--rw-rw-rw-   0        0        0     1737 2022-06-13 14:44:57.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/patscorestomostrecent.py
--rw-rw-rw-   0        0        0     1807 2022-06-13 14:44:57.000000 vicedtools-0.0.7.1/src/vicedtools/workflows/patsittingstoscores.py
-drwxrwxrwx   0        0        0        0 2022-06-13 14:55:37.597088 vicedtools-0.0.7.1/src/vicedtools.egg-info/
--rw-rw-rw-   0        0        0     1374 2022-06-13 14:55:36.000000 vicedtools-0.0.7.1/src/vicedtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3343 2022-06-13 14:55:37.000000 vicedtools-0.0.7.1/src/vicedtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-13 14:55:37.000000 vicedtools-0.0.7.1/src/vicedtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2022-06-13 14:55:37.000000 vicedtools-0.0.7.1/src/vicedtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-06-13 14:55:37.000000 vicedtools-0.0.7.1/src/vicedtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.799431 vicedtools-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2021-05-29 17:10:03.000000 vicedtools-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5210 2023-04-14 07:48:37.799431 vicedtools-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4636 2023-04-14 07:45:30.000000 vicedtools-0.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2021-05-29 17:13:52.000000 vicedtools-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      860 2023-04-14 07:48:37.831735 vicedtools-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     3857 2023-04-14 06:14:58.000000 vicedtools-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.231913 vicedtools-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.334756 vicedtools-0.0.8/src/vicedtools/
+-rw-rw-rw-   0        0        0     1498 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.550889 vicedtools-0.0.8/src/vicedtools/acer/
+-rw-rw-rw-   0        0        0     1341 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/acer/__init__.py
+-rw-rw-rw-   0        0        0     4191 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/ewritesittings.py
+-rw-rw-rw-   0        0        0     1188 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/extraoarsauthenticators.py
+-rw-rw-rw-   0        0        0     7223 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oars.py
+-rw-rw-rw-   0        0        0     2269 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oarsauthenticators.py
+-rw-rw-rw-   0        0        0     4902 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oarscandidates.py
+-rw-rw-rw-   0        0        0    16115 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oarssession.py
+-rw-rw-rw-   0        0        0     5368 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oarstests.py
+-rw-rw-rw-   0        0        0     1878 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/patitems.py
+-rw-rw-rw-   0        0        0    15529 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/patresults.py
+-rw-rw-rw-   0        0        0     6964 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/patsittings.py
+-rw-rw-rw-   0        0        0    21888 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/acer/plots.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.618889 vicedtools-0.0.8/src/vicedtools/compass/
+-rw-rw-rw-   0        0        0      982 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/compassauthenticators.py
+-rw-rw-rw-   0        0        0    19553 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/compasssession.py
+-rw-rw-rw-   0        0        0     1113 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/extraauthenticators.py
+-rw-rw-rw-   0        0        0    18015 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/reports.py
+-rw-rw-rw-   0        0        0     3645 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/educationperfect.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.683796 vicedtools-0.0.8/src/vicedtools/gcp/
+-rw-rw-rw-   0        0        0     1338 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/gcp/__init__.py
+-rw-rw-rw-   0        0        0     2725 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/gcp/api.py
+-rw-rw-rw-   0        0        0     2042 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/gcp/format.py
+-rw-rw-rw-   0        0        0     6566 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/gcp/schema.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.733900 vicedtools-0.0.8/src/vicedtools/naplan/
+-rw-rw-rw-   0        0        0      815 2023-04-13 17:39:12.000000 vicedtools-0.0.8/src/vicedtools/naplan/__init__.py
+-rw-rw-rw-   0        0        0     5815 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/naplan/dataservicesession.py
+-rw-rw-rw-   0        0        0     6193 2023-04-14 07:39:34.000000 vicedtools-0.0.8/src/vicedtools/naplan/sssrdata.py
+-rw-rw-rw-   0        0        0     2004 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/sportstrak.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.797145 vicedtools-0.0.8/src/vicedtools/vce/
+-rw-rw-rw-   0        0        0      798 2023-04-13 17:39:14.000000 vicedtools-0.0.8/src/vicedtools/vce/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-04-13 17:39:13.000000 vicedtools-0.0.8/src/vicedtools/vce/schoolscores.py
+-rw-rw-rw-   0        0        0    34328 2023-04-13 17:39:13.000000 vicedtools-0.0.8/src/vicedtools/vce/vasssession.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.425447 vicedtools-0.0.8/src/vicedtools.egg-info/
+-rw-rw-rw-   0        0        0     5210 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1326 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3162 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/top_level.txt
```

### Comparing `vicedtools-0.0.7.1/LICENSE` & `vicedtools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/setup.cfg` & `vicedtools-0.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6963 6564 746f 6f6c 730d 0a76   = vicedtools..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e37 2e31  ersion = 0.0.7.1
-00000030: 0d0a 6175 7468 6f72 203d 2047 7265 6720  ..author = Greg 
-00000040: 4272 6565 7365 0d0a 6465 7363 7269 7074  Breese..descript
-00000050: 696f 6e20 3d20 4120 636f 6c6c 6563 7469  ion = A collecti
-00000060: 6f6e 206f 6620 746f 6f6c 7320 666f 7220  on of tools for 
-00000070: 7363 686f 6f6c 2064 6174 6120 696e 2056  school data in V
-00000080: 6963 746f 7269 616e 2073 6368 6f6f 6c73  ictorian schools
-00000090: 2e0d 0a6c 6f6e 675f 6465 7363 7269 7074  ...long_descript
-000000a0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000b0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-000000c0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-000000d0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
-000000e0: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
-000000f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
-00000100: 7265 6762 7265 6573 652f 7669 6365 6474  regbreese/vicedt
-00000110: 6f6f 6c73 0d0a 7072 6f6a 6563 745f 7572  ools..project_ur
-00000120: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
-00000130: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
-00000140: 7468 7562 2e63 6f6d 2f67 7265 6762 7265  thub.com/gregbre
-00000150: 6573 652f 7669 6365 6474 6f6f 6c73 2f69  ese/vicedtools/i
-00000160: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
-00000170: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
-00000180: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000190: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
-000001a0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001b0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
-000001c0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
-000001d0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-000001e0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000001f0: 6e64 656e 740d 0a09 4465 7665 6c6f 706d  ndent...Developm
-00000200: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
-00000210: 2d20 416c 7068 610d 0a0d 0a5b 6f70 7469  - Alpha....[opti
-00000220: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-00000230: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
-00000240: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000250: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000260: 3d20 3e3d 332e 380d 0a69 6e73 7461 6c6c  = >=3.8..install
-00000270: 5f72 6571 7569 7265 7320 3d20 0d0a 0962  _requires = ...b
-00000280: 726f 7773 6572 5f63 6f6f 6b69 6533 0d0a  rowser_cookie3..
-00000290: 0962 7334 0d0a 0964 656d 6a73 6f6e 0d0a  .bs4...demjson..
-000002a0: 0967 6f6f 676c 652d 636c 6f75 642d 6269  .google-cloud-bi
-000002b0: 6771 7565 7279 0d0a 0967 6f6f 676c 652d  gquery...google-
-000002c0: 636c 6f75 642d 7374 6f72 6167 650d 0a09  cloud-storage...
-000002d0: 6d61 7470 6c6f 746c 6962 0d0a 096e 756d  matplotlib...num
-000002e0: 7079 0d0a 0970 616e 6461 730d 0a09 7365  py...pandas...se
-000002f0: 6162 6f72 6e0d 0a09 7365 6c65 6e69 756d  aborn...selenium
-00000300: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000310: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000320: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
-00000330: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000340: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000350: 2030 0d0a 0d0a                            0....
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e38 0d0a  ersion = 0.0.8..
+00000030: 6175 7468 6f72 203d 2047 7265 6720 4272  author = Greg Br
+00000040: 6565 7365 0d0a 6465 7363 7269 7074 696f  eese..descriptio
+00000050: 6e20 3d20 4120 636f 6c6c 6563 7469 6f6e  n = A collection
+00000060: 206f 6620 746f 6f6c 7320 666f 7220 7363   of tools for sc
+00000070: 686f 6f6c 2064 6174 6120 696e 2056 6963  hool data in Vic
+00000080: 746f 7269 616e 2073 6368 6f6f 6c73 2e0d  torian schools..
+00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000a0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000b0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+000000c0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000000d0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+000000e0: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
+000000f0: 2f2f 6769 7468 7562 2e63 6f6d 2f67 7265  //github.com/gre
+00000100: 6762 7265 6573 652f 7669 6365 6474 6f6f  gbreese/vicedtoo
+00000110: 6c73 0d0a 7072 6f6a 6563 745f 7572 6c73  ls..project_urls
+00000120: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
+00000130: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+00000140: 7562 2e63 6f6d 2f67 7265 6762 7265 6573  ub.com/gregbrees
+00000150: 652f 7669 6365 6474 6f6f 6c73 2f69 7373  e/vicedtools/iss
+00000160: 7565 730d 0a63 6c61 7373 6966 6965 7273  ues..classifiers
+00000170: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+00000180: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000190: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
+000001a0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000001b0: 7665 6420 3a3a 2041 7061 6368 6520 536f  ved :: Apache So
+000001c0: 6674 7761 7265 204c 6963 656e 7365 0d0a  ftware License..
+000001d0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000001e0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000001f0: 656e 740d 0a09 4465 7665 6c6f 706d 656e  ent...Developmen
+00000200: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
+00000210: 416c 7068 610d 0a0d 0a5b 6f70 7469 6f6e  Alpha....[option
+00000220: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000230: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000240: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000250: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000260: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
+00000270: 6571 7569 7265 7320 3d20 0d0a 0962 726f  equires = ...bro
+00000280: 7773 6572 5f63 6f6f 6b69 6533 0d0a 0962  wser_cookie3...b
+00000290: 7334 0d0a 0964 656d 6a73 6f6e 0d0a 0967  s4...demjson...g
+000002a0: 6f6f 676c 652d 636c 6f75 642d 6269 6771  oogle-cloud-bigq
+000002b0: 7565 7279 0d0a 0967 6f6f 676c 652d 636c  uery...google-cl
+000002c0: 6f75 642d 7374 6f72 6167 650d 0a09 6d61  oud-storage...ma
+000002d0: 7470 6c6f 746c 6962 0d0a 096e 756d 7079  tplotlib...numpy
+000002e0: 0d0a 0970 616e 6461 730d 0a09 7365 6162  ...pandas...seab
+000002f0: 6f72 6e0d 0a09 7365 6c65 6e69 756d 0d0a  orn...selenium..
+00000300: 0974 6f6d 6c69 0d0a 0d0a 5b6f 7074 696f  .tomli....[optio
+00000310: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000320: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+00000330: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000340: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000350: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/__init__.py` & `vicedtools-0.0.8/src/vicedtools/acer/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,24 @@
+# Copyright 2023 VicEdTools authors
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from vicedtools.acer.ewritesittings import EWriteSittings
 from vicedtools.acer.oars import student_imports
-from vicedtools.acer.oarssession import OARSSession, OARSAuthenticator, OARSAuthenticateError, OARSConfigAuthenticator, OARSFirefoxCookieAuthenticator
+from vicedtools.acer.oarsauthenticators import OARSAuthenticator, OARSAuthenticateError, OARSBasicAuthenticator
+from vicedtools.acer.oarssession import OARSSession
 from vicedtools.acer.oarscandidates import OARSCandidate, OARSCandidates
 from vicedtools.acer.patitems import PATItem, PATItems
 from vicedtools.acer.patsittings import PATSitting, PATSittings
 from vicedtools.acer.patresults import is_group_report_file, score_categoriser, PATResults, PATResultsCollection, group_reports_to_patresults
 from vicedtools.acer.oarstests import OARSTest, OARSTests
 from vicedtools.acer.plots import item_analysis_plot, item_analysis_plots
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/ewritesittings.py` & `vicedtools-0.0.8/src/vicedtools/acer/ewritesittings.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/oars.py` & `vicedtools-0.0.8/src/vicedtools/acer/oars.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         "Year level", "Form Group"
     ]
     student_details_df = student_details_df[columns]
     # create other columns
     student_details_df["Middle names"] = ""
     student_details_df["Password"] = student_details_df["Date of birth"]
     student_details_df["Unique ID"] = student_details_df["Username"]
-    student_details_df["School year"] = datetime.today().stftime('%Y')
+    student_details_df["School year"] = datetime.today().strftime('%Y')
     student_details_df["Enrolled"] = "Enrolled"
 
     student_enrolment_df[[
         "Subject", "Class code"
     ]] = student_enrolment_df["Section SIS ID"].apply(class_selector)
     student_enrolment_df.dropna(subset=["Subject"], inplace=True)
     # remove multiple enrolments (keep most recent)
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/oarscandidates.py` & `vicedtools-0.0.8/src/vicedtools/acer/oarscandidates.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/oarssession.py` & `vicedtools-0.0.8/src/vicedtools/acer/oarssession.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A requests.requests.Session class for accessing the OARS API."""
 
 from __future__ import annotations
 
-from abc import abstractmethod
 from datetime import datetime
 from html.parser import HTMLParser
 import json
 import re
 import requests
 import time
-from typing import Protocol
 from urllib.parse import quote
 
 import pandas as pd
 
-import browser_cookie3
-
 from vicedtools.acer.ewritesittings import EWriteSittings
+from vicedtools.acer.oarsauthenticators import OARSAuthenticator, OARSBasicAuthenticator, OARSAuthenticateError
 from vicedtools.acer.oarscandidates import OARSCandidates
+from vicedtools.acer.oarstests import OARSTests
 from vicedtools.acer.patitems import PATItems
 from vicedtools.acer.patsittings import PATSittings
-from vicedtools.acer.oarstests import OARSTests
 
 
 class OARSSession(requests.sessions.Session):
     """A requests Session extension with methods for accessing data from OARS."""
 
     def __init__(self, school: str, authenticator: OARSAuthenticator):
         """Creates a requests Session with OARS authentication completed.
@@ -54,15 +51,15 @@
         self.headers.update(headers)
 
         self.school = school
         authenticator.authenticate(self)
         r = self.get(f"https://oars.acer.edu.au/{school}/reports-new")
         pattern = r'"securityToken":"(?P<token>[\$0-9A-Za-z+/\.\\]*)"'
         m = re.search(pattern, r.text)
-        self.security_token = m.group('token')
+        self.security_token = m.group('token').replace('\\/', '/')
 
         self._get_test_metadata()
         self._get_scale_constructs()
 
     def _get_test_metadata(self):
         """Downloads test metadata from OARS."""
         url = f"https://oars.acer.edu.au/api/{self.school}/reports-new/getTests/"
@@ -121,26 +118,27 @@
             }
             r = self.post(sittings_url, json=payload)
             sittings += r.json()
         return PATSittings(sittings)
 
     def get_all_pat_sittings(self, from_date: str, to_date: str) -> PATSittings:
         """Downloads the results for all PAT sittings between the given dates.
-        
-        Includes both PAT Maths 4th Edition and PAT Reading 5th Edition.
-        
+                
         Args:
             from_date: The start date to download results for in 
                 dd-mm-yyyy format.
             to_date: The end date to download results for in dd-mm-yyyy format.
             
         Returns:
             A list of test sittings.
         """
-        test_names = ["PAT Maths 4th Edition", "PAT Reading 5th Edition"]
+        test_names = []
+        for t in self.tests:
+            if t['reportType'] == "Pat":
+                test_names.append(t['name'])
 
         sittings = []
 
         for test_name in test_names:
             test = self.tests.get_test_from_name(test_name)
             test_id = test['testId']
             scale_id = test['scale_id']
@@ -156,25 +154,38 @@
                 r = self.get(ids_url)
                 ids = r.json()
 
                 self.headers.update(
                     {"Content-Type": "application/json;charset=utf-8"})
 
                 if ids:
-                    sittings_url = f"https://oars.acer.edu.au/api/{self.school}/reports-new/getGroupReportSittingsByIds.ajax/?scale_slug={scale_slug}&test_id={test_id}&form_id={form_id}&from={from_date}&to={to_date}&match_criterion=all&date-type=between&form_name={form_name}&test_name={test_name}&report_type=pat&tag_year_match_criterion=and&report_template=pat"
+                    sittings_url = f"https://oars.acer.edu.au/api/{self.school}/reports-new/getScaleReportSittingsByIds.ajax?scale_slug={scale_slug}&test_id={test_id}&form_id={form_id}&extra_candidate_fields=true&include_sitting_responses=true"
                     sittings_url = sittings_url.replace(" ", "%20")
+                    responses_url = f"https://oars.acer.edu.au/api/{self.school}/reports-new/getSittingResponses.ajax?scale_slug={scale_slug}&test_id={test_id}&form_id={form_id}"
+                    responses_url = responses_url.replace(" ", "%20")
 
                     for i in range(0, len(ids[test_id][form_id]), 100):
                         payload = {
                             'ids': ids[test_id][form_id][i:i + 100],
                             'security_token': self.security_token
                         }
                         r = self.post(sittings_url, json=payload)
-                        sittings += r.json()
-                del self.headers["Content-Type"]
+                        new_sittings = r.json()
+
+                        r = self.post(responses_url, json=payload)
+                        responses = r.json()
+
+                        for sitting in new_sittings:
+                            sitting["responses"] = responses[
+                                sitting["sittingId"]]["responses"]
+
+                        sittings += new_sittings
+
+        del self.headers["Content-Type"]
+
         return PATSittings(sittings)
 
     def get_ewrite_sittings(self, candidates: OARSCandidates, from_date: str,
                             to_date: str) -> EWriteSittings:
         """Downloads the results for eWrite sittings for the candidates.
 
         Downloads results between to_date and from_date.
@@ -290,27 +301,32 @@
             An instance of OARSCandidates.
         """
 
         ids_url = f"https://oars.acer.edu.au/api/{self.school}/candidates/getCandidateIds?enrolled={enrolled}"
         r = self.get(ids_url)
         ids = r.json()
 
+        headers = {'Content-Type': 'application/json; charset=utf-8'}
+        self.headers.update(headers)
+
         candidates = []
         if ids:
             candidates_url = f"https://oars.acer.edu.au/api/{self.school}/candidates/getCandidatesByIds/"
             for i in range(0, len(ids), 50):
                 payload = {
-                    'extraFields': ['password_visible'],
                     'ids': ids[i:i + 50],
-                    'security_token': self.security_token,
-                    'withForms': 'true'
+                    'extraFields': ['password_visible'],
+                    'withForms': 'true',
+                    'security_token': self.security_token
                 }
                 r = self.post(candidates_url, json=payload)
                 candidates += r.json()
 
+        del self.headers["Content-Type"]
+
         return OARSCandidates(candidates)
 
     def get_staff_xlsx(self, xlsx_filename):
         """Downloads a XLSX of all staff details.
         
         Downloads the XLSX that is provided through the bulk edit staff
         interface.
@@ -337,72 +353,21 @@
                 details.
 
         Returns:
             True if the upload was successful.
         """
         del self.headers['Content-Type']
 
-        upload_url = f"https://oars.acer.edu.au/api/{s.school}/staff/bulkUpdate"
+        upload_url = f"https://oars.acer.edu.au/api/{self.school}/staff/bulkUpdate"
         files = {'upload': open(staff_xlsx, 'rb')}
         payload = {'security_token': self.security_token}
         r = self.post(upload_url, files=files, data=payload)
         return r.status_code == 200
 
 
 class SecurityTokenParser(HTMLParser):
     """Extracts the OARS security token from a page."""
 
     def handle_data(self, data):
         if 'oarsData' in data:
             data = json.loads(data[22:])
             self.security_token = data['securityToken']
-
-
-class OARSAuthenticator(Protocol):
-    """An abstract class for generic OARS authenticators."""
-
-    @abstractmethod
-    def authenticate(self, session: OARSSession):
-        raise NotImplementedError
-
-
-class OARSFirefoxCookieAuthenticator(OARSAuthenticator):
-    """An OARS authenticator that gets login details from the local Firefox installation."""
-
-    def authenticate(self, s: OARSSession):
-        cj = browser_cookie3.firefox(domain_name='oars.acer.edu.au')
-
-        for cookie in cj:
-            c = {cookie.name: cookie.value}
-            s.cookies.update(c)
-
-
-class OARSConfigAuthenticator(OARSAuthenticator):
-    """Authenticates using a provided username and password."""
-
-    def __init__(self, username: str, password: str):
-        self.username = username
-        self.password = password
-
-    def authenticate(self, s: OARSSession):
-
-        login_url = f"https://oars.acer.edu.au/{s.school}"
-        # get security token
-        r = s.get(login_url)
-        pattern = r'name="security\[token\]" value="(?P<token>[\$0-9A-Za-z+/\.\\]*)"'
-        m = re.search(pattern, r.text)
-        security_token = quote(m.group('token'))
-        # url encode username and password
-        headers = {"Content-Type": "application/x-www-form-urlencoded"}
-        s.headers.update(headers)
-        username = quote(self.username)
-        password = quote(self.password)
-        # auth
-        payload = f'security%5Btoken%5D={security_token}&username={username}&password={password}'
-        r = s.post(login_url, data=payload)
-        if r.status_code != 200:
-            raise OARSAuthenticateError
-
-
-class OARSAuthenticateError(Exception):
-    """Raised if an error occurs related to OARS authentication."""
-    pass
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/oarstests.py` & `vicedtools-0.0.8/src/vicedtools/acer/oarstests.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/patitems.py` & `vicedtools-0.0.8/src/vicedtools/acer/patitems.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/patresults.py` & `vicedtools-0.0.8/src/vicedtools/acer/patresults.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,63 +341,63 @@
         score: the PAT scale score the student achieved
 
     Returns:
         One of "Very low", "Low", "Average", "High", or "Very high".
     '''
     means = {
         'Reading': {
-            1: 87.1,
-            2: 100.5,
-            3: 110.9,
-            4: 118.7,
-            5: 124.5,
+            1: 84.2,
+            2: 101.1,
+            3: 113.0,
+            4: 120.9,
+            5: 125.8,
             6: 128.8,
-            7: 132.0,
-            8: 134.7,
-            9: 137.3,
-            10: 140.4
+            7: 130.7,
+            8: 132.6,
+            9: 135.5,
+            10: 140.5
         },
         'Maths': {
-            1: 93.2,
-            2: 103.0,
-            3: 110.9,
-            4: 117.4,
-            5: 122.7,
-            6: 127,
-            7: 130.5,
+            1: 99.5,
+            2: 108.3,
+            3: 115.4,
+            4: 121.1,
+            5: 125.5,
+            6: 128.9,
+            7: 131.6,
             8: 133.6,
-            9: 136.5,
-            10: 139.4
+            9: 135.4,
+            10: 137.1
         }
     }
 
     stdevs = {
         'Reading': {
-            1: 17.4,
-            2: 16.2,
-            3: 14.7,
-            4: 15.0,
-            5: 12.8,
-            6: 12.0,
-            7: 12.6,
-            8: 10.7,
-            9: 11.4,
-            10: 10.4
+            1: 16.3,
+            2: 15.0,
+            3: 15.9,
+            4: 16.2,
+            5: 13.2,
+            6: 12.8,
+            7: 13.0,
+            8: 12.8,
+            9: 12.4,
+            10: 12.2
         },
         'Maths': {
-            1: 14.6,
-            2: 14.9,
-            3: 14.6,
-            4: 14.2,
-            5: 12.8,
-            6: 12.6,
-            7: 11.5,
-            8: 12.2,
+            1: 11.4,
+            2: 12.2,
+            3: 13.0,
+            4: 11.4,
+            5: 12.6,
+            6: 11.9,
+            7: 13.1,
+            8: 12.3,
             9: 12.9,
-            10: 13.1
+            10: 12.4
         }
     }
     # expect year_level as "Year 7"
     pattern = r"[A-Za-z ]*(?P<yearlevel>[0-9]+)"
     m = re.search(pattern, year_level)
     if m:
         year_level_num = int(m.group('yearlevel'))
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/acer/patsittings.py` & `vicedtools-0.0.8/src/vicedtools/acer/patsittings.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from vicedtools.acer.patresults import score_categoriser
 from vicedtools.acer.oarstests import OARSTests
 
 
 class PATSitting(dict):
     """A class for storing a PAT sitting result."""
 
-    def group_report(self, tests: PATTests) -> dict:
+    def group_report(self, tests: OARSTests) -> dict:
         """Returns the data provided in a PAT group report export for this sitting."""
         data = {}
         try:
             data['Unique ID'] = self['unique_id']
         except KeyError:
             data['Unique ID'] = ""
         data['Family name'] = self['family_name']
@@ -51,64 +51,68 @@
             self['yearLevel'], self['sitting']['updated'])
         data['Active tags'] = ""
         data['Inactive tags'] = ""
         for key, value in self['responses'].items():
             data[key] = extract_response(value)
         data['Score'] = self['score']['score']
         data['Scale'] = self['score']['scale']
-        data['Score'] = self['score']['score']
         data['Stanine'] = self['score']['norms'][1]['stanine']
         data['Percentile'] = self['score']['norms'][1]['percentile']
-
         test_id = self['sitting']['test_id']
         form_id = self['sitting']['form_id']
         test_name = tests.get_name_from_id(test_id)
         form_name = tests.get_test_from_id(test_id).get_form_name_from_id(
             form_id)
         data['Test'] = test_name
         data['Test form'] = form_name
 
         return data
 
-    def summary(self, tests: PATTests) -> dict:
+    def summary(self, tests: OARSTests) -> dict:
         """Extracts a summary of the results.
         
         Args:
             tests: An instance of PATTests containing the relevant test metadata.
         
         Returns:
             A dictionary containing the summary.
         """
         test_name_stub = {
             "PAT Maths 4th Edition": "Maths",
             "PAT Reading 5th Edition": "Reading",
             "PAT Maths Adaptive": "Maths",
             "PAT Reading Adaptive": "Reading",
-            "eWrite": "eWrite"
+            "PAT-R Comprehension": "Reading",
+            "PAT Maths Plus": "Maths",
+            "eWrite": "eWrite",
+            "AGAT 1st Edition": "AGAT",
+            "PAT Vocabulary Skills": "Vocabulary",
+            "PAT Grammar and Punctuation": "Grammar and Punctuation"
         }
 
-        test_id = self['sitting']['test_id']
-        form_id = self['sitting']['form_id']
-        test = tests.get_test_from_id(test_id)
-        test_name = test['name']
-        form_name = test.get_form_name_from_id(form_id)
-
         data = {}
         data['Username'] = self['username']
         data['Completed'] = datetime.strptime(
-            time.ctime(self['sitting']['completed']), "%a %b %d %H:%M:%S %Y")
-        data[
-            'Year level (at time of test)'] = "Year " + year_level_at_time_of_test(
-                self['yearLevel'], self['sitting']['updated'])
-        data['Test'] = test_name_stub[test_name]
-        data['Test form'] = form_name
-        data['Scale'] = self['score']['scale']
-        data['Score category'] = score_categoriser(
-            data['Test'], data['Year level (at time of test)'],
-            data['Completed'], data['Scale'])
+            time.ctime(self['sittingTimeStamp']), "%a %b %d %H:%M:%S %Y")
+        data['Year level (at time of test)'] = self['yearLevel']
+        data['Scale'] = self['scaleScore']
+        data["Error"] = self['scaleScoreErrorMargin']
+        data['rawScore'] = self['rawScore']
+
+        data['Test form'] = self['formName']
+        try:
+            data['Test'] = test_name_stub[self['testName']]
+        except KeyError:
+            data['Test'] = self['testName']
+        try:
+            data['Score category'] = score_categoriser(
+                data['Test'], data['Year level (at time of test)'],
+                data['Completed'], data['Scale'])
+        except KeyError:
+            data["Score category"] = ""
 
         return data
 
 
 class PATSittings(list):
     """A class for storing PAT sitting results."""
 
@@ -116,15 +120,15 @@
         if isinstance(sittings, PATSittings):
             super().__init__(sittings)
         if isinstance(sittings, abc.Sequence):
             super().__init__([PATSitting(i) for i in sittings])
         else:
             raise TypeError(f"Unsupported type: {type(sittings)}")
 
-    def group_report(self, tests: PATTests, test_name: str,
+    def group_report(self, tests: OARSTests, test_name: str,
                      form_name: str) -> list:
         """Extracts data for the preparation of a group report spreadsheet.
         
         Args:
             tests: A PATTests instance containing the relevant test metadata.
             test_name: The name of the test to export. E.g. "PAT Maths 4th Edition"
             form_name: The name of the form to export. E.g. "PAT Maths Test 6"
@@ -139,15 +143,15 @@
         for sitting in self:
             if sitting["sitting"]["test_id"] == test_id and sitting["sitting"][
                     "form_id"] == form_id:
                 data.append(sitting.group_report(tests))
         return data
 
     def summary(self,
-                tests: PATTests,
+                tests: OARSTests,
                 recent_only: bool = False) -> pd.DataFrame:
         """Extracts a basic summary of results.
         
         Args:
             tests: A PATTests instance containing the relevant test metadata.
             recent_only: If True, only give the most recent result for each student.
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/compass/__init__.py` & `vicedtools-0.0.8/src/vicedtools/vce/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,10 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from vicedtools.compass.compasssession import (
-    CompassSession, CompassAuthenticator, CompassAuthenticationError,
-    CompassLongRunningFileRequestError, CompassConfigAuthenticator,
-    CompassCLIAuthenticator, CompassFirefoxCookieAuthenticator,
-    get_report_cycle_id, sanitise_filename)
-
-from vicedtools.compass.reports import Reports, class_code_parser
+from vicedtools.vce.vasssession import (VASSAuthenticator,
+                                        VASSBasicAuthenticator,
+                                        VASSAuthenticationError, VASSSession)
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/compass/compasssession.py` & `vicedtools-0.0.8/src/vicedtools/compass/compasssession.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,145 +11,85 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A requests.requests.Session class for accessing the Compass API."""
 
 from __future__ import annotations
 
-from abc import abstractmethod
 from datetime import datetime
 from math import ceil
 import os
 import re
 import requests
 import time
-from typing import Protocol
-from urllib.parse import quote
 import zipfile
 
-import browser_cookie3
+from vicedtools.compass import CompassAuthenticator
+
+# Minimum interval between requests
+MIN_REQUEST_INTERVAL = 500000000  # 500 milliseconds in nanoseconds
 
 
 def current_ms_time() -> int:
     """Returns the current millisecond time."""
     return round(time.time() * 1000)
 
 
 def sanitise_filename(filename):
     filename = re.sub(r'[/\\:\*\?<>|]+', '', filename)
     filename = re.sub(' +', ' ', filename)
     return filename
 
 
-class CompassAuthenticator(Protocol):
-    """An abstract class for generic Compass authenticators."""
-
-    @abstractmethod
-    def authenticate(self, session: CompassSession):
-        raise NotImplementedError
-
-
-class CompassFirefoxCookieAuthenticator(CompassAuthenticator):
-    """A Compass authenaticator that gets login details from the local Firefox installation."""
-
-    def authenticate(self, s: CompassSession):
-        cj = browser_cookie3.firefox(
-            domain_name=f'{s.school_code}.compass.education')
-
-        for cookie in cj:
-            c = {cookie.name: cookie.value}
-            s.cookies.update(c)
-
-
-class CompassAuthenticationError(Exception):
-    """Authentication with Compass failed."""
-    pass
-
-
 class CompassLongRunningFileRequestError(Exception):
     """Long running file request failed."""
     pass
 
 
-class CompassConfigAuthenticator(CompassAuthenticator):
-    """Authenticates using a provided username and password."""
-
-    def __init__(self, username: str, password: str):
-        self.username = username
-        self.password = password
-
-    def authenticate(self, s: CompassSession):
-        headers = {"Content-Type": "application/x-www-form-urlencoded"}
-        s.headers.update(headers)
-        login_url = f"https://{s.school_code}.compass.education/login.aspx?sessionstate=disabled"
-        # get viewstate
-        r = s.get(login_url)
-        pattern = 'id="__VIEWSTATE" value="(?P<viewstate>[0-9A-Za-z+/]*)"'
-        m = re.search(pattern, r.text)
-        viewstate = quote(m.group('viewstate'))
-        pattern = 'id="__VIEWSTATEGENERATOR" value="(?P<viewstategenerator>[0-9A-Za-z+/]*)"'
-        m = re.search(pattern, r.text)
-        viewstategenerator = quote(m.group('viewstategenerator'))
-        # url encode username and password
-        username = quote(self.username)
-        password = quote(self.password)
-        # auth
-        payload = f'__EVENTTARGET=button1&__EVENTARGUMENT=&__VIEWSTATE={viewstate}&browserFingerprint=3597254041&username={username}&password={password}&g-recaptcha-response=&rememberMeChk=on&__VIEWSTATEGENERATOR={viewstategenerator}'
-        r = s.post(login_url, data=payload)
-        if r.status_code != 200:
-            raise CompassAuthenticationError
-
-
-class CompassCLIAuthenticator(CompassAuthenticator):
-    """Authenticates using login details from CLI prompt."""
-
-    def authenticate(self, s: CompassSession):
-        username = input("Compass username: ")
-        password = input("Compass password: ")
-        headers = {"Content-Type": "application/x-www-form-urlencoded"}
-        s.headers.update(headers)
-        login_url = f"https://{s.school_code}.compass.education/login.aspx?sessionstate=disabled"
-        # get viewstate
-        r = s.get(login_url)
-        pattern = 'id="__VIEWSTATE" value="(?P<viewstate>[0-9A-Za-z+/]*)"'
-        m = re.search(pattern, r.text)
-        viewstate = quote(m.group('viewstate'))
-        pattern = 'id="__VIEWSTATEGENERATOR" value="(?P<viewstategenerator>[0-9A-Za-z+/]*)"'
-        m = re.search(pattern, r.text)
-        viewstategenerator = quote(m.group('viewstategenerator'))
-        # url encode username and password
-        username = quote(username)
-        password = quote(password)
-        # auth
-        payload = f'__EVENTTARGET=button1&__EVENTARGUMENT=&__VIEWSTATE={viewstate}&browserFingerprint=3597254041&username={username}&password={password}&g-recaptcha-response=&rememberMeChk=on&__VIEWSTATEGENERATOR={viewstategenerator}'
-        r = s.post(login_url, data=payload)
-        if r.status_code != 200:
-            raise CompassAuthenticationError
-
-
 class CompassSession(requests.sessions.Session):
     """A requests Session extension with methods for accessing data from Compass."""
 
     def __init__(self, school_code: str, authenticator: CompassAuthenticator):
         """Creates a requests Session with Compass authentication completed.
         
         Args:
             school_code: Your school's compass school code.
             authenticator: An instance of CompassAuthenticator to perform the
                 required authentication with Compass.
         """
         requests.sessions.Session.__init__(self)
         headers = {
             "User-Agent":
-                "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:96.0) Gecko/20100101 Firefox/96.0"
+                "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:105.0) Gecko/20100101 Firefox/105.0"
         }
         self.headers.update(headers)
         self.school_code = school_code
 
+        self.last_request_time = 0
+
         authenticator.authenticate(self)
+        self.MAX_POLL_REQUESTS = 100
+
+    def get(self, *args, **kwargs):
+        """Enforce a minimum delay between requests."""
+        now = time.time_ns()
+        wait_time = MIN_REQUEST_INTERVAL - now + self.last_request_time
+        if wait_time > 0:
+            time.sleep(wait_time / 1000000000)
+        self.last_request_time = time.time_ns()
+        return super().get(*args, **kwargs)
+
+    def post(self, *args, **kwargs):
+        """Enforce a minimum delay between requests."""
+        now = time.time_ns()
+        wait_time = MIN_REQUEST_INTERVAL - now + self.last_request_time
+        if wait_time > 0:
+            time.sleep(wait_time / 1000000000)
+        self.last_request_time = time.time_ns()
+        return super().post(*args, **kwargs)
 
     def long_running_file_request(self, request_payload: str,
                                   save_dir: str) -> str:
         headers = {'Content-Type': 'application/json; charset=utf-8'}
         self.headers.update(headers)
 
         request_url = f"https://{self.school_code}.compass.education/Services/LongRunningFileRequest.svc/QueueTask"
@@ -162,31 +102,34 @@
                 break
             else:
                 if i < max_attempts - 1:
                     time.sleep(5)
                     print(
                         f"File request error. Retrying {max_attempts - i - 1} more times."
                     )
+                    print(r.text)
                 else:
                     print('File request failed.')
                     return ""
         # poll for status
         time.sleep(1)
         poll_requests = 1
         poll_url = f"https://{self.school_code}.compass.education/Services/LongRunningFileRequest.svc/PollTaskStatus"
         payload = {"guid": guid}
         r = self.post(poll_url, json=payload)
         data = r.json()
         status = data['d']['requestStatus']
-        while status == 2:
+        while status <= 2:
             time.sleep(6)
             r = self.post(poll_url, json=payload)
             data = r.json()
             status = data['d']['requestStatus']
             poll_requests += 1
+            if poll_requests > self.MAX_POLL_REQUESTS:
+                break
         if status != 3:
             raise CompassLongRunningFileRequestError(
                 f"Unexpected Compass response, after {poll_requests} poll requests received status: {status}"
             )
         # get file details
         get_task_url = f"https://{self.school_code}.compass.education/Services/LongRunningFileRequest.svc/GetTask"
         payload = {"guid": guid}
@@ -236,15 +179,15 @@
         Args:
             cycle_id: The Compass cycle id for the cycle to download.
             cycle_title: The title of the cycle to download.
             save_dir: The folder to save the export into.
         """
         payload = f'{{"type":"2","parameters":"{{\\"cycleId\\":{cycle_id}}}"}}'
         filename = self.long_running_file_request(payload, save_dir)
-        head, tail = os.path.split(filename)
+        head, _tail = os.path.split(filename)
         sanitised_title = sanitise_filename(cycle_title)
         new_tail = f"SemesterReports-{cycle_year}-{sanitised_title}.csv"
         new_filename = os.path.join(head, new_tail)
         if os.path.exists(new_filename):
             os.remove(new_filename)
         os.rename(filename, new_filename)
 
@@ -302,15 +245,15 @@
         
         Returns:
             A list containing the metadata for each academic group.
         """
         headers = {'Content-Type': 'application/json; charset=utf-8'}
         self.headers.update(headers)
 
-        learning_tasks_admin_url = f"https://{self.school_code}.compass.education/Communicate/LearningTasksAdministration.aspx"
+        learning_tasks_admin_url = f"https://{self.school_code}.compass.education/Learn/Subjects.aspx"
         r = self.get(learning_tasks_admin_url)
         pattern = "Compass.referenceDataCacheKeys.schoolConfigKey = '(?P<key>[0-9a-z-]*)'"
         m = re.search(pattern, r.text)
         key = m.group('key')
         groups = []
         page = 1
         academic_groups_url = f"https://{self.school_code}.compass.education/Services/ReferenceDataCache.svc/GetAllAcademicGroups?sessionstate=readonly&v={key}&page={page}&start={25*(page-1)}&limit=25"
@@ -318,14 +261,16 @@
         new_groups = r.json()['d']
         groups += new_groups
         while len(new_groups) == 25:
             page += 1
             academic_groups_url = f"https://{self.school_code}.compass.education/Services/ReferenceDataCache.svc/GetAllAcademicGroups?sessionstate=readonly&v={key}&page={page}&start={25*(page-1)}&limit=25"
             r = self.get(academic_groups_url)
             new_groups = r.json()['d']
+            if new_groups[0]['id'] != 25 * (page - 1):
+                break
             groups += new_groups
         return groups
 
     def export_student_details(self,
                                file_name: str = "student details.csv",
                                detailed: bool = False) -> None:
         '''Exports student details from Compass.
@@ -400,27 +345,14 @@
                     info = zip_ref.getinfo(content)
                     info.filename = new_filename
                     zip_ref.extract(info, path=save_dir)
                 else:
                     zip_ref.extract(content, path=save_dir)
         os.remove(archive_file_name)
 
-    def get_subject_metadata(self, file_name: str, academic_group: int = -1):
-        """Downloads a CSV with subject metadata.
-        
-        Args:
-            file_name: The file name to save the CSV to.
-            academic_group: Optional, the academic group id to download the
-                metadata for. Defaults to the currently active academic group.
-        """
-        url = f"https://{self.school_code}.compass.education/Learn/Subjects.aspx?action=export-csv&academicGroup={academic_group}"
-        r = self.get(url)
-        with open(file_name, 'wb') as f:
-            f.write(r.content)
-
     def get_classes_for_subject(self, subject_id: int) -> list[dict]:
         """Downloads a CSV with subject metadata.
         
         Args:
             subject_id: The Compass subject id number for the subject.
 
         Returns:
@@ -444,20 +376,31 @@
                 currently active group.
                 
         Returns:
             A list of dictionaries containing subject metadata.
         """
         headers = {'Content-Type': 'application/json; charset=utf-8'}
         self.headers.update(headers)
-        subjects_url = f"https://{self.school_code}.compass.education/Services/Subjects.svc/GetSubjectsInAcademicGroup?sessionstate=readonly&_dc={current_ms_time}"
-        payload = f'{{"academicGroupId":{academic_group},"includeDataSyncSubjects":true,"page":1,"start":0,"limit":50,"sort":"[{{\\"property\\":\\"importIdentifier\\",\\"direction\\":\\"ASC\\"}}]"}}'
+        subjects_url = f"https://{self.school_code}.compass.education/Services/Subjects.svc/GetSubjectsInAcademicGroup?sessionstate=readonly&_dc={current_ms_time()}"
+
+        subjects = []
+        page = 1
+        payload = f'{{"academicGroupId":{academic_group},"includeDataSyncSubjects":true,"page":{page},"start":{50*page-50},"limit":50,"sort":"[{{\\"property\\":\\"importIdentifier\\",\\"direction\\":\\"ASC\\"}}]"}}'
         r = self.post(subjects_url, data=payload)
+        new_subjects = r.json()['d']['data']
+        subjects += new_subjects
+        while len(new_subjects) == 50:
+            page += 1
+            payload = f'{{"academicGroupId":{academic_group},"includeDataSyncSubjects":true,"page":{page},"start":{50*page-50},"limit":50,"sort":"[{{\\"property\\":\\"importIdentifier\\",\\"direction\\":\\"ASC\\"}}]"}}'
+            r = self.post(subjects_url, data=payload)
+            new_subjects = r.json()['d']['data']
+            subjects += new_subjects
+
         del self.headers['Content-Type']
-        decoded_response = r.json()['d']['data']
-        return decoded_response
+        return subjects
 
     def get_classes(self, academic_group: int = -1) -> list[dict]:
         """Gets a list of all classes in an academic group.
         
         Args:
             academic_group: The academic group to export. Defaults to the
                 currently active group.
@@ -468,13 +411,39 @@
         subjects = self.get_subjects(academic_group)
         classes = []
         for subject in subjects:
             new_classes = self.get_classes_for_subject(subject['id'])
             classes += new_classes
         return classes
 
+    def get_class_enrolments(self,
+                             activity_id: int,
+                             add_activity_id: bool = False) -> list[dict]:
+        """Gets a list of all enrolments in a class.
+        
+        Args:
+            activity_id: An activity id for one lesson for the class.
+        
+        Returns:
+            A list of dictionaries containing student metadata.
+        """
+        headers = {'Content-Type': 'application/json; charset=utf-8'}
+        self.headers.update(headers)
+
+        payload = f'{{"activityId":{activity_id},"page":1,"start":0,"limit":25}}'
+        url = f"https://{self.school_code}.compass.education/Services/Activity.svc/GetEnrolmentsByActivityId?sessionstate=readonly&_dc={current_ms_time()}"
+        r = self.post(url, data=payload)
+        new_enrolments = r.json()['d']
+        if add_activity_id:
+            for enrolment in new_enrolments:
+                enrolment.update({"activity_id": activity_id})
+
+        del self.headers['Content-Type']
+
+        return new_enrolments
+
 
 def get_report_cycle_id(cycles, year, name):
     for c in cycles:
         if c['year'] == year and c['name'] == name:
             return c['id']
     return None
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/compass/reports.py` & `vicedtools-0.0.8/src/vicedtools/compass/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                                            ignore_index=True)
 
     @classmethod
     def fromReportsExport(cls,
                           filename: str,
                           year: str = None,
                           semester: str = None,
-                          grade_score_mapper: Callable[[str], float] = None,
+                          grade_score_mapper: dict[str, float] = None,
                           grade_dtype: pd.api.types.CategoricalDtype = None,
                           replace_values: dict[str, dict] = None) -> Reports:
         """Creates a new Reports instance from a Compass reports export."""
         try:
             temp_df = pd.read_csv(filename,
                                   na_values=None,
                                   keep_default_na=False)
@@ -110,15 +110,15 @@
 
         if replace_values:
             temp_df.replace(replace_values, inplace=True)
         if grade_dtype:
             temp_df["Result"] = temp_df["Result"].astype(grade_dtype)
             temp_df.dropna(subset=["Result"], inplace=True)
         if grade_score_mapper:
-            temp_df["ResultScore"] = temp_df["Result"].apply(grade_score_mapper)
+            temp_df["ResultScore"] = temp_df["Result"].map(grade_score_mapper)
         else:
             temp_df["ResultScore"] = None
 
         temp_df.rename(columns={
             "Result": "ResultGrade",
             "AssessmentArea": "ResultName",
             "AssessmentType": "Type"
@@ -174,15 +174,15 @@
 
         if replace_values:
             temp_df.replace(replace_values, inplace=True)
         if grade_dtype:
             temp_df["Result"] = temp_df["Result"].astype(grade_dtype)
             temp_df.dropna(subset=["Result"], inplace=True)
         if grade_score_mapper:
-            temp_df["ResultScore"] = temp_df["Result"].apply(grade_score_mapper)
+            temp_df["ResultScore"] = temp_df["Result"].map(grade_score_mapper)
         else:
             temp_df["ResultScore"] = None
         temp_df.rename(columns={
             'Code': 'ClassCode',
             'TaskName': 'ResultName',
             'Result': 'ResultGrade',
             "TeacherImportIdentifier": "TeacherCode"
@@ -250,15 +250,15 @@
 
         if replace_values:
             temp_df.replace(replace_values, inplace=True)
         if grade_dtype:
             temp_df["ResultGrade"] = temp_df["ResultGrade"].astype(grade_dtype)
             temp_df.dropna(subset=["ResultGrade"], inplace=True)
         if grade_score_mapper:
-            temp_df["ResultScore"] = temp_df["ResultGrade"].apply(
+            temp_df["ResultScore"] = temp_df["ResultGrade"].map(
                 grade_score_mapper)
         else:
             temp_df["ResultScore"] = None
 
         temp_df["SubjectName"] = None
 
         class_details_columns = ['Time', 'ClassCode', 'TeacherCode']
@@ -295,15 +295,15 @@
             return str(year) + "-12-31"
         else:
             return None
 
     def addLearningTasksExport(
             self,
             filename: str,
-            grade_score_mapper: Callable[[str], float] = None,
+            grade_score_mapper: dict[str, float] = None,
             grade_dtype: pd.api.types.CategoricalDtype = None,
             learning_task_filter: Callable[[pd.DataFrame], pd.DataFrame] = None,
             replace_values: dict[str, dict] = None) -> None:
         """Adds data from a Compass Learning Tasks export."""
 
         temp = Reports.fromLearningTasksExport(
             filename,
@@ -320,15 +320,15 @@
             temp.class_details.dropna(subset=["TeacherCode"])
         ],
                                        ignore_index=True)
         self.class_details.drop_duplicates(inplace=True)
 
     def addReportsExport(self,
                          filename: str,
-                         grade_score_mapper: Callable[[str], float] = None,
+                         grade_score_mapper: dict[str, float] = None,
                          grade_dtype: pd.api.types.CategoricalDtype = None,
                          replace_values: dict[str, dict] = None) -> None:
         """Adds data from a Compass reports export."""
 
         temp = Reports.fromReportsExport(filename,
                                          grade_score_mapper=grade_score_mapper,
                                          grade_dtype=grade_dtype,
@@ -338,15 +338,15 @@
             subset=["Time", "StudentCode", "ClassCode", "ResultName"],
             inplace=True)
 
     def addProgressReportsExport(
             self,
             filename: str,
             progress_report_items: list[str],
-            grade_score_mapper: Callable[[str], float] = None,
+            grade_score_mapper: dict[str, float] = None,
             grade_dtype: pd.api.types.CategoricalDtype = None,
             replace_values: dict[str, dict] = None) -> None:
         """Adds data from a Compass progress reports export."""
 
         temp = Reports.fromProgressReportsExport(
             filename,
             progress_report_items,
@@ -368,52 +368,53 @@
         data = pd.concat([self.data, other.data], ignore_index=True)
         data.drop_duplicates(
             subset=["Time", "StudentCode", "ClassCode", "ResultName"],
             inplace=True)
         return Reports(data)
 
     def importSubjectsData(self,
-                           subjects_file: str,
-                           class_code_parser: Callable[[str, str],
-                                                       str] = class_code_parser,
+                           classes_csv: str,
                            replace_values: dict[str, dict] = None) -> None:
         """Adds subject metadata from a separate csv file.
         
-        Expects a csv with columns 'SubjectCode', 'LearningArea', 'SubjectName'.
+        Imports subject codes and names from the Compass classes csv export.
 
         Args:
-            subjects_file: The path to the csv file containing the subjects
-                metadata.
-            class_code_parser: A function that takes the class code, a regex
-                pattern to recognise the subject code and returns the subject
-                code.
+            classes_csv: The path to the classes csv file.
             replace_values: A dictionary to be passed to DataFrame.replace().
                 Keys are columns and values are dictionaries containing 
                 remappings for values in that column. Can be used to
                 standardise things where your school has changed the name of a
-                subject over time or has changed their grading system.
+                subject or learning area over time.
         """
 
-        subjects_df = pd.read_csv(subjects_file)
-
-        subjects = subjects_df["SubjectCode"].values
-        pattern_string = "(?P<code>" + "|".join(subjects) + ")"
+        classes_df = pd.read_csv(classes_csv)
 
-        self.data["SubjectCode"] = self.data["ClassCode"].apply(
-            class_code_parser, pattern_string=pattern_string)
-        if replace_values:
-            self.data.replace(replace_values, inplace=True)
-        columns = [
-            'Time', 'ClassCode', 'StudentCode', 'ResultName', 'ResultGrade',
-            'ResultScore', 'Type', 'SubjectCode', 'TeacherCode'
+        self.data["Year"] = self.data["Time"].dt.year
+        reports_columns = [
+            'Time',
+            'ClassCode',
+            'StudentCode',
+            'ResultName',
+            'ResultGrade',
+            'ResultScore',
+            'Type',
+            'Year',
+        ]
+        classes_columns = [
+            'LearningArea', 'ClassCode', 'SubjectCode', 'SubjectName',
+            'TeacherCode', 'Year'
         ]
-        self.data = pd.merge(self.data[columns],
-                             subjects_df,
+        self.data = pd.merge(self.data[reports_columns],
+                             classes_df[classes_columns],
                              how="left",
-                             on="SubjectCode")
+                             on=["ClassCode", "Year"])
+        if replace_values:
+            self.data.replace(replace_values, inplace=True)
+        self.data.drop(columns="Year", inplace=False)
 
     def updateFromClassDetails(self) -> None:
         """Infills TeacherCode data with data available from other reports."""
 
         self.data.drop(columns="TeacherCode", inplace=True, errors="ignore")
         self.data = pd.merge(self.data,
                              self.class_details,
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/educationperfect.py` & `vicedtools-0.0.8/src/vicedtools/educationperfect.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/gcp/__init__.py` & `vicedtools-0.0.8/src/vicedtools/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/gcp/api.py` & `vicedtools-0.0.8/src/vicedtools/gcp/api.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/gcp/format.py` & `vicedtools-0.0.8/src/vicedtools/gcp/format.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/gcp/schema.py` & `vicedtools-0.0.8/src/vicedtools/gcp/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     bigquery.SchemaField("DateOfBirth", "DATE")
 ]
 STUDENT_DETAILS_CLUSTERING_FIELDS = [
     "Status", "StudentCode", "YearLevel", "Gender"
 ]
 
 STUDENT_ENROLMENTS_SCHEMA = [
-    bigquery.SchemaField("ClassGroupCode", "STRING"),
+    bigquery.SchemaField("ClassCode", "STRING"),
     bigquery.SchemaField("StudentCode", "STRING")
 ]
 
-STUDENT_ENROLMENTS_CLUSTERING_FIELDS = ["ClassGroupCode", "StudentCode"]
+STUDENT_ENROLMENTS_CLUSTERING_FIELDS = ["ClassCode", "StudentCode"]
 
 REPORTS_SCHEMA = [
     bigquery.SchemaField("Time", "DATE"),
     bigquery.SchemaField("ClassCode", "STRING"),
     bigquery.SchemaField("StudentCode", "STRING"),
     bigquery.SchemaField("ResultName", "STRING"),
     bigquery.SchemaField("ResultGrade", "STRING"),
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/naplan/dataservicesession.py` & `vicedtools-0.0.8/src/vicedtools/naplan/dataservicesession.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 class DataserviceAuthenticationError(Exception):
     """Authentication with Data Service failed."""
     pass
 
 
-class DataServiceConfigAuthenticator(DataserviceAuthenticator):
+class DataServiceBasicAuthenticator(DataserviceAuthenticator):
     """Authenticates using a provided username and password."""
 
     def __init__(self, username: str, password: str):
         self.username = username
         self.password = password
 
     def authenticate(self, s: DataserviceSession):
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/naplan/sssrdata.py` & `vicedtools-0.0.8/src/vicedtools/naplan/sssrdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """A class for extracting data from the NAPLAN SSSR data.js file."""
 
 import requests
 import time
 import urllib3
 import os.path
 
-import demjson
+import demjson3
 import numpy as np
 import pandas as pd
 
 
 class SSSRdata:
     """A class for extracting data from the NAPLAN SSSR data.js file.
     
@@ -40,15 +40,15 @@
         """Parses the data contained in the data.js file.
         
         Args:
             js_file: The path to the SSSR data.js file.
         """
         with open(js_file, 'r', encoding='utf8') as f:
             js_data = f.readline()
-        self.data = demjson.decode(js_data[11:])
+        self.data = demjson3.decode(js_data[11:])
 
         self.domains = pd.DataFrame(self.data['domains'])
         self.domains.set_index("domainId", inplace=True)
         self.subdomains = pd.DataFrame(self.data['subdomains'])
         self.subdomains.set_index("domainId", inplace=True)
         self.questions = pd.DataFrame(self.data['questions'])
 
@@ -94,15 +94,15 @@
         Args:
             path: The folder to save the images in.
         """
         urllib3.disable_warnings()
 
         if path[-1] not in {'/', '\\'}:
             path += '/'
-        for index, row in self.questions.iterrows():
+        for _index, row in self.questions.iterrows():
             if type(row["exemplarItemImageFile"]) is str:
                 filename = path + row["exemplarItemImageFile"]
                 if not os.path.isfile(filename):
                     img_data = requests.get(row["exemplarItemImageURL"],
                                             verify=False).content
                     with open(filename, 'wb') as handler:
                         handler.write(img_data)
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/vce/__init__.py` & `vicedtools-0.0.8/src/vicedtools/compass/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,9 +8,15 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from vicedtools.vce.vasswebdriver import VASSWebDriver
-from vicedtools.vce.vasssession import VASSSession
+from vicedtools.compass.compassauthenticators import (
+    CompassAuthenticator, CompassAuthenticationError, CompassBasicAuthenticator,
+    CompassCLIAuthenticator)
+from vicedtools.compass.compasssession import (
+    CompassSession, CompassLongRunningFileRequestError, get_report_cycle_id,
+    sanitise_filename)
+
+from vicedtools.compass.reports import Reports, class_code_parser
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/vce/schoolscores.py` & `vicedtools-0.0.8/src/vicedtools/vce/schoolscores.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.7.1/src/vicedtools/vce/vasssession.py` & `vicedtools-0.0.8/src/vicedtools/vce/vasssession.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,91 +11,112 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A requests Session class for exporting data from VASS."""
 
 from __future__ import annotations
 
+from abc import abstractmethod
 from io import StringIO
 import math
 import re
 import requests
 import time
+from typing import Protocol
 import xml.etree.ElementTree as ET
 
 import pandas as pd
 
 
-class VassLoginError(Exception):
-    """Error with vass login."""
-    pass
+class VASSAuthenticator(Protocol):
+    """An abstract class for generic VASS authenticators."""
 
+    @abstractmethod
+    def authenticate(self, session: VASSSession):
+        raise NotImplementedError
 
-class VASSSession(requests.Session):
 
-    def __init__(
-        self,
-        username="",
-        password="",
-        grid_password="",
-    ):
-        """Creates a requests Session with VASS authentication completed.
-    
-        Args:
-            username: The username to login with
-            password: The password to login with
-            grid_password: The grid password to login with. A sequence of
-                tuples, each tuple being the grid coordinate of the next
-                password character. Must be given in top-> bottom, left->
-                right order.
-        
-        Returns:
-            An instance of requests.Session with authentication to
-            VASS completed.
-        """
-        requests.sessions.Session.__init__(self)
+class VASSAuthenticationError(Exception):
+    """Authentication with VASS failed."""
+    pass
 
-        headers = {
-            "User-Agent":
-                "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko",
-            "Accept":
-                "text/html, application/xhtml+xml, image/jxr, */*"
-        }
-        self.headers.update(headers)
 
+class VASSBasicAuthenticator(VASSAuthenticator):
+    """Authenticates using a provided username, password and grid password."""
+
+    def __init__(self, username: str, password: str,
+                 grid_password: list[list[int, int]]):
+        self.username = username
+        self.password = password
+        self.grid_password = grid_password
+
+    def authenticate(self, s: VASSSession):
+        this_year = str(time.localtime().tm_year)
         # username and password login
-        payload = {"Login": "Login", "password": password, "username": username}
+        payload = {
+            "Login": "Login",
+            "password": self.password,
+            "username": self.username
+        }
         submit_login_url = "https://www.vass.vic.edu.au/login/VerifyAuthLogin.cfm"
-        r = self.post(submit_login_url, data=payload)
+        r = s.post(submit_login_url, data=payload)
 
         if "https://www.vass.vic.edu.au/login/schoolcode.cfm" not in r.text:
             # login unsuccessful
-            raise VassLoginError()
+            raise VASSAuthenticationError()
 
         # get passcode grid and login with grid code
         school_code_url = "https://www.vass.vic.edu.au/login/schoolcode.cfm"
-        r = self.get(school_code_url)
+        r = s.get(school_code_url)
 
         pattern = r'passlist="(?P<s>.*?)"'
         m = re.search(pattern, r.text)
         grid_values = m.group('s').split(',')
-        grid_password = [(int(a), int(b)) for (a, b) in grid_password]
+        grid_password = [(int(a), int(b)) for (a, b) in self.grid_password]
         grid_response = "".join(
             [grid_values[(b - 1) * 8 + (a - 1)] for (a, b) in grid_password])
         payload = []
         for value in grid_values:
             payload.append(("PASSCODEGRID", value))
         payload.append(("PassCode", grid_response))
-        payload.append(("Year", "2022"))
+        payload.append(("Year", this_year))
         payload.append(("AcceptButton", "Accept"))
         school_code_submit_url = "https://www.vass.vic.edu.au/login/SchoolCodeAction.cfm"
-        r = self.post(school_code_submit_url, data=payload)
+        r = s.post(school_code_submit_url, data=payload)
         if "https://www.vass.vic.edu.au/menu/Home.cfm" not in r.text:
-            raise VassLoginError()
-        self.year = "2022"
+            raise VASSAuthenticationError()
+        s.year = this_year
+
+
+class VASSSession(requests.Session):
+
+    def __init__(
+        self,
+        authenticator: VASSAuthenticator,
+    ):
+        """Creates a requests Session with VASS authentication completed.
+    
+        Args:
+            authenticator: A VASSAuthenticator instance.
+        
+        Returns:
+            An instance of requests.Session with authentication to
+            VASS completed.
+        """
+        requests.sessions.Session.__init__(self)
+
+        headers = {
+            "User-Agent":
+                "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko",
+            "Accept":
+                "text/html, application/xhtml+xml, image/jxr, */*"
+        }
+        self.headers.update(headers)
+
+        authenticator.authenticate(self)
 
     def change_year(self, year: str) -> None:
         """Changes the year in VASS.
         
         Args:
             year: The year to change to.
         """
@@ -256,15 +277,15 @@
                 for child in root.iter('student'):
                     school_scores.append({**child.attrib, **params})
         if school_scores:
             # convert to a DataFrame and save scores
             df = pd.DataFrame(school_scores)
             subject_names = {}
             unit_names = df["Unit"]
-            pattern = "(?P<code>[A-Z]{2}[0-9]{2})[34] - (?P<name>[A-Z :\(\)]+) [34]"
+            pattern = r"(?P<code>[A-Z]{2}[0-9]{2})[34] - (?P<name>[A-Z :\(\)]+) [34]"
             for unit in unit_names:
                 m = re.match(pattern, unit)
                 if m:
                     subject_names[unit] = m.group('name')
             df["Unit Code"] = df["Unit"].str[:4]
             df["Unit Name"] = df["Unit"].map(subject_names)
             #df.drop(["Unit"], inplace=True)
@@ -705,15 +726,15 @@
     
     :meta private:
     """
     subject_name_pattern = r'>(?P<subject>[A-Za-z :\(\)]+):&nbsp;&nbsp;Student Results by Study'
     m = re.search(subject_name_pattern, response)
     subject = m.group('subject')
     # get student results
-    pattern = '''<tr>\\r\\n(?:\\t)*<td align="left" style="font-weight:normal;width:150px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">&nbsp;(?P<surname>[A-Za-z-']+)<\/td><td align="left" style="font-weight:normal;width:150px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">&nbsp;(?P<firstname>[A-Za-z- ]+)<\/td><td align="center" style="font-weight:normal;width:100px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">(?P<yearlevel>[0-9]+)<\/td><td align="center" style="font-weight:normal;width:100px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">(?P<classgroup>[A-Za-z0-9 ]+)<\/td><td align="center" style="font-size:8pt;font-weight:normal;width:100px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">(?P<achieved>[0-9\.]+)<\/td><td align="center" style="font-size:8pt;font-weight:normal;width:100px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">(?P<predicted>[0-9\.]+|N\/A)<\/td>\\r\\n(?:\\t)*<\/tr>'''
+    pattern = '''<tr>\\r\\n(?:\\t)*<td align="left" style="font-weight:normal;width:150px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">&nbsp;(?P<surname>[A-Za-z- ']+)<\/td><td align="left" style="font-weight:normal;width:150px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">&nbsp;(?P<firstname>[A-Za-z- ]+)<\/td><td align="center" style="font-weight:normal;width:100px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">(?P<yearlevel>[0-9]+)<\/td><td align="center" style="font-weight:normal;width:100px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">(?P<classgroup>[A-Za-z0-9 ]+)<\/td><td align="center" style="font-size:8pt;font-weight:normal;width:100px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">(?P<achieved>[0-9\.]+)<\/td><td align="center" style="font-size:8pt;font-weight:normal;width:100px;BORDER-LEFT: black 1px solid; BORDER-Bottom: black 1px solid; BORDER-Top: black 1px solid; BORDER-RIGHT: black 1px solid;">(?P<predicted>[0-9\.]+|N\/A)<\/td>\\r\\n(?:\\t)*<\/tr>'''
     ms = re.findall(pattern, response)
     new_results = [{
         'Year': year,
         'Subject': subject,
         'Surname': m[0],
         'FirstName': m[1],
         'YearLevel': m[2],
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassacademicgroups.py` & `vicedtools-0.0.8/src/vicedtools/compass/extraauthenticators.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-# Copyright 2021 VicEdTools authors
+# Copyright 2023 VicEdTools authors
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Executable script for exporting Compass academic groups."""
 
-import json
-import sys
-import os
-
-from vicedtools.compass.compasssession import CompassSession, CompassAuthenticator
-
-if __name__ == "__main__":
-    from config import (academic_groups_json, compass_authenticator,
-                        compass_school_code)
-    parent_dir = os.path.dirname(academic_groups_json)
-    if not os.path.exists(parent_dir):
-        os.makedirs(parent_dir)
-
-    s = CompassSession(compass_school_code, compass_authenticator)
-    cycles = s.get_academic_groups()
-    with open(academic_groups_json, "w", encoding='utf-8') as f:
-        json.dump(cycles, f)
+import browser_cookie3
 
-    sys.exit(0)
+from vicedtools.compass import CompassAuthenticator, CompassSession
+
+
+class CompassFirefoxCookieAuthenticator(CompassAuthenticator):
+    """A Compass authenaticator that gets login details from the local Firefox installation."""
+
+    def authenticate(self, s: CompassSession):
+        cj = browser_cookie3.firefox(
+            domain_name=f'{s.school_code}.compass.education')
+
+        for cookie in cj:
+            c = {cookie.name: cookie.value}
+            s.cookies.update(c)
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/workflows/exportcompassreport.py` & `vicedtools-0.0.8/src/vicedtools/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,28 @@
-# Copyright 2021 VicEdTools authors
+# Copyright 2023 VicEdTools authors
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Executable script for exporting Compass reports data."""
 
-from __future__ import annotations
-
-import argparse
-import json
-import os
-
-from vicedtools.compass import CompassSession, get_report_cycle_id
-
-if __name__ == "__main__":
-    from config import (reports_dir, compass_authenticator, compass_school_code,
-                        report_cycles_json)
-
-    parser = argparse.ArgumentParser(
-        description='Export all Compass progress reports.')
-    parser.add_argument('year', type=int, help='the report year')
-    parser.add_argument('title', help='the report title')
-    args = parser.parse_args()
-
-    if not os.path.exists(reports_dir):
-        os.makedirs(reports_dir)
-
-    with open(report_cycles_json, 'r', encoding='utf-8') as f:
-        cycles = json.load(f)
-
-    cycle_id = get_report_cycle_id(cycles, args.year, args.title)
-    s = CompassSession(compass_school_code, compass_authenticator)
-    s.export_reports(cycle_id, args.year, args.title, save_dir=reports_dir)
+from vicedtools.acer import (
+    EWriteSittings, student_imports, OARSSession, OARSAuthenticateError,
+    OARSBasicAuthenticator, OARSCandidate, OARSCandidates, PATItem, PATItems,
+    PATSitting, PATSittings, is_group_report_file, score_categoriser,
+    PATResults, PATResultsCollection, group_reports_to_patresults, OARSTest,
+    OARSTests, item_analysis_plot, item_analysis_plots)
+from vicedtools.compass import (CompassSession, CompassAuthenticationError,
+                                CompassLongRunningFileRequestError,
+                                CompassBasicAuthenticator, Reports)
+from vicedtools.naplan import (DataserviceSession,
+                               DataServiceBasicAuthenticator,
+                               DataserviceAuthenticationError)
+from vicedtools.vce import (VASSBasicAuthenticator, VASSAuthenticationError,
+                            VASSSession)
```

### Comparing `vicedtools-0.0.7.1/src/vicedtools/workflows/exportoarsstaff.py` & `vicedtools-0.0.8/src/vicedtools/acer/extraoarsauthenticators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# Copyright 2021 VicEdTools authors
+# Copyright 2023 VicEdTools authors
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Executable script for exporting staff details from OARS."""
+"""Additional authenticator functions for the OARSSession class."""
 
-import json
-import os
+import browser_cookie3
 
-from vicedtools.acer import OARSSession
+from vicedtools.acer.oarsauthenticators import OARSAuthenticator
+from vicedtools.acer.oarssession import OARSSession
 
-if __name__ == "__main__":
-    from config import (oars_staff_xlsx, oars_authenticator, oars_school_code)
 
-    parent_dir = os.path.dirname(oars_staff_xlsx)
-    if not os.path.exists(parent_dir):
-        os.makedirs(parent_dir)
+class OARSFirefoxCookieAuthenticator(OARSAuthenticator):
+    """An OARS authenticator that gets login details from the local Firefox installation."""
 
-    s = OARSSession(oars_school_code, oars_authenticator)
-    s.get_staff_xlsx(oars_staff_xlsx)
+    def authenticate(self, s: OARSSession):
+        cj = browser_cookie3.firefox(domain_name='oars.acer.edu.au')
+
+        for cookie in cj:
+            c = {cookie.name: cookie.value}
+            s.cookies.update(c)
```

