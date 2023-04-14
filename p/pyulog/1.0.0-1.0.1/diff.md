# Comparing `tmp/pyulog-1.0.0.tar.gz` & `tmp/pyulog-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyulog-1.0.0.tar", last modified: Tue Oct  4 08:39:08 2022, max compression
+gzip compressed data, was "pyulog-1.0.1.tar", last modified: Fri Apr 14 18:40:23 2023, max compression
```

## Comparing `pyulog-1.0.0.tar` & `pyulog-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2022-10-04 08:39:08.521279 pyulog-1.0.0/
--rw-rw-r--   0 beat      (1000) beat      (1000)     1492 2016-07-03 18:43:02.000000 pyulog-1.0.0/LICENSE.md
--rw-r--r--   0 beat      (1000) beat      (1000)       99 2022-10-04 08:35:35.000000 pyulog-1.0.0/MANIFEST.in
--rw-r--r--   0 beat      (1000) beat      (1000)     1335 2022-10-04 08:39:08.521279 pyulog-1.0.0/PKG-INFO
--rw-r--r--   0 beat      (1000) beat      (1000)     7502 2022-10-04 08:35:35.000000 pyulog-1.0.0/README.md
-drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2022-10-04 08:39:08.521279 pyulog-1.0.0/pyulog/
--rw-rw-r--   0 beat      (1000) beat      (1000)      209 2017-01-26 07:47:44.000000 pyulog-1.0.0/pyulog/__init__.py
--rw-r--r--   0 beat      (1000) beat      (1000)      497 2022-10-04 08:39:08.521279 pyulog-1.0.0/pyulog/_version.py
--rw-r--r--   0 beat      (1000) beat      (1000)    47500 2022-10-04 08:35:35.000000 pyulog-1.0.0/pyulog/core.py
--rw-r--r--   0 beat      (1000) beat      (1000)    24606 2022-10-04 08:35:35.000000 pyulog-1.0.0/pyulog/db.py
--rw-rw-r--   0 beat      (1000) beat      (1000)     3581 2020-12-08 08:37:00.000000 pyulog-1.0.0/pyulog/extract_gps_dump.py
--rw-r--r--   0 beat      (1000) beat      (1000)     4345 2022-10-04 08:35:35.000000 pyulog-1.0.0/pyulog/info.py
--rw-rw-r--   0 beat      (1000) beat      (1000)     1023 2022-04-29 08:52:38.000000 pyulog-1.0.0/pyulog/messages.py
--rw-r--r--   0 beat      (1000) beat      (1000)     6149 2022-10-04 08:35:35.000000 pyulog-1.0.0/pyulog/migrate_db.py
--rw-r--r--   0 beat      (1000) beat      (1000)     5612 2021-03-15 07:18:46.000000 pyulog-1.0.0/pyulog/params.py
--rw-rw-r--   0 beat      (1000) beat      (1000)     4257 2019-06-07 05:44:53.000000 pyulog-1.0.0/pyulog/px4.py
-drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2022-10-04 08:39:08.520280 pyulog-1.0.0/pyulog/sql/
--rw-r--r--   0 beat      (1000) beat      (1000)     3017 2022-10-04 08:35:35.000000 pyulog-1.0.0/pyulog/sql/pyulog.1.sql
--rw-r--r--   0 beat      (1000) beat      (1000)     3507 2022-05-03 05:53:52.000000 pyulog-1.0.0/pyulog/ulog2csv.py
--rw-rw-r--   0 beat      (1000) beat      (1000)     8646 2020-06-29 12:14:23.000000 pyulog-1.0.0/pyulog/ulog2kml.py
--rw-r--r--   0 beat      (1000) beat      (1000)     3473 2022-05-03 05:53:52.000000 pyulog-1.0.0/pyulog/ulog2rosbag.py
-drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2022-10-04 08:39:08.519279 pyulog-1.0.0/pyulog.egg-info/
--rw-r--r--   0 beat      (1000) beat      (1000)     1335 2022-10-04 08:39:08.000000 pyulog-1.0.0/pyulog.egg-info/PKG-INFO
--rw-r--r--   0 beat      (1000) beat      (1000)      612 2022-10-04 08:39:08.000000 pyulog-1.0.0/pyulog.egg-info/SOURCES.txt
--rw-r--r--   0 beat      (1000) beat      (1000)        1 2022-10-04 08:39:08.000000 pyulog-1.0.0/pyulog.egg-info/dependency_links.txt
--rw-r--r--   0 beat      (1000) beat      (1000)      312 2022-10-04 08:39:08.000000 pyulog-1.0.0/pyulog.egg-info/entry_points.txt
--rw-r--r--   0 beat      (1000) beat      (1000)        6 2022-10-04 08:39:08.000000 pyulog-1.0.0/pyulog.egg-info/requires.txt
--rw-r--r--   0 beat      (1000) beat      (1000)       12 2022-10-04 08:39:08.000000 pyulog-1.0.0/pyulog.egg-info/top_level.txt
--rw-rw-r--   0 beat      (1000) beat      (1000)      198 2022-10-04 08:39:08.521279 pyulog-1.0.0/setup.cfg
--rw-r--r--   0 beat      (1000) beat      (1000)     2168 2022-10-04 08:35:35.000000 pyulog-1.0.0/setup.py
-drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2022-10-04 08:39:08.520280 pyulog-1.0.0/test/
--rw-rw-r--   0 beat      (1000) beat      (1000)        0 2016-11-14 08:05:31.000000 pyulog-1.0.0/test/__init__.py
--rw-r--r--   0 beat      (1000) beat      (1000)     4024 2022-10-04 08:35:35.000000 pyulog-1.0.0/test/test_db.py
--rw-r--r--   0 beat      (1000) beat      (1000)     7214 2022-10-04 08:35:35.000000 pyulog-1.0.0/test/test_migration.py
--rw-rw-r--   0 beat      (1000) beat      (1000)     2665 2022-05-02 07:53:18.000000 pyulog-1.0.0/test/test_ulog2csv.py
--rw-r--r--   0 beat      (1000) beat      (1000)     2494 2022-05-03 06:01:37.000000 pyulog-1.0.0/test/test_ulog_write.py
--rw-rw-r--   0 beat      (1000) beat      (1000)    70144 2021-03-15 08:29:44.000000 pyulog-1.0.0/versioneer.py
+drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2023-04-14 18:40:23.211211 pyulog-1.0.1/
+-rw-rw-r--   0 beat      (1000) beat      (1000)     1492 2016-07-03 18:43:02.000000 pyulog-1.0.1/LICENSE.md
+-rw-r--r--   0 beat      (1000) beat      (1000)       99 2022-10-04 08:35:35.000000 pyulog-1.0.1/MANIFEST.in
+-rw-r--r--   0 beat      (1000) beat      (1000)     1335 2023-04-14 18:40:23.211211 pyulog-1.0.1/PKG-INFO
+-rw-r--r--   0 beat      (1000) beat      (1000)     7742 2023-04-14 11:45:26.000000 pyulog-1.0.1/README.md
+drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2023-04-14 18:40:23.212211 pyulog-1.0.1/pyulog/
+-rw-rw-r--   0 beat      (1000) beat      (1000)      209 2017-01-26 07:47:44.000000 pyulog-1.0.1/pyulog/__init__.py
+-rw-r--r--   0 beat      (1000) beat      (1000)      497 2023-04-14 18:40:23.212211 pyulog-1.0.1/pyulog/_version.py
+-rw-r--r--   0 beat      (1000) beat      (1000)    47590 2023-04-14 18:38:44.000000 pyulog-1.0.1/pyulog/core.py
+-rw-r--r--   0 beat      (1000) beat      (1000)    29229 2023-04-14 11:45:26.000000 pyulog-1.0.1/pyulog/db.py
+-rw-rw-r--   0 beat      (1000) beat      (1000)     3581 2020-12-08 08:37:00.000000 pyulog-1.0.1/pyulog/extract_gps_dump.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     4345 2023-04-10 18:47:09.000000 pyulog-1.0.1/pyulog/info.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     1023 2023-03-23 13:31:26.000000 pyulog-1.0.1/pyulog/messages.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     6149 2022-10-04 08:35:35.000000 pyulog-1.0.1/pyulog/migrate_db.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     5613 2023-04-14 11:45:26.000000 pyulog-1.0.1/pyulog/params.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     4488 2023-04-14 11:45:26.000000 pyulog-1.0.1/pyulog/px4.py
+drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2023-04-14 18:40:23.210210 pyulog-1.0.1/pyulog/sql/
+-rw-r--r--   0 beat      (1000) beat      (1000)     3017 2022-10-04 08:35:35.000000 pyulog-1.0.1/pyulog/sql/pyulog.1.sql
+-rw-r--r--   0 beat      (1000) beat      (1000)     6660 2023-04-14 11:45:26.000000 pyulog-1.0.1/pyulog/sql/pyulog.2.sql
+-rw-r--r--   0 beat      (1000) beat      (1000)       64 2023-04-14 11:45:26.000000 pyulog-1.0.1/pyulog/sql/pyulog.3.sql
+-rw-r--r--   0 beat      (1000) beat      (1000)     4451 2023-04-14 11:45:29.000000 pyulog-1.0.1/pyulog/ulog2csv.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     8645 2023-04-14 11:45:26.000000 pyulog-1.0.1/pyulog/ulog2kml.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     3473 2022-05-03 05:53:52.000000 pyulog-1.0.1/pyulog/ulog2rosbag.py
+drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2023-04-14 18:40:23.210210 pyulog-1.0.1/pyulog.egg-info/
+-rw-r--r--   0 beat      (1000) beat      (1000)     1335 2023-04-14 18:40:23.000000 pyulog-1.0.1/pyulog.egg-info/PKG-INFO
+-rw-r--r--   0 beat      (1000) beat      (1000)      660 2023-04-14 18:40:23.000000 pyulog-1.0.1/pyulog.egg-info/SOURCES.txt
+-rw-r--r--   0 beat      (1000) beat      (1000)        1 2023-04-14 18:40:23.000000 pyulog-1.0.1/pyulog.egg-info/dependency_links.txt
+-rw-r--r--   0 beat      (1000) beat      (1000)      312 2023-04-14 18:40:23.000000 pyulog-1.0.1/pyulog.egg-info/entry_points.txt
+-rw-r--r--   0 beat      (1000) beat      (1000)        6 2023-04-14 18:40:23.000000 pyulog-1.0.1/pyulog.egg-info/requires.txt
+-rw-r--r--   0 beat      (1000) beat      (1000)       12 2023-04-14 18:40:23.000000 pyulog-1.0.1/pyulog.egg-info/top_level.txt
+-rw-rw-r--   0 beat      (1000) beat      (1000)      198 2023-04-14 18:40:23.212211 pyulog-1.0.1/setup.cfg
+-rw-r--r--   0 beat      (1000) beat      (1000)     2168 2022-10-04 08:35:35.000000 pyulog-1.0.1/setup.py
+drwxr-xr-x   0 beat      (1000) beat      (1000)        0 2023-04-14 18:40:23.211211 pyulog-1.0.1/test/
+-rw-rw-r--   0 beat      (1000) beat      (1000)        0 2016-11-14 08:05:31.000000 pyulog-1.0.1/test/__init__.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     8018 2023-04-14 11:45:26.000000 pyulog-1.0.1/test/test_db.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     7214 2022-10-04 08:35:35.000000 pyulog-1.0.1/test/test_migration.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     2719 2023-02-22 12:47:16.000000 pyulog-1.0.1/test/test_ulog2csv.py
+-rw-r--r--   0 beat      (1000) beat      (1000)     2494 2022-05-03 06:01:37.000000 pyulog-1.0.1/test/test_ulog_write.py
+-rw-rw-r--   0 beat      (1000) beat      (1000)    70144 2021-03-15 08:29:44.000000 pyulog-1.0.1/versioneer.py
```

### Comparing `pyulog-1.0.0/LICENSE.md` & `pyulog-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/PKG-INFO` & `pyulog-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyulog
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python log parser for ULog.
 Home-page: https://github.com/PX4/pyulog
 Download-URL: https://github.com/PX4/pyulog
 Author: Beat Kueng
 Author-email: beat-kueng@gmx.net
 Maintainer: James Goppert
 Maintainer-email: james.goppert@gmail.com
