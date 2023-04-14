# Comparing `tmp/tg_upload-1.0.1-py3-none-any.whl.zip` & `tmp/tg_upload-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 16557 bytes, number of entries: 7
+Zip file size: 16559 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-14 05:05 tg-upload/__init__.py
--rw-rw-rw-  2.0 fat    14058 b- defN 23-Apr-13 17:50 tg-upload/tg-upload.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-14 05:15 tg_upload-1.0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      594 b- defN 23-Apr-14 05:15 tg_upload-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-14 05:15 tg_upload-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-14 05:15 tg_upload-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      555 b- defN 23-Apr-14 05:15 tg_upload-1.0.1.dist-info/RECORD
-7 files, 50458 bytes uncompressed, 15571 bytes compressed:  69.1%
+-rw-rw-rw-  2.0 fat    14058 b- defN 23-Apr-14 05:18 tg-upload/tg-upload.py
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-14 05:22 tg_upload-1.0.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      594 b- defN 23-Apr-14 05:22 tg_upload-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-14 05:22 tg_upload-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-14 05:22 tg_upload-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      555 b- defN 23-Apr-14 05:22 tg_upload-1.0.2.dist-info/RECORD
+7 files, 50458 bytes uncompressed, 15573 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: tg-upload/__init__.py
 Comment: 
 
 Filename: tg-upload/tg-upload.py
 Comment: 
 
-Filename: tg_upload-1.0.1.dist-info/LICENSE.txt
+Filename: tg_upload-1.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: tg_upload-1.0.1.dist-info/METADATA
+Filename: tg_upload-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: tg_upload-1.0.1.dist-info/WHEEL
+Filename: tg_upload-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: tg_upload-1.0.1.dist-info/top_level.txt
+Filename: tg_upload-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tg_upload-1.0.1.dist-info/RECORD
+Filename: tg_upload-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tg-upload/tg-upload.py

```diff
@@ -47,15 +47,15 @@
 parser.add_argument("--recursive", action="store_true", help="Upload files recursively if path is a folder.")
 parser.add_argument("--prefix", help="Add given prefix text to each filename (prefix + filename) before upload.")
 parser.add_argument("--no_warn", action="store_true", help="Don't show warning messages.")
 
 # MISC FLAGS
 parser.add_argument("--device_model", help="Overwrite device model before starting client, by default 'tg-upload', can be anything like your name.")
 parser.add_argument("--system_version", help="Overwrite system version before starting client, by default installed python version, can be anything like 'Windows 11'.")
-parser.add_argument("--version", action="version", help="Display current tg-upload & dependencies version.", version=f"tg-upload: 1.0.1\nPython: {py_ver[0]}.{py_ver[1]}.{py_ver[2]}\nPyrogram: {get_dist('pyrogram').version}\nTgCrypto: {get_dist('tgcrypto').version}")
+parser.add_argument("--version", action="version", help="Display current tg-upload & dependencies version.", version=f"tg-upload: 1.0.2\nPython: {py_ver[0]}.{py_ver[1]}.{py_ver[2]}\nPyrogram: {get_dist('pyrogram').version}\nTgCrypto: {get_dist('tgcrypto').version}")
 args = parser.parse_args()
 
 
 def upload_progress(current,total):
   elapsed_time = time() - start_time
   upload_speed = current / elapsed_time / 1024 / 1024
   print(f"\rUP: [{filename}] - {current/total*100:.2f}% | {upload_speed:.2f}MB/s", end="")
@@ -82,15 +82,15 @@
 if args.phone:
   client = Client(
     args.profile,
     api_id=args.api_id,
     api_hash=args.api_hash,
     phone_number=args.phone,
     hide_password=args.hide_pswd,
-    app_version="1.0.1",
+    app_version="1.0.2",
     device_model=args.device_model or "tg-upload",
     system_version=args.system_version or f"{py_ver[0]}.{py_ver[1]}.{py_ver[2]}"
   )
 elif args.bot:
   client = Client(
     args.profile,
     api_id=args.api_id,
```

## Comparing `tg_upload-1.0.1.dist-info/LICENSE.txt` & `tg_upload-1.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `tg_upload-1.0.1.dist-info/METADATA` & `tg_upload-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-upload
-Version: 1.0.1
+Version: 1.0.2
 Summary: An open-source Python program to upload files/folder to Telegram effortlessly.
 Home-page: https://github.com/TheCaduceus/tg-upload
 Author: Dr.Caduceus
 Author-email: pypi@thecaduceus.eu.org
 Project-URL: Documentation, https://github.com/TheCaduceus/tg-upload#readme
 Project-URL: Source, https://github.com/TheCaduceus/tg-upload
 Project-URL: Tracker, https://github.com/TheCaduceus/tg-upload/issues
```

