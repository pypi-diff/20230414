# Comparing `tmp/gitarootools-0.1.6.tar.gz` & `tmp/gitarootools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitarootools-0.1.6.tar", max compression
+gzip compressed data, was "gitarootools-0.1.7.tar", max compression
```

## Comparing `gitarootools-0.1.6.tar` & `gitarootools-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1148 2020-04-19 09:51:48.000000 gitarootools-0.1.6/LICENSE
--rw-r--r--   0        0        0     1241 2020-04-30 21:03:55.000000 gitarootools-0.1.6/README.md
--rw-r--r--   0        0        0       86 2022-08-08 06:59:32.010948 gitarootools-0.1.6/gitarootools/__init__.py
--rw-r--r--   0        0        0        0 2020-04-27 00:50:59.000000 gitarootools-0.1.6/gitarootools/archive/__init__.py
--rw-r--r--   0        0        0     6238 2023-04-12 05:26:23.575401 gitarootools-0.1.6/gitarootools/archive/pakcontainer.py
--rw-r--r--   0        0        0     4463 2023-04-12 04:10:21.677616 gitarootools-0.1.6/gitarootools/archive/paktoml.py
--rw-r--r--   0        0        0     3142 2023-04-12 05:22:28.649251 gitarootools-0.1.6/gitarootools/archive/xgmcontainer.py
--rw-r--r--   0        0        0     6801 2020-04-27 20:20:16.000000 gitarootools-0.1.6/gitarootools/archive/xgmitem.py
--rw-r--r--   0        0        0     7894 2023-04-10 04:43:31.018329 gitarootools-0.1.6/gitarootools/archive/xgmtoml.py
--rw-r--r--   0        0        0       63 2020-04-19 09:47:08.000000 gitarootools-0.1.6/gitarootools/audio/__init__.py
--rw-r--r--   0        0        0    10947 2023-04-12 05:23:18.615425 gitarootools-0.1.6/gitarootools/audio/imccontainer.py
--rw-r--r--   0        0        0    18977 2020-04-28 19:26:33.000000 gitarootools-0.1.6/gitarootools/audio/imctoml.py
--rw-r--r--   0        0        0    28944 2023-04-12 05:30:24.349667 gitarootools-0.1.6/gitarootools/audio/subsong.py
--rw-r--r--   0        0        0       63 2020-04-19 09:40:53.000000 gitarootools-0.1.6/gitarootools/cmdline/__init__.py
--rw-r--r--   0        0        0     2986 2023-04-13 05:13:35.976581 gitarootools-0.1.6/gitarootools/cmdline/gmo2animnames.py
--rw-r--r--   0        0        0     4156 2020-04-28 19:18:13.000000 gitarootools-0.1.6/gitarootools/cmdline/imcpack.py
--rw-r--r--   0        0        0     4286 2020-04-28 19:26:33.000000 gitarootools-0.1.6/gitarootools/cmdline/imcunpack.py
--rw-r--r--   0        0        0     3362 2022-08-08 05:14:21.786361 gitarootools-0.1.6/gitarootools/cmdline/imx2png.py
--rw-r--r--   0        0        0     4132 2023-04-12 03:41:12.325154 gitarootools-0.1.6/gitarootools/cmdline/pakpack.py
--rw-r--r--   0        0        0     4846 2023-04-12 03:37:25.211594 gitarootools-0.1.6/gitarootools/cmdline/pakunpack.py
--rw-r--r--   0        0        0     4921 2021-01-18 04:02:54.689117 gitarootools-0.1.6/gitarootools/cmdline/png2imx.py
--rw-r--r--   0        0        0     3998 2020-04-28 19:28:46.000000 gitarootools-0.1.6/gitarootools/cmdline/subsong2common.py
--rw-r--r--   0        0        0      408 2020-04-19 09:50:28.000000 gitarootools-0.1.6/gitarootools/cmdline/subsong2subimc.py
--rw-r--r--   0        0        0      398 2020-04-19 09:50:28.000000 gitarootools-0.1.6/gitarootools/cmdline/subsong2wav.py
--rw-r--r--   0        0        0     1539 2020-04-19 09:50:28.000000 gitarootools-0.1.6/gitarootools/cmdline/subsongconv.py
--rw-r--r--   0        0        0     4149 2020-04-28 19:18:13.000000 gitarootools-0.1.6/gitarootools/cmdline/xgmpack.py
--rw-r--r--   0        0        0     4074 2023-04-12 04:16:46.510728 gitarootools-0.1.6/gitarootools/cmdline/xgmunpack.py
--rw-r--r--   0        0        0        0 2020-04-29 19:36:52.000000 gitarootools-0.1.6/gitarootools/image/__init__.py
--rw-r--r--   0        0        0    17764 2023-04-12 04:56:23.341827 gitarootools-0.1.6/gitarootools/image/imximage.py
--rw-r--r--   0        0        0       63 2020-04-19 09:47:08.000000 gitarootools-0.1.6/gitarootools/miscutils/__init__.py
--rw-r--r--   0        0        0     5011 2021-01-25 04:11:23.223912 gitarootools-0.1.6/gitarootools/miscutils/cmdutils.py
--rw-r--r--   0        0        0     6391 2023-04-12 04:45:21.484101 gitarootools-0.1.6/gitarootools/miscutils/datautils.py
--rw-r--r--   0        0        0     4413 2023-04-12 00:50:22.767259 gitarootools-0.1.6/gitarootools/miscutils/extutils.py
--rw-r--r--   0        0        0       63 2023-04-13 02:58:32.253643 gitarootools-0.1.6/gitarootools/other/__init__.py
--rw-r--r--   0        0        0     1826 2023-04-13 05:13:20.716138 gitarootools-0.1.6/gitarootools/other/gmomodel.py
--rw-r--r--   0        0        0     1143 2023-04-13 05:16:32.873794 gitarootools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 gitarootools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1148 2020-04-19 09:51:48.000000 gitarootools-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1484 2023-04-13 05:37:14.239121 gitarootools-0.1.7/README.md
+-rw-r--r--   0        0        0       86 2023-04-13 05:30:54.589070 gitarootools-0.1.7/gitarootools/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-27 00:50:59.000000 gitarootools-0.1.7/gitarootools/archive/__init__.py
+-rw-r--r--   0        0        0     6238 2023-04-12 05:26:23.575401 gitarootools-0.1.7/gitarootools/archive/pakcontainer.py
+-rw-r--r--   0        0        0     4463 2023-04-12 04:10:21.677616 gitarootools-0.1.7/gitarootools/archive/paktoml.py
+-rw-r--r--   0        0        0     3142 2023-04-12 05:22:28.649251 gitarootools-0.1.7/gitarootools/archive/xgmcontainer.py
+-rw-r--r--   0        0        0     6801 2020-04-27 20:20:16.000000 gitarootools-0.1.7/gitarootools/archive/xgmitem.py
+-rw-r--r--   0        0        0     7894 2023-04-10 04:43:31.018329 gitarootools-0.1.7/gitarootools/archive/xgmtoml.py
+-rw-r--r--   0        0        0       63 2020-04-19 09:47:08.000000 gitarootools-0.1.7/gitarootools/audio/__init__.py
+-rw-r--r--   0        0        0    10947 2023-04-12 05:23:18.615425 gitarootools-0.1.7/gitarootools/audio/imccontainer.py
+-rw-r--r--   0        0        0    18977 2020-04-28 19:26:33.000000 gitarootools-0.1.7/gitarootools/audio/imctoml.py
+-rw-r--r--   0        0        0    28944 2023-04-12 05:30:24.349667 gitarootools-0.1.7/gitarootools/audio/subsong.py
+-rw-r--r--   0        0        0       63 2020-04-19 09:40:53.000000 gitarootools-0.1.7/gitarootools/cmdline/__init__.py
+-rw-r--r--   0        0        0     2986 2023-04-13 05:13:35.976581 gitarootools-0.1.7/gitarootools/cmdline/gmo2animnames.py
+-rw-r--r--   0        0        0     4156 2020-04-28 19:18:13.000000 gitarootools-0.1.7/gitarootools/cmdline/imcpack.py
+-rw-r--r--   0        0        0     4286 2020-04-28 19:26:33.000000 gitarootools-0.1.7/gitarootools/cmdline/imcunpack.py
+-rw-r--r--   0        0        0     3362 2022-08-08 05:14:21.786361 gitarootools-0.1.7/gitarootools/cmdline/imx2png.py
+-rw-r--r--   0        0        0     4132 2023-04-12 03:41:12.325154 gitarootools-0.1.7/gitarootools/cmdline/pakpack.py
+-rw-r--r--   0        0        0     4854 2023-04-13 22:50:21.896371 gitarootools-0.1.7/gitarootools/cmdline/pakunpack.py
+-rw-r--r--   0        0        0     4921 2021-01-18 04:02:54.689117 gitarootools-0.1.7/gitarootools/cmdline/png2imx.py
+-rw-r--r--   0        0        0     3998 2020-04-28 19:28:46.000000 gitarootools-0.1.7/gitarootools/cmdline/subsong2common.py
+-rw-r--r--   0        0        0      408 2020-04-19 09:50:28.000000 gitarootools-0.1.7/gitarootools/cmdline/subsong2subimc.py
+-rw-r--r--   0        0        0      398 2020-04-19 09:50:28.000000 gitarootools-0.1.7/gitarootools/cmdline/subsong2wav.py
+-rw-r--r--   0        0        0     1539 2020-04-19 09:50:28.000000 gitarootools-0.1.7/gitarootools/cmdline/subsongconv.py
+-rw-r--r--   0        0        0     4149 2020-04-28 19:18:13.000000 gitarootools-0.1.7/gitarootools/cmdline/xgmpack.py
+-rw-r--r--   0        0        0     4074 2023-04-12 04:16:46.510728 gitarootools-0.1.7/gitarootools/cmdline/xgmunpack.py
+-rw-r--r--   0        0        0        0 2020-04-29 19:36:52.000000 gitarootools-0.1.7/gitarootools/image/__init__.py
+-rw-r--r--   0        0        0    17764 2023-04-12 04:56:23.341827 gitarootools-0.1.7/gitarootools/image/imximage.py
+-rw-r--r--   0        0        0       63 2020-04-19 09:47:08.000000 gitarootools-0.1.7/gitarootools/miscutils/__init__.py
+-rw-r--r--   0        0        0     5011 2021-01-25 04:11:23.223912 gitarootools-0.1.7/gitarootools/miscutils/cmdutils.py
+-rw-r--r--   0        0        0     6391 2023-04-12 04:45:21.484101 gitarootools-0.1.7/gitarootools/miscutils/datautils.py
+-rw-r--r--   0        0        0     4413 2023-04-12 00:50:22.767259 gitarootools-0.1.7/gitarootools/miscutils/extutils.py
+-rw-r--r--   0        0        0       63 2023-04-13 02:58:32.253643 gitarootools-0.1.7/gitarootools/other/__init__.py
+-rw-r--r--   0        0        0     1826 2023-04-13 05:13:20.716138 gitarootools-0.1.7/gitarootools/other/gmomodel.py
+-rw-r--r--   0        0        0     1143 2023-04-13 05:30:08.090678 gitarootools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 gitarootools-0.1.7/PKG-INFO
```

### Comparing `gitarootools-0.1.6/LICENSE` & `gitarootools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/README.md` & `gitarootools-0.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 ## Included tools
 ### Archive
 
 **`gm-xgmpack`**: pack files into an XGM container
 
 **`gm-xgmunpack`**: unpack files from an XGM container
 