```

### Comparing `pyulog-1.0.0/README.md` & `pyulog-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -231,19 +231,24 @@
   -m MESSAGES, --messages MESSAGES
                         Only consider given messages. Must be a comma-
                         separated list of names, like
                         'sensor_combined,vehicle_gps_position'
 ```
 ### Migrate/setup the database for use with the DatabaseULog class (ulog_migratedb)
 
+> **Warning** This command must be run whenever the schema changes, otherwise DatabaseULog won't function.
+
+> **Warning** Even if you store logs in the database, you should keep the original .ulg files. Otherwise you may lose your data.
+
+
 Usage:
 ```
 usage: ulog_migratedb [-h] [-d DB_PATH] [-n] [-s SQL_DIR] [-f]
 
-Setup the database for DatabaseULog
+Setup the database for DatabaseULog.
 
 optional arguments:
   -h, --help            show this help message and exit
   -d DB_PATH, --database DB_PATH
                         Path to the database file
   -n, --noop            Only print results, do not execute migration scripts.
   -s SQL_DIR, --sql SQL_DIR
```

### Comparing `pyulog-1.0.0/pyulog/core.py` & `pyulog-1.0.1/pyulog/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
 
     def _write_file_header(self, file):
         header_data = bytearray()
         header_data.extend(self.HEADER_BYTES)
         header_data.extend(struct.pack('B', self._file_version))
         header_data.extend(struct.pack('<Q', self._start_timestamp))
         if len(header_data) != 16:
-            raise Exception("Written header is too short")
+            raise TypeError("Written header is too short")
 
         file.write(header_data)
 
     def _write_flags(self, file):
         data = bytearray()
         data.extend(struct.pack('<' + 'B' * 8, *self._compat_flags))
 
@@ -331,15 +331,15 @@
 
     def _make_parameter_data(self, name: str, value) -> bytes:
         if isinstance(value, int):
             value_type = "int32_t"
         elif isinstance(value, float):
             value_type = "float"
         else:
-            raise Exception("Found unknown parameter value type")
+            raise TypeError("Found unknown parameter value type")
 
         key: str = value_type + ' ' + name
 
         return self._make_info_message_data(key, value, value_type)
 
     def _make_info_message_data(self, key: str, value, value_type: str, continued=None) -> bytes:
         key_bytes = bytes(key, 'utf-8')
@@ -350,14 +350,16 @@
 
         data.extend(struct.pack('<B', len(key_bytes)))
         data.extend(key_bytes)
 
         if value_type.startswith('char['):
             value_bytes = bytes(value, 'utf-8')
             data.extend(value_bytes)
+        elif value_type.startswith('uint8_t['):
+            data.extend(value)
         else:
             code = self._UNPACK_TYPES[value_type][0]
             data.extend(struct.pack('<' + code, value))
 
         return data
 
     def _write_format_messages(self, file):