+**`gm-pakpack`**: pack files into a PAK container (Gitaroo Man Lives)
+
+**`gm-pakunpack`**: unpack files from a PAK container (Gitaroo Man Lives)
+
 ### Audio
 
 **`gm-imcpack`**: pack subsongs into an IMC audio container
 
 **`gm-imcunpack`**: unpack subsongs from an IMC audio container
 
 **`gm-subsongconv`**: convert a subsong to another format
@@ -36,10 +40,14 @@
 
 ### Image
 
 **`gm-imx2png`**: convert IMX images to PNG
 
 **`gm-png2imx`**: convert PNG images to IMX
 
+### Other
+
+**`gm-gmo2animnames`**: extract animation names from a GMO model (Gitaroo Man Lives)
+
 ## Resources
 * [Gitaroo Pals](https://discord.gg/ed6P8Jt) Discord server for help and support
 * [Issue Tracker](https://github.com/boringhexi/gitarootools/issues)
```

### Comparing `gitarootools-0.1.6/gitarootools/archive/pakcontainer.py` & `gitarootools-0.1.7/gitarootools/archive/pakcontainer.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/archive/paktoml.py` & `gitarootools-0.1.7/gitarootools/archive/paktoml.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/archive/xgmcontainer.py` & `gitarootools-0.1.7/gitarootools/archive/xgmcontainer.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/archive/xgmitem.py` & `gitarootools-0.1.7/gitarootools/archive/xgmitem.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/archive/xgmtoml.py` & `gitarootools-0.1.7/gitarootools/archive/xgmtoml.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/audio/imccontainer.py` & `gitarootools-0.1.7/gitarootools/audio/imccontainer.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/audio/imctoml.py` & `gitarootools-0.1.7/gitarootools/audio/imctoml.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/audio/subsong.py` & `gitarootools-0.1.7/gitarootools/audio/subsong.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/gmo2animnames.py` & `gitarootools-0.1.7/gitarootools/cmdline/gmo2animnames.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/imcpack.py` & `gitarootools-0.1.7/gitarootools/cmdline/imcpack.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/imcunpack.py` & `gitarootools-0.1.7/gitarootools/cmdline/imcunpack.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/imx2png.py` & `gitarootools-0.1.7/gitarootools/cmdline/imx2png.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/pakpack.py` & `gitarootools-0.1.7/gitarootools/cmdline/pakpack.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/pakunpack.py` & `gitarootools-0.1.7/gitarootools/cmdline/pakunpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             outer_dir, f"{namebase}{suf}_PAK"  # outer/file_suf_PAK/
         )
         output_tomlbase = f"{namebase}{suf}{PAKTOML_EXT}"  # file_suf.PAK.toml
 
         # unpack PAK container file
         if parsed_args.verbose:
             print(f"unpacking {inpath!r} -> {output_dirpath!r}")
-        pakc = read_pak(inpath, ssqfile=ssqpath)
+        pakc = read_pak(inpath, ssqfile_or_path=ssqpath)
         write_pak_to_toml(
             pakc, output_dirpath, output_tomlbase, progressfunc=verbosefunc,
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/png2imx.py` & `gitarootools-0.1.7/gitarootools/cmdline/png2imx.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/subsong2common.py` & `gitarootools-0.1.7/gitarootools/cmdline/subsong2common.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/subsongconv.py` & `gitarootools-0.1.7/gitarootools/cmdline/subsongconv.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/xgmpack.py` & `gitarootools-0.1.7/gitarootools/cmdline/xgmpack.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/cmdline/xgmunpack.py` & `gitarootools-0.1.7/gitarootools/cmdline/xgmunpack.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/image/imximage.py` & `gitarootools-0.1.7/gitarootools/image/imximage.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/miscutils/cmdutils.py` & `gitarootools-0.1.7/gitarootools/miscutils/cmdutils.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/miscutils/datautils.py` & `gitarootools-0.1.7/gitarootools/miscutils/datautils.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/miscutils/extutils.py` & `gitarootools-0.1.7/gitarootools/miscutils/extutils.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/gitarootools/other/gmomodel.py` & `gitarootools-0.1.7/gitarootools/other/gmomodel.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.6/pyproject.toml` & `gitarootools-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitarootools"
-version = "0.1.6"
+version = "0.1.7"
 description = "command line tools to work with Gitaroo Man game data"
 license = "MIT"
 authors = ["boringhexi <boringhexi@pm.me>"]
 readme = "README.md"
 repository = "https://github.com/boringhexi/gitarootools"
 
 [tool.poetry.dependencies]
```

### Comparing `gitarootools-0.1.6/PKG-INFO` & `gitarootools-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitarootools
-Version: 0.1.6
+Version: 0.1.7
 Summary: command line tools to work with Gitaroo Man game data
 Home-page: https://github.com/boringhexi/gitarootools
 License: MIT
 Author: boringhexi
 Author-email: boringhexi@pm.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,18 @@
 ## Included tools
 ### Archive
 
 **`gm-xgmpack`**: pack files into an XGM container
 
 **`gm-xgmunpack`**: unpack files from an XGM container
 
+**`gm-pakpack`**: pack files into a PAK container (Gitaroo Man Lives)
+
+**`gm-pakunpack`**: unpack files from a PAK container (Gitaroo Man Lives)
+
 ### Audio
 
 **`gm-imcpack`**: pack subsongs into an IMC audio container
 
 **`gm-imcunpack`**: unpack subsongs from an IMC audio container
 
 **`gm-subsongconv`**: convert a subsong to another format
@@ -57,10 +61,14 @@
 
 ### Image
 
 **`gm-imx2png`**: convert IMX images to PNG
 
 **`gm-png2imx`**: convert PNG images to IMX
 
+### Other
+
+**`gm-gmo2animnames`**: extract animation names from a GMO model (Gitaroo Man Lives)
+
 ## Resources
 * [Gitaroo Pals](https://discord.gg/ed6P8Jt) Discord server for help and support
 * [Issue Tracker](https://github.com/boringhexi/gitarootools/issues)
```