@@ -837,17 +839,17 @@
 
         self._file_handle.close()
         del self._file_handle
 
     def _read_file_header(self):
         header_data = self._file_handle.read(16)
         if len(header_data) != 16:
-            raise Exception("Invalid file format (Header too short)")
+            raise TypeError("Invalid file format (Header too short)")
         if header_data[:7] != self.HEADER_BYTES:
-            raise Exception("Invalid file format (Failed to parse header)")
+            raise TypeError("Invalid file format (Failed to parse header)")
         self._file_version, = struct.unpack('B', header_data[7:8])
         if self._file_version > 1:
             print("Warning: unknown file version. Will attempt to read it anyway")
 
         # read timestamp
         self._start_timestamp, = ULog._unpack_uint64(header_data[8:])
 
@@ -894,18 +896,18 @@
                         print('incompat flags:', self._incompat_flags)
                         print('appended offsets:', self._appended_offsets)
 
                     # check if there are bits set that we don't know
                     unknown_incompat_flag_msg = \
                     "Unknown incompatible flag set: cannot parse the log"
                     if self._incompat_flags[0] & ~1:
-                        raise Exception(unknown_incompat_flag_msg)
+                        raise ValueError(unknown_incompat_flag_msg)
                     for i in range(1, 8):
                         if self._incompat_flags[i]:
-                            raise Exception(unknown_incompat_flag_msg)
+                            raise NotImplementedError(unknown_incompat_flag_msg)
 
                 else:
                     if self._debug:
                         print('read_file_definitions: unknown message type: %i (%s)' %
                               (header.msg_type, chr(header.msg_type)))
                         file_position = self._file_handle.tell()
                         print('file position: %i (0x%x) msg size: %i' % (
```

### Comparing `pyulog-1.0.0/pyulog/db.py` & `pyulog-1.0.1/pyulog/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,74 @@
 '''
 Module containing the DatabaseULog class.
 '''
 
 import sqlite3
+import hashlib
 import contextlib
 import numpy as np
 from pyulog import ULog
 
 # pylint: disable=too-many-instance-attributes
 class DatabaseULog(ULog):
     '''
     This class can be used in place of a ULog, except that it reads from and
     writes to a sqlite3 database instead of a file.
 
     The first time you see a ulog file, instantiate a DatabaseULog directly
     from a ulog file, and then call save() to write it to the database. Later
     it can be accessed by providing the primary_key, upon which this class
-    loads all needed fields from the database.
+    loads all needed fields from the database. If you don't have the
+    primary_key value available, but you have the .ulg file and know it is in
+    the database, you can retrieve the hash with DatabaseULog.calc_sha256sum
+    and DatabaseULog.primary_key_from_sha256sum.
 
     This class is currently designed to be write-once only, so you cannot
-    update existing database entries. This could and should be changed in the
-    future.
+    update existing database entries. To do so, first call delete() and then
+    save() again.
 
     A weakness of the implementation is that there are some silently failing
     states if you don't call save() immediately after instantiating from a ULog
     object. The requirement of explicit save() is to prevent unexpected, sudden
     side effects, which is considered worse than the current solution.
 
     Example usage:
     > from pyulog.db import DatabaseULog
     >
     > db_handle = DatabaseULog.get_db_handle('dbulog.sqlite3')
     > dbulog = DatabaseULog(db_handle, log_file='example.ulg') # Slow
-    > pk = dbulog.save()
+    > dbulog.save()
+    > pk = dbulog.primary_key()
     > # [...]
     > dbulog = DatabaseULog(db_handle, primary_key=pk) # Fast
 
     SCHEMA_VERSION specifies which version of the database schema (as read from
     "PRAGMA user_version") this file is supposed to match. This is done to
     ensure consistency between the database operations and the state of the
     database. If SCHEMA_VERSION is higher than what is found in the database,
     then it means that the datbaase is has not been updated, and the
     contsructor will throw an exception. See the documentation of
     "ulog_migratedb" for more information.
     '''
-    SCHEMA_VERSION = 1
+    SCHEMA_VERSION = 3
 
     @staticmethod
     def get_db_handle(db_path):
         '''
         Generate a database handle that can be used in subsequent database access.
         '''
         def db_handle():
-            return sqlite3.connect(
+            con = sqlite3.connect(
                 db_path,
                 detect_types=sqlite3.PARSE_DECLTYPES|sqlite3.PARSE_COLNAMES
             )
+            # The next line is necessary for sqlite3 to actually respect
+            # FOREIGN KEY constraints and ON DELETE CASCADE.
+            con.execute('PRAGMA foreign_keys=on')
+            return con
         return db_handle
 
     @staticmethod
     def exists_in_db(db_handle, primary_key):
         '''
         Check whether an ULog row with Id=primary_key exists in the database
         accessed with db_handle.
@@ -73,23 +82,68 @@
                 WHERE Id = ?
                 ''', (primary_key,))
             count, = cur.fetchone()
             cur.close()
 
             return count == 1
 
+    @staticmethod
+    def primary_key_from_sha256sum(db_handle, sha256sum):
+        '''
+        Search the database for a row with the given SHA256 digest and returns
+        the corresponding primary key. Returns None if not found.
+        '''
+        primary_key = None
+        with db_handle() as con:
+            cur = con.cursor()
+            cur.execute('''
+                SELECT Id
+                FROM ULog
+                WHERE SHA256Sum = ?
+                ''', (sha256sum,))
+            row = cur.fetchone()
+            if row:
+                primary_key = row[0]
+            cur.close()
+        return primary_key
+
+    @staticmethod
+    def calc_sha256sum(log_file):
+        '''
+        Compute the SHA256 digest of a file, specified as a file or a valid file path.
+        '''
+        if log_file is None:
+            return None
+        if isinstance(log_file, str):
+            log_file = open(log_file, 'rb') # pylint: disable=consider-using-with
+            log_context = log_file
+        else:
+            log_context = contextlib.nullcontext()
+
+        file_hash = hashlib.sha256()
+        with log_context:
+            while True:
+                block = log_file.read(4096)
+                file_hash.update(block)
+                if block == b'':
+                    break
+        return file_hash.hexdigest()
+
+
     def __init__(self, db_handle, primary_key=None, log_file=None, lazy=True, **kwargs):
         '''
         You always need the database handle (which can be generated with
         DatabaseULog.get_db_handle), but there are two options for the
         parameters "primary_key" and "log_file":
         - For storing a new log in the database, supply the corresponding
           log_file parameter, but leave the primary_key field at None.
         - For reading an existing log from the database, supply the desired
-          primary_key parameter, but leave the log_file parameter at None.
+          primary_key parameter, but leave the log_file parameter at None. If
+          you don't know the primary_key, you can try finding it with
+          DatabaseULog.primary_key_from_sha256sum.
         You cannot supply both of these parameters.
 
         Furthermore, the "lazy" parameter specifies whether all data fields
         should be read on-demand when get_dataset is called, or if they should
         all be read and populated into data_list when the object is
         instantiated.
 
@@ -109,35 +163,46 @@
             ))
 
         if log_file is not None and primary_key is not None:
             raise ValueError('You cannot provide both primary_key and log_file.')
         if log_file is None and primary_key is None:
             raise ValueError('You must provide either a primary_key or log_file.')
 
+
         self._pk = primary_key
         self._db = db_handle
+        if log_file is not None:
+            self._sha256sum = DatabaseULog.calc_sha256sum(log_file)
 
         super().__init__(log_file, **kwargs)
         if primary_key is not None:
             self.load(lazy=lazy)
 
     @property
     def primary_key(self):
-        '''The primary of the key, pointing to the correct "ULog" row in the database.'''
+        '''The primary key of the ulog, pointing to the correct "ULog" row in the database.'''
         return self._pk
 
+    @property
+    def sha256sum(self):
+        '''The computed SHA256 digest of the file, stored for later use.'''
+        return self._sha256sum
+
     # pylint: disable=too-many-locals,too-many-branches
     def load(self, lazy=True):
         '''
         Load all necessary data from the database, possibly except for the data series
         themselves, which can cost unnecessary resources.
 
         If lazy=True, then the data series will be left unread, deferred until
         get_dataset is called. If however lazy=False, then all data series will
         be read at once.
+
+        Even if the log was originally saved with append_json=True, this
+        function will always use the faster BLOB column for retrieval.
         '''
         if not DatabaseULog.exists_in_db(self._db, self._pk):
             raise KeyError(f'No ULog in database with Id={self._pk}')
 
         with self._db() as con:
             cur = con.cursor()
 
@@ -145,26 +210,28 @@
             cur.execute('''
                 SELECT FileVersion,
                        StartTimestamp,
                        LastTimestamp,
                        CompatFlags,
                        IncompatFlags,
                        SyncCount,
-                       HasSync
+                       HasSync,
+                       SHA256Sum
                 FROM ULog
                 WHERE Id = ?
                 ''', (self._pk,))
             ulog_result = cur.fetchone()
             self._file_version = ulog_result[0]
             self._start_timestamp = ulog_result[1]
             self._last_timestamp = ulog_result[2]
             self._compat_flags = [ord(c) for c in ulog_result[3]]
             self._incompat_flags = [ord(c) for c in ulog_result[4]]
             self._sync_seq_cnt = ulog_result[5]
             self._has_sync = ulog_result[6]
+            self._sha256sum = ulog_result[7]
 
             # appended_offsets
             cur.execute('''
                 SELECT Offset
                 FROM ULogAppendedOffsets
                 WHERE ULogId = ?
                 ORDER BY SeriesIndex
@@ -371,39 +438,51 @@
                 msg_id=msg_id,
                 timestamp_idx=timestamp_idx,
                 field_data=fields,
                 data=data,
             )
         return dataset
 
-    def save(self):
+    def save(self, append_json=False):
         '''
         Save the DatabaseULog to the database. Throws a KeyError if the primary
         key is already in the database.
+
+        The datasets are stored in a sqlite BLOB for fast retrieval, but if
+        append_json=True, then datasets are additionally stored in a JSON
+        field. This allows them to be directly queried using the sqlite
+        function json_each, but increases the writing time and database size.
         '''
+
         if self._pk is not None:
             raise KeyError('Cannot save logs that are already in the database')
 
+        pk_from_hash = DatabaseULog.primary_key_from_sha256sum(self._db, self._sha256sum)
+        if pk_from_hash is not None:
+            self._pk = pk_from_hash
+            raise KeyError(f'Hash {self._sha256sum} already in database with Id={pk_from_hash}')
+
         with self._db() as con:
             cur = con.cursor()
 
             # ULog metadata
             cur.execute('''
                 INSERT INTO ULog
-                (FileVersion, StartTimestamp, LastTimestamp, CompatFlags, IncompatFlags, SyncCount, HasSync)
+                (FileVersion, StartTimestamp, LastTimestamp, CompatFlags, IncompatFlags, SyncCount, HasSync, SHA256Sum)
                 VALUES
-                (?, ?, ?, ?, ?, ?, ?)
+                (?, ?, ?, ?, ?, ?, ?, ?)
             ''', (
                     self._file_version,
                     self._start_timestamp,
                     self._last_timestamp,
                     ''.join([chr(n) for n in self._compat_flags]),
                     ''.join([chr(n) for n in self._incompat_flags]),
                     self._sync_seq_cnt,
                     self._has_sync,
+                    self._sha256sum,
                 )
             )
             self._pk = cur.lastrowid
 
             # appended_offsets
             cur.executemany('''
                 INSERT INTO ULogAppendedOffsets
@@ -429,23 +508,42 @@
                         dataset.msg_id,
                         dataset.timestamp_idx,
                         self._pk,
                     )
                 )
                 dataset_id = cur.lastrowid
                 for field in dataset.field_data:
-                    cur.execute('''
+                    values = dataset.data[field.field_name]
+                    values_bytes = values.tobytes()
+                    if append_json:
+                        # Precision is only good enough up to a few decimals,
+                        # depending on the default float formatter. The
+                        # function np.array2string was tested, but was slower.
+                        # Also note that doing the slow json.dumps is also
+                        # unnecessary since we know that the object to be
+                        # formatted is an array.
+                        timestamp_list = [str(s) for s in dataset.data['timestamp'].tolist()]
+                        values_json = str(
+                            dict(zip(timestamp_list, values.tolist()))
+                        ).replace('nan', 'null').replace('inf', 'null').replace("'", '"')
+                        json_placeholder = 'json(?)'  # Saves some space
+                    else:
+                        values_json = None
+                        json_placeholder = '?'
+
+                    cur.execute(f'''
                         INSERT INTO ULogField
-                        (TopicName, DataType, ValueArray, DatasetId)
+                        (TopicName, DataType, ValueArray, ValueJson, DatasetId)
                         VALUES
-                        (?, ?, ?, ?)
+                        (?, ?, ?, {json_placeholder}, ?)
                         ''', (
                             field.field_name,
                             field.type_str,
-                            dataset.data[field.field_name].tobytes(),
+                            values_bytes,
+                            values_json,
                             dataset_id,
                         )
                     )
 
             # dropouts
             cur.executemany('''
                 INSERT INTO ULogMessageDropout
@@ -580,14 +678,31 @@
                     key,
                     value,
                     self._pk,
                 ) for timestamp, key, value in self.changed_parameters])
 
             cur.close()
 
+    def delete(self):
+        '''
+        Deletes the ULog row and cascading rows from the database.
+        '''
+        if self._pk is None:
+            raise KeyError('Cannot delete logs that are not in the database')
+
+        with self._db() as con:
+            cur = con.cursor()
+            cur.execute('''
+                DELETE FROM ULog
+                WHERE Id = ?
+            ''', (self._pk,)
+            )
+            cur.close()
+        self._pk = None
+
     class DatabaseData(ULog.Data):
         '''
         Overrides the ULog.Data class since its constructor only
         reads ULog.MessageLogAdded objects, and we want to specify
         the fields directly.
         '''
         # pylint: disable=super-init-not-called,too-many-arguments
```

### Comparing `pyulog-1.0.0/pyulog/extract_gps_dump.py` & `pyulog-1.0.1/pyulog/extract_gps_dump.py`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/pyulog/info.py` & `pyulog-1.0.1/pyulog/info.py`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/pyulog/messages.py` & `pyulog-1.0.1/pyulog/messages.py`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/pyulog/migrate_db.py` & `pyulog-1.0.1/pyulog/migrate_db.py`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/pyulog/params.py` & `pyulog-1.0.1/pyulog/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def get_defaults(ulog, default):
     """ get default params from ulog """
     assert ulog.has_default_parameters, "Log does not contain default parameters"
 
     if default == 'system': return ulog.get_default_parameters(0)
     if default == 'current_setup': return ulog.get_default_parameters(1)
-    raise Exception('invalid value \'{}\' for --default'.format(default))
+    raise ValueError('invalid value \'{}\' for --default'.format(default))
 
 def main():
     """Commande line interface"""
     parser = argparse.ArgumentParser(description='Extract parameters from an ULog file')
     parser.add_argument('filename', metavar='file.ulg', help='ULog input file')
 
     parser.add_argument('-l', '--delimiter', dest='delimiter', action='store',
```

### Comparing `pyulog-1.0.0/pyulog/px4.py` & `pyulog-1.0.1/pyulog/px4.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,25 +61,34 @@
         mc_est_group = self._ulog.initial_parameters.get('SYS_MC_EST_GROUP', 2)
         return {0: 'INAV',
                 1: 'LPE',
                 2: 'EKF2',
                 3: 'Q'}.get(mc_est_group, 'unknown ({})'.format(mc_est_group))
 
 
-    def add_roll_pitch_yaw(self):
+    def add_roll_pitch_yaw(self, messages=None):
         """ convenience method to add the fields 'roll', 'pitch', 'yaw' to the
         loaded data using the quaternion fields (does not update field_data).
 
-        Messages are: 'vehicle_attitude.q' and 'vehicle_attitude_setpoint.q_d',
-        'vehicle_attitude_groundtruth.q' and 'vehicle_vision_attitude.q' """
-
-        self._add_roll_pitch_yaw_to_message('vehicle_attitude')
-        self._add_roll_pitch_yaw_to_message('vehicle_vision_attitude')
-        self._add_roll_pitch_yaw_to_message('vehicle_attitude_groundtruth')
-        self._add_roll_pitch_yaw_to_message('vehicle_attitude_setpoint', '_d')
+        By default, messages are: 'vehicle_attitude.q',
+        'vehicle_attitude_setpoint.q_d', 'vehicle_attitude_groundtruth.q' and
+        'vehicle_vision_attitude.q' """
+
+        if messages is None:
+            messages = ['vehicle_attitude',
+                        'vehicle_vision_attitude',
+                        'vehicle_attitude_groundtruth',
+                        'vehicle_attitude_setpoint:_d']
+        for message in messages:
+            if message.endswith(':_d'):
+                suffix = '_d'
+                message = message[:-3]
+            else:
+                suffix = ''
+            self._add_roll_pitch_yaw_to_message(message, suffix)
 
 
     def _add_roll_pitch_yaw_to_message(self, message_name, field_name_suffix=''):
 
         message_data_all = [elem for elem in self._ulog.data_list if elem.name == message_name]
         for message_data in message_data_all:
             q = [message_data.data['q'+field_name_suffix+'['+str(i)+']'] for i in range(4)]
```

### Comparing `pyulog-1.0.0/pyulog/sql/pyulog.1.sql` & `pyulog-1.0.1/pyulog/sql/pyulog.1.sql`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/pyulog/ulog2csv.py` & `pyulog-1.0.1/pyulog/ulog2csv.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Convert a ULog file into CSV file(s)
 """
 
 from __future__ import print_function
 
 import argparse
 import os
+import numpy as np
 
 from .core import ULog
 
 #pylint: disable=too-many-locals, invalid-name, consider-using-enumerate
 
 def main():
     """Command line interface"""
@@ -29,31 +30,43 @@
 
     parser.add_argument('-o', '--output', dest='output', action='store',
                         help='Output directory (default is same as input file)',
                         metavar='DIR')
     parser.add_argument('-i', '--ignore', dest='ignore', action='store_true',
                         help='Ignore string parsing exceptions', default=False)
 
+    parser.add_argument(
+        '-ts', '--time_s', dest='time_s', type = int,
+        help="Only convert data after this timestamp (in seconds)")
+
+    parser.add_argument(
+        '-te', '--time_e', dest='time_e', type=int,
+        help="Only convert data upto this timestamp (in seconds)")
+
     args = parser.parse_args()
 
     if args.output and not os.path.isdir(args.output):
         print('Creating output directory {:}'.format(args.output))
         os.mkdir(args.output)
 
-    convert_ulog2csv(args.filename, args.messages, args.output, args.delimiter, args.ignore)
+    convert_ulog2csv(args.filename, args.messages, args.output, args.delimiter,
+                     args.time_s, args.time_e, args.ignore)
 
 
-def convert_ulog2csv(ulog_file_name, messages, output, delimiter, disable_str_exceptions=False):
+def convert_ulog2csv(ulog_file_name, messages, output, delimiter, time_s, time_e,
+                     disable_str_exceptions=False):
     """
     Coverts and ULog file to a CSV file.
 
     :param ulog_file_name: The ULog filename to open and read
     :param messages: A list of message names
     :param output: Output file path
     :param delimiter: CSV delimiter
+    :param time_s: Offset time for conversion in seconds
+    :param time_e: Limit until time for conversion in seconds
 
     :return: None
     """
 
     msg_filter = messages.split(',') if messages else None
 
     ulog = ULog(ulog_file_name, msg_filter, disable_str_exceptions)
@@ -67,15 +80,15 @@
     # write to different output path?
     if output:
         base_name = os.path.basename(output_file_prefix)
         output_file_prefix = os.path.join(output, base_name)
 
     for d in data:
         fmt = '{0}_{1}_{2}.csv'
-        output_file_name = fmt.format(output_file_prefix, d.name, d.multi_id)
+        output_file_name = fmt.format(output_file_prefix, d.name.replace('/', '_'), d.multi_id)
         fmt = 'Writing {0} ({1} data points)'
         # print(fmt.format(output_file_name, len(d.data['timestamp'])))
         with open(output_file_name, 'w', encoding='utf-8') as csvfile:
 
             # use same field order as in the log, except for the timestamp
             data_keys = [f.field_name for f in d.field_data]
             data_keys.remove('timestamp')
@@ -84,15 +97,23 @@
             # we don't use np.savetxt, because we have multiple arrays with
             # potentially different data types. However the following is quite
             # slow...
 
             # write the header
             csvfile.write(delimiter.join(data_keys) + '\n')
 
+            #get the index for row where timestamp exceeds or equals the required value
+            time_s_i = np.where(d.data['timestamp'] >= time_s * 1e6)[0][0] \
+                    if time_s else 0
+            #get the index for row upto the timestamp of the required value
+            time_e_i = np.where(d.data['timestamp'] >= time_e * 1e6)[0][0] \
+                    if time_e else len(d.data['timestamp'])
+
             # write the data
             last_elem = len(data_keys)-1
-            for i in range(len(d.data['timestamp'])):
+            for i in range(time_s_i, time_e_i):
                 for k in range(len(data_keys)):
                     csvfile.write(str(d.data[data_keys[k]][i]))
                     if k != last_elem:
                         csvfile.write(delimiter)
                 csvfile.write('\n')
+
```

### Comparing `pyulog-1.0.0/pyulog/ulog2kml.py` & `pyulog-1.0.1/pyulog/ulog2kml.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     topic_instance = 0
     if flight_mode_changes is None:
         flight_mode_changes = []
 
     cur_dataset = [elem for elem in data
                    if elem.name == position_topic_name and elem.multi_id == topic_instance]
     if len(cur_dataset) == 0:
-        raise Exception(position_topic_name+' not found in data')
+        raise KeyError(position_topic_name+' not found in data')
 
     cur_dataset = cur_dataset[0]
 
 
     pos_lon = cur_dataset.data['lon']
     pos_lat = cur_dataset.data['lat']
     pos_alt = cur_dataset.data['alt']
```

### Comparing `pyulog-1.0.0/pyulog/ulog2rosbag.py` & `pyulog-1.0.1/pyulog/ulog2rosbag.py`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/pyulog.egg-info/PKG-INFO` & `pyulog-1.0.1/pyulog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyulog
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python log parser for ULog.
 Home-page: https://github.com/PX4/pyulog
 Download-URL: https://github.com/PX4/pyulog
 Author: Beat Kueng
 Author-email: beat-kueng@gmx.net
 Maintainer: James Goppert
 Maintainer-email: james.goppert@gmail.com
```

### Comparing `pyulog-1.0.0/setup.py` & `pyulog-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/test/test_migration.py` & `pyulog-1.0.1/test/test_migration.py`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/test/test_ulog2csv.py` & `pyulog-1.0.1/test/test_ulog2csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,17 @@
     def test_ulog2csv(self, test_case):
         tmpdir = tempfile.gettempdir()
         print('writing files to ', tmpdir)
         ulog_file_name = os.path.join(TEST_PATH, test_case+'.ulg')
         messages = []
         output=tmpdir
         delimiter=','
-        ulog2csv.convert_ulog2csv(ulog_file_name, messages, output, delimiter)
+        time_s = 0
+        time_e = 0
+        ulog2csv.convert_ulog2csv(ulog_file_name, messages, output, delimiter, time_s, time_e)
 
     @data('sample', 'sample_appended', 'sample_appended_multiple')
     def test_pyulog_info_cli(self, test_case):
         sys.argv = [
             '',
             os.path.join(TEST_PATH, test_case+'.ulg'),
             '-v'
```

### Comparing `pyulog-1.0.0/test/test_ulog_write.py` & `pyulog-1.0.1/test/test_ulog_write.py`

 * *Files identical despite different names*

### Comparing `pyulog-1.0.0/versioneer.py` & `pyulog-1.0.1/versioneer.py`

 * *Files identical despite different names*

